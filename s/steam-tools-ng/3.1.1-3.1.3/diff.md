# Comparing `tmp/steam-tools-ng-3.1.1.rc1.tar.gz` & `tmp/steam-tools-ng-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-tools-ng-3.1.1.tar", last modified: Sat Aug  5 09:26:28 2023, max compression
+gzip compressed data, was "steam-tools-ng-3.1.3.tar", last modified: Sat Aug  5 11:35:28 2023, max compression
```

## Comparing `steam-tools-ng-3.1.1.rc1.tar` & `steam-tools-ng-3.1.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.573988 steam-tools-ng-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-05 09:26:28.573988 steam-tools-ng-3.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3334 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.565988 steam-tools-ng-3.1.1/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/i18n/fr.po
--rwxr-xr-x   0 runner    (1001) docker     (123)    47681 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/i18n/pt_BR.po
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:26:28.573988 steam-tools-ng-3.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     6010 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.561988 steam-tools-ng-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.565988 steam-tools-ng-3.1.1/src/steam_tools_ng/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.569988 steam-tools-ng-3.1.1/src/steam_tools_ng/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.569988 steam-tools-ng-3.1.1/src/steam_tools_ng/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/cardfarming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/confirmations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/coupons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/fakerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamgifts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamtrades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.573988 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    15749 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/async_gtk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/confirmation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    28329 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39035 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.573988 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   245142 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.ico
--rw-r--r--   0 runner    (1001) docker     (123)    97830 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.png
--rw-r--r--   0 runner    (1001) docker     (123)   231041 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31925 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.png
--rw-r--r--   0 runner    (1001) docker     (123)   229900 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.ico
--rw-r--r--   0 runner    (1001) docker     (123)    66900 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.png
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/logger_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.565988 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-05 09:26:28.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-05 09:26:28.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:26:28.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-05 09:26:28.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:26:28.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-05 09:26:28.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 09:26:28.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/steam-tools-ng.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:26:28.573988 steam-tools-ng-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-05 09:26:07.000000 steam-tools-ng-3.1.1/tests/test_placeholder.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:28.901734 steam-tools-ng-3.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)    35148 2023-03-17 08:22:26.000000 steam-tools-ng-3.1.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      208 2023-03-17 08:22:26.000000 steam-tools-ng-3.1.3/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     4444 2023-08-05 11:35:28.898735 steam-tools-ng-3.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3334 2023-07-25 13:28:20.000000 steam-tools-ng-3.1.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:27.152580 steam-tools-ng-3.1.3/i18n/
+-rwxrwxrwx   0 root         (0) root         (0)    35901 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/i18n/fr.po
+-rwxrwxrwx   0 root         (0) root         (0)    47681 2023-07-27 13:40:42.000000 steam-tools-ng-3.1.3/i18n/pt_BR.po
+-rwxrwxrwx   0 root         (0) root         (0)     1908 2023-08-05 11:35:10.000000 steam-tools-ng-3.1.3/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-05 11:35:28.902234 steam-tools-ng-3.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     6010 2023-07-21 18:43:56.000000 steam-tools-ng-3.1.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:26.988581 steam-tools-ng-3.1.3/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:27.396597 steam-tools-ng-3.1.3/src/steam_tools_ng/
+-rwxrwxrwx   0 root         (0) root         (0)     1412 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      788 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4766 2023-07-20 13:34:52.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)    10620 2023-07-27 13:40:42.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/config.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:27.816734 steam-tools-ng-3.1.3/src/steam_tools_ng/console/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 10:06:38.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/console/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6221 2023-07-21 14:57:43.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/console/authenticator.py
+-rwxrwxrwx   0 root         (0) root         (0)     8338 2023-07-21 14:57:43.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/console/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     6948 2023-07-19 15:16:11.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/console/login.py
+-rwxrwxrwx   0 root         (0) root         (0)     4562 2023-07-21 14:57:43.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/console/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:28.158734 steam-tools-ng-3.1.3/src/steam_tools_ng/core/
+-rwxrwxrwx   0 root         (0) root         (0)     1436 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9996 2023-07-21 14:57:43.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/cardfarming.py
+-rwxrwxrwx   0 root         (0) root         (0)     2677 2023-06-23 01:04:12.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/confirmations.py
+-rwxrwxrwx   0 root         (0) root         (0)     7445 2023-07-25 13:28:20.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/coupons.py
+-rwxrwxrwx   0 root         (0) root         (0)     4769 2023-06-17 04:45:13.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/fakerun.py
+-rwxrwxrwx   0 root         (0) root         (0)     8881 2023-07-21 14:57:43.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/steamgifts.py
+-rwxrwxrwx   0 root         (0) root         (0)     3169 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/steamguard.py
+-rwxrwxrwx   0 root         (0) root         (0)     5070 2023-07-21 14:57:44.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/steamtrades.py
+-rwxrwxrwx   0 root         (0) root         (0)     3313 2023-06-27 00:18:22.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/core/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:28.596235 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/
+-rwxrwxrwx   0 root         (0) root         (0)      976 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1881 2023-06-17 04:40:18.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/about.py
+-rwxrwxrwx   0 root         (0) root         (0)    15749 2023-07-27 14:17:50.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/application.py
+-rwxrwxrwx   0 root         (0) root         (0)     2191 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/async_gtk.py
+-rwxrwxrwx   0 root         (0) root         (0)    11015 2023-07-21 14:57:44.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/authenticator.py
+-rwxrwxrwx   0 root         (0) root         (0)     7068 2023-07-21 14:57:44.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/confirmation.py
+-rwxrwxrwx   0 root         (0) root         (0)     9423 2023-07-21 14:57:44.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/coupon.py
+-rwxrwxrwx   0 root         (0) root         (0)    12574 2023-07-25 14:08:19.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/login.py
+-rwxrwxrwx   0 root         (0) root         (0)     5780 2023-07-27 13:40:42.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)    28329 2023-08-05 09:21:46.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    39035 2023-08-05 09:19:09.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/window.py
+-rwxrwxrwx   0 root         (0) root         (0)     4490 2023-07-21 18:43:56.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/gui.py
+-rwxrwxrwx   0 root         (0) root         (0)     1430 2023-06-17 07:55:20.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/i18n.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:28.839236 steam-tools-ng-3.1.3/src/steam_tools_ng/icons/
+-rwxrwxrwx   0 root         (0) root         (0)   245142 2023-03-17 10:06:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng.ico
+-rwxrwxrwx   0 root         (0) root         (0)    97830 2023-03-17 10:06:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng.png
+-rwxrwxrwx   0 root         (0) root         (0)   231041 2023-03-17 10:06:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_console.ico
+-rwxrwxrwx   0 root         (0) root         (0)    31925 2023-03-17 10:06:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_console.png
+-rwxrwxrwx   0 root         (0) root         (0)   229900 2023-03-17 10:06:41.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_nc.ico
+-rwxrwxrwx   0 root         (0) root         (0)    66900 2023-03-17 10:06:41.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_nc.png
+-rwxrwxrwx   0 root         (0) root         (0)     4195 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/logger_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 10:06:41.000000 steam-tools-ng-3.1.3/src/steam_tools_ng/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:27.629726 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4444 2023-08-05 11:35:25.000000 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1792 2023-08-05 11:35:26.000000 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-05 11:35:25.000000 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      104 2023-08-05 11:35:25.000000 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-05 11:35:24.000000 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       84 2023-08-05 11:35:25.000000 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-08-05 11:35:25.000000 steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      238 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/steam-tools-ng.desktop
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-05 11:35:28.868237 steam-tools-ng-3.1.3/tests/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-22 10:24:40.000000 steam-tools-ng-3.1.3/tests/test_placeholder.py
```

### Comparing `steam-tools-ng-3.1.1/LICENSE` & `steam-tools-ng-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/PKG-INFO` & `steam-tools-ng-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.1.1
+Version: 3.1.3
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
```

### Comparing `steam-tools-ng-3.1.1/README.md` & `steam-tools-ng-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/i18n/fr.po` & `steam-tools-ng-3.1.3/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/i18n/pt_BR.po` & `steam-tools-ng-3.1.3/i18n/pt_BR.po`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/pyproject.toml` & `steam-tools-ng-3.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "certifi", "cx_Freeze; sys_platform == 'win32'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "steam-tools-ng"
-version = "3.1.1"
+version = "3.1.3"
 description = "Steam Tools NG"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 keywords = ["steam", "valve"]
 authors = [{email = "dev@lara.monster"}, {name = "Lara Maia"}]
 classifiers = [
```

### Comparing `steam-tools-ng-3.1.1/setup.py` & `steam-tools-ng-3.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/__init__.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/__main__.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/__main__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/cli.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/cli.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/config.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/config.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/console/authenticator.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/console/authenticator.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/console/cli.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/console/cli.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/console/login.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/console/login.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/console/utils.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/console/utils.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/__init__.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/cardfarming.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/cardfarming.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/confirmations.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/confirmations.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/coupons.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/coupons.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/fakerun.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/fakerun.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamgifts.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/steamgifts.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamguard.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/steamguard.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamtrades.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/steamtrades.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/core/utils.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/core/utils.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/__init__.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/about.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/about.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/application.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/application.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/async_gtk.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/async_gtk.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/authenticator.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/authenticator.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/confirmation.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/confirmation.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/coupon.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/coupon.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/login.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/login.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/settings.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/settings.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/utils.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/utils.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/window.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gtk/window.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/gui.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/gui.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/i18n.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/i18n.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.ico` & `steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.png` & `steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.ico` & `steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_console.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.png` & `steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_console.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.ico` & `steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_nc.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.png` & `steam-tools-ng-3.1.3/src/steam_tools_ng/icons/stng_nc.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng/logger_handlers.py` & `steam-tools-ng-3.1.3/src/steam_tools_ng/logger_handlers.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/PKG-INFO` & `steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.1.1
+Version: 3.1.3
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
```

### Comparing `steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/SOURCES.txt` & `steam-tools-ng-3.1.3/src/steam_tools_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

