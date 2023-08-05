# Comparing `tmp/Quart-Kroket-1.0.6.tar.gz` & `tmp/Quart-Kroket-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quart-Kroket-1.0.6.tar", last modified: Fri Mar 31 18:59:10 2023, max compression
+gzip compressed data, was "Quart-Kroket-1.0.7.tar", last modified: Sat Aug  5 16:25:08 2023, max compression
```

## Comparing `Quart-Kroket-1.0.6.tar` & `Quart-Kroket-1.0.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.232352 Quart-Kroket-1.0.6/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1455 2023-02-22 04:27:16.000000 Quart-Kroket-1.0.6/LICENSE
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      351 2023-02-24 12:24:37.000000 Quart-Kroket-1.0.6/MANIFEST.in
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     7584 2023-03-31 18:59:10.232352 Quart-Kroket-1.0.6/PKG-INFO
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/Quart_Kroket.egg-info/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     7584 2023-03-31 18:59:10.000000 Quart-Kroket-1.0.6/Quart_Kroket.egg-info/PKG-INFO
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1455 2023-03-31 18:59:10.000000 Quart-Kroket-1.0.6/Quart_Kroket.egg-info/SOURCES.txt
--rw-rw-r--   0 dsc       (1000) dsc       (1000)        1 2023-03-31 18:59:10.000000 Quart-Kroket-1.0.6/Quart_Kroket.egg-info/dependency_links.txt
--rw-rw-r--   0 dsc       (1000) dsc       (1000)        1 2023-02-24 12:14:02.000000 Quart-Kroket-1.0.6/Quart_Kroket.egg-info/not-zip-safe
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      489 2023-03-31 18:59:10.000000 Quart-Kroket-1.0.6/Quart_Kroket.egg-info/requires.txt
--rw-rw-r--   0 dsc       (1000) dsc       (1000)       13 2023-03-31 18:59:10.000000 Quart-Kroket-1.0.6/Quart_Kroket.egg-info/top_level.txt
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     6847 2023-02-24 09:22:43.000000 Quart-Kroket-1.0.6/README.md
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     6125 2023-03-31 17:26:41.000000 Quart-Kroket-1.0.6/quart_kroket/__init__.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/data/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/data/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1089 2023-02-24 09:41:55.000000 Quart-Kroket-1.0.6/quart_kroket/data/checksum.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1471 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/data/structures.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/database/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1112 2023-02-22 17:42:03.000000 Quart-Kroket-1.0.6/quart_kroket/database/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     2615 2023-02-21 06:58:11.000000 Quart-Kroket-1.0.6/quart_kroket/database/enums.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      984 2023-02-24 11:41:33.000000 Quart-Kroket-1.0.6/quart_kroket/database/model.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/email/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1484 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/email/__init__.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/email/mjml/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1286 2023-02-24 11:36:23.000000 Quart-Kroket-1.0.6/quart_kroket/email/mjml/__init__.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/email/mjml/templates/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1298 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/email/mjml/templates/basic.jinja2
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/finance/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/finance/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1541 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/finance/validation.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/imaging/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)   340712 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/imaging/DejaVuSansMono.ttf
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      272 2023-02-23 22:03:32.000000 Quart-Kroket-1.0.6/quart_kroket/imaging/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     4307 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/imaging/avatars.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1443 2023-02-20 17:24:36.000000 Quart-Kroket-1.0.6/quart_kroket/imaging/captchav2.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     8016 2023-03-11 16:30:13.000000 Quart-Kroket-1.0.6/quart_kroket/imaging/imaging.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     2464 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/imaging/qr.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     3161 2023-02-24 11:14:42.000000 Quart-Kroket-1.0.6/quart_kroket/imaging/routes.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/localization/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-03-30 19:22:39.000000 Quart-Kroket-1.0.6/quart_kroket/localization/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)    10427 2023-03-30 19:24:49.000000 Quart-Kroket-1.0.6/quart_kroket/localization/countries.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.228352 Quart-Kroket-1.0.6/quart_kroket/markup/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-02-20 15:18:43.000000 Quart-Kroket-1.0.6/quart_kroket/markup/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     8609 2023-02-26 02:00:19.000000 Quart-Kroket-1.0.6/quart_kroket/markup/markdown.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.232352 Quart-Kroket-1.0.6/quart_kroket/media/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      342 2023-03-10 16:48:29.000000 Quart-Kroket-1.0.6/quart_kroket/media/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      169 2023-03-10 16:40:40.000000 Quart-Kroket-1.0.6/quart_kroket/media/constants.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)    10064 2023-03-21 20:08:54.000000 Quart-Kroket-1.0.6/quart_kroket/media/enums.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     2471 2023-03-09 13:49:40.000000 Quart-Kroket-1.0.6/quart_kroket/media/youtube.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.232352 Quart-Kroket-1.0.6/quart_kroket/net/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      161 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/net/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     4419 2023-02-28 09:25:36.000000 Quart-Kroket-1.0.6/quart_kroket/net/ftp.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      846 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/net/gravatar.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)   694041 2022-11-05 11:19:41.000000 Quart-Kroket-1.0.6/quart_kroket/net/http_agents.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1266 2023-03-22 12:43:35.000000 Quart-Kroket-1.0.6/quart_kroket/net/http_requests.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.232352 Quart-Kroket-1.0.6/quart_kroket/oidc/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-02-20 17:50:17.000000 Quart-Kroket-1.0.6/quart_kroket/oidc/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1893 2023-02-22 04:22:03.000000 Quart-Kroket-1.0.6/quart_kroket/oidc/models.py
-drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-03-31 18:59:10.232352 Quart-Kroket-1.0.6/quart_kroket/pdf/
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1496 2023-02-24 09:41:55.000000 Quart-Kroket-1.0.6/quart_kroket/pdf/__init__.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      694 2023-02-21 03:59:53.000000 Quart-Kroket-1.0.6/quart_kroket/template_filters.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1541 2023-03-29 15:16:29.000000 Quart-Kroket-1.0.6/quart_kroket/utils.py
--rw-rw-r--   0 dsc       (1000) dsc       (1000)      465 2023-03-31 18:58:48.000000 Quart-Kroket-1.0.6/requirements.txt
--rw-rw-r--   0 dsc       (1000) dsc       (1000)       61 2023-03-31 18:59:10.232352 Quart-Kroket-1.0.6/setup.cfg
--rw-rw-r--   0 dsc       (1000) dsc       (1000)     1246 2023-03-31 18:58:55.000000 Quart-Kroket-1.0.6/setup.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1455 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/LICENSE
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      351 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/MANIFEST.in
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     7584 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/PKG-INFO
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.990590 Quart-Kroket-1.0.7/Quart_Kroket.egg-info/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     7584 2023-08-05 16:25:07.000000 Quart-Kroket-1.0.7/Quart_Kroket.egg-info/PKG-INFO
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1455 2023-08-05 16:25:07.000000 Quart-Kroket-1.0.7/Quart_Kroket.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)        1 2023-08-05 16:25:07.000000 Quart-Kroket-1.0.7/Quart_Kroket.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)        1 2023-08-05 16:25:07.000000 Quart-Kroket-1.0.7/Quart_Kroket.egg-info/not-zip-safe
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      489 2023-08-05 16:25:07.000000 Quart-Kroket-1.0.7/Quart_Kroket.egg-info/requires.txt
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)       13 2023-08-05 16:25:07.000000 Quart-Kroket-1.0.7/Quart_Kroket.egg-info/top_level.txt
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     6847 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/README.md
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.990590 Quart-Kroket-1.0.7/quart_kroket/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     6125 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/__init__.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.990590 Quart-Kroket-1.0.7/quart_kroket/data/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/data/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1089 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/data/checksum.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1471 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/data/structures.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.990590 Quart-Kroket-1.0.7/quart_kroket/database/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1112 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/database/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     2615 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/database/enums.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      984 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/database/model.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.990590 Quart-Kroket-1.0.7/quart_kroket/email/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1484 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/email/__init__.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.990590 Quart-Kroket-1.0.7/quart_kroket/email/mjml/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1286 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/email/mjml/__init__.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/email/mjml/templates/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1298 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/email/mjml/templates/basic.jinja2
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/finance/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/finance/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1541 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/finance/validation.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/imaging/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)   340712 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/imaging/DejaVuSansMono.ttf
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      272 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/imaging/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     4307 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/imaging/avatars.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1443 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/imaging/captchav2.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     8016 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/imaging/imaging.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     2464 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/imaging/qr.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     3161 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/imaging/routes.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/localization/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/localization/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)    10427 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/localization/countries.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/markup/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/markup/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     8609 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/markup/markdown.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/media/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      342 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/media/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      169 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/media/constants.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)    10026 2023-08-05 16:23:50.000000 Quart-Kroket-1.0.7/quart_kroket/media/enums.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     2471 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/media/youtube.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/net/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      161 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/net/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     4419 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/net/ftp.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      846 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/net/gravatar.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)   694041 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/net/http_agents.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1266 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/net/http_requests.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/oidc/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/oidc/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1893 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/oidc/models.py
+drwxrwxr-x   0 dsc       (1000) dsc       (1000)        0 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/quart_kroket/pdf/
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1496 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/pdf/__init__.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      694 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/template_filters.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1541 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/quart_kroket/utils.py
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)      465 2023-08-05 16:23:37.000000 Quart-Kroket-1.0.7/requirements.txt
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)       61 2023-08-05 16:25:07.994590 Quart-Kroket-1.0.7/setup.cfg
+-rw-rw-r--   0 dsc       (1000) dsc       (1000)     1246 2023-08-05 16:24:01.000000 Quart-Kroket-1.0.7/setup.py
```

### Comparing `Quart-Kroket-1.0.6/LICENSE` & `Quart-Kroket-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/PKG-INFO` & `Quart-Kroket-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quart-Kroket
-Version: 1.0.6
+Version: 1.0.7
 Summary: zZzZ
 Home-page: https://git.kroket.io/labs/quart-kroket
 Author: Kroket Ltd.
 Author-email: code@kroket.io
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Quart-Kroket-1.0.6/Quart_Kroket.egg-info/PKG-INFO` & `Quart-Kroket-1.0.7/Quart_Kroket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quart-Kroket
-Version: 1.0.6
+Version: 1.0.7
 Summary: zZzZ
 Home-page: https://git.kroket.io/labs/quart-kroket
 Author: Kroket Ltd.
 Author-email: code@kroket.io
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Quart-Kroket-1.0.6/Quart_Kroket.egg-info/SOURCES.txt` & `Quart-Kroket-1.0.7/Quart_Kroket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/README.md` & `Quart-Kroket-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/__init__.py` & `Quart-Kroket-1.0.7/quart_kroket/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/data/checksum.py` & `Quart-Kroket-1.0.7/quart_kroket/data/checksum.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/data/structures.py` & `Quart-Kroket-1.0.7/quart_kroket/data/structures.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/database/__init__.py` & `Quart-Kroket-1.0.7/quart_kroket/database/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/database/enums.py` & `Quart-Kroket-1.0.7/quart_kroket/database/enums.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/database/model.py` & `Quart-Kroket-1.0.7/quart_kroket/database/model.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/email/__init__.py` & `Quart-Kroket-1.0.7/quart_kroket/email/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/email/mjml/__init__.py` & `Quart-Kroket-1.0.7/quart_kroket/email/mjml/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/email/mjml/templates/basic.jinja2` & `Quart-Kroket-1.0.7/quart_kroket/email/mjml/templates/basic.jinja2`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/finance/validation.py` & `Quart-Kroket-1.0.7/quart_kroket/finance/validation.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/imaging/DejaVuSansMono.ttf` & `Quart-Kroket-1.0.7/quart_kroket/imaging/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/imaging/avatars.py` & `Quart-Kroket-1.0.7/quart_kroket/imaging/avatars.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/imaging/captchav2.py` & `Quart-Kroket-1.0.7/quart_kroket/imaging/captchav2.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/imaging/imaging.py` & `Quart-Kroket-1.0.7/quart_kroket/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/imaging/qr.py` & `Quart-Kroket-1.0.7/quart_kroket/imaging/qr.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/imaging/routes.py` & `Quart-Kroket-1.0.7/quart_kroket/imaging/routes.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/localization/countries.py` & `Quart-Kroket-1.0.7/quart_kroket/localization/countries.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/markup/markdown.py` & `Quart-Kroket-1.0.7/quart_kroket/markup/markdown.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/media/enums.py` & `Quart-Kroket-1.0.7/quart_kroket/media/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from dataclasses import dataclass
 from io import BytesIO
 
 import exiftool
 from quart_kroket.data.checksum import md5_string
 from quart_kroket.media import proportional_scale
 from slugify import slugify
-from wfs.db.utils import ts_vectorize
 from quart_kroket.data.checksum import md5_string
 
 
 import magic
 import mutagen
 import ffmpeg
```

### Comparing `Quart-Kroket-1.0.6/quart_kroket/media/youtube.py` & `Quart-Kroket-1.0.7/quart_kroket/media/youtube.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/net/ftp.py` & `Quart-Kroket-1.0.7/quart_kroket/net/ftp.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/net/gravatar.py` & `Quart-Kroket-1.0.7/quart_kroket/net/gravatar.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/net/http_agents.py` & `Quart-Kroket-1.0.7/quart_kroket/net/http_agents.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/net/http_requests.py` & `Quart-Kroket-1.0.7/quart_kroket/net/http_requests.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/oidc/models.py` & `Quart-Kroket-1.0.7/quart_kroket/oidc/models.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/pdf/__init__.py` & `Quart-Kroket-1.0.7/quart_kroket/pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/template_filters.py` & `Quart-Kroket-1.0.7/quart_kroket/template_filters.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/quart_kroket/utils.py` & `Quart-Kroket-1.0.7/quart_kroket/utils.py`

 * *Files identical despite different names*

### Comparing `Quart-Kroket-1.0.6/setup.py` & `Quart-Kroket-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 
 INSTALL_REQUIRES = open("requirements.txt").read().splitlines()
 
 setup(
     name='Quart-Kroket',
-    version='1.0.6',
+    version='1.0.7',
     url='https://git.kroket.io/labs/quart-kroket',
     author='Kroket Ltd.',
     author_email='code@kroket.io',
     description='zZzZ',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['quart_kroket'],
```

