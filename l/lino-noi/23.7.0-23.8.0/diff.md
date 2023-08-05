# Comparing `tmp/lino-noi-23.7.0.tar.gz` & `tmp/lino-noi-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-noi-23.7.0.tar", last modified: Thu Jul 13 12:25:42 2023, max compression
+gzip compressed data, was "lino-noi-23.8.0.tar", last modified: Sat Aug  5 10:19:37 2023, max compression
```

## Comparing `lino-noi-23.7.0.tar` & `lino-noi-23.8.0.tar`

### file list

```diff
@@ -1,120 +1,112 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/.idea/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/encodings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1839 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/misc.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/modules.xml
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/.idea/scopes/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      139 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/scopes/scope_settings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/vcs.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2202 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/workspace.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:54:16.000000 lino-noi-23.7.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      109 2016-08-14 01:22:00.000000 lino-noi-23.7.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1518 2023-07-13 12:25:42.888773 lino-noi-23.7.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-03-29 14:44:08.000000 lino-noi-23.7.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2022-08-17 01:06:46.000000 lino-noi-23.7.0/lino_noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/cal/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      299 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/cal/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3523 2023-04-15 09:49:10.000000 lino-noi-23.7.0/lino_noi/lib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      274 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      245 2021-04-07 10:22:55.000000 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2020-04-04 06:56:19.000000 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-05-26 22:13:00.000000 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3239 2023-07-09 03:53:22.000000 lino-noi-23.7.0/lino_noi/lib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/courses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      812 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/courses/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      717 2022-11-08 12:29:27.000000 lino-noi-23.7.0/lino_noi/lib/courses/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2532 2022-11-08 12:30:48.000000 lino-noi-23.7.0/lino_noi/lib/courses/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/groups/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      319 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/groups/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      749 2021-08-16 10:54:17.000000 lino-noi-23.7.0/lino_noi/lib/groups/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      329 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:02.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    19620 2023-07-01 05:01:29.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6630 2022-10-18 23:19:00.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/linotickets.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      198 2023-05-12 19:49:16.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/minimal_ledger.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2138 2023-07-13 08:56:42.000000 lino-noi-23.7.0/lino_noi/lib/noi/help_texts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      540 2021-06-15 17:12:44.000000 lino-noi-23.7.0/lino_noi/lib/noi/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    14514 2019-03-29 11:25:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13858 2019-03-29 11:25:55.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13846 2019-03-29 11:25:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)    22188 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1131 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     6755 2023-06-23 08:25:25.000000 lino-noi-23.7.0/lino_noi/lib/noi/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3039 2023-05-12 19:54:48.000000 lino-noi-23.7.0/lino_noi/lib/noi/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      383 2023-05-12 19:27:14.000000 lino-noi-23.7.0/lino_noi/lib/noi/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/products/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      301 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/products/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      947 2023-05-28 02:47:30.000000 lino-noi-23.7.0/lino_noi/lib/products/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/public/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1166 2021-12-22 12:48:36.000000 lino-noi-23.7.0/lino_noi/lib/public/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/public/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/public/config/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2019-11-25 17:29:52.000000 lino-noi-23.7.0/lino_noi/lib/public/config/noi/index.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      720 2022-09-01 18:33:50.000000 lino-noi-23.7.0/lino_noi/lib/public/config/noi/tickets.Ticket.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      554 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/public/renderer.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1583 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/public/views.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/sales/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      311 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/sales/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/sales/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/sales/config/sales/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/sales/config/sales/VatProductInvoice/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1413 2023-02-15 06:31:52.000000 lino-noi-23.7.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/sales/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-05-09 16:04:58.000000 lino-noi-23.7.0/lino_noi/lib/sales/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2017-02-26 08:07:55.000000 lino-noi-23.7.0/lino_noi/lib/sales/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      985 2022-12-26 16:50:31.000000 lino-noi-23.7.0/lino_noi/lib/sales/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/subscriptions/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2023-01-06 20:30:18.000000 lino-noi-23.7.0/lino_noi/lib/subscriptions/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      378 2023-01-06 20:50:15.000000 lino-noi-23.7.0/lino_noi/lib/subscriptions/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/tickets/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1658 2023-01-08 01:21:19.000000 lino-noi-23.7.0/lino_noi/lib/tickets/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    15885 2023-02-16 20:05:18.000000 lino-noi-23.7.0/lino_noi/lib/tickets/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3858 2022-10-30 00:45:53.000000 lino-noi-23.7.0/lino_noi/lib/tickets/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/topics/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/topics/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      622 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/topics/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)       37 2023-03-06 06:43:39.000000 lino-noi-23.7.0/lino_noi/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:00.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:49.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:50.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:50.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-11-08 12:29:27.000000 lino-noi-23.7.0/lino_noi/lib/users/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1639 2023-07-10 20:32:06.000000 lino-noi-23.7.0/lino_noi/lib/users/ui.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3080 2023-07-13 12:23:53.000000 lino-noi-23.7.0/lino_noi/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1518 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2585 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-08-31 16:13:18.000000 lino-noi-23.7.0/lino_noi.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      263 2021-05-05 05:16:56.000000 lino-noi-23.7.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-07-13 12:25:42.888773 lino-noi-23.7.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      179 2020-07-10 07:49:24.000000 lino-noi-23.7.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2021-04-25 11:53:26.000000 lino-noi-23.7.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-18 18:50:53.000000 lino-noi-23.7.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2019-12-18 18:51:44.000000 lino-noi-23.7.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      186 2019-12-18 18:51:08.000000 lino-noi-23.7.0/tests/test_packages.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:18.000000 lino-noi-23.8.0/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      109 2023-02-28 05:23:18.000000 lino-noi-23.8.0/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1481 2023-08-05 10:19:37.795389 lino-noi-23.8.0/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      716 2023-03-30 05:51:22.000000 lino-noi-23.8.0/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      457 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      297 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.787389 lino-noi-23.8.0/lino_noi/lib/cal/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      299 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/cal/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.787389 lino-noi-23.8.0/lino_noi/lib/cal/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/cal/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       49 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/cal/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3523 2023-04-27 13:13:36.000000 lino-noi-23.8.0/lino_noi/lib/cal/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.787389 lino-noi-23.8.0/lino_noi/lib/contacts/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      274 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/contacts/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.787389 lino-noi-23.8.0/lino_noi/lib/contacts/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      245 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/contacts/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       55 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/contacts/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/contacts/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3239 2023-07-11 05:44:45.000000 lino-noi-23.8.0/lino_noi/lib/contacts/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.787389 lino-noi-23.8.0/lino_noi/lib/courses/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      812 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/courses/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      717 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/courses/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2532 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/courses/ui.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.787389 lino-noi-23.8.0/lino_noi/lib/groups/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      319 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/groups/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      749 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/groups/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/noi/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      329 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/noi/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    19620 2023-07-11 05:44:45.000000 lino-noi-23.8.0/lino_noi/lib/noi/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6630 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/fixtures/linotickets.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      198 2023-07-11 05:44:45.000000 lino-noi-23.8.0/lino_noi/lib/noi/fixtures/minimal_ledger.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2138 2023-04-04 07:26:45.000000 lino-noi-23.8.0/lino_noi/lib/noi/help_texts.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      540 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/layouts.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/noi/locale/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/noi/locale/de/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2008 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    14514 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/noi/locale/et/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      660 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13858 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/noi/locale/fr/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      490 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13846 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    22188 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/migrate.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1131 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6755 2023-07-11 05:44:45.000000 lino-noi-23.8.0/lino_noi/lib/noi/settings.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3039 2023-07-11 05:44:45.000000 lino-noi-23.8.0/lino_noi/lib/noi/user_types.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      383 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/noi/workflows.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/products/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      301 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/products/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      947 2023-07-11 05:44:45.000000 lino-noi-23.8.0/lino_noi/lib/products/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/public/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1166 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/public/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/public/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/public/config/noi/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      474 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/public/config/noi/index.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      720 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/public/config/noi/tickets.Ticket.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      554 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/public/renderer.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1583 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/public/views.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/sales/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      311 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/sales/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/sales/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi/lib/sales/config/sales/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.791389 lino-noi-23.8.0/lino_noi/lib/sales/config/sales/VatProductInvoice/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1413 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/lino_noi/lib/sales/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/sales/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       51 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/sales/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      985 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/sales/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/lino_noi/lib/subscriptions/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      189 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/subscriptions/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      378 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/subscriptions/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/lino_noi/lib/tickets/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1658 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/tickets/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    15885 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/tickets/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3885 2023-07-12 07:33:49.000000 lino-noi-23.8.0/lino_noi/lib/tickets/workflows.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/lino_noi/lib/topics/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      213 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/topics/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      622 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/topics/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/lino_noi/lib/users/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       37 2023-03-06 06:57:25.000000 lino-noi-23.8.0/lino_noi/lib/users/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/lino_noi/lib/users/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/users/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       46 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/users/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/users/fixtures/demo2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       52 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/users/fixtures/demo_users.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      248 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi/lib/users/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1639 2023-06-28 13:37:39.000000 lino-noi-23.8.0/lino_noi/lib/users/ui.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3080 2023-08-05 10:19:05.000000 lino-noi-23.8.0/lino_noi/setup_info.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.783389 lino-noi-23.8.0/lino_noi.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1481 2023-08-05 10:19:37.000000 lino-noi-23.8.0/lino_noi.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2466 2023-08-05 10:19:37.000000 lino-noi-23.8.0/lino_noi.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-08-05 10:19:37.000000 lino-noi-23.8.0/lino_noi.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:18.000000 lino-noi-23.8.0/lino_noi.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        8 2023-08-05 10:19:37.000000 lino-noi-23.8.0/lino_noi.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        9 2023-08-05 10:19:37.000000 lino-noi-23.8.0/lino_noi.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      263 2023-02-28 05:23:18.000000 lino-noi-23.8.0/requirements.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-08-05 10:19:37.795389 lino-noi-23.8.0/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      179 2023-02-28 05:23:18.000000 lino-noi-23.8.0/setup.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      487 2023-02-28 05:23:18.000000 lino-noi-23.8.0/tasks.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-05 10:19:37.795389 lino-noi-23.8.0/tests/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-noi-23.8.0/tests/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      189 2023-02-28 05:23:18.000000 lino-noi-23.8.0/tests/test_docs.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      186 2023-02-28 05:23:18.000000 lino-noi-23.8.0/tests/test_packages.py
```

### Comparing `lino-noi-23.7.0/COPYING` & `lino-noi-23.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/PKG-INFO` & `lino-noi-23.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 23.7.0
+Version: 23.8.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -37,9 +35,7 @@
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
-
-
```

### Comparing `lino-noi-23.7.0/README.rst` & `lino-noi-23.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/cal/models.py` & `lino-noi-23.8.0/lino_noi/lib/cal/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/contacts/models.py` & `lino-noi-23.8.0/lino_noi/lib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/courses/__init__.py` & `lino-noi-23.8.0/lino_noi/lib/courses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/courses/models.py` & `lino-noi-23.8.0/lino_noi/lib/courses/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/courses/ui.py` & `lino-noi-23.8.0/lino_noi/lib/courses/ui.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/groups/models.py` & `lino-noi-23.8.0/lino_noi/lib/groups/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/fixtures/demo.py` & `lino-noi-23.8.0/lino_noi/lib/noi/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/fixtures/linotickets.py` & `lino-noi-23.8.0/lino_noi/lib/noi/fixtures/linotickets.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/help_texts.py` & `lino-noi-23.8.0/lino_noi/lib/noi/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/layouts.py` & `lino-noi-23.8.0/lino_noi/lib/noi/layouts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo` & `lino-noi-23.8.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po` & `lino-noi-23.8.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo` & `lino-noi-23.8.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po` & `lino-noi-23.8.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po` & `lino-noi-23.8.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/migrate.py` & `lino-noi-23.8.0/lino_noi/lib/noi/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/models.py` & `lino-noi-23.8.0/lino_noi/lib/noi/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/settings.py` & `lino-noi-23.8.0/lino_noi/lib/noi/settings.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/noi/user_types.py` & `lino-noi-23.8.0/lino_noi/lib/noi/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/products/models.py` & `lino-noi-23.8.0/lino_noi/lib/products/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/public/__init__.py` & `lino-noi-23.8.0/lino_noi/lib/public/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/public/config/noi/tickets.Ticket.html` & `lino-noi-23.8.0/lino_noi/lib/public/config/noi/tickets.Ticket.html`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/public/renderer.py` & `lino-noi-23.8.0/lino_noi/lib/public/renderer.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/public/views.py` & `lino-noi-23.8.0/lino_noi/lib/public/views.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html` & `lino-noi-23.8.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/sales/models.py` & `lino-noi-23.8.0/lino_noi/lib/sales/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/tickets/__init__.py` & `lino-noi-23.8.0/lino_noi/lib/tickets/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/tickets/models.py` & `lino-noi-23.8.0/lino_noi/lib/tickets/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/tickets/workflows.py` & `lino-noi-23.8.0/lino_noi/lib/tickets/workflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2016-2022 Rumma & Ko Ltd
+# Copyright 2016-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 """The default :attr:`workflows_module
 <lino.core.site.Site.workflows_module>` for :ref:`noi` applications.
 
 If :attr:`use_new_unicode_symbols
 <lino.core.site.Site.use_new_unicode_symbols>` is True, ticket states
 are represented using symbols from the `Miscellaneous Symbols and
@@ -13,21 +13,20 @@
 `Miscellaneous Symbols
 <https://en.wikipedia.org/wiki/Miscellaneous_Symbols>`
 `fileformat.info
 <http://www.fileformat.info/info/unicode/block/miscellaneous_symbols/list.htm>`__.
 
 """
 
-from lino.api import dd, rt, _, pgettext
-
-from lino.utils.instantiator import create_row
+from lino.api import dd, pgettext
 
 from lino_xl.lib.tickets.choicelists import TicketStates
 from lino_xl.lib.tickets.roles import Triager
 
+
 class TicketAction(dd.ChangeStateAction):
     """Base class for ticket actions.
 
     Make sure that only *triagers* can act on tickets of other users.
 
     """
     needs_site = False
@@ -69,22 +68,24 @@
 
 class MarkTicketReady(TicketAction):
     """Mark this ticket as ready.
     """
     action_name = 'mark_ready'
     required_states = "new opened working talk"
 
+
 class MarkTicketClosed(TicketAction):
     """Mark this ticket as closed.
     """
     # label = pgettext("verb", "Close")
     action_name = 'mark_closed'
     required_states = 'new talk working opened ready'
     needs_site = True
 
+
 class MarkTicketRefused(TicketAction):
     """Mark this ticket as refused.
     """
     required_states = 'talk working opened ready'
     action_name = 'mark_refused'
 
 
@@ -111,12 +112,12 @@
     required_states="new talk opened working")
 TicketStates.talk.add_transition(MarkTicketTalk)
 TicketStates.opened.add_transition(MarkTicketOpened)
 TicketStates.working.add_transition(MarkTicketWorking)
 TicketStates.ready.add_transition(MarkTicketReady)
 TicketStates.closed.add_transition(MarkTicketClosed)
 TicketStates.cancelled.add_transition(MarkTicketRefused)
-
+TicketStates.waiting.add_transition(required_states="new opened talk sleeping")
 
 # TicketStates.favorite_states = (TicketStates.sticky, )
 # TicketStates.work_states = (TicketStates.todo, TicketStates.new)
 # TicketStates.waiting_states = (TicketStates.done, )
```

### Comparing `lino-noi-23.7.0/lino_noi/lib/topics/models.py` & `lino-noi-23.8.0/lino_noi/lib/topics/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/lib/users/ui.py` & `lino-noi-23.8.0/lino_noi/lib/users/ui.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.7.0/lino_noi/setup_info.py` & `lino-noi-23.8.0/lino_noi/setup_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # srcref_url='https://gitlab.com/lino-framework/cosi/blob/master/%s',
     intersphinx_urls = dict(
         docs="https://noi.lino-framework.org"))
 
 
 SETUP_INFO = dict(
     name='lino-noi',
-    version='23.7.0',
+    version='23.8.0',
     install_requires=['lino-xl'],
     # tests_require=['pytest', 'mock'],
     test_suite='tests',
     description=("Manage support tickets and working time."),
     long_description="""\
 
 Lino Noi is a customizable ticket management and time tracking
```

### Comparing `lino-noi-23.7.0/lino_noi.egg-info/PKG-INFO` & `lino-noi-23.8.0/lino_noi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 23.7.0
+Version: 23.8.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -37,9 +35,7 @@
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
-
-
```

### Comparing `lino-noi-23.7.0/lino_noi.egg-info/SOURCES.txt` & `lino-noi-23.8.0/lino_noi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 COPYING
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 tasks.py
-.idea/encodings.xml
-.idea/misc.xml
-.idea/modules.xml
-.idea/vcs.xml
-.idea/workspace.xml
-.idea/scopes/scope_settings.xml
 lino_noi/__init__.py
 lino_noi/setup_info.py
 lino_noi.egg-info/PKG-INFO
 lino_noi.egg-info/SOURCES.txt
 lino_noi.egg-info/dependency_links.txt
 lino_noi.egg-info/not-zip-safe
 lino_noi.egg-info/requires.txt
```

