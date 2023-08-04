# Comparing `tmp/django-iubenda-0.1.12.dev0.tar.gz` & `tmp/django-iubenda-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-0.1.12.dev0.tar", last modified: Sun Feb 26 10:49:17 2023, max compression
+gzip compressed data, was "django-iubenda-1.2.6.tar", last modified: Fri Aug  4 23:01:08 2023, max compression
```

## Comparing `django-iubenda-0.1.12.dev0.tar` & `django-iubenda-1.2.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.397651 django-iubenda-0.1.12.dev0/
--rw-rw-rw-   0        0        0      423 2023-02-26 10:49:11.000000 django-iubenda-0.1.12.dev0/.bumpversion.cfg
--rw-rw-rw-   0        0        0     1189 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      100 2021-11-12 13:28:56.000000 django-iubenda-0.1.12.dev0/CHANGELOG.rst
--rw-rw-rw-   0        0        0      134 2023-02-01 16:09:19.000000 django-iubenda-0.1.12.dev0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1134 2021-11-12 09:51:39.000000 django-iubenda-0.1.12.dev0/LICENSE
--rw-rw-rw-   0        0        0      336 2023-02-22 09:22:06.000000 django-iubenda-0.1.12.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     6508 2023-02-26 10:49:17.398627 django-iubenda-0.1.12.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     4931 2023-02-04 22:23:44.000000 django-iubenda-0.1.12.dev0/README.md
--rw-rw-rw-   0        0        0     1980 2023-02-01 16:09:18.000000 django-iubenda-0.1.12.dev0/mkdocs.yml
--rw-rw-rw-   0        0        0     1639 2023-02-26 10:49:11.000000 django-iubenda-0.1.12.dev0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.204434 django-iubenda-0.1.12.dev0/requirements/
--rw-rw-rw-   0        0        0       58 2021-11-12 16:17:16.000000 django-iubenda-0.1.12.dev0/requirements/docs.in
--rw-rw-rw-   0        0        0    15726 2022-03-17 16:23:55.000000 django-iubenda-0.1.12.dev0/requirements/docs.txt
--rw-rw-rw-   0        0        0     7125 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py310-django32.txt
--rw-rw-rw-   0        0        0     6920 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py310-django40.txt
--rw-rw-rw-   0        0        0     7125 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py311-django32.txt
--rw-rw-rw-   0        0        0     6920 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py311-django40.txt
--rw-rw-rw-   0        0        0     7629 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py37-django22.txt
--rw-rw-rw-   0        0        0     7861 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py37-django32.txt
--rw-rw-rw-   0        0        0     7778 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py38-django22.txt
--rw-rw-rw-   0        0        0     7984 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py38-django32.txt
--rw-rw-rw-   0        0        0     9406 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py38-django40.txt
--rw-rw-rw-   0        0        0     7360 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py39-django22.txt
--rw-rw-rw-   0        0        0     7566 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py39-django32.txt
--rw-rw-rw-   0        0        0     7361 2022-12-20 21:47:14.000000 django-iubenda-0.1.12.dev0/requirements/py39-django40.txt
--rw-rw-rw-   0        0        0       83 2023-02-01 16:19:38.000000 django-iubenda-0.1.12.dev0/requirements/requirements.in
--rw-rw-rw-   0        0        0     1608 2021-11-15 15:50:56.000000 django-iubenda-0.1.12.dev0/runtests.py
--rw-rw-rw-   0        0        0     1966 2023-02-26 10:49:17.403506 django-iubenda-0.1.12.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-02-01 16:29:32.000000 django-iubenda-0.1.12.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.070744 django-iubenda-0.1.12.dev0/src/
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.239565 django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/
--rw-rw-rw-   0        0        0     6508 2023-02-26 10:49:16.000000 django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1591 2023-02-26 10:49:16.000000 django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 10:49:16.000000 django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-04 21:57:36.000000 django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2023-02-26 10:49:16.000000 django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-26 10:49:16.000000 django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.303970 django-iubenda-0.1.12.dev0/src/iubenda/
--rw-rw-rw-   0        0        0      433 2023-02-26 10:49:11.000000 django-iubenda-0.1.12.dev0/src/iubenda/__init__.py
--rw-rw-rw-   0        0        0      376 2022-05-02 20:53:17.000000 django-iubenda-0.1.12.dev0/src/iubenda/admin.py
--rw-rw-rw-   0        0        0      179 2023-01-16 17:00:40.000000 django-iubenda-0.1.12.dev0/src/iubenda/apps.py
--rw-rw-rw-   0        0        0     1455 2023-02-04 23:04:16.000000 django-iubenda-0.1.12.dev0/src/iubenda/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.307874 django-iubenda-0.1.12.dev0/src/iubenda/fixtures/
--rw-rw-rw-   0        0        0      275 2023-01-18 09:07:55.000000 django-iubenda-0.1.12.dev0/src/iubenda/fixtures/data.json
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.072697 django-iubenda-0.1.12.dev0/src/iubenda/locale/
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.072697 django-iubenda-0.1.12.dev0/src/iubenda/locale/it/
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.324463 django-iubenda-0.1.12.dev0/src/iubenda/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0      380 2023-02-04 21:57:40.000000 django-iubenda-0.1.12.dev0/src/iubenda/locale/it/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      966 2023-01-06 21:29:45.000000 django-iubenda-0.1.12.dev0/src/iubenda/locale/it/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.333246 django-iubenda-0.1.12.dev0/src/iubenda/migrations/
--rw-rw-rw-   0        0        0     1585 2023-01-16 17:00:40.000000 django-iubenda-0.1.12.dev0/src/iubenda/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2022-04-27 19:36:59.000000 django-iubenda-0.1.12.dev0/src/iubenda/migrations/__init__.py
--rw-rw-rw-   0        0        0      588 2022-04-27 19:35:55.000000 django-iubenda-0.1.12.dev0/src/iubenda/models.py
--rw-rw-rw-   0        0        0      501 2022-06-22 10:27:06.000000 django-iubenda-0.1.12.dev0/src/iubenda/sitemaps.py
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.074648 django-iubenda-0.1.12.dev0/src/iubenda/static/
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.074648 django-iubenda-0.1.12.dev0/src/iubenda/static/iubenda/
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.339101 django-iubenda-0.1.12.dev0/src/iubenda/static/iubenda/css/
--rw-rw-rw-   0        0        0     6020 2022-04-27 20:53:15.000000 django-iubenda-0.1.12.dev0/src/iubenda/static/iubenda/css/iubenda_badge.css
--rw-rw-rw-   0        0        0    42614 2022-04-27 21:25:48.000000 django-iubenda-0.1.12.dev0/src/iubenda/static/iubenda/css/iubenda_policy.css
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.075623 django-iubenda-0.1.12.dev0/src/iubenda/templates/
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.360570 django-iubenda-0.1.12.dev0/src/iubenda/templates/iubenda/
--rw-rw-rw-   0        0        0     1755 2023-02-26 10:48:58.000000 django-iubenda-0.1.12.dev0/src/iubenda/templates/iubenda/cookie.html
--rw-rw-rw-   0        0        0     1373 2023-02-04 23:25:52.000000 django-iubenda-0.1.12.dev0/src/iubenda/templates/iubenda/include-content.html
--rw-rw-rw-   0        0        0     1810 2023-02-26 10:48:58.000000 django-iubenda-0.1.12.dev0/src/iubenda/templates/iubenda/privacy.html
--rw-rw-rw-   0        0        0      211 2022-04-27 19:38:26.000000 django-iubenda-0.1.12.dev0/src/iubenda/translation.py
--rw-rw-rw-   0        0        0      907 2022-04-27 20:16:48.000000 django-iubenda-0.1.12.dev0/src/iubenda/urls.py
--rw-rw-rw-   0        0        0     2346 2023-02-04 22:44:49.000000 django-iubenda-0.1.12.dev0/src/iubenda/views.py
-drwxrwxrwx   0        0        0        0 2023-02-26 10:49:17.389844 django-iubenda-0.1.12.dev0/tests/
--rw-rw-rw-   0        0        0        0 2020-04-19 11:28:18.000000 django-iubenda-0.1.12.dev0/tests/__init__.py
--rw-rw-rw-   0        0        0      393 2023-02-04 22:09:32.000000 django-iubenda-0.1.12.dev0/tests/settings.py
--rw-rw-rw-   0        0        0      425 2023-02-04 22:09:32.000000 django-iubenda-0.1.12.dev0/tests/test_iubenda.py
--rw-rw-rw-   0        0        0       45 2023-02-04 22:09:32.000000 django-iubenda-0.1.12.dev0/tests/urls.py
--rw-rw-rw-   0        0        0       38 2023-02-04 22:09:32.000000 django-iubenda-0.1.12.dev0/tests/views.py
--rw-rw-rw-   0        0        0      930 2023-02-04 22:09:32.000000 django-iubenda-0.1.12.dev0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.712355 django-iubenda-1.2.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-04 23:01:08.720355 django-iubenda-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.712355 django-iubenda-1.2.6/src/django_iubenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/fixtures/data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/static/iubenda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/static/iubenda/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_badge.css
+-rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_policy.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/templates/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/cookie-compress.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/cookie.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/include-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy-compress.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/fixtures/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/test_iubenda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/test_iubenda_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/test_iubenda_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tox.ini
```

### Comparing `django-iubenda-0.1.12.dev0/LICENSE` & `django-iubenda-1.2.6/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2010-present DLRSP (https://dlrsp.org) and other contributors.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2010-present DLRSP (https://dlrsp.org) and other contributors.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `django-iubenda-0.1.12.dev0/PKG-INFO` & `django-iubenda-1.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,161 +1,204 @@
-Metadata-Version: 2.1
-Name: django-iubenda
-Version: 0.1.12.dev0
-Summary: Django application for handling privacy and cookie policies configured with Iubenda.
-Home-page: https://github.com/DLRSP/django-iubenda
-Author: DLRSP
-Author-email: dlrsp.dev@gmail.com
-License: MIT License
-Keywords: django,iubenda,privacy,cookie
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: linting
-License-File: LICENSE
-
-# django-iubenda [![PyPi license](https://img.shields.io/pypi/l/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-
-[![PyPi status](https://img.shields.io/pypi/status/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi version](https://img.shields.io/pypi/v/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi downloads](https://img.shields.io/pypi/dw/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi downloads](https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-
-## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-iubenda.svg)
-
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yml)
-
-## Compliance for websites and apps
-Click [here](http://iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda
-[![Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/dlrspapi)
-
-
-## Check Demo Project
-* Browser the demo app on-line on [Heroku](https://django-iubenda.herokuapp.com/)
-* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-iubenda)
-
-## Requirements
--   Python 3.7 to 3.10 supported.
--   Django 3.2 to 4.0 supported.
-
-## Setup
-1. Install from **pip**:
-```shell
-pip install django-iubenda
-```
-
-2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
-```python
-INSTALLED_APPS = (
-    "modeltranslation",
-    # ...
-    "iubenda",
-    # ...
-)
-```
-
-3. Modify `settings.py` by adding the app's context processor to `TEMPLATES`:
-```python
-TEMPLATES = [
-    {
-        # ...
-        'OPTIONS': {
-            'context_processors': [
-                # ...
-                'iubenda.context_processors.iubenda',
-                # ...
-            ],
-        },
-    },
-]
-```
-
-4. Be sure the Django's Locale middleware is enabled inside `settings.py`:
-```python
-MIDDLEWARE = (
-    # ...
-    'django.middleware.locale.LocaleMiddleware',
-    # ...
-)
-```
-
-5. Be sure the variable `LANGUAGE_CODE` is available for HTML templates:
-```html
-{% load i18n %}
-{% get_current_language as LANGUAGE_CODE %}
-```
-
-6. Modify your project's template to add privacy and cookie policies. 
-   For example inside the `footer.html` add following code:
-```html
-{% if not debug %}
-    {% block iubenda %}{% include "iubenda/include-content.html" %}{% endblock iubenda %}
-{% endif %}
-```
-
-## Optional
-
-### Content Security Policy
-If Content Security Policy are implemented in your server and inline scripts are disabled,
-the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
-```html
-<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
-```
-
-### Iubenda's Options
-To personalize the Iubenda script behaviour, the dict `IUBENDA_OPTIONS` can be configured inside `settings.py`
-```python
-IUBENDA_OPTIONS = {"ccpaAcknowledgeOnDisplay": "true",
-                   "ccpaApplies": "true",
-                   "consentOnContinuedBrowsing": "false",
-                   "enableCcpa": "true",
-                   "floatingPreferencesButtonDisplay": "bottom-left",
-                   "invalidateConsentWithoutLog": "true",
-                   "perPurposeConsent": "true",
-                   "whitelabel": "false",
-                   "banner": {
-                       "acceptButtonDisplay": "true",
-                       "backgroundOverlay": "true",
-                       "closeButtonRejects": "true",
-                       "customizeButtonDisplay": "true",
-                       "explicitWithdrawal": "true",
-                       "fontSize": "14px",
-                       "listPurposes": "true",
-                       "position": "float-center",
-                       "rejectButtonDisplay": "true"
-                   }
-                   }
-```
-
-## Run Example Project
-
-```shell
-git clone --depth=50 --branch=django-iubenda https://github.com/DLRSP/example.git DLRSP/example
-cd DLRSP/example
-python manage.py runserver
-```
-
-Now browser the app @ http://127.0.0.1:8000
+Metadata-Version: 2.1
+Name: django-iubenda
+Version: 1.2.6
+Summary: Django application for handling privacy and cookie policies configured with Iubenda.
+Home-page: https://github.com/DLRSP/django-iubenda
+Author: DLRSP
+Author-email: dlrsp.dev@gmail.com
+License: MIT License
+Keywords: django,iubenda,privacy,cookie
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: linting
+License-File: LICENSE
+
+# django-iubenda [![PyPi license](https://img.shields.io/pypi/l/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+
+[![PyPi status](https://img.shields.io/pypi/status/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi version](https://img.shields.io/pypi/v/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi downloads](https://img.shields.io/pypi/dw/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi downloads](https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+
+## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-iubenda.svg)
+
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
+
+## Compliance for websites and apps
+Click [here](http://iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda
+[![Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/dlrspapi)
+
+
+## Check Demo Project
+* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-iubenda)
+
+## Requirements
+-   Python +3.8 supported.
+-   Django +3.2 supported.
+
+## Setup
+1. Install from **pip**:
+```shell
+pip install django-iubenda
+```
+
+2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = (
+    "modeltranslation",
+    # ...
+    "iubenda",
+    # ...
+)
+```
+
+3. Modify `settings.py` by adding the app's context processor to `TEMPLATES`:
+```python
+TEMPLATES = [
+    {
+        # ...
+        "OPTIONS": {
+            "context_processors": [
+                # ...
+                "iubenda.context_processors.iubenda",
+                # ...
+            ],
+        },
+    },
+]
+```
+
+4. Be sure the Django's Locale middleware is enabled inside `settings.py`:
+```python
+MIDDLEWARE = (
+    # ...
+    "django.middleware.locale.LocaleMiddleware",
+    # ...
+)
+```
+
+5. Modify `url.py` by adding the app's urls to `urlpatterns`:
+```python
+urlpatterns += [
+    path("", include("iubenda.urls")),
+]
+```
+
+6. Modify `url.py` by adding the app's sitemaps to `sitemaps`:
+```python
+from iubenda.sitemaps import PrivacySitemap, CookieSitemap
+
+sitemaps = {
+    # ...
+    "privacy": PrivacySitemap,
+    "cookie": CookieSitemap,
+    # ...
+}
+```
+
+7. Be sure the variable `LANGUAGE_CODE` is available for HTML templates:
+```html
+{% load i18n %}
+{% get_current_language as LANGUAGE_CODE %}
+```
+
+8. Modify your project's template to add privacy and cookie policies.
+   For example inside the `footer.html` add following code:
+```html
+{% if not debug %}
+    {% block iubenda %}{% include "iubenda/include-content.html" %}{% endblock iubenda %}
+{% endif %}
+```
+
+## Optional
+
+### Content Security Policy
+If Content Security Policy are implemented in your server and inline scripts are disabled,
+the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
+```html
+<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
+```
+Inside your webserver's configurations, a rule to dynamically replace your CONSTANT nonce in a random string is needed.
+
+To allow  external source from Iubenda domains, please implement these rules:
+```editorconfig
+Content-Security-Policy:
+    script-src-elem https://*.iubenda.com";
+    img-src https://*.iubenda.com data:";
+    style-src https://*.iubenda.com";
+    connect-src https://*.iubenda.com";
+    frame-src https://*.iubenda.com";
+```
+
+If you prefer to not allow ***unsafe-inline*** inside your CSP, please also add the two specific hash for your
+script prompted as error in Javascript Console.
+```editorconfig
+# Iubenda Privacy And Cookie Policy - API
+Content-Security-Policy:
+    ...
+    script-src-elem https://*.iubenda.com 'sha256-YOUR-FIRST-HASH-PROMPTED-INSIDE-CONSOLE' 'sha256-YOUR-SECOND-HASH-PROMPTED-INSIDE-CONSOLE';
+    ...
+```
+
+Check this article from [Iubenda help](https://www.iubenda.com/it/help/12347-come-configurare-il-content-security-policy-per-consentire-lesecuzione-degli-script-di-iubenda)
+
+### Iubenda's Options
+(To-Do: new feuture)
+
+To personalize the Iubenda script behaviour, the dict `IUBENDA_OPTIONS` can be configured inside `settings.py`
+```python
+IUBENDA_OPTIONS = {
+    "ccpaAcknowledgeOnDisplay": "true",
+    "ccpaApplies": "true",
+    "consentOnContinuedBrowsing": "false",
+    "enableCcpa": "true",
+    "floatingPreferencesButtonDisplay": "bottom-left",
+    "invalidateConsentWithoutLog": "true",
+    "perPurposeConsent": "true",
+    "whitelabel": "false",
+    "banner": {
+        "acceptButtonDisplay": "true",
+        "backgroundOverlay": "true",
+        "closeButtonRejects": "true",
+        "customizeButtonDisplay": "true",
+        "explicitWithdrawal": "true",
+        "fontSize": "14px",
+        "listPurposes": "true",
+        "position": "float-center",
+        "rejectButtonDisplay": "true",
+    },
+}
+```
+
+## Run Example Project
+
+```shell
+git clone --depth=50 --branch=django-iubenda https://github.com/DLRSP/example.git DLRSP/example
+cd DLRSP/example
+python manage.py runserver
+```
+
+Now browser the app @ http://127.0.0.1:8000
```

### Comparing `django-iubenda-0.1.12.dev0/requirements/docs.txt` & `django-iubenda-1.2.6/requirements/py39-django32.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,231 +1,291 @@
-#
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
-#
-#    pip-compile --allow-unsafe --generate-hashes --output-file=docs.txt docs.in
-#
-click==8.0.3 \
-    --hash=sha256:353f466495adaeb40b6b5f592f9f91cb22372351c84caeb068132442a4518ef3 \
-    --hash=sha256:410e932b050f5eed773c4cda94de75971c89cdb3155a72a0831139a79e5ecb5b
-    # via mkdocs
-ghp-import==2.0.2 \
-    --hash=sha256:5f8962b30b20652cdffa9c5a9812f7de6bcb56ec475acac579807719bf242c46 \
-    --hash=sha256:947b3771f11be850c852c64b561c600fdddf794bab363060854c1ee7ad05e071
-    # via mkdocs
-gitdb==4.0.9 \
-    --hash=sha256:8033ad4e853066ba6ca92050b9df2f89301b8fc8bf7e9324d412a63f8bf1a8fd \
-    --hash=sha256:bac2fd45c0a1c9cf619e63a90d62bdc63892ef92387424b855792a6cabe789aa
-    # via gitpython
-gitpython==3.1.24 \
-    --hash=sha256:dc0a7f2f697657acc8d7f89033e8b1ea94dd90356b2983bca89dc8d2ab3cc647 \
-    --hash=sha256:df83fdf5e684fef7c6ee2c02fc68a5ceb7e7e759d08b694088d0cacb4eba59e5
-    # via mkdocs-git-revision-date-plugin
-importlib-metadata==4.8.2 \
-    --hash=sha256:53ccfd5c134223e497627b9815d5030edf77d2ed573922f7a0b8f8bb81a1c100 \
-    --hash=sha256:75bdec14c397f528724c1bfd9709d660b33a4d2e77387a3358f20b848bb5e5fb
-    # via mkdocs
-jinja2==3.0.3 \
-    --hash=sha256:077ce6014f7b40d03b47d1f1ca4b0fc8328a692bd284016f806ed0eaca390ad8 \
-    --hash=sha256:611bb273cd68f3b993fabdc4064fc858c5b47a973cb5aa7999ec1ba405c87cd7
-    # via
-    #   mkdocs
-    #   mkdocs-git-revision-date-plugin
-    #   mkdocs-material
-markdown==3.3.4 \
-    --hash=sha256:31b5b491868dcc87d6c24b7e3d19a0d730d59d3e46f4eea6430a321bed387a49 \
-    --hash=sha256:96c3ba1261de2f7547b46a00ea8463832c921d3f9d6aba3f255a6f71386db20c
-    # via
-    #   mkdocs
-    #   mkdocs-material
-    #   pymdown-extensions
-markupsafe==2.0.1 \
-    --hash=sha256:01a9b8ea66f1658938f65b93a85ebe8bc016e6769611be228d797c9d998dd298 \
-    --hash=sha256:023cb26ec21ece8dc3907c0e8320058b2e0cb3c55cf9564da612bc325bed5e64 \
-    --hash=sha256:0446679737af14f45767963a1a9ef7620189912317d095f2d9ffa183a4d25d2b \
-    --hash=sha256:04635854b943835a6ea959e948d19dcd311762c5c0c6e1f0e16ee57022669194 \
-    --hash=sha256:0717a7390a68be14b8c793ba258e075c6f4ca819f15edfc2a3a027c823718567 \
-    --hash=sha256:0955295dd5eec6cb6cc2fe1698f4c6d84af2e92de33fbcac4111913cd100a6ff \
-    --hash=sha256:0d4b31cc67ab36e3392bbf3862cfbadac3db12bdd8b02a2731f509ed5b829724 \
-    --hash=sha256:10f82115e21dc0dfec9ab5c0223652f7197feb168c940f3ef61563fc2d6beb74 \
-    --hash=sha256:168cd0a3642de83558a5153c8bd34f175a9a6e7f6dc6384b9655d2697312a646 \
-    --hash=sha256:1d609f577dc6e1aa17d746f8bd3c31aa4d258f4070d61b2aa5c4166c1539de35 \
-    --hash=sha256:1f2ade76b9903f39aa442b4aadd2177decb66525062db244b35d71d0ee8599b6 \
-    --hash=sha256:20dca64a3ef2d6e4d5d615a3fd418ad3bde77a47ec8a23d984a12b5b4c74491a \
-    --hash=sha256:2a7d351cbd8cfeb19ca00de495e224dea7e7d919659c2841bbb7f420ad03e2d6 \
-    --hash=sha256:2d7d807855b419fc2ed3e631034685db6079889a1f01d5d9dac950f764da3dad \
-    --hash=sha256:2ef54abee730b502252bcdf31b10dacb0a416229b72c18b19e24a4509f273d26 \
-    --hash=sha256:36bc903cbb393720fad60fc28c10de6acf10dc6cc883f3e24ee4012371399a38 \
-    --hash=sha256:37205cac2a79194e3750b0af2a5720d95f786a55ce7df90c3af697bfa100eaac \
-    --hash=sha256:3c112550557578c26af18a1ccc9e090bfe03832ae994343cfdacd287db6a6ae7 \
-    --hash=sha256:3dd007d54ee88b46be476e293f48c85048603f5f516008bee124ddd891398ed6 \
-    --hash=sha256:4296f2b1ce8c86a6aea78613c34bb1a672ea0e3de9c6ba08a960efe0b0a09047 \
-    --hash=sha256:47ab1e7b91c098ab893b828deafa1203de86d0bc6ab587b160f78fe6c4011f75 \
-    --hash=sha256:49e3ceeabbfb9d66c3aef5af3a60cc43b85c33df25ce03d0031a608b0a8b2e3f \
-    --hash=sha256:4dc8f9fb58f7364b63fd9f85013b780ef83c11857ae79f2feda41e270468dd9b \
-    --hash=sha256:4efca8f86c54b22348a5467704e3fec767b2db12fc39c6d963168ab1d3fc9135 \
-    --hash=sha256:53edb4da6925ad13c07b6d26c2a852bd81e364f95301c66e930ab2aef5b5ddd8 \
-    --hash=sha256:5855f8438a7d1d458206a2466bf82b0f104a3724bf96a1c781ab731e4201731a \
-    --hash=sha256:594c67807fb16238b30c44bdf74f36c02cdf22d1c8cda91ef8a0ed8dabf5620a \
-    --hash=sha256:5b6d930f030f8ed98e3e6c98ffa0652bdb82601e7a016ec2ab5d7ff23baa78d1 \
-    --hash=sha256:5bb28c636d87e840583ee3adeb78172efc47c8b26127267f54a9c0ec251d41a9 \
-    --hash=sha256:60bf42e36abfaf9aff1f50f52644b336d4f0a3fd6d8a60ca0d054ac9f713a864 \
-    --hash=sha256:611d1ad9a4288cf3e3c16014564df047fe08410e628f89805e475368bd304914 \
-    --hash=sha256:6300b8454aa6930a24b9618fbb54b5a68135092bc666f7b06901f897fa5c2fee \
-    --hash=sha256:63f3268ba69ace99cab4e3e3b5840b03340efed0948ab8f78d2fd87ee5442a4f \
-    --hash=sha256:6557b31b5e2c9ddf0de32a691f2312a32f77cd7681d8af66c2692efdbef84c18 \
-    --hash=sha256:693ce3f9e70a6cf7d2fb9e6c9d8b204b6b39897a2c4a1aa65728d5ac97dcc1d8 \
-    --hash=sha256:6a7fae0dd14cf60ad5ff42baa2e95727c3d81ded453457771d02b7d2b3f9c0c2 \
-    --hash=sha256:6c4ca60fa24e85fe25b912b01e62cb969d69a23a5d5867682dd3e80b5b02581d \
-    --hash=sha256:6fcf051089389abe060c9cd7caa212c707e58153afa2c649f00346ce6d260f1b \
-    --hash=sha256:7d91275b0245b1da4d4cfa07e0faedd5b0812efc15b702576d103293e252af1b \
-    --hash=sha256:89c687013cb1cd489a0f0ac24febe8c7a666e6e221b783e53ac50ebf68e45d86 \
-    --hash=sha256:8d206346619592c6200148b01a2142798c989edcb9c896f9ac9722a99d4e77e6 \
-    --hash=sha256:905fec760bd2fa1388bb5b489ee8ee5f7291d692638ea5f67982d968366bef9f \
-    --hash=sha256:97383d78eb34da7e1fa37dd273c20ad4320929af65d156e35a5e2d89566d9dfb \
-    --hash=sha256:984d76483eb32f1bcb536dc27e4ad56bba4baa70be32fa87152832cdd9db0833 \
-    --hash=sha256:99df47edb6bda1249d3e80fdabb1dab8c08ef3975f69aed437cb69d0a5de1e28 \
-    --hash=sha256:9f02365d4e99430a12647f09b6cc8bab61a6564363f313126f775eb4f6ef798e \
-    --hash=sha256:a30e67a65b53ea0a5e62fe23682cfe22712e01f453b95233b25502f7c61cb415 \
-    --hash=sha256:ab3ef638ace319fa26553db0624c4699e31a28bb2a835c5faca8f8acf6a5a902 \
-    --hash=sha256:aca6377c0cb8a8253e493c6b451565ac77e98c2951c45f913e0b52facdcff83f \
-    --hash=sha256:add36cb2dbb8b736611303cd3bfcee00afd96471b09cda130da3581cbdc56a6d \
-    --hash=sha256:b2f4bf27480f5e5e8ce285a8c8fd176c0b03e93dcc6646477d4630e83440c6a9 \
-    --hash=sha256:b7f2d075102dc8c794cbde1947378051c4e5180d52d276987b8d28a3bd58c17d \
-    --hash=sha256:baa1a4e8f868845af802979fcdbf0bb11f94f1cb7ced4c4b8a351bb60d108145 \
-    --hash=sha256:be98f628055368795d818ebf93da628541e10b75b41c559fdf36d104c5787066 \
-    --hash=sha256:bf5d821ffabf0ef3533c39c518f3357b171a1651c1ff6827325e4489b0e46c3c \
-    --hash=sha256:c47adbc92fc1bb2b3274c4b3a43ae0e4573d9fbff4f54cd484555edbf030baf1 \
-    --hash=sha256:cdfba22ea2f0029c9261a4bd07e830a8da012291fbe44dc794e488b6c9bb353a \
-    --hash=sha256:d6c7ebd4e944c85e2c3421e612a7057a2f48d478d79e61800d81468a8d842207 \
-    --hash=sha256:d7f9850398e85aba693bb640262d3611788b1f29a79f0c93c565694658f4071f \
-    --hash=sha256:d8446c54dc28c01e5a2dbac5a25f071f6653e6e40f3a8818e8b45d790fe6ef53 \
-    --hash=sha256:deb993cacb280823246a026e3b2d81c493c53de6acfd5e6bfe31ab3402bb37dd \
-    --hash=sha256:e0f138900af21926a02425cf736db95be9f4af72ba1bb21453432a07f6082134 \
-    --hash=sha256:e9936f0b261d4df76ad22f8fee3ae83b60d7c3e871292cd42f40b81b70afae85 \
-    --hash=sha256:f0567c4dc99f264f49fe27da5f735f414c4e7e7dd850cfd8e69f0862d7c74ea9 \
-    --hash=sha256:f5653a225f31e113b152e56f154ccbe59eeb1c7487b39b9d9f9cdb58e6c79dc5 \
-    --hash=sha256:f826e31d18b516f653fe296d967d700fddad5901ae07c622bb3705955e1faa94 \
-    --hash=sha256:f8ba0e8349a38d3001fae7eadded3f6606f0da5d748ee53cc1dab1d6527b9509 \
-    --hash=sha256:f9081981fe268bd86831e5c75f7de206ef275defcb82bc70740ae6dc507aee51 \
-    --hash=sha256:fa130dd50c57d53368c9d59395cb5526eda596d3ffe36666cd81a44d56e48872
-    # via jinja2
-mergedeep==1.3.4 \
-    --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
-    --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
-    # via mkdocs
-mkdocs==1.2.3 \
-    --hash=sha256:89f5a094764381cda656af4298727c9f53dc3e602983087e1fe96ea1df24f4c1 \
-    --hash=sha256:a1fa8c2d0c1305d7fc2b9d9f607c71778572a8b110fb26642aa00296c9e6d072
-    # via
-    #   -r requirements/docs.in
-    #   mkdocs-git-revision-date-plugin
-    #   mkdocs-material
-mkdocs-git-revision-date-plugin==0.3.2 \
-    --hash=sha256:2e67956cb01823dd2418e2833f3623dee8604cdf223bddd005fe36226a56f6ef
-    # via -r requirements/docs.in
-mkdocs-material==8.2.5 \
-    --hash=sha256:95283c6af633809f32ba688fcf9bce4604af320e188d3e26fcb40d0e5ab9b823 \
-    --hash=sha256:cdfb39edc77f5c2bbfca02b4fc3764de38b2093eff121aed37674204439901ce
-    # via -r requirements/docs.in
-mkdocs-material-extensions==1.0.3 \
-    --hash=sha256:a82b70e533ce060b2a5d9eb2bc2e1be201cf61f901f93704b4acf6e3d5983a44 \
-    --hash=sha256:bfd24dfdef7b41c312ede42648f9eb83476ea168ec163b613f9abd12bbfddba2
-    # via mkdocs-material
-packaging==21.2 \
-    --hash=sha256:096d689d78ca690e4cd8a89568ba06d07ca097e3306a4381635073ca91479966 \
-    --hash=sha256:14317396d1e8cdb122989b916fa2c7e9ca8e2be9e8060a6eff75b6b7b4d8a7e0
-    # via mkdocs
-pygments==2.10.0 \
-    --hash=sha256:b8e67fe6af78f492b3c4b3e2970c0624cbf08beb1e493b2c99b9fa1b67a20380 \
-    --hash=sha256:f398865f7eb6874156579fdf36bc840a03cab64d1cde9e93d68f46a425ec52c6
-    # via mkdocs-material
-pymdown-extensions==9.0 \
-    --hash=sha256:01e4bec7f4b16beaba0087a74496401cf11afd69e3a11fe95cb593e5c698ef40 \
-    --hash=sha256:430cc2fbb30cef2df70edac0b4f62614a6a4d2b06462e32da4ca96098b7c1dfb
-    # via mkdocs-material
-pyparsing==2.4.7 \
-    --hash=sha256:c203ec8783bf771a155b207279b9bccb8dea02d8f0c9e5f8ead507bc3246ecc1 \
-    --hash=sha256:ef9d7589ef3c200abe66653d3f1ab1033c3c419ae9b9bdb1240a85b024efc88b
-    # via packaging
-python-dateutil==2.8.2 \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-    # via ghp-import
-pyyaml==6.0 \
-    --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
-    --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
-    --hash=sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57 \
-    --hash=sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b \
-    --hash=sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4 \
-    --hash=sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07 \
-    --hash=sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba \
-    --hash=sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9 \
-    --hash=sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287 \
-    --hash=sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513 \
-    --hash=sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0 \
-    --hash=sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0 \
-    --hash=sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92 \
-    --hash=sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f \
-    --hash=sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2 \
-    --hash=sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc \
-    --hash=sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c \
-    --hash=sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86 \
-    --hash=sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4 \
-    --hash=sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c \
-    --hash=sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34 \
-    --hash=sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b \
-    --hash=sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c \
-    --hash=sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb \
-    --hash=sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737 \
-    --hash=sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3 \
-    --hash=sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d \
-    --hash=sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53 \
-    --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
-    --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
-    --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
-    --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
-    --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
-    # via
-    #   mkdocs
-    #   pyyaml-env-tag
-pyyaml-env-tag==0.1 \
-    --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
-    --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
-    # via mkdocs
-six==1.16.0 \
-    --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
-    --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-    # via python-dateutil
-smmap==5.0.0 \
-    --hash=sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94 \
-    --hash=sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936
-    # via gitdb
-watchdog==2.1.6 \
-    --hash=sha256:25fb5240b195d17de949588628fdf93032ebf163524ef08933db0ea1f99bd685 \
-    --hash=sha256:3386b367e950a11b0568062b70cc026c6f645428a698d33d39e013aaeda4cc04 \
-    --hash=sha256:3becdb380d8916c873ad512f1701f8a92ce79ec6978ffde92919fd18d41da7fb \
-    --hash=sha256:4ae38bf8ba6f39d5b83f78661273216e7db5b00f08be7592062cb1fc8b8ba542 \
-    --hash=sha256:8047da932432aa32c515ec1447ea79ce578d0559362ca3605f8e9568f844e3c6 \
-    --hash=sha256:8f1c00aa35f504197561060ca4c21d3cc079ba29cf6dd2fe61024c70160c990b \
-    --hash=sha256:922a69fa533cb0c793b483becaaa0845f655151e7256ec73630a1b2e9ebcb660 \
-    --hash=sha256:9693f35162dc6208d10b10ddf0458cc09ad70c30ba689d9206e02cd836ce28a3 \
-    --hash=sha256:a0f1c7edf116a12f7245be06120b1852275f9506a7d90227648b250755a03923 \
-    --hash=sha256:a36e75df6c767cbf46f61a91c70b3ba71811dfa0aca4a324d9407a06a8b7a2e7 \
-    --hash=sha256:aba5c812f8ee8a3ff3be51887ca2d55fb8e268439ed44110d3846e4229eb0e8b \
-    --hash=sha256:ad6f1796e37db2223d2a3f302f586f74c72c630b48a9872c1e7ae8e92e0ab669 \
-    --hash=sha256:ae67501c95606072aafa865b6ed47343ac6484472a2f95490ba151f6347acfc2 \
-    --hash=sha256:b2fcf9402fde2672545b139694284dc3b665fd1be660d73eca6805197ef776a3 \
-    --hash=sha256:b52b88021b9541a60531142b0a451baca08d28b74a723d0c99b13c8c8d48d604 \
-    --hash=sha256:b7d336912853d7b77f9b2c24eeed6a5065d0a0cc0d3b6a5a45ad6d1d05fb8cd8 \
-    --hash=sha256:bd9ba4f332cf57b2c1f698be0728c020399ef3040577cde2939f2e045b39c1e5 \
-    --hash=sha256:be9be735f827820a06340dff2ddea1fb7234561fa5e6300a62fe7f54d40546a0 \
-    --hash=sha256:cca7741c0fcc765568350cb139e92b7f9f3c9a08c4f32591d18ab0a6ac9e71b6 \
-    --hash=sha256:d0d19fb2441947b58fbf91336638c2b9f4cc98e05e1045404d7a4cb7cddc7a65 \
-    --hash=sha256:e02794ac791662a5eafc6ffeaf9bcc149035a0e48eb0a9d40a8feb4622605a3d \
-    --hash=sha256:e0f30db709c939cabf64a6dc5babb276e6d823fd84464ab916f9b9ba5623ca15 \
-    --hash=sha256:e92c2d33858c8f560671b448205a268096e17870dcf60a9bb3ac7bfbafb7f5f9
-    # via mkdocs
-zipp==3.6.0 \
-    --hash=sha256:71c644c5369f4a6e07636f0aa966270449561fcea2e3d6747b8d23efaa9d7832 \
-    --hash=sha256:9fe5ea21568a0a70e50f273397638d39b03353731e6cbbb3fd8502a33fec40bc
-    # via importlib-metadata
+#
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
+#
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
+#
+asgiref==3.7.2 \
+    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
+    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+    # via django
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
+    # via requests
+charset-normalizer==3.2.0 \
+    --hash=sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96 \
+    --hash=sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c \
+    --hash=sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710 \
+    --hash=sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706 \
+    --hash=sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020 \
+    --hash=sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252 \
+    --hash=sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad \
+    --hash=sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329 \
+    --hash=sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a \
+    --hash=sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f \
+    --hash=sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6 \
+    --hash=sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4 \
+    --hash=sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a \
+    --hash=sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46 \
+    --hash=sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2 \
+    --hash=sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23 \
+    --hash=sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace \
+    --hash=sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd \
+    --hash=sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982 \
+    --hash=sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10 \
+    --hash=sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2 \
+    --hash=sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea \
+    --hash=sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09 \
+    --hash=sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5 \
+    --hash=sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149 \
+    --hash=sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489 \
+    --hash=sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9 \
+    --hash=sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80 \
+    --hash=sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592 \
+    --hash=sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3 \
+    --hash=sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6 \
+    --hash=sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed \
+    --hash=sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c \
+    --hash=sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200 \
+    --hash=sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a \
+    --hash=sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e \
+    --hash=sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d \
+    --hash=sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6 \
+    --hash=sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623 \
+    --hash=sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669 \
+    --hash=sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3 \
+    --hash=sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa \
+    --hash=sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9 \
+    --hash=sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2 \
+    --hash=sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f \
+    --hash=sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1 \
+    --hash=sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4 \
+    --hash=sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a \
+    --hash=sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8 \
+    --hash=sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3 \
+    --hash=sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029 \
+    --hash=sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f \
+    --hash=sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959 \
+    --hash=sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22 \
+    --hash=sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7 \
+    --hash=sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952 \
+    --hash=sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346 \
+    --hash=sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e \
+    --hash=sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d \
+    --hash=sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299 \
+    --hash=sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd \
+    --hash=sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a \
+    --hash=sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3 \
+    --hash=sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037 \
+    --hash=sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94 \
+    --hash=sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c \
+    --hash=sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858 \
+    --hash=sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a \
+    --hash=sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449 \
+    --hash=sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c \
+    --hash=sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918 \
+    --hash=sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1 \
+    --hash=sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c \
+    --hash=sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac \
+    --hash=sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa
+    # via requests
+coverage==7.2.7 \
+    --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
+    --hash=sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2 \
+    --hash=sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a \
+    --hash=sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a \
+    --hash=sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01 \
+    --hash=sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6 \
+    --hash=sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7 \
+    --hash=sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f \
+    --hash=sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02 \
+    --hash=sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c \
+    --hash=sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063 \
+    --hash=sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a \
+    --hash=sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5 \
+    --hash=sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959 \
+    --hash=sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97 \
+    --hash=sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6 \
+    --hash=sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f \
+    --hash=sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9 \
+    --hash=sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5 \
+    --hash=sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f \
+    --hash=sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562 \
+    --hash=sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe \
+    --hash=sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9 \
+    --hash=sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f \
+    --hash=sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb \
+    --hash=sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb \
+    --hash=sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1 \
+    --hash=sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb \
+    --hash=sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250 \
+    --hash=sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e \
+    --hash=sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511 \
+    --hash=sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5 \
+    --hash=sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59 \
+    --hash=sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2 \
+    --hash=sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d \
+    --hash=sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3 \
+    --hash=sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4 \
+    --hash=sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de \
+    --hash=sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9 \
+    --hash=sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833 \
+    --hash=sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0 \
+    --hash=sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9 \
+    --hash=sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d \
+    --hash=sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050 \
+    --hash=sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d \
+    --hash=sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6 \
+    --hash=sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353 \
+    --hash=sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb \
+    --hash=sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e \
+    --hash=sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8 \
+    --hash=sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495 \
+    --hash=sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2 \
+    --hash=sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd \
+    --hash=sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27 \
+    --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
+    --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
+    --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
+    --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
+    --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
+    --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
+    # via -r requirements/requirements.in
+django==3.2.20 \
+    --hash=sha256:a477ab326ae7d8807dc25c186b951ab8c7648a3a23f9497763c37307a2b5ef87 \
+    --hash=sha256:dec2a116787b8e14962014bf78e120bba454135108e1af9e9b91ade7b2964c40
+    # via
+    #   -r requirements/requirements.in
+    #   django-appconf
+    #   django-modeltranslation
+django-appconf==1.0.5 \
+    --hash=sha256:ae9f864ee1958c815a965ed63b3fba4874eec13de10236ba063a788f9a17389d \
+    --hash=sha256:be3db0be6c81fa84742000b89a81c016d70ae66a7ccb620cdef592b1f1a6aaa4
+    # via django-compressor
+django-compressor==4.4 \
+    --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
+    --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
+    # via -r requirements/requirements.in
+django-modeltranslation==0.18.11 \
+    --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
+    --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
+    # via -r requirements/requirements.in
+exceptiongroup==1.1.2 \
+    --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
+    --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
+    # via pytest
+idna==3.4 \
+    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
+    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
+    # via requests
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
+    # via pytest-randomly
+iniconfig==2.0.0 \
+    --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
+    --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
+    # via pytest
+packaging==23.1 \
+    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
+    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
+    # via pytest
+pluggy==1.2.0 \
+    --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
+    --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
+    # via pytest
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
+    # via
+    #   -r requirements/requirements.in
+    #   pytest-django
+    #   pytest-randomly
+pytest-django==4.5.2 \
+    --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
+    --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
+    # via -r requirements/requirements.in
+pytest-randomly==3.13.0 \
+    --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
+    --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
+    # via -r requirements/requirements.in
+pytz==2023.3 \
+    --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
+    --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
+    # via django
+rcssmin==1.1.1 \
+    --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
+    --hash=sha256:35da6a6999e9e2c5b0e691b42ed56cc479373e0ecab33ef5277dfecce625e44a \
+    --hash=sha256:42576d95dfad53d77df2e68dfdec95b89b10fad320f241f1af3ca1438578254a \
+    --hash=sha256:4f9400b4366d29f5f5446f58e78549afa8338e6a59740c73115e9f6ac413dc64 \
+    --hash=sha256:705c9112d0ed54ea40aecf97e7fd29bdf0f1c46d278a32d8f957f31dde90778a \
+    --hash=sha256:79421230dd67c37ec61ed9892813d2b839b68f2f48ef55c75f976e81701d60b4 \
+    --hash=sha256:868215e1fd0e92a6122e0ed5973dfc7bb8330fe1e92274d05b2585253b38c0ca \
+    --hash=sha256:8a26fec3c1e6b7a3765ccbaccc20fbb5c0ed3422cc381e01a2607f08d7621c44 \
+    --hash=sha256:8fcfd10ae2a1c4ce231a33013f2539e07c3836bf17cc945cc25cc30bf8e68e45 \
+    --hash=sha256:908fe072efd2432fb0975a61124609a8e05021367f6a3463d45f5e3e74c4fdda \
+    --hash=sha256:914e589f40573035006913861ed2adc28fbe70082a8b6bff5be7ee430b7b5c2e \
+    --hash=sha256:a04d58a2a21e9a089306d3f99c4b12bf5b656a79c198ef2321e80f8fd9afab06 \
+    --hash=sha256:a417735d4023d47d048a6288c88dbceadd20abaaf65a11bb4fda1e8458057019 \
+    --hash=sha256:c30f8bc839747b6da59274e0c6e4361915d66532e26448d589cb2b1846d7bf11 \
+    --hash=sha256:c7278c1c25bb90d8e554df92cfb3b6a1195004ead50f764653d3093933ee0877 \
+    --hash=sha256:c7728e3b546b1b6ea08cab721e8e21409dbcc11b881d0b87d10b0be8930af2a2 \
+    --hash=sha256:cf74d7ea5e191f0f344b354eed8b7c83eeafbd9a97bec3a579c3d26edf11b005 \
+    --hash=sha256:d0afc6e7b64ef30d6dcde88830ec1a237b9f16a39f920a8fd159928684ccf8db \
+    --hash=sha256:d4e263fa9428704fd94c2cb565c7519ca1d225217943f71caffe6741ab5b9df1 \
+    --hash=sha256:e923c105100ab70abde1c01d3196ddd6b07255e32073685542be4e3a60870c8e \
+    --hash=sha256:ee386bec6d62f8c814d65c011d604a7c82d24aa3f718facd66e850eea8d6a5a1 \
+    --hash=sha256:f15673e97f0a68b4c378c4d15b088fe96d60bc106d278c88829923118833c20f \
+    --hash=sha256:f7a1fcdbafaacac0530da04edca4a44303baab430ea42e7d59aece4b3f3e9a51
+    # via django-compressor
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+    # via -r requirements/requirements.in
+rjsmin==1.2.1 \
+    --hash=sha256:113132a40ce7d03b2ced4fac215f0297338ed1c207394b739266efab7831988b \
+    --hash=sha256:122aa52bcf7ad9f12728d309012d1308c6ecfe4d6b09ea867a110dcad7b7728c \
+    --hash=sha256:145c6af8df42d8af102d0d39a6de2e5fa66aef9e38947cfb9d65377d1b9940b2 \
+    --hash=sha256:1f982be8e011438777a94307279b40134a3935fc0f079312ee299725b8af5411 \
+    --hash=sha256:3453ee6d5e7a2723ec45c2909e2382371783400e8d51952b692884c6d850a3d0 \
+    --hash=sha256:35827844d2085bd59d34214dfba6f1fc42a215c455887437b07dbf9c73019cc1 \
+    --hash=sha256:35f21046504544e2941e04190ce24161255479133751550e36ddb3f4af0ecdca \
+    --hash=sha256:5d67ec09da46a492186e35cabca02a0d092eda5ef5b408a419b99ee4acf28d5c \
+    --hash=sha256:747bc9d3bc8a220f40858e6aad50b2ae2eb7f69c924d4fa3803b81be1c1ddd02 \
+    --hash=sha256:7dd58b5ed88233bc61dc80b0ed87b93a1786031d9977c70d335221ef1ac5581a \
+    --hash=sha256:812af25c08d6a5ae98019a2e1b47ebb47f7469abd351670c353d619eaeae4064 \
+    --hash=sha256:8a6710e358c661dcdcfd027e67de3afd72a6af4c88101dcf110de39e9bbded39 \
+    --hash=sha256:8c340e251619c97571a5ade20f147f1f7e8664f66a2d6d7319e05e3ef6a4423c \
+    --hash=sha256:99c074cd6a8302ff47118a9c3d086f89328dc8e5c4b105aa1f348fb85c765a30 \
+    --hash=sha256:b8464629a18fe69f70677854c93a3707976024b226a0ce62707c618f923e1346 \
+    --hash=sha256:bbd7a0abaa394afd951f5d4e05249d306fec1c9674bfee179787674dddd0bdb7 \
+    --hash=sha256:bc5bc2f94e59bc81562c572b7f1bdd6bcec4f61168dc68a2993bad2d355b6e19 \
+    --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
+    --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
+    --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
+    --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
+    --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
+    --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
+    # via django-compressor
+sqlparse==0.4.4 \
+    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
+    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+    # via django
+tomli==2.0.1 \
+    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
+    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+    # via pytest
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
+    # via
+    #   asgiref
+    #   django-modeltranslation
+urllib3==2.0.4 \
+    --hash=sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11 \
+    --hash=sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4
+    # via requests
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
+    # via importlib-metadata
```

### Comparing `django-iubenda-0.1.12.dev0/runtests.py` & `django-iubenda-1.2.6/runtests.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import sys
-
-import pytest
-
-
-def split_class_and_function(string):
-    class_string, function_string = string.split(".", 1)
-    return f"{class_string} and {function_string}"
-
-
-def is_function(string):
-    # `True` if it looks like a test function is included in the string.
-    return string.startswith("test_") or ".test_" in string
-
-
-def is_class(string):
-    # `True` if first character is uppercase - assume it's a class name.
-    return string[0] == string[0].upper()
-
-
-if __name__ == "__main__":
-    if len(sys.argv) > 1:
-        pytest_args = sys.argv[1:]
-        first_arg = pytest_args[0]
-
-        try:
-            pytest_args.remove("--coverage")
-        except ValueError:
-            pass
-        else:
-            pytest_args = [
-                "--cov",
-                ".",
-                "--cov-report",
-                "xml",
-            ] + pytest_args
-
-        if first_arg.startswith("-"):
-            # `runtests.py [flags]`
-            pytest_args = ["tests"] + pytest_args
-        elif is_class(first_arg) and is_function(first_arg):
-            # `runtests.py TestCase.test_function [flags]`
-            expression = split_class_and_function(first_arg)
-            pytest_args = ["tests", "-k", expression] + pytest_args[1:]
-        elif is_class(first_arg) or is_function(first_arg):
-            # `runtests.py TestCase [flags]`
-            # `runtests.py test_function [flags]`
-            pytest_args = ["tests", "-k", pytest_args[0]] + pytest_args[1:]
-    else:
-        pytest_args = []
-
-    sys.exit(pytest.main(pytest_args))
+import sys
+
+import pytest
+
+
+def split_class_and_function(string):
+    class_string, function_string = string.split(".", 1)
+    return f"{class_string} and {function_string}"
+
+
+def is_function(string):
+    # `True` if it looks like a test function is included in the string.
+    return string.startswith("test_") or ".test_" in string
+
+
+def is_class(string):
+    # `True` if first character is uppercase - assume it's a class name.
+    return string[0] == string[0].upper()
+
+
+if __name__ == "__main__":
+    if len(sys.argv) > 1:
+        pytest_args = sys.argv[1:]
+        first_arg = pytest_args[0]
+
+        try:
+            pytest_args.remove("--coverage")
+        except ValueError:
+            pass
+        else:
+            pytest_args = [
+                "--cov",
+                ".",
+                "--cov-report",
+                "xml",
+            ] + pytest_args
+
+        if first_arg.startswith("-"):
+            # `runtests.py [flags]`
+            pytest_args = ["tests"] + pytest_args
+        elif is_class(first_arg) and is_function(first_arg):
+            # `runtests.py TestCase.test_function [flags]`
+            expression = split_class_and_function(first_arg)
+            pytest_args = ["tests", "-k", expression] + pytest_args[1:]
+        elif is_class(first_arg) or is_function(first_arg):
+            # `runtests.py TestCase [flags]`
+            # `runtests.py test_function [flags]`
+            pytest_args = ["tests", "-k", pytest_args[0]] + pytest_args[1:]
+    else:
+        pytest_args = []
+
+    sys.exit(pytest.main(pytest_args))
```

### Comparing `django-iubenda-0.1.12.dev0/setup.cfg` & `django-iubenda-1.2.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,115 @@
-00000000: 5b62 6469 7374 5f77 6865 656c 5d0d 0a75  [bdist_wheel]..u
-00000010: 6e69 7665 7273 616c 203d 2031 0d0a 0d0a  niversal = 1....
-00000020: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000030: 203d 2064 6a61 6e67 6f2d 6975 6265 6e64   = django-iubend
-00000040: 610d 0a76 6572 7369 6f6e 203d 2030 2e31  a..version = 0.1
-00000050: 2e31 322d 6465 760d 0a75 726c 203d 2068  .12-dev..url = h
-00000060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000070: 6d2f 444c 5253 502f 646a 616e 676f 2d69  m/DLRSP/django-i
-00000080: 7562 656e 6461 0d0a 6175 7468 6f72 203d  ubenda..author =
-00000090: 2044 4c52 5350 0d0a 6175 7468 6f72 5f65   DLRSP..author_e
-000000a0: 6d61 696c 203d 2064 6c72 7370 2e64 6576  mail = dlrsp.dev
-000000b0: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
-000000c0: 7269 7074 696f 6e20 3d20 446a 616e 676f  ription = Django
-000000d0: 2061 7070 6c69 6361 7469 6f6e 2066 6f72   application for
-000000e0: 2068 616e 646c 696e 6720 7072 6976 6163   handling privac
-000000f0: 7920 616e 6420 636f 6f6b 6965 2070 6f6c  y and cookie pol
-00000100: 6963 6965 7320 636f 6e66 6967 7572 6564  icies configured
-00000110: 2077 6974 6820 4975 6265 6e64 612e 0d0a   with Iubenda...
-00000120: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000130: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000140: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-00000150: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000160: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000170: 6e0d 0a6c 6963 656e 7365 203d 204d 4954  n..license = MIT
-00000180: 204c 6963 656e 7365 0d0a 6c69 6365 6e73   License..licens
-00000190: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
-000001a0: 450d 0a6b 6579 776f 7264 7320 3d20 0d0a  E..keywords = ..
-000001b0: 0964 6a61 6e67 6f0d 0a09 6975 6265 6e64  .django...iubend
-000001c0: 610d 0a09 7072 6976 6163 790d 0a09 636f  a...privacy...co
-000001d0: 6f6b 6965 0d0a 636c 6173 7369 6669 6572  okie..classifier
-000001e0: 7320 3d20 0d0a 0944 6576 656c 6f70 6d65  s = ...Developme
-000001f0: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
-00000200: 2042 6574 610d 0a09 456e 7669 726f 6e6d   Beta...Environm
-00000210: 656e 7420 3a3a 2057 6562 2045 6e76 6972  ent :: Web Envir
-00000220: 6f6e 6d65 6e74 0d0a 0946 7261 6d65 776f  onment...Framewo
-00000230: 726b 203a 3a20 446a 616e 676f 0d0a 0946  rk :: Django...F
+00000000: 5b62 6469 7374 5f77 6865 656c 5d0a 756e  [bdist_wheel].un
+00000010: 6976 6572 7361 6c20 3d20 310a 0a5b 6d65  iversal = 1..[me
+00000020: 7461 6461 7461 5d0a 6e61 6d65 203d 2064  tadata].name = d
+00000030: 6a61 6e67 6f2d 6975 6265 6e64 610a 7665  jango-iubenda.ve
+00000040: 7273 696f 6e20 3d20 312e 322e 360a 7572  rsion = 1.2.6.ur
+00000050: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000060: 7562 2e63 6f6d 2f44 4c52 5350 2f64 6a61  ub.com/DLRSP/dja
+00000070: 6e67 6f2d 6975 6265 6e64 610a 6175 7468  ngo-iubenda.auth
+00000080: 6f72 203d 2044 4c52 5350 0a61 7574 686f  or = DLRSP.autho
+00000090: 725f 656d 6169 6c20 3d20 646c 7273 702e  r_email = dlrsp.
+000000a0: 6465 7640 676d 6169 6c2e 636f 6d0a 6465  dev@gmail.com.de
+000000b0: 7363 7269 7074 696f 6e20 3d20 446a 616e  scription = Djan
+000000c0: 676f 2061 7070 6c69 6361 7469 6f6e 2066  go application f
+000000d0: 6f72 2068 616e 646c 696e 6720 7072 6976  or handling priv
+000000e0: 6163 7920 616e 6420 636f 6f6b 6965 2070  acy and cookie p
+000000f0: 6f6c 6963 6965 7320 636f 6e66 6967 7572  olicies configur
+00000100: 6564 2077 6974 6820 4975 6265 6e64 612e  ed with Iubenda.
+00000110: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000120: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+00000130: 2e6d 640a 6c6f 6e67 5f64 6573 6372 6970  .md.long_descrip
+00000140: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000150: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000160: 6e0a 6c69 6365 6e73 6520 3d20 4d49 5420  n.license = MIT 
+00000170: 4c69 6365 6e73 650a 6c69 6365 6e73 655f  License.license_
+00000180: 6669 6c65 7320 3d20 4c49 4345 4e53 450a  files = LICENSE.
+00000190: 6b65 7977 6f72 6473 203d 200a 0964 6a61  keywords = ..dja
+000001a0: 6e67 6f0a 0969 7562 656e 6461 0a09 7072  ngo..iubenda..pr
+000001b0: 6976 6163 790a 0963 6f6f 6b69 650a 636c  ivacy..cookie.cl
+000001c0: 6173 7369 6669 6572 7320 3d20 0a09 4465  assifiers = ..De
+000001d0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+000001e0: 203a 3a20 3420 2d20 4265 7461 0a09 456e   :: 4 - Beta..En
+000001f0: 7669 726f 6e6d 656e 7420 3a3a 2057 6562  vironment :: Web
+00000200: 2045 6e76 6972 6f6e 6d65 6e74 0a09 4672   Environment..Fr
+00000210: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
+00000220: 6f0a 0946 7261 6d65 776f 726b 203a 3a20  o..Framework :: 
+00000230: 446a 616e 676f 203a 3a20 332e 320a 0946  Django :: 3.2..F
 00000240: 7261 6d65 776f 726b 203a 3a20 446a 616e  ramework :: Djan
-00000250: 676f 203a 3a20 332e 320d 0a09 4672 616d  go :: 3.2...Fram
-00000260: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f20  ework :: Django 
-00000270: 3a3a 2034 2e30 0d0a 0949 6e74 656e 6465  :: 4.0...Intende
-00000280: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000290: 7665 6c6f 7065 7273 0d0a 094c 6963 656e  velopers...Licen
-000002a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-000002b0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-000002c0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-000002d0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000002e0: 656e 6465 6e74 0d0a 0950 726f 6772 616d  endent...Program
-000002f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000300: 2050 7974 686f 6e0d 0a09 5072 6f67 7261   Python...Progra
-00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000320: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-00000330: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000340: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000350: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
-00000360: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000370: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000380: 332e 370d 0a09 5072 6f67 7261 6d6d 696e  3.7...Programmin
-00000390: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003a0: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
-000003b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000003c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003d0: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
-000003e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003f0: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
-00000400: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000410: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000420: 2033 2e31 310d 0a09 4f70 6572 6174 696e   3.11...Operatin
-00000430: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000440: 6e64 6570 656e 6465 6e74 0d0a 0954 6f70  ndependent...Top
+00000250: 676f 203a 3a20 342e 300a 0949 6e74 656e  go :: 4.0..Inten
+00000260: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000270: 4465 7665 6c6f 7065 7273 0a09 4c69 6365  Developers..Lice
+00000280: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000290: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+000002a0: 7365 0a09 4f70 6572 6174 696e 6720 5379  se..Operating Sy
+000002b0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000002c0: 656e 6465 6e74 0a09 5072 6f67 7261 6d6d  endent..Programm
+000002d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002e0: 5079 7468 6f6e 0a09 5072 6f67 7261 6d6d  Python..Programm
+000002f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000300: 5079 7468 6f6e 203a 3a20 330a 0950 726f  Python :: 3..Pro
+00000310: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000320: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000330: 203a 3a20 4f6e 6c79 0a09 5072 6f67 7261   :: Only..Progra
+00000340: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000350: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+00000360: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000370: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000380: 3a3a 2033 2e39 0a09 5072 6f67 7261 6d6d  :: 3.9..Programm
+00000390: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003a0: 5079 7468 6f6e 203a 3a20 332e 3130 0a09  Python :: 3.10..
+000003b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003d0: 3a20 332e 3131 0a09 4f70 6572 6174 696e  : 3.11..Operatin
+000003e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+000003f0: 6e64 6570 656e 6465 6e74 0a09 546f 7069  ndependent..Topi
+00000400: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
+00000410: 2057 5757 2f48 5454 500a 0954 6f70 6963   WWW/HTTP..Topic
+00000420: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
+00000430: 5757 572f 4854 5450 203a 3a20 4479 6e61  WWW/HTTP :: Dyna
+00000440: 6d69 6320 436f 6e74 656e 740a 0954 6f70  mic Content..Top
 00000450: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000460: 3a20 5757 572f 4854 5450 0d0a 0954 6f70  : WWW/HTTP...Top
-00000470: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000480: 3a20 5757 572f 4854 5450 203a 3a20 4479  : WWW/HTTP :: Dy
-00000490: 6e61 6d69 6320 436f 6e74 656e 740d 0a09  namic Content...
-000004a0: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
-000004b0: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
-000004c0: 2057 5347 4920 3a3a 2041 7070 6c69 6361   WSGI :: Applica
-000004d0: 7469 6f6e 0d0a 0954 6f70 6963 203a 3a20  tion...Topic :: 
-000004e0: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-000004f0: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
-00000500: 7320 3a3a 2041 7070 6c69 6361 7469 6f6e  s :: Application
-00000510: 2046 7261 6d65 776f 726b 730d 0a09 546f   Frameworks...To
-00000520: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-00000530: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-00000540: 6962 7261 7269 6573 0d0a 0d0a 5b6f 7074  ibraries....[opt
-00000550: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-00000560: 6972 203d 200d 0a09 3d73 7263 0d0a 7365  ir = ...=src..se
-00000570: 7475 705f 7265 7175 6972 6573 203d 2044  tup_requires = D
-00000580: 6a61 6e67 6f3e 3d32 2e32 0d0a 696e 7374  jango>=2.2..inst
-00000590: 616c 6c5f 7265 7175 6972 6573 203d 2044  all_requires = D
-000005a0: 6a61 6e67 6f3e 3d32 2e32 0d0a 7061 636b  jango>=2.2..pack
-000005b0: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-000005c0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-000005d0: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
-000005e0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000005f0: 2e37 0d0a 7a69 705f 7361 6665 203d 2046  .7..zip_safe = F
-00000600: 616c 7365 0d0a 0d0a 5b6f 7074 696f 6e73  alse....[options
-00000610: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
-00000620: 0d0a 7465 7374 696e 6720 3d20 0d0a 0963  ..testing = ...c
-00000630: 6f76 6572 6167 650d 0a09 636f 6465 636f  overage...codeco
-00000640: 760d 0a6c 696e 7469 6e67 203d 200d 0a09  v..linting = ...
-00000650: 666c 616b 6538 0d0a 0970 796c 696e 740d  flake8...pylint.
-00000660: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000670: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-00000680: 6520 3d20 7372 630d 0a0d 0a5b 636f 7665  e = src....[cove
-00000690: 7261 6765 3a72 756e 5d0d 0a62 7261 6e63  rage:run]..branc
-000006a0: 6820 3d20 5472 7565 0d0a 736f 7572 6365  h = True..source
-000006b0: 203d 2064 6a61 6e67 6f5f 6572 726f 7273   = django_errors
-000006c0: 0d0a 0d0a 5b63 6f76 6572 6167 653a 7061  ....[coverage:pa
-000006d0: 7468 735d 0d0a 736f 7572 6365 203d 200d  ths]..source = .
-000006e0: 0a09 7372 630d 0a09 2e74 6f78 2f2a 2f73  ..src....tox/*/s
-000006f0: 6974 652d 7061 636b 6167 6573 0d0a 0d0a  ite-packages....
-00000700: 5b63 6f76 6572 6167 653a 7265 706f 7274  [coverage:report
-00000710: 5d0d 0a73 686f 775f 6d69 7373 696e 6720  ]..show_missing 
-00000720: 3d20 5472 7565 0d0a 0d0a 5b66 6c61 6b65  = True....[flake
-00000730: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
-00000740: 6774 6820 3d20 3830 0d0a 7365 6c65 6374  gth = 80..select
-00000750: 203d 2045 2c46 2c57 2c42 2c42 3935 302c   = E,F,W,B,B950,
-00000760: 432c 492c 5459 500d 0a69 676e 6f72 6520  C,I,TYP..ignore 
-00000770: 3d20 4532 3033 2c45 3530 312c 5735 3033  = E203,E501,W503
-00000780: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000790: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000007a0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000460: 3a20 5757 572f 4854 5450 203a 3a20 5753  : WWW/HTTP :: WS
+00000470: 4749 203a 3a20 4170 706c 6963 6174 696f  GI :: Applicatio
+00000480: 6e0a 0954 6f70 6963 203a 3a20 536f 6674  n..Topic :: Soft
+00000490: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+000004a0: 203a 3a20 4c69 6272 6172 6965 7320 3a3a   :: Libraries ::
+000004b0: 2041 7070 6c69 6361 7469 6f6e 2046 7261   Application Fra
+000004c0: 6d65 776f 726b 730a 0954 6f70 6963 203a  meworks..Topic :
+000004d0: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+000004e0: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
+000004f0: 6965 730a 0a5b 6f70 7469 6f6e 735d 0a70  ies..[options].p
+00000500: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
+00000510: 7372 630a 7365 7475 705f 7265 7175 6972  src.setup_requir
+00000520: 6573 203d 2044 6a61 6e67 6f3e 3d33 2e32  es = Django>=3.2
+00000530: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000540: 7320 3d20 446a 616e 676f 3e3d 332e 320a  s = Django>=3.2.
+00000550: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000560: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+00000570: 5f64 6174 6120 3d20 5472 7565 0a70 7974  _data = True.pyt
+00000580: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000590: 3d33 2e38 0a7a 6970 5f73 6166 6520 3d20  =3.8.zip_safe = 
+000005a0: 4661 6c73 650a 0a5b 6f70 7469 6f6e 732e  False..[options.
+000005b0: 6578 7472 6173 5f72 6571 7569 7265 5d0a  extras_require].
+000005c0: 7465 7374 696e 6720 3d20 0a09 636f 7665  testing = ..cove
+000005d0: 7261 6765 0a09 636f 6465 636f 760a 6c69  rage..codecov.li
+000005e0: 6e74 696e 6720 3d20 0a09 666c 616b 6538  nting = ..flake8
+000005f0: 0a09 7079 6c69 6e74 0a0a 5b6f 7074 696f  ..pylint..[optio
+00000600: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000610: 5d0a 7768 6572 6520 3d20 7372 630a 0a5b  ].where = src..[
+00000620: 636f 7665 7261 6765 3a72 756e 5d0a 6272  coverage:run].br
+00000630: 616e 6368 203d 2054 7275 650a 736f 7572  anch = True.sour
+00000640: 6365 203d 2069 7562 656e 6461 0a0a 5b63  ce = iubenda..[c
+00000650: 6f76 6572 6167 653a 7061 7468 735d 0a73  overage:paths].s
+00000660: 6f75 7263 6520 3d20 0a09 7372 630a 092e  ource = ..src...
+00000670: 746f 782f 2a2f 7369 7465 2d70 6163 6b61  tox/*/site-packa
+00000680: 6765 730a 0a5b 636f 7665 7261 6765 3a72  ges..[coverage:r
+00000690: 6570 6f72 745d 0a73 686f 775f 6d69 7373  eport].show_miss
+000006a0: 696e 6720 3d20 5472 7565 0a0a 5b66 6c61  ing = True..[fla
+000006b0: 6b65 385d 0a6d 6178 2d6c 696e 652d 6c65  ke8].max-line-le
+000006c0: 6e67 7468 203d 2038 300a 7365 6c65 6374  ngth = 80.select
+000006d0: 203d 2045 2c46 2c57 2c42 2c42 3935 302c   = E,F,W,B,B950,
+000006e0: 432c 492c 5459 500a 6967 6e6f 7265 203d  C,I,TYP.ignore =
+000006f0: 2045 3230 332c 4535 3031 2c57 3530 330a   E203,E501,W503.
+00000700: 0a5b 6567 675f 696e 666f 5d0a 7461 675f  .[egg_info].tag_
+00000710: 6275 696c 6420 3d20 0a74 6167 5f64 6174  build = .tag_dat
+00000720: 6520 3d20 300a 0a                        e = 0..
```

### Comparing `django-iubenda-0.1.12.dev0/setup.py` & `django-iubenda-1.2.6/setup.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import os
-from distutils.cmd import Command
-from distutils.command.build import build as _build
-
-from setuptools.command.install_lib import install_lib as _install_lib
-
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-
-class CompileTranslations(Command):
-    description = "compile message catalogs to MO files via django compilemessages"
-    user_options = []  # type: list
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        curdir = os.getcwd()
-        os.chdir(os.path.realpath(os.path.join("src", "iubenda")))
-        from django.core.management import call_command
-
-        call_command("compilemessages")
-        os.chdir(curdir)
-
-
-class Build(_build):
-    sub_commands = [("compile_translations", None)] + _build.sub_commands
-
-
-class InstallLib(_install_lib):
-    def run(self):
-        self.run_command("compile_translations")
-        _install_lib.run(self)
-
-
-setup(
-    cmdclass={
-        "build": Build,
-        "install_lib": InstallLib,
-        "compile_translations": CompileTranslations,
-    },
-)
+import os
+from distutils.cmd import Command
+from distutils.command.build import build as _build
+
+from setuptools.command.install_lib import install_lib as _install_lib
+
+try:
+    from setuptools import setup
+except ImportError:
+    from distutils.core import setup
+
+
+class CompileTranslations(Command):
+    description = "compile message catalogs to MO files via django compilemessages"
+    user_options = []  # type: list
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        curdir = os.getcwd()
+        os.chdir(os.path.realpath(os.path.join("src", "iubenda")))
+        from django.core.management import call_command
+
+        call_command("compilemessages")
+        os.chdir(curdir)
+
+
+class Build(_build):
+    sub_commands = [("compile_translations", None)] + _build.sub_commands
+
+
+class InstallLib(_install_lib):
+    def run(self):
+        self.run_command("compile_translations")
+        _install_lib.run(self)
+
+
+setup(
+    cmdclass={
+        "build": Build,
+        "install_lib": InstallLib,
+        "compile_translations": CompileTranslations,
+    },
+)
```

### Comparing `django-iubenda-0.1.12.dev0/src/django_iubenda.egg-info/PKG-INFO` & `django-iubenda-1.2.6/src/django_iubenda.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,161 +1,204 @@
-Metadata-Version: 2.1
-Name: django-iubenda
-Version: 0.1.12.dev0
-Summary: Django application for handling privacy and cookie policies configured with Iubenda.
-Home-page: https://github.com/DLRSP/django-iubenda
-Author: DLRSP
-Author-email: dlrsp.dev@gmail.com
-License: MIT License
-Keywords: django,iubenda,privacy,cookie
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: linting
-License-File: LICENSE
-
-# django-iubenda [![PyPi license](https://img.shields.io/pypi/l/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-
-[![PyPi status](https://img.shields.io/pypi/status/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi version](https://img.shields.io/pypi/v/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi downloads](https://img.shields.io/pypi/dw/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-[![PyPi downloads](https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
-
-## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-iubenda.svg)
-
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yml)
-
-## Compliance for websites and apps
-Click [here](http://iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda
-[![Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/dlrspapi)
-
-
-## Check Demo Project
-* Browser the demo app on-line on [Heroku](https://django-iubenda.herokuapp.com/)
-* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-iubenda)
-
-## Requirements
--   Python 3.7 to 3.10 supported.
--   Django 3.2 to 4.0 supported.
-
-## Setup
-1. Install from **pip**:
-```shell
-pip install django-iubenda
-```
-
-2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
-```python
-INSTALLED_APPS = (
-    "modeltranslation",
-    # ...
-    "iubenda",
-    # ...
-)
-```
-
-3. Modify `settings.py` by adding the app's context processor to `TEMPLATES`:
-```python
-TEMPLATES = [
-    {
-        # ...
-        'OPTIONS': {
-            'context_processors': [
-                # ...
-                'iubenda.context_processors.iubenda',
-                # ...
-            ],
-        },
-    },
-]
-```
-
-4. Be sure the Django's Locale middleware is enabled inside `settings.py`:
-```python
-MIDDLEWARE = (
-    # ...
-    'django.middleware.locale.LocaleMiddleware',
-    # ...
-)
-```
-
-5. Be sure the variable `LANGUAGE_CODE` is available for HTML templates:
-```html
-{% load i18n %}
-{% get_current_language as LANGUAGE_CODE %}
-```
-
-6. Modify your project's template to add privacy and cookie policies. 
-   For example inside the `footer.html` add following code:
-```html
-{% if not debug %}
-    {% block iubenda %}{% include "iubenda/include-content.html" %}{% endblock iubenda %}
-{% endif %}
-```
-
-## Optional
-
-### Content Security Policy
-If Content Security Policy are implemented in your server and inline scripts are disabled,
-the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
-```html
-<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
-```
-
-### Iubenda's Options
-To personalize the Iubenda script behaviour, the dict `IUBENDA_OPTIONS` can be configured inside `settings.py`
-```python
-IUBENDA_OPTIONS = {"ccpaAcknowledgeOnDisplay": "true",
-                   "ccpaApplies": "true",
-                   "consentOnContinuedBrowsing": "false",
-                   "enableCcpa": "true",
-                   "floatingPreferencesButtonDisplay": "bottom-left",
-                   "invalidateConsentWithoutLog": "true",
-                   "perPurposeConsent": "true",
-                   "whitelabel": "false",
-                   "banner": {
-                       "acceptButtonDisplay": "true",
-                       "backgroundOverlay": "true",
-                       "closeButtonRejects": "true",
-                       "customizeButtonDisplay": "true",
-                       "explicitWithdrawal": "true",
-                       "fontSize": "14px",
-                       "listPurposes": "true",
-                       "position": "float-center",
-                       "rejectButtonDisplay": "true"
-                   }
-                   }
-```
-
-## Run Example Project
-
-```shell
-git clone --depth=50 --branch=django-iubenda https://github.com/DLRSP/example.git DLRSP/example
-cd DLRSP/example
-python manage.py runserver
-```
-
-Now browser the app @ http://127.0.0.1:8000
+Metadata-Version: 2.1
+Name: django-iubenda
+Version: 1.2.6
+Summary: Django application for handling privacy and cookie policies configured with Iubenda.
+Home-page: https://github.com/DLRSP/django-iubenda
+Author: DLRSP
+Author-email: dlrsp.dev@gmail.com
+License: MIT License
+Keywords: django,iubenda,privacy,cookie
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: linting
+License-File: LICENSE
+
+# django-iubenda [![PyPi license](https://img.shields.io/pypi/l/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+
+[![PyPi status](https://img.shields.io/pypi/status/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi version](https://img.shields.io/pypi/v/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi downloads](https://img.shields.io/pypi/dw/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+[![PyPi downloads](https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
+
+## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-iubenda.svg)
+
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
+
+## Compliance for websites and apps
+Click [here](http://iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda
+[![Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/dlrspapi)
+
+
+## Check Demo Project
+* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-iubenda)
+
+## Requirements
+-   Python +3.8 supported.
+-   Django +3.2 supported.
+
+## Setup
+1. Install from **pip**:
+```shell
+pip install django-iubenda
+```
+
+2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = (
+    "modeltranslation",
+    # ...
+    "iubenda",
+    # ...
+)
+```
+
+3. Modify `settings.py` by adding the app's context processor to `TEMPLATES`:
+```python
+TEMPLATES = [
+    {
+        # ...
+        "OPTIONS": {
+            "context_processors": [
+                # ...
+                "iubenda.context_processors.iubenda",
+                # ...
+            ],
+        },
+    },
+]
+```
+
+4. Be sure the Django's Locale middleware is enabled inside `settings.py`:
+```python
+MIDDLEWARE = (
+    # ...
+    "django.middleware.locale.LocaleMiddleware",
+    # ...
+)
+```
+
+5. Modify `url.py` by adding the app's urls to `urlpatterns`:
+```python
+urlpatterns += [
+    path("", include("iubenda.urls")),
+]
+```
+
+6. Modify `url.py` by adding the app's sitemaps to `sitemaps`:
+```python
+from iubenda.sitemaps import PrivacySitemap, CookieSitemap
+
+sitemaps = {
+    # ...
+    "privacy": PrivacySitemap,
+    "cookie": CookieSitemap,
+    # ...
+}
+```
+
+7. Be sure the variable `LANGUAGE_CODE` is available for HTML templates:
+```html
+{% load i18n %}
+{% get_current_language as LANGUAGE_CODE %}
+```
+
+8. Modify your project's template to add privacy and cookie policies.
+   For example inside the `footer.html` add following code:
+```html
+{% if not debug %}
+    {% block iubenda %}{% include "iubenda/include-content.html" %}{% endblock iubenda %}
+{% endif %}
+```
+
+## Optional
+
+### Content Security Policy
+If Content Security Policy are implemented in your server and inline scripts are disabled,
+the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
+```html
+<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
+```
+Inside your webserver's configurations, a rule to dynamically replace your CONSTANT nonce in a random string is needed.
+
+To allow  external source from Iubenda domains, please implement these rules:
+```editorconfig
+Content-Security-Policy:
+    script-src-elem https://*.iubenda.com";
+    img-src https://*.iubenda.com data:";
+    style-src https://*.iubenda.com";
+    connect-src https://*.iubenda.com";
+    frame-src https://*.iubenda.com";
+```
+
+If you prefer to not allow ***unsafe-inline*** inside your CSP, please also add the two specific hash for your
+script prompted as error in Javascript Console.
+```editorconfig
+# Iubenda Privacy And Cookie Policy - API
+Content-Security-Policy:
+    ...
+    script-src-elem https://*.iubenda.com 'sha256-YOUR-FIRST-HASH-PROMPTED-INSIDE-CONSOLE' 'sha256-YOUR-SECOND-HASH-PROMPTED-INSIDE-CONSOLE';
+    ...
+```
+
+Check this article from [Iubenda help](https://www.iubenda.com/it/help/12347-come-configurare-il-content-security-policy-per-consentire-lesecuzione-degli-script-di-iubenda)
+
+### Iubenda's Options
+(To-Do: new feuture)
+
+To personalize the Iubenda script behaviour, the dict `IUBENDA_OPTIONS` can be configured inside `settings.py`
+```python
+IUBENDA_OPTIONS = {
+    "ccpaAcknowledgeOnDisplay": "true",
+    "ccpaApplies": "true",
+    "consentOnContinuedBrowsing": "false",
+    "enableCcpa": "true",
+    "floatingPreferencesButtonDisplay": "bottom-left",
+    "invalidateConsentWithoutLog": "true",
+    "perPurposeConsent": "true",
+    "whitelabel": "false",
+    "banner": {
+        "acceptButtonDisplay": "true",
+        "backgroundOverlay": "true",
+        "closeButtonRejects": "true",
+        "customizeButtonDisplay": "true",
+        "explicitWithdrawal": "true",
+        "fontSize": "14px",
+        "listPurposes": "true",
+        "position": "float-center",
+        "rejectButtonDisplay": "true",
+    },
+}
+```
+
+## Run Example Project
+
+```shell
+git clone --depth=50 --branch=django-iubenda https://github.com/DLRSP/example.git DLRSP/example
+cd DLRSP/example
+python manage.py runserver
+```
+
+Now browser the app @ http://127.0.0.1:8000
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/context_processors.py` & `django-iubenda-1.2.6/src/iubenda/context_processors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-# -*- coding: utf-8 -*-
 """
 Context processors for Iubenda app
 """
 
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.sites.models import Site
 from django.core.cache import cache
+
 from .models import Iubenda
 
 
 def iubenda(request):
     """Returns the info for:
-        - iub_site_id: Iubenda Site ID
-        - iub_policy_id: Iubenda Policy ID
+    - iub_site_id: Iubenda Site ID
+    - iub_policy_id: Iubenda Policy ID
     """
 
     cache_key = f"iubenda_{request.LANGUAGE_CODE}"
     context_cache = {}
     try:
         context_cache = cache.get(cache_key)
     except Exception as err:
+        messages.warning(request, err)
         context_cache = {}
 
     if not context_cache or context_cache is None:
         try:
             context = {
-                'cx_iubenda': Iubenda.objects.filter(site=Site.objects.get_current()).values('iub_site_id', 'iub_policy_id').get(),
+                "cx_iubenda": Iubenda.objects.filter(site=Site.objects.get_current())
+                .values("iub_site_id", "iub_policy_id")
+                .get(),
             }
 
             cx_iubenda_options = getattr(settings, "IUBENDA_OPTIONS", False)
             if cx_iubenda_options:
-                context.update({
-                    'cx_iubenda_options': cx_iubenda_options
-                })
+                context.update({"cx_iubenda_options": cx_iubenda_options})
 
             cx_iubenda_nonce = getattr(settings, "IUBENDA_CSP_NONCE", False)
             if cx_iubenda_nonce:
-                context.update({
-                    'cx_iubenda_nonce': cx_iubenda_nonce
-                })
+                context.update({"cx_iubenda_nonce": cx_iubenda_nonce})
 
             context_cache = cache.set(cache_key, context, timeout=86400)
             return context
         except Exception as err:
             messages.error(request, err)
     return context_cache
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/models.py` & `django-iubenda-1.2.6/src/iubenda/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from django.contrib.sites.models import Site
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class Iubenda(models.Model):
-    site = models.ForeignKey(Site, verbose_name=_("Django Site"), on_delete=models.CASCADE)
+    site = models.ForeignKey(
+        Site, verbose_name=_("Django Site"), on_delete=models.CASCADE
+    )
     iub_site_id = models.IntegerField(verbose_name=_("Iubenda Site ID"), unique=True)
-    iub_policy_id = models.IntegerField(verbose_name=_("Iubenda Policy ID"), unique=True)
+    iub_policy_id = models.IntegerField(
+        verbose_name=_("Iubenda Policy ID"), unique=True
+    )
     active = models.BooleanField(default=True)
 
     class Meta:
         verbose_name = _("Iubenda Policy")
         verbose_name_plural = _("Iubenda Policies")
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/static/iubenda/css/iubenda_badge.css` & `django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_badge.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-.iubenda-embed:not(.iubenda-nostyle){font-size:100% !important;width:auto !important;-webkit-appearance:none !important;-moz-appearance:none !important;appearance:none !important;background:none !important;-webkit-box-sizing:border-box !important;-moz-box-sizing:border-box !important;box-sizing:border-box !important;-webkit-tap-highlight-color:transparent !important;-webkit-backface-visibility:hidden !important;backface-visibility:hidden !important;font-family:-apple-system,sans-serif !important;text-decoration:none !important;color:currentColor !important;background-attachment:scroll !important;background-color:transparent !important;background-image:none !important;background-position:0 0 !important;background-repeat:repeat !important;border:0 !important;border-color:#000 !important;border-color:currentColor !important;border-radius:0 !important;border-style:none !important;border-width:medium !important;bottom:auto !important;clear:none !important;clip:auto !important;counter-increment:none !important;counter-reset:none !important;cursor:auto !important;direction:inherit !important;float:none !important;font-style:inherit !important;font-variant:normal !important;font-weight:inherit !important;height:auto !important;left:auto !important;letter-spacing:normal !important;line-height:inherit !important;list-style-type:inherit !important;list-style-position:outside !important;list-style-image:none !important;margin:0 !important;max-height:none !important;max-width:none !important;min-height:0 !important;min-width:0 !important;opacity:1;outline:0 !important;overflow:visible !important;padding:0 !important;position:static !important;quotes:"" "" !important;right:auto !important;table-layout:auto !important;text-align:left !important;text-indent:0 !important;text-transform:none !important;top:auto !important;unicode-bidi:normal !important;vertical-align:baseline !important;visibility:inherit !important;white-space:normal !important;width:auto !important;word-spacing:normal !important;z-index:auto !important;background-origin:padding-box !important;background-origin:padding-box !important;background-clip:border-box !important;background-size:auto !important;-o-border-image:none !important;border-image:none !important;border-radius:0 !important;border-radius:0 !important;-webkit-box-shadow:none !important;box-shadow:none !important;-webkit-column-count:auto !important;-moz-column-count:auto !important;column-count:auto !important;-webkit-column-gap:normal !important;-moz-column-gap:normal !important;column-gap:normal !important;-webkit-column-rule:medium none #000 !important;-moz-column-rule:medium none #000 !important;column-rule:medium none #000 !important;-webkit-column-span:none !important;-moz-column-span:none !important;column-span:none !important;-webkit-column-width:auto !important;-moz-column-width:auto !important;column-width:auto !important;-webkit-font-feature-settings:normal !important;-moz-font-feature-settings:normal !important;font-feature-settings:normal !important;overflow-x:visible !important;overflow-y:visible !important;-webkit-hyphens:manual !important;-moz-hyphens:manual !important;-ms-hyphens:manual !important;hyphens:manual !important;-webkit-perspective:none !important;perspective:none !important;-webkit-perspective-origin:50% 50% !important;perspective-origin:50% 50% !important;text-shadow:none !important;-webkit-transition:all 0s ease 0s !important;transition:all 0s ease 0s !important;-webkit-transform:none !important;-ms-transform:none !important;transform:none !important;-webkit-transform-origin:50% 50% !important;-ms-transform-origin:50% 50% !important;transform-origin:50% 50% !important;-webkit-transform-style:flat !important;transform-style:flat !important;word-break:normal !important;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;appearance:none !important;line-height:1.25 !important;min-width:20px !important;border-radius:3px !important;cursor:pointer !important;font-weight:bold !important;font-size:11px !important;-webkit-box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;color:rgba(0,0,0,0.65) !important;background-color:#fff !important;display:inline-block !important;vertical-align:middle !important;-webkit-text-size-adjust:100% !important}.iubenda-embed:not(.iubenda-nostyle){padding:4px 8px !important}.iubenda-embed:not(.iubenda-nostyle):hover{-webkit-box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;background-color:rgba(0,0,0,0.035) !important}.iubenda-embed:not(.iubenda-nostyle):active{background-color:rgba(0,0,0,0.065) !important}.iubenda-embed:not(.no-brand):not(.iubenda-nostyle){background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='32' height='32' viewBox='0 0 32 32'%3E%3Cpath fill='%231CC691' fill-rule='evenodd' d='M16 7a4 4 0 0 1 2.627 7.016L19.5 25h-7l.873-10.984A4 4 0 0 1 16 7z'/%3E%3C/svg%3E") !important;background-repeat:no-repeat !important;background-size:21px 21px !important;background-position:top left !important;padding-left:20px !important}.iubenda-embed.iubenda-black{background-color:#444 !important;color:#F4F4F4 !important}.iubenda-embed.iubenda-black:hover{-webkit-box-shadow:inset 0 0 0 1px rgba(0,0,0,0.75),0 1px 1px -1px rgba(0,0,0,0.15) !important;box-shadow:inset 0 0 0 1px rgba(0,0,0,0.75),0 1px 1px -1px rgba(0,0,0,0.15) !important;background-color:#555 !important}.iubenda-embed.iubenda-black:active{background-color:#444 !important}.iubenda-embed.iubenda-black:not(.no-brand):not(.iubenda-nostyle){background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='32' height='32' viewBox='0 0 32 32'%3E%3Cpath fill='%23FFFFFF' fill-rule='evenodd' d='M16 7a4 4 0 0 1 2.627 7.016L19.5 25h-7l.873-10.984A4 4 0 0 1 16 7z'/%3E%3C/svg%3E") !important}
+.iubenda-embed:not(.iubenda-nostyle){font-size:100% !important;width:auto !important;-webkit-appearance:none !important;-moz-appearance:none !important;appearance:none !important;background:none !important;-webkit-box-sizing:border-box !important;-moz-box-sizing:border-box !important;box-sizing:border-box !important;-webkit-tap-highlight-color:transparent !important;-webkit-backface-visibility:hidden !important;backface-visibility:hidden !important;font-family:-apple-system,sans-serif !important;text-decoration:none !important;color:currentColor !important;background-attachment:scroll !important;background-color:transparent !important;background-image:none !important;background-position:0 0 !important;background-repeat:repeat !important;border:0 !important;border-color:#000 !important;border-color:currentColor !important;border-radius:0 !important;border-style:none !important;border-width:medium !important;bottom:auto !important;clear:none !important;clip:auto !important;counter-increment:none !important;counter-reset:none !important;cursor:auto !important;direction:inherit !important;float:none !important;font-style:inherit !important;font-variant:normal !important;font-weight:inherit !important;height:auto !important;left:auto !important;letter-spacing:normal !important;line-height:inherit !important;list-style-type:inherit !important;list-style-position:outside !important;list-style-image:none !important;margin:0 !important;max-height:none !important;max-width:none !important;min-height:0 !important;min-width:0 !important;opacity:1;outline:0 !important;overflow:visible !important;padding:0 !important;position:static !important;quotes:"" "" !important;right:auto !important;table-layout:auto !important;text-align:left !important;text-indent:0 !important;text-transform:none !important;top:auto !important;unicode-bidi:normal !important;vertical-align:baseline !important;visibility:inherit !important;white-space:normal !important;width:auto !important;word-spacing:normal !important;z-index:auto !important;background-origin:padding-box !important;background-origin:padding-box !important;background-clip:border-box !important;background-size:auto !important;-o-border-image:none !important;border-image:none !important;border-radius:0 !important;border-radius:0 !important;-webkit-box-shadow:none !important;box-shadow:none !important;-webkit-column-count:auto !important;-moz-column-count:auto !important;column-count:auto !important;-webkit-column-gap:normal !important;-moz-column-gap:normal !important;column-gap:normal !important;-webkit-column-rule:medium none #000 !important;-moz-column-rule:medium none #000 !important;column-rule:medium none #000 !important;-webkit-column-span:none !important;-moz-column-span:none !important;column-span:none !important;-webkit-column-width:auto !important;-moz-column-width:auto !important;column-width:auto !important;-webkit-font-feature-settings:normal !important;-moz-font-feature-settings:normal !important;font-feature-settings:normal !important;overflow-x:visible !important;overflow-y:visible !important;-webkit-hyphens:manual !important;-moz-hyphens:manual !important;-ms-hyphens:manual !important;hyphens:manual !important;-webkit-perspective:none !important;perspective:none !important;-webkit-perspective-origin:50% 50% !important;perspective-origin:50% 50% !important;text-shadow:none !important;-webkit-transition:all 0s ease 0s !important;transition:all 0s ease 0s !important;-webkit-transform:none !important;-ms-transform:none !important;transform:none !important;-webkit-transform-origin:50% 50% !important;-ms-transform-origin:50% 50% !important;transform-origin:50% 50% !important;-webkit-transform-style:flat !important;transform-style:flat !important;word-break:normal !important;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;appearance:none !important;line-height:1.25 !important;min-width:20px !important;border-radius:3px !important;cursor:pointer !important;font-weight:bold !important;font-size:11px !important;-webkit-box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;color:rgba(0,0,0,0.65) !important;background-color:#fff !important;display:inline-block !important;vertical-align:middle !important;-webkit-text-size-adjust:100% !important}.iubenda-embed:not(.iubenda-nostyle){padding:4px 8px !important}.iubenda-embed:not(.iubenda-nostyle):hover{-webkit-box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;box-shadow:inset 0 0 0 1px rgba(0,0,0,0.15),0 1px 1px -1px rgba(0,0,0,0.15) !important;background-color:rgba(0,0,0,0.035) !important}.iubenda-embed:not(.iubenda-nostyle):active{background-color:rgba(0,0,0,0.065) !important}.iubenda-embed:not(.no-brand):not(.iubenda-nostyle){background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='32' height='32' viewBox='0 0 32 32'%3E%3Cpath fill='%231CC691' fill-rule='evenodd' d='M16 7a4 4 0 0 1 2.627 7.016L19.5 25h-7l.873-10.984A4 4 0 0 1 16 7z'/%3E%3C/svg%3E") !important;background-repeat:no-repeat !important;background-size:21px 21px !important;background-position:top left !important;padding-left:20px !important}.iubenda-embed.iubenda-black{background-color:#444 !important;color:#F4F4F4 !important}.iubenda-embed.iubenda-black:hover{-webkit-box-shadow:inset 0 0 0 1px rgba(0,0,0,0.75),0 1px 1px -1px rgba(0,0,0,0.15) !important;box-shadow:inset 0 0 0 1px rgba(0,0,0,0.75),0 1px 1px -1px rgba(0,0,0,0.15) !important;background-color:#555 !important}.iubenda-embed.iubenda-black:active{background-color:#444 !important}.iubenda-embed.iubenda-black:not(.no-brand):not(.iubenda-nostyle){background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='32' height='32' viewBox='0 0 32 32'%3E%3Cpath fill='%23FFFFFF' fill-rule='evenodd' d='M16 7a4 4 0 0 1 2.627 7.016L19.5 25h-7l.873-10.984A4 4 0 0 1 16 7z'/%3E%3C/svg%3E") !important}
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/static/iubenda/css/iubenda_policy.css` & `django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_policy.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-html#iubenda_policy,#iubenda_policy body{margin:0;padding:0}html#iubenda_policy{overflow-y:scroll;font-size:100%;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}#iubenda_policy h1,#iubenda_policy h2,#iubenda_policy h3,#iubenda_policy h4,#iubenda_policy h5,#iubenda_policy h6,#iubenda_policy p,#iubenda_policy blockquote,#iubenda_policy pre,#iubenda_policy a,#iubenda_policy abbr,#iubenda_policy acronym,#iubenda_policy address,#iubenda_policy cite,#iubenda_policy code,#iubenda_policy del,#iubenda_policy dfn,#iubenda_policy em,#iubenda_policy img,#iubenda_policy q,#iubenda_policy s,#iubenda_policy samp,#iubenda_policy small,#iubenda_policy strike,#iubenda_policy strong,#iubenda_policy sub,#iubenda_policy sup,#iubenda_policy tt,#iubenda_policy var,#iubenda_policy dd,#iubenda_policy dl,#iubenda_policy dt,#iubenda_policy li,#iubenda_policy ol,#iubenda_policy ul,#iubenda_policy fieldset,#iubenda_policy form,#iubenda_policy label,#iubenda_policy legend,#iubenda_policy button,#iubenda_policy table,#iubenda_policy caption,#iubenda_policy tbody,#iubenda_policy tfoot,#iubenda_policy thead,#iubenda_policy tr,#iubenda_policy th,#iubenda_policy td{margin:0;padding:0;border:0;font-weight:normal;font-style:normal;font-size:100%;line-height:1;font-family:inherit}#iubenda_policy table{border-collapse:collapse;border-spacing:0}#iubenda_policy ol,#iubenda_policy ul{list-style:none}#iubenda_policy q:before,#iubenda_policy q:after,#iubenda_policy blockquote:before,#iubenda_policy blockquote:after{content:""}#iubenda_policy a:focus{outline:thin dotted}#iubenda_policy a:hover,#iubenda_policy a:active{outline:0}#iubenda_policy article,#iubenda_policy aside,#iubenda_policy details,#iubenda_policy figcaption,#iubenda_policy figure,#iubenda_policy footer,#iubenda_policy header,#iubenda_policy hgroup,#iubenda_policy nav,#iubenda_policy section{display:block}#iubenda_policy audio,#iubenda_policy canvas,#iubenda_policy video{display:inline-block;*display:inline;*zoom:1}#iubenda_policy audio:not([controls]){display:none}#iubenda_policy sub,#iubenda_policy sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}#iubenda_policy sup{top:-0.5em}#iubenda_policy sub{bottom:-0.25em}#iubenda_policy img{border:0;-ms-interpolation-mode:bicubic}#iubenda_policy button,#iubenda_policy input,#iubenda_policy select,#iubenda_policy textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}#iubenda_policy button,#iubenda_policy input{line-height:normal;*overflow:visible}#iubenda_policy button::-moz-focus-inner,#iubenda_policy input::-moz-focus-inner{border:0;padding:0}#iubenda_policy button,#iubenda_policy input[type="button"],#iubenda_policy input[type="reset"],#iubenda_policy input[type="submit"]{cursor:pointer;-webkit-appearance:button}#iubenda_policy input[type="search"]{-webkit-appearance:textfield;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}#iubenda_policy input[type="search"]::-webkit-search-decoration{-webkit-appearance:none}#iubenda_policy textarea{overflow:auto;vertical-align:top}html#iubenda_policy{-webkit-font-smoothing:antialiased}#iubenda_policy p{font-size:13px;font-weight:normal;line-height:18px;margin-bottom:9px}#iubenda_policy p small{font-size:11px;color:#bfbfbf}#iubenda_policy h1,#iubenda_policy h2,#iubenda_policy h3,#iubenda_policy h4,#iubenda_policy h5,#iubenda_policy h6{font-weight:bold;color:#59636D}#iubenda_policy h1{margin-bottom:18px;font-size:30px;line-height:2}#iubenda_policy h1 small{font-size:18px}#iubenda_policy h2{font-size:24px;margin-bottom:18px;line-height:1.5}#iubenda_policy h2 small{font-size:14px}#iubenda_policy h3,#iubenda_policy h4,#iubenda_policy h5,#iubenda_policy h6{margin-bottom:9px}#iubenda_policy h3{font-size:18px}#iubenda_policy h3 small{font-size:14px}#iubenda_policy h4{font-size:16px}#iubenda_policy h4 small{font-weight:bold;font-size:13px}#iubenda_policy h5{font-size:13px;padding-top:19px}#iubenda_policy h6{font-size:13px;color:#bfbfbf;text-transform:uppercase}#iubenda_policy ul ul,#iubenda_policy ul ol,#iubenda_policy ol ol,#iubenda_policy ol ul{margin:0}#iubenda_policy ul.styled,#iubenda_policy ul{list-style:disc;padding-top:5px}#iubenda_policy ul.styled li,#iubenda_policy ul li{list-style:disc;line-height:19px;font-size:13px;margin-left:30px;margin-top:2px}#iubenda_policy ol{list-style:decimal}#iubenda_policy ul.unstyled{list-style:none;margin-left:0}#iubenda_policy dl{margin-bottom:18px}#iubenda_policy dl dt,#iubenda_policy dl dd{line-height:18px}#iubenda_policy dl dt{font-weight:bold}#iubenda_policy dl dd{margin-left:9px}#iubenda_policy hr{margin:0 0 19px;border:0;border-bottom:1px solid #eee}#iubenda_policy strong{font-style:inherit;font-weight:bold}#iubenda_policy em{font-style:italic;font-weight:inherit;line-height:inherit}#iubenda_policy .muted{color:#bfbfbf}#iubenda_policy blockquote{margin-bottom:18px;border-left:5px solid #eee;padding-left:15px}#iubenda_policy blockquote p{font-size:14px;font-weight:300;line-height:18px;margin-bottom:0}#iubenda_policy blockquote small{display:block;font-size:12px;font-weight:300;line-height:18px;color:#bfbfbf}#iubenda_policy blockquote small:before{content:'\2014 \00A0'}#iubenda_policy address{display:block;line-height:18px;margin-bottom:18px}#iubenda_policy code,#iubenda_policy pre{padding:0 3px 2px;font-family:Monaco, Andale Mono, Courier New, monospace;font-size:12px;border-radius:3px}#iubenda_policy code{background-color:#fee9cc;color:rgba(0,0,0,0.75);padding:1px 3px}#iubenda_policy pre{background-color:#f5f5f5;display:block;padding:17px;margin:0 0 18px;line-height:18px;font-size:12px;border:1px solid #ccc;border:1px solid rgba(0,0,0,0.15);border-radius:3px;white-space:pre;white-space:pre-wrap;word-wrap:break-word}#iubenda_policy .breadcrumbs{padding:0 0 10px 0;margin-bottom:30px;border-bottom:1px solid #F6F6F6;width:100%}#iubenda_policy .breadcrumbs>li{float:left;filter:alpha(opacity=50);-khtml-opacity:0.5;-moz-opacity:0.5;opacity:0.5}#iubenda_policy .breadcrumbs>li:not(:last-child):after{color:#333B43;padding:0 10px;content:"\203a"}#iubenda_policy .breadcrumbs+.pills,#iubenda_policy .breadcrumbs+.sec_tabs{margin-top:-15px}#iubenda_policy .table{display:table;border-collapse:collapse;padding:0 !important;margin:0}#iubenda_policy .cust_row{display:table-row;margin:0}#iubenda_policy .column{display:table-cell;vertical-align:top;padding:30px}#iubenda_policy .box_primary{border:1px solid #C0C1C1;border-bottom-color:#A8AAAB;-webkit-box-shadow:0 1px 0 #ebebec;box-shadow:0 1px 0 #ebebec;-webkit-box-shadow:0 1px 0 rgba(0,0,0,0.1);box-shadow:0 1px 0 rgba(0,0,0,0.1);background:#FFF}#iubenda_policy .box_content{border-radius:4px;padding:30px}#iubenda_policy .box_content .iub_content{padding:30px}#iubenda_policy .box_content .iub_content>hr{width:686px;margin-left:-30px;margin-right:-30px}#iubenda_policy .box_content .aside{width:191px;padding:30px}#iubenda_policy .box_content .aside.aside-right{border-left:1px solid #DFDFDF}#iubenda_policy .table>.box_content{padding:0}#iubenda_policy .box_10{padding:10px;border-radius:3px;margin-bottom:15px}#iubenda_policy .box_10>h4{margin-bottom:0;font-size:13px}#iubenda_policy .box_10>.w_icon,#iubenda_policy .box_10.expand>.w_icon,#iubenda_policy .box_10>.w_icon.expand-click,#iubenda_policy .box_10.expand>.w_icon.expand-click{padding-left:45px;background-repeat:no-repeat;background-color:transparent;background-position-x:10px;background-position-y:7px;background-position:10px 7px}#iubenda_policy .box_10>.w_icon_16,#iubenda_policy .box_10.expand>.w_icon_16,#iubenda_policy .box_10>.w_icon_16.expand-click,#iubenda_policy .box_10.expand>.w_icon_16.expand-click{padding-left:40px;background-repeat:no-repeat;background-color:transparent;background-position-x:11px;background-position-y:11px;background-position:11px 11px}#iubenda_policy .box_10>.w_icon_24,#iubenda_policy .box_10.expand>.w_icon_24,#iubenda_policy .box_10>.w_icon_24.expand-click,#iubenda_policy .box_10.expand>.w_icon_24.expand-click{padding-left:45px;background-repeat:no-repeat;background-color:transparent;background-position-x:10px;background-position-y:10px;background-position:10px 10px}#iubenda_policy .box_5{padding:5px;border-radius:3px;font-size:11px;margin-bottom:15px}#iubenda_policy .box_5 hr{padding-top:5px;margin:0 -5px 5px -5px;border:0;border-bottom:1px solid #AC3737}#iubenda_policy .box_5.w_icon_16{padding-left:30px;background-repeat:no-repeat;background-position-x:8px;background-position-y:6px;background-position:8px 6px}#iubenda_policy .box_5.w_icon_16 hr{width:100%;padding-left:30px;padding-right:5px;margin-left:-30px;margin-right:-5px}#iubenda_policy .box_5.w_icon_16.red{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAATlBMVEUAAAD%2F%2F%2F8AAAD%2F%2F%2F8AAAAAAAD%2F%2F%2F%2F%2F%2F%2F%2FT09P%2F%2F%2F%2F9%2Ff3Y2Nj9%2Ff39%2Ff3d3d3%2F%2F%2F%2F8%2FPz39%2Ff19fX%2B%2Fv79%2Ff34%2BPj5%2Bfn8%2FPz9%2Ff3%2F%2F%2F8ZO4GEAAAAGXRSTlMAEB0gMDNAUHSAgYSRoaWwsra3weLl5fLyUJhrdwAAAF1JREFUeF6NzUcWhCAAwFAQsIPOWCD3v6gPxLYjy7%2BJKE1Ok%2FxAD%2BMbFIB6wYIxLA%2FUbEJAc8PKHmG9oAOkArq8DICdgXCuLUA7EDkBsd%2BfWALnyXmXoNImpytR0AEwdQcUE5t8VQAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .box_thumb{background:#FFF;-webkit-box-shadow:0 0 1px #a3a3a3, 0 1px 1px #a3a3a3;box-shadow:0 0 1px #a3a3a3, 0 1px 1px #a3a3a3;padding:6px}#iubenda_policy footer{margin-top:17px;padding-top:17px;border-top:1px solid #eee}#iubenda_policy hr{padding-top:15px;margin:0 0 15px 0}#iubenda_policy hr.primary{border:0;border-bottom:1px solid #DFDFDF;-webkit-box-shadow:0 1px 0 #f7f7f7;box-shadow:0 1px 0 #f7f7f7}#iubenda_policy .btn{cursor:pointer;display:inline-block;font-weight:bold;background-color:rgba(0,0,0,0.08);padding:0 20px;line-height:38px;color:#54616B;font-size:13px;border:0;border-radius:4rem;border-collapse:separate;-webkit-transition:0.1s linear all;transition:0.1s linear all}#iubenda_policy .btn:hover{background-position:0 -15px;text-decoration:none}#iubenda_policy .btn:focus{outline:1px dotted #666}#iubenda_policy .btn.primary{color:#fff;background-color:#0073CE}#iubenda_policy .btn:active{-webkit-box-shadow:inset 0 2px 4px rgba(0,0,0,0.25),0 1px 2px rgba(0,0,0,0.05);box-shadow:inset 0 2px 4px rgba(0,0,0,0.25),0 1px 2px rgba(0,0,0,0.05)}#iubenda_policy .btn.disabled{cursor:default;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=65);-khtml-opacity:0.65;-moz-opacity:0.65;opacity:0.65;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy .btn[disabled]{cursor:default;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=65);-khtml-opacity:0.65;-moz-opacity:0.65;opacity:0.65;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy .btn.large{font-size:16px;line-height:normal;padding:0 14px;border-radius:6px}#iubenda_policy .btn.mid_large{padding:0 10px;line-height:32px;font-size:13px}#iubenda_policy .btn.mid{padding:0 10px;line-height:28px;font-size:11px}#iubenda_policy .btn.small{padding:0 8px;line-height:18px;font-size:11px}#iubenda_policy :root .alert-message,#iubenda_policy :root .btn{border-radius:0 \0}#iubenda_policy button.btn::-moz-focus-inner,#iubenda_policy input.btn[type=submit]::-moz-focus-inner{padding:0;border:0}#iubenda_policy .circle{font-size:11px;line-height:18px;width:18px;padding:0;text-align:center;border-radius:11px}#iubenda_policy .circle.small{width:14px;line-height:14px;border-radius:9px;padding:0}#iubenda_policy .blue{color:#fff;background-color:#0073CE}#iubenda_policy .yellow{color:#6D693D;background-color:#FFD24D}#iubenda_policy .red{color:#FFF;background-color:#FF5D4D}#iubenda_policy .red a,#iubenda_policy .red a:hover:not(.btn){color:#FFF}#iubenda_policy .red a{border-bottom-color:rgba(247,247,247,0.3)}#iubenda_policy .red a:hover{border-bottom-color:rgba(247,247,247,0.6)}#iubenda_policy .green{color:#4D6C47;background-color:#F1FFD5}#iubenda_policy .iubgreen{color:#ffffff;background-color:#1CC691}#iubenda_policy .azure{color:#364048;background-color:#D2ECFE}#iubenda_policy .white{color:#54616B;background-color:#F8F8F8}#iubenda_policy .black{color:#FFF;background-color:#333333}#iubenda_policy .trasp{color:#333B43;background-color:#FFFFFF}#iubenda_policy .alert-message{position:relative;padding:7px 15px;margin-bottom:18px;color:#404040;background-color:#eedc94;background-repeat:repeat-x;background-image:-khtml-gradient(linear, left top, left bottom, from(#fceec1), to(#eedc94));background-image:-webkit-gradient(linear, left top, left bottom, from(#fceec1), to(#eedc94));background-image:linear-gradient(to bottom, #fceec1, #eedc94);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fceec1', endColorstr='#eedc94', GradientType=0);text-shadow:0 -1px 0 rgba(0,0,0,0.25);border-color:#eedc94 #eedc94 #e4c652;border-color:rgba(0,0,0,0.1) rgba(0,0,0,0.1) rgba(0,0,0,0.25);text-shadow:0 1px 0 rgba(255,255,255,0.5);border-width:1px;border-style:solid;border-radius:4px;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,0.25);box-shadow:inset 0 1px 0 rgba(255,255,255,0.25)}#iubenda_policy .alert-message .close{*margin-top:3px}#iubenda_policy .alert-message h5{line-height:18px}#iubenda_policy .alert-message p{margin-bottom:0}#iubenda_policy .alert-message div{margin-top:5px;margin-bottom:2px;line-height:28px}#iubenda_policy .alert-message .btn{-webkit-box-shadow:0 1px 0 rgba(255,255,255,0.25);box-shadow:0 1px 0 rgba(255,255,255,0.25)}#iubenda_policy .alert-message.block-message{background-image:none;background-color:#fdf5d9;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);padding:14px;border-color:#fceec1;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy .alert-message.block-message ul,#iubenda_policy .alert-message.block-message p{margin-right:30px}#iubenda_policy .alert-message.block-message ul{margin-bottom:0}#iubenda_policy .alert-message.block-message li{color:#404040}#iubenda_policy .alert-message.block-message .alert-actions{margin-top:5px}#iubenda_policy .alert-message.block-message.error,#iubenda_policy .alert-message.block-message.success,#iubenda_policy .alert-message.block-message.info{color:#404040;text-shadow:0 1px 0 rgba(255,255,255,0.5)}#iubenda_policy .alert-message.block-message.error{background-color:#fddfde;border-color:#fbc7c6}#iubenda_policy .alert-message.block-message.success{background-color:#d1eed1;border-color:#bfe7bf}#iubenda_policy .alert-message.block-message.info{background-color:#ddf4fb;border-color:#c6edf9}#iubenda_policy .fade{-webkit-transition:opacity 0.15s linear;transition:opacity 0.15s linear;opacity:0}#iubenda_policy .fade.in{opacity:1}#iubenda_policy .expand-click{cursor:pointer;position:relative}#iubenda_policy .box_10.expand .expand-click{margin:-10px;padding:12px 25px 13px 10px}#iubenda_policy .box_10.expand .expand-content{margin-top:10px}#iubenda_policy .box_10.expand .expand-content>*:first-child{margin-top:0;padding-top:0}#iubenda_policy .expand.expanded .expand-click:after,#iubenda_policy .box_10.expand.expanded .expand-click:after{content:"";position:absolute;right:10px;top:19px;border:5px;border-color:transparent;border-style:solid;border-top-color:#333B43}#iubenda_policy .expand .expand-click,#iubenda_policy .box_10.expand .expand-click,#iubenda_policy .expand.expanded .expand-click,#iubenda_policy .box_10.expand.expanded .expand-click{border-bottom:1px dotted #DDD;margin-bottom:10px;-webkit-transition:0.2s linear all;transition:0.2s linear all}#iubenda_policy .expand.collapsed .expand-click{border-bottom:0;margin-bottom:-10px}#iubenda_policy .expand.collapsed .expand-click:after{content:"";position:absolute;right:10px;top:17px;border:5px;border-color:transparent;border-style:solid;border-right-color:#333B43}#iubenda_policy .all-collapsed .expand .expand-click:after{content:"";position:absolute;right:10px;top:17px;border:5px;border-color:transparent;border-style:solid;border-right-color:#333B43}#iubenda_policy .all-collapsed .expand .expand-click{border-bottom:0;margin-bottom:-10px}#iubenda_policy .all-collapsed .expand-content{display:none}html#iubenda_policy,#iubenda_policy body{background-color:#FFF}#iubenda_policy{font-family:"Helvetica Neue", Helvetica, Arial, FreeSans, sans-serif;font-size:13px;font-weight:normal;line-height:18px;color:#59636D}#iubenda_policy body{margin:0}#iubenda_policy .iub_container-fluid{position:relative;min-width:940px;padding-left:20px;padding-right:20px;zoom:1}#iubenda_policy .iub_container-fluid:before,#iubenda_policy .iub_container-fluid:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy .iub_container-fluid:after{clear:both}#iubenda_policy .iub_container-fluid>.sidebar{float:left;width:220px}#iubenda_policy .iub_container-fluid>.iub_content{margin-left:240px}#iubenda_policy a{text-decoration:none;font-weight:bold;border-bottom:1px solid #F6F6F6;color:#333b43}#iubenda_policy a.unstyled{border-bottom:0}#iubenda_policy a:hover:not(.btn){color:#121518;border-bottom-color:#D6D6D6;-webkit-transition:0.1s linear all;transition:0.1s linear all}#iubenda_policy a.no_border,#iubenda_policy a.no_border:hover{border-bottom-width:0}#iubenda_policy .pull-right{float:right}#iubenda_policy .pull-left{float:left}#iubenda_policy .hide{display:none}#iubenda_policy .show{display:block}#iubenda_policy .link_on_dark a{border-bottom-color:rgba(247,247,247,0.3)}#iubenda_policy .link_on_dark a:hover{border-bottom-color:rgba(247,247,247,0.6)}#iubenda_policy [class*="policyicon_"]{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYBAMAAAASWSDLAAAAGFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz9%2BjSc3AAAAB3RSTlMAEEBQgMzQxeXuPgAAADJJREFUGFdjYMAJWEPhIAAPh70cDgoGK6cI5B8Yp6S8TACJk4gkA5RAcBKR9BQLoAUOAATNYYOCulUNAAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_pdt_68{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAKVJREFUeF51jlmWwyAMBGXEboT6%2FqedIZAAJqnfer3QJKpGOrkKakW5noIrAlFA5V0EKL%2B8Iqw1d%2B%2FojflTx4JlNUJGnVe1tOBUfRMZYmjDCDKRINFBglCLnXiltnTClfAtEgACxvHJldHF4xYL3gLq1l1Mgfk5AZtQx%2FYfdroL4TySXFeRWTAQc0%2Fhe0FHbRiicsJGZG3iNgUPiimgYBUHlQP94g9%2BZg8xOTGEFAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .policyicon_purpose_5{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYBAMAAAASWSDLAAAAElBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2BtTDCxAAAABXRSTlMAECBAgLf%2B2%2BsAAABGSURBVBhXY2AAA5ZQBwY4YA0NIJfjCjYHygkNDUTmBGPhgOyFc1iB6pE4wSAOUAGCIxoaiOCYhgYjOKqhQThkyODAAR4OAI98N9LK6tL3AAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_purpose_7{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAINJREFUeF6V0UsOxCAIBmB8tVoZ4f6nnUqaoFUW%2FVeEj0hUMOKM9kE7CBcxr93SuGcCf%2FRZniCmXGVUwZV2M78DgYRXQDaAP0OzIJIB4C%2FaQo%2BTCyK9ISFizimAPyuNACjlKXW6SMF30B9I9YFndRieuZCCHKU0QIU1LDEhrvDrQG6EP%2FDZElAL0vLHAAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_purpose_9{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAQAAABKfvVzAAACC0lEQVQ4y7XSO2gWVhQH8BPxDRG%2BEhurMcSI4GsoPqjkZ6BLwcFFHUQJKqbEwRciDqZDF90cpIsILtZHh0KTIdQMgkTRiIshBoWgTRpbsVaxgqRf4uM4JCHfRzpIwXun8%2Bf%2BuHDOifj%2FxwoD2qek7Qat%2FG9Qr1%2FblLRNv%2FqyqKHCjIgIqw3oGE9mmtlQERGhw4DVERFmNFREhG91uq6gxUspnVdlky5dNqlyXkovtSi4rtPe8JeUaq1yWLN9tkVoklJThK1a7HXISrVSehpSGrXb5woWqFZljZNSOmmtBRapUe0Lu4xKOQZSr0633dejS7chKQ25p0%2BvHn3u6Bt7OQFSeuWG3pI6DbvpZ5dc8WwimwTPbYswx49Sei89sDNCpaoI6%2FyqWA5OmxUR4StF6Z0hX5puvyH%2FOmeeudrLwXfjg1prUCo6FuGyty444W89CpYZKQU%2FmF3ywwvVthtxwpwImz1yzjSdpWBYq2nWuzbWoQgX%2FaPOAd%2Br1O55hDOl4LHdDRXqnPVWehLhlPSNgiURFlof4adJMGC7eRERarRKr32t2qBn9lhlg%2BVq7fDbJDhasp%2BfueW9brOscdULv7vntlselnZpadlKH5fSRYvN16ytdJgT4KBGGzVqtNFmv4yndzWrt8WjqSCNGFZUNOxN2Xq8K6%2FD47Et%2FKg7ajAc9edHgz8ciU9%2BPgBKt4%2FTzlslzAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .policyicon_purpose_10,#iubenda_policy .policyicon_purpose_15{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAKVJREFUeF51jlmWwyAMBGXEboT6%2FqedIZAAJqnfer3QJKpGOrkKakW5noIrAlFA5V0EKL%2B8Iqw1d%2B%2FojflTx4JlNUJGnVe1tOBUfRMZYmjDCDKRINFBglCLnXiltnTClfAtEgACxvHJldHF4xYL3gLq1l1Mgfk5AZtQx%2FYfdroL4TySXFeRWTAQc0%2Fhe0FHbRiicsJGZG3iNgUPiimgYBUHlQP94g9%2BZg8xOTGEFAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .policyicon_purpose_13{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAJ1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz9PhkGkAAAADHRSTlMAECBAUHCQoLDA4PB7ua%2BoAAAAa0lEQVR42p3QQQ6AIAxE0aEIFdr7n1eMxIAOMfEt%2B9sF4IOkYt5YSTKO1Qd6p%2BQP6Zqrvyjd7zdiLJggO5VReajwhR%2FBnDIoDwrhQcAfkhd%2FtQO0KDqf1A0kmEZgDjk2AZPzPoJo6wFEYOsHFFISOn%2BKxfoAAAAASUVORK5CYII%3D)}#iubenda_policy .policyicon_purpose_14{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAMFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2Fjai5RAAAAD3RSTlMAECAwUGBwgJCgsMDQ4PASl6hyAAAAfklEQVR42pXRUQ6EMAgE0MEWW21l7n9btanJWnE3%2Bz4hhCHgq5jKooKD6FJS7OVQebIIROOphlY3dqrsLABidJgg0ZWw0bWBL%2F5vvO%2FIdGVM%2Fh0TMNMx47DwYcVJKgdV0MgwUwSXfA%2F0QY2dKW7CxutHA1lbHMFTavE9qsBvOztlFTRVyS%2BYAAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_purpose_16{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAJFJREFUeF6V0NsOAyEIRVE6I4rFwvn%2Fr63N3CR10nQnPK2IUdpbpKmsorJQqOKTl2xeRhDsycMgA7QDGkmfq9cI%2FvNEhGcAO8CowAbAGTEwX1XDKvYNnJM7f78clVqfydOlgwRIG6S1TwDdQEnD3cv1iWw4f54VQ1qfUO5QDDGYVLNCmOQ5O2Ea8R2kP8FWobvefhoT%2FSVCMbAAAAAASUVORK5CYII%3D)}#iubenda_policy .icon_ribbon{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAW0lEQVR42u3OwQkAIQxE0XSWVrazlJpdQdGDC0pQEf7A3ELmibsPV1V9pDM%2FAQAAAAAAAAAAAAAAEAXY1%2BcUwCQnITYD6niL2ASo4z3EaoDKf8qNBQHxArgK8ALKMXCw%2Bim7vwAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .icon_owner{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAMFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2Fjai5RAAAAD3RSTlMAECAwQGBwgJCgsMDQ4PC8YWy5AAAAiElEQVR42o2QwRKFIAhFIcwyRP7%2Fb3uNlkBv0dkw3jODd4AbPHhNC7xAafqjYBRZOzUa0cHmc9IbiZsefIFtiuQ68RS7FUkNnwTWmRewLE9ewSPh73dfCgJbzxkiRxcrDGJhWVxa5MqYr1HzcLSPRo2ojcoZAcyV2F1MzaPoxIqcP4gGkP5BcAIxQBCQ7o5t3AAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .icon_general{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYBAMAAAASWSDLAAAAGFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz9%2BjSc3AAAAB3RSTlMAEEBQgMzQxeXuPgAAADJJREFUGFdjYMAJWEPhIAAPh70cDgoGK6cI5B8Yp6S8TACJk4gkA5RAcBKR9BQLoAUOAATNYYOCulUNAAAAAElFTkSuQmCC)}#iubenda_policy .icon_temple_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABwklEQVR42s3Wu0vDUBjGYS%2BLsbZSSaWgguAFHFztYEmFbp0E%2FwOrgotQFyetOKiTLqKCWCenbl20S8FFERydBLt1KV7QwUGR4094hQymjYpi4SGH9zvf%2BUgCoQ3GmF%2F1dwNq%2FRzHaUwkEn24lP73rEaL%2FwEcZmEcJexiDyfKrG8P0OG9OIDBrCvPKMuh98sDaApiAmWYj8fiqg%2FjSrWy9gbrDlDzEHIwLi9YRieiWMOrakIPvZ4DKHYhjTsYD%2Be48Kqrdwpdnw1I4RAFbCKHHWxhX%2BtjHGFb2ZbynHoKOiNV7x3YrnWLrmFFWqvm6vH7DmK4ho0l5NGGCialoiyvPbZ6Yn4GOHhCFBsoIQSDOTHKStoTVY%2FjZ0Act7CxiiICqGJaqsqK2mOrJ%2F6VARGs6ZA2ZTNyq6yoPZF%2FNWC0xiOaEq9HNOpnQBIG3djFGcLKFsQoO8UOepQl%2FQyIIKtP9BjSylcwghhWlKWR0N4sIp4D1NCKDgR0DSIEGxbCYikLibvH8voWNWMdD6jiEXe4waOye1GdGntc9Qcso8nrDtoxgEFdIcp81INed7CIBWQw%2F00ZnbH42YAXef4RnfNn%2FyreALybXwSLU3v7AAAAAElFTkSuQmCC)}#iubenda_policy .icon_box_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABv0lEQVR42t3Vz0uTcRzAcUMyWhmWdAgqkKDMiBHt0A%2FYsploddwpO1gk0l%2BQEEQU0iUPgd0LIpCOCh2KkG4GTaI6mqAmWhG0CQ5jfXsdntN4bJPRxS%2B84IFnz%2Ff97Nl4Pg0hhP9qkwT%2BtTKZTCN7uM0qeTrZuc4ltQVs0EqK%2B3xmigc8Z5E39HOI7TUFfHAbJxngNQtM0kdzg5VOp7c4TvKYeeZ4wmXaYgNONHGcW7zjA6Mkqzy%2BZq4zzgxj5DhcGUgxwzSZ9TasEtvFCL%2F4WBm4SKDAPXrZV%2BPGWznFVSYIhMpAliILhEieO5ynMWbjDgZ4xjxlAn%2FiAt0skeMG44TIT8boo51zDPOeEqFSXKAnCrRHd5fgNMN8IrDCFLOUCVB74CsdZBlkL03s5xG%2FCcAGA73M0cIViswyQisn%2BFZPoIdljkWP6AIvKDFIiuV6Al2s8JIciSh0hqNk%2BVHvNwiRNd5ylwNRqKvewNnYv1z0O%2FCQ7xsIFCsDCS4xyhKhwiprhCqmGaIz%2Fm0qxBGu8YoCoYpFntLNwbS3ba3zYDdJhshTohwpMEE%2FbeyoMg%2BqTrQWbvKFSSxDJn5tsqH%2FF0QW2NxzTlYFAAAAAElFTkSuQmCC)}#iubenda_policy .icon_tools_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABdklEQVR42rXVzyuDcRzA8WU3ctOag0RiO5mEg8MKcaJc%2FAlcdxppKPlZdpeTE0dqxZWaaEnh7DShlYuJbG0f78Nz%2BPj2zfM89Wz1qmff5%2FPdu%2B27tpCINNTfJzySyeQGhkPGg7UljBtrEbxDMOkaYCiKJ8QtgR0cGWt9EMe8l8AIBAOWwCGKxtqMCux5CSRQxyW61QtNo4yCEVhWgRzCboFm5CF4xTVuUYUgZQTOVeAZHV4OeRSfEMMFWoxAVt2%2FQtQ14Gzsx43anEWr5Vx61Eza9Qz%2B%2BXw71S09M6hm1v0GVtXmWCMCa2pz3BpgXc1kAg2w1oW0mjnGRJCBOYjhLshAO96MQCroM3hQMzUMBfkOZvEDUU78BFbUxl5LYBdiqPgJbKmNCUtg2xL48PpTMYVvFFDEPdqCDDwi51xHIVi0%2FAGJoew18IJ957oJFWx6CHx5DSygjgPkUULM8i2qGoFTP4ecgaCEMcshh5FFDYIzRGyBhvoF3n%2ByMxzF1ykAAAAASUVORK5CYII%3D)}#iubenda_policy .icon_paper_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABYklEQVR42t3VP0vDQBjH8Tq4SKXiWFwcRHARVyspgq9AOjkoLoKTcymk%2BjKKYDcnO6iLKPgHRJ11aVGkgt2M2IiWlobzKzyB4zBwBGvBwIdc7rnjR8ITLqGU6qm%2FC8hms%2Bo39TWgg0fUUJX7PV7RlVo1Qtsm4Ckhl%2BM4A%2BGY%2BQJ8TCYiLmp1m4AHWbyGa%2BxiFEtQMneIY80RTtCyCahJwDpOsYc0FtHGDS5wbjjDp03AM6aRRhIpTGAbH5jBEJIm208UwMcbmuIFHam34KEZ0tYGNgEeXFEUW9jAKvLYRFHjCs8moIEMZpHRxnNwzJrx3Oj%2Fj2a%2BQbT4b%2BDBjcmz6iK9M6LF76I6UnHY%2Fgc%2BythB2YK%2B1tcC%2Ful54COPMeT0tsMBxsW%2B0dY52VPAe1RAgAoGw7OA8QoUbvVzgPEU7qS2HJ4b33tRQfBTQBcl4wBZgMIlhrX5EVxJbd7YU0JXD%2BipLw8sG8DBrCLzAAAAAElFTkSuQmCC)}#iubenda_policy .icon_man_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABLUlEQVR42t3VsUrDUBSAYaWtSwSp6NAH6CbOVSHZ9QEEBx9AEPc6OAh9Bp0KDg6igqs4tktXFQQnKQiKiNRAp%2BT4C2cImqbXc3Fp4VsazvlpuUmmRORfTUig6BNFURnbeISoB2yhlDPiHvhegF18Qn74wA5KPoE13EFGuEXDFGBwBoeQMQ5QsQSqOHUInGDOEljElUPgEguWwDzOHQJnqFoCszh2CBwhsAQq2EdSsDxFE2XrMV3HS0HgFRs%2B90ENNwWBa9TMgTAMp%2FWR8J6z%2FA2bXo8K%2FRXLuB9xFy%2BZAwwHWMUF4pxArNdWnE%2BRLm2ghS76SMecoj66aOls8CvAl3XsoYNnDCF%2FNNTZju6qZwO93L%2FBLkYvGxggVeIpVYNsoI0nJBBPie5qT8ZL%2FwsLLryq%2FnnTDAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .icon_keyhole_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABIUlEQVR42rXUP0vCQRjA8bIoiAppLmwQEmehSX5RLTb2Huw9RGODLvUCXG0Kp16ALhENNRjRXLRlIeafJOyevkNu14M89%2FPgMx133%2BF4bkZEpkrdHK8oipIoowuHK2QxGxzgkk1cYgD3R9BEAQlzgMOruMA3xOMZuZDAEToQxRkWrYEHOIiiibQ1IBMEOtixBn4mCLSRtwbqIKIGbrFhDRzgA6I4xpw1kMA5ep6LHa6RCh20ddx4Aq%2FYj2OSF1D3BJ6QjCOQwosn8IbtOAK7%2BPQEvlAcf3ghj1zE4J9HrmApJDCPkvLZ3WMtJLCCmjLNLWRCAmk8KkPWxyHMgQLaSmCIk5BJPkVfCYxQxbI10MBQCTjcYcsaeMcIomhhTwtM1S9g12NLa1YPRQAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .iub_base_container{border-radius:3px;background:#ffffff;color:#6B6B6B;position:relative}#iubenda_policy .iub_base_container>.close{background:transparent url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABcAAAAYCAMAAAAmopZHAAAAw1BMVEUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAB4eHh1dXUAAAAAAAAAAAAAAAAAAABfX18AAAAAAAAAAAAAAAAAAAAAAAA2NjYAAAAAAAArKyvJycne3t7X19eFhYWxsbGVlZWsrKzr6%2BvLy8vJycnv7%2B%2Fp6enS0tLi4uL09PTv7%2B%2F8%2FPz7%2B%2Fv4%2BPj39%2FcAAABPT09fX19vb2%2F%2F%2F%2F9S%2BfXQAAAAPHRSTlMAAgMEBQYHCgsMDQ4PEhMWGRobHB8gIiMkJScoKSs0NT1DRUpMWF5gjpOYmaGjpr%2FIys3S1dnZ7vP09vfFQC13AAAA9ElEQVR42oXQZ6%2BCMBiG4aeCAoqiuPceuPes8P7%2FX6Xn5RgBTbw%2BNO3dpG2KH0RcM5JJQ4uLUE2UnSM9HZ1y4r0TM50z%2FTs7ZuyVSysKWJX8DZHeUsg2zUfpU4qY6gBE8xLtl6YAtAnP79Ij8uSdFxMNsHY8lVK67nPgxc4CisQ8yTxiRaBGPvcvu%2BSrAY1vvQHUv51TByqHz3sPFcCef75zbgOpwZUiroMUoFSX0b6sKgDMzjqc1x2Tvznb2wTzppf1P1q1u7PTq55mXVuFT7Va48X%2BRnTbL8YtizMTRqHdH45Gw367YAgEKHoml8%2FnMroC9gCKfVabzD1q%2BwAAAABJRU5ErkJggg%3D%3D) no-repeat;border:none;display:block;position:absolute;z-index:110;top:-10px;right:-9px;height:24px;width:23px}#iubenda_policy p{line-height:19px;margin:0;padding-top:11px}#iubenda_policy address{margin:0;line-height:inherit;display:inline}#iubenda_policy a{font-weight:normal;border-bottom:1px solid #F0F0F0}#iubenda_policy .iub_content{position:relative;padding:25px 30px;margin:0 auto;border-radius:3px 3px 0 0}#iubenda_policy #wbars{position:relative;overflow-y:auto;overflow-x:hidden}#iubenda_policy #wbars .horizontal{display:none}#iubenda_policy .iub_header{border-bottom:1px dotted #DFDFDF;padding-bottom:25px;position:relative}#iubenda_policy .iub_header p{margin:0;padding:0}#iubenda_policy .iub_header img{display:block;position:absolute;top:5px;right:0}#iubenda_policy h1,#iubenda_policy h2,#iubenda_policy h3{color:#3F3F3F;margin:0}#iubenda_policy h1+p,#iubenda_policy h2+p,#iubenda_policy h3+p{padding-top:5px}#iubenda_policy h1{font-size:19px;font-weight:normal;line-height:23px;margin-bottom:5px}#iubenda_policy h2{font-size:17px;font-weight:bold;line-height:21px;padding-top:21px}#iubenda_policy h3{font-size:13px;line-height:19px;font-weight:bold;padding-top:24px}#iubenda_policy h3+p{padding-top:0}#iubenda_policy .iconed ul li h3{padding-top:10px;color:#615e5e}#iubenda_policy h4{font-size:13px;font-weight:bold;padding-top:19px;margin-bottom:0}#iubenda_policy h4:first-child{padding-top:0}#iubenda_policy ul.for_boxes,#iubenda_policy ul.for_boxes>li,#iubenda_policy ul.unstyled,#iubenda_policy ul.unstyled>li{list-style:none;padding:0;margin:0}#iubenda_policy ul.for_boxes{zoom:1}#iubenda_policy ul.for_boxes:before,#iubenda_policy ul.for_boxes:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy ul.for_boxes:after{clear:both}#iubenda_policy .half_col{float:left;width:50%;zoom:1}#iubenda_policy .half_col:before,#iubenda_policy .half_col:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy .half_col:after{clear:both}#iubenda_policy .half_col:nth-child(2n+1)>*{margin-right:15px}#iubenda_policy .half_col:nth-child(2n)>*{margin-left:15px}#iubenda_policy .half_col+.one_line_col,#iubenda_policy .half_col+.iub_footer{border-top:1px dotted #DFDFDF}#iubenda_policy .one_line_col{zoom:1;float:left;width:100%;border-bottom:1px dotted #DFDFDF}#iubenda_policy .one_line_col:before,#iubenda_policy .one_line_col:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy .one_line_col:after{clear:both}#iubenda_policy .one_line_col>ul.for_boxes>li{float:left;width:50%}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1){clear:left}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:15px}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n){clear:right}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:15px}#iubenda_policy .one_line_col.wide{width:100%}#iubenda_policy .one_line_col.wide>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy .one_line_col.wide>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy .one_line_col.wide>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy ul.normal_list{list-style:disc;display:block;padding-top:11px}#iubenda_policy ul.normal_list li{list-style:disc;float:none;line-height:19px;margin:5px 25px}#iubenda_policy .simple_pp>ul>li{padding-bottom:21px}#iubenda_policy .simple_pp>ul>li>ul .iconed{padding-left:40px;background-repeat:no-repeat;background-color:transparent;background-position-x:2px;background-position-y:26px;background-position:2px 26px}#iubenda_policy .simple_pp .for_boxes>.one_line_col>ul.for_boxes{margin-top:0}#iubenda_policy .legal_pp .one_line_col{float:none;border-top:0;padding-bottom:21px}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes{margin-top:21px}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n+1){clear:left;float:left}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n){float:right;clear:right}#iubenda_policy .legal_pp .definitions{margin-top:21px}#iubenda_policy .legal_pp .definitions .expand-click.w_icon_24{margin-top:-11px;padding:14px 10px 12px 45px;background-repeat:no-repeat;background-color:transparent;background-position-x:5px;background-position-y:0;background-position:5px 0}#iubenda_policy .legal_pp .definitions .expand-content{padding-left:5px;padding-right:5px}#iubenda_policy .wrap p{display:inline-block}#iubenda_policy .iub_footer{clear:both;position:relative;font-size:11px}#iubenda_policy .iub_footer p{font-size:11px;padding:0}#iubenda_policy .iub_content .iub_footer{padding:24px 0}#iubenda_policy .iub_content .iub_footer p{margin:10px 0;clear:both}#iubenda_policy .iub_content .iub_footer .show_comp_link{display:block;float:right}#iubenda_policy .iub_container>.iub_footer{min-height:21px;background-color:#F6F6F6;color:#717171;padding:30px;-webkit-box-shadow:0 -1px 6px #cfcfcf;box-shadow:0 -1px 6px #cfcfcf;border-radius:0 0 3px 3px}#iubenda_policy .iub_container>.iub_footer>.btn{position:absolute;top:25px;right:30px}#iubenda_policy .iub_container>.iub_footer .btn{padding:0px 24px;line-height:29px}#iubenda_policy .iub_container>.iub_footer .button-stack{margin:-4px 0}#iubenda_policy .iub_container>.iub_footer .button-stack .btn+.btn{margin-left:5px}#iubenda_policy .iub_container>.iub_footer img{margin:-4px 3px 0;vertical-align:middle;width:70px;height:25px}#iubenda_policy .wide{width:150px}@media (max-width: 767px){#iubenda_policy .legal_pp .one_line_col,#iubenda_policy .legal_pp .half_col{width:100%}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li,#iubenda_policy .legal_pp .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy .legal_pp .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy .legal_pp .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy .iub_header img{position:static;margin-bottom:12.5px}#iubenda_policy .iub_content>.iub_footer .show_comp_link{position:static;display:inline}#iubenda_policy .iub_container>.iub_footer{padding:20px}#iubenda_policy .iub_container>.iub_footer .btn{top:15px;right:15px}#iubenda_policy .iub_base_container>.close{content:"X";color:#000;font-size:11px;line-height:18px;padding:0;text-align:center;border-radius:30px;display:block;background:#fff url(../design/images/close_big.png) no-repeat;background-position-x:18px;background-position-y:18px;background-position:18px 18px;position:absolute;z-index:110;top:-10px;right:-10px;margin:5px 5px 0 0;height:57px;width:60px;-webkit-box-shadow:0 1px 1px #000000;box-shadow:0 1px 1px #000000}#iubenda_policy .iub_base_container>.close.small{width:14px;line-height:14px;border-radius:9px;padding:0}}@media (max-width: 480px){html#iubenda_policy{padding:0}#iubenda_policy body{padding:0}#iubenda_policy .iub_base_container,#iubenda_policy .iub_container{margin:0}#iubenda_policy .half_col:nth-child(2n+1)>*{margin-right:0}#iubenda_policy .half_col:nth-child(2n)>*{margin-left:0}#iubenda_policy .one_line_col,#iubenda_policy .half_col{width:100%}#iubenda_policy .one_line_col>ul.for_boxes>li,#iubenda_policy .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy .iub_header img{position:static;margin-bottom:12.5px}#iubenda_policy .iub_content>.iub_footer .show_comp_link{position:static;display:inline}#iubenda_policy .iub_container>.iub_footer{padding:10px;text-align:center}#iubenda_policy .iub_container>.iub_footer .btn{position:static;width:auto;display:block;margin:10px auto 0 auto;max-width:200px}#iubenda_policy .iub_container>.iub_footer.in_preview{padding:30px 10px}#iubenda_policy .iub_content{padding-left:20px;padding-right:20px}#iubenda_policy .iub_base_container>.close{content:"X";color:#000;font-size:11px;line-height:18px;padding:0;text-align:center;border-radius:30px;display:block;background:#fff url(../design/images/close_big.png) no-repeat;background-position-x:18px;background-position-y:18px;background-position:18px 18px;position:absolute;z-index:110;top:-10px;right:-10px;margin:5px 5px 0 0;height:57px;width:60px;-webkit-box-shadow:0 1px 1px #000000;box-shadow:0 1px 1px #000000}#iubenda_policy .iub_base_container>.close.small{width:14px;line-height:14px;border-radius:9px;padding:0}}#iubenda_policy.iubenda_fixed_policy .iub_base_container{max-width:800px}#iubenda_policy.iubenda_fixed_policy .iub_container{margin-left:auto;margin-right:auto;zoom:1}#iubenda_policy.iubenda_fixed_policy .iub_container:before,#iubenda_policy.iubenda_fixed_policy .iub_container:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy.iubenda_fixed_policy .iub_container:after{clear:both}#iubenda_policy.iubenda_fluid_policy #wbars{overflow-y:auto;-webkit-box-shadow:none;box-shadow:none;height:auto}#iubenda_policy.iubenda_fluid_policy .iub_container{margin-top:30px;margin-bottom:30px}#iubenda_policy.iubenda_fluid_policy .half_col:nth-child(2n+1)>*{margin-right:0}#iubenda_policy.iubenda_fluid_policy .half_col:nth-child(2n)>*{margin-left:0}#iubenda_policy.iubenda_fluid_policy .one_line_col,#iubenda_policy.iubenda_fluid_policy .half_col{width:100%}#iubenda_policy.iubenda_fluid_policy .one_line_col>ul.for_boxes>li,#iubenda_policy.iubenda_fluid_policy .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy.iubenda_fluid_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy.iubenda_fluid_policy .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy.iubenda_fluid_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy.iubenda_fluid_policy .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy.iubenda_embed_policy .iub_base_container{background:none}#iubenda_policy.iubenda_embed_policy .iub_container>.iub_footer{-webkit-box-shadow:none;box-shadow:none;border-radius:none}#iubenda_policy.iubenda_embed_policy .expand-click{cursor:default}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .iub_base_container{color:#666}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h2{font-size:24px;padding-top:50px}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h3{color:#444;font-size:20px;padding-top:45px}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h4{font-size:16px;padding-top:40px;color:#555}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h5{font-size:14px;padding-top:35px;margin-bottom:0;color:#666}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h6{font-size:12px;color:#505050;text-transform:uppercase;padding-top:32px;margin-bottom:0}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions{margin-top:60px !important}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions .expand-content{padding:25px 15px !important}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions .expand-content h4{font-size:15px !important}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions:before{content:"";border-top:1px dotted rgba(0,0,0,0.1);display:block;margin:0 -10px;position:relative;top:-45px}#iubenda_policy.iubenda_vip_policy.iubenda_fixed_policy .iub_container{max-width:660px;padding-top:80px}#iubenda_policy.iubenda_vip_policy .iub_base_container{color:#6B6B6B}#iubenda_policy.iubenda_vip_policy p{font-size:14px;line-height:1.6}#iubenda_policy.iubenda_vip_policy .allcaps,#iubenda_policy.iubenda_vip_policy p.allcaps,#iubenda_policy.iubenda_vip_policy ul.allcaps li{font-variant:small-caps !important;font-weight:bold !important;font-size:16px !important;font-family:-apple-system, BlinkMacSystemFont, Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif !important}#iubenda_policy.iubenda_vip_policy ul li{font-size:14px;line-height:1.6}#iubenda_policy.iubenda_vip_policy h1{font-size:30px;color:#141414;line-height:1.6;margin-bottom:60px}#iubenda_policy.iubenda_vip_policy h2{font-size:18px;color:#141414;line-height:1.6;padding-top:50px;padding-bottom:15px}#iubenda_policy.iubenda_vip_policy h3{color:#141414;font-size:16px;line-height:1.6;margin-bottom:10px}#iubenda_policy.iubenda_vip_policy .legal_pp .one_line_col{padding-bottom:50px}#iubenda_policy.iubenda_vip_policy .half_col:nth-child(2n+1)>*{margin-right:0}#iubenda_policy.iubenda_vip_policy .half_col:nth-child(2n)>*{margin-left:0}#iubenda_policy.iubenda_vip_policy .one_line_col,#iubenda_policy.iubenda_vip_policy .half_col{width:100%}#iubenda_policy.iubenda_vip_policy .one_line_col>ul.for_boxes>li,#iubenda_policy.iubenda_vip_policy .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy.iubenda_vip_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy.iubenda_vip_policy .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy.iubenda_vip_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy.iubenda_vip_policy .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy.iubenda_vip_policy .definitions,#iubenda_policy.iubenda_vip_policy .iub_footer,#iubenda_policy.iubenda_vip_policy .for_boxes{color:#59636D}#iubenda_policy.iubenda_vip_policy .definitions h3,#iubenda_policy.iubenda_vip_policy .iub_footer h3,#iubenda_policy.iubenda_vip_policy .for_boxes h3,#iubenda_policy.iubenda_vip_policy .definitions p,#iubenda_policy.iubenda_vip_policy .iub_footer p,#iubenda_policy.iubenda_vip_policy .for_boxes p,#iubenda_policy.iubenda_vip_policy .definitions li,#iubenda_policy.iubenda_vip_policy .iub_footer li,#iubenda_policy.iubenda_vip_policy .for_boxes li{font-size:13px}#iubenda_policy.iubenda_vip_policy .w_icon_24{background-image:none}#iubenda_policy.iubenda_vip_policy .box_10.expand .expand-click.w_icon_24{padding-left:10px}#iubenda_policy.iubenda_vip_policy .box_primary{border-color:#E0E0E0;border-bottom-color:#D3D3D3;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy.iubenda_vip_policy .box_primary h3{color:#333}#iubenda_policy.iubenda_vip_policy .tc-deactivated h1{font-size:20px;margin-bottom:10px}#iubenda_policy.iubenda_vip_policy .legal_pp .one_line_col{padding-bottom:21px}
+html#iubenda_policy,#iubenda_policy body{margin:0;padding:0}html#iubenda_policy{overflow-y:scroll;font-size:100%;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}#iubenda_policy h1,#iubenda_policy h2,#iubenda_policy h3,#iubenda_policy h4,#iubenda_policy h5,#iubenda_policy h6,#iubenda_policy p,#iubenda_policy blockquote,#iubenda_policy pre,#iubenda_policy a,#iubenda_policy abbr,#iubenda_policy acronym,#iubenda_policy address,#iubenda_policy cite,#iubenda_policy code,#iubenda_policy del,#iubenda_policy dfn,#iubenda_policy em,#iubenda_policy img,#iubenda_policy q,#iubenda_policy s,#iubenda_policy samp,#iubenda_policy small,#iubenda_policy strike,#iubenda_policy strong,#iubenda_policy sub,#iubenda_policy sup,#iubenda_policy tt,#iubenda_policy var,#iubenda_policy dd,#iubenda_policy dl,#iubenda_policy dt,#iubenda_policy li,#iubenda_policy ol,#iubenda_policy ul,#iubenda_policy fieldset,#iubenda_policy form,#iubenda_policy label,#iubenda_policy legend,#iubenda_policy button,#iubenda_policy table,#iubenda_policy caption,#iubenda_policy tbody,#iubenda_policy tfoot,#iubenda_policy thead,#iubenda_policy tr,#iubenda_policy th,#iubenda_policy td{margin:0;padding:0;border:0;font-weight:normal;font-style:normal;font-size:100%;line-height:1;font-family:inherit}#iubenda_policy table{border-collapse:collapse;border-spacing:0}#iubenda_policy ol,#iubenda_policy ul{list-style:none}#iubenda_policy q:before,#iubenda_policy q:after,#iubenda_policy blockquote:before,#iubenda_policy blockquote:after{content:""}#iubenda_policy a:focus{outline:thin dotted}#iubenda_policy a:hover,#iubenda_policy a:active{outline:0}#iubenda_policy article,#iubenda_policy aside,#iubenda_policy details,#iubenda_policy figcaption,#iubenda_policy figure,#iubenda_policy footer,#iubenda_policy header,#iubenda_policy hgroup,#iubenda_policy nav,#iubenda_policy section{display:block}#iubenda_policy audio,#iubenda_policy canvas,#iubenda_policy video{display:inline-block;*display:inline;*zoom:1}#iubenda_policy audio:not([controls]){display:none}#iubenda_policy sub,#iubenda_policy sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}#iubenda_policy sup{top:-0.5em}#iubenda_policy sub{bottom:-0.25em}#iubenda_policy img{border:0;-ms-interpolation-mode:bicubic}#iubenda_policy button,#iubenda_policy input,#iubenda_policy select,#iubenda_policy textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}#iubenda_policy button,#iubenda_policy input{line-height:normal;*overflow:visible}#iubenda_policy button::-moz-focus-inner,#iubenda_policy input::-moz-focus-inner{border:0;padding:0}#iubenda_policy button,#iubenda_policy input[type="button"],#iubenda_policy input[type="reset"],#iubenda_policy input[type="submit"]{cursor:pointer;-webkit-appearance:button}#iubenda_policy input[type="search"]{-webkit-appearance:textfield;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}#iubenda_policy input[type="search"]::-webkit-search-decoration{-webkit-appearance:none}#iubenda_policy textarea{overflow:auto;vertical-align:top}html#iubenda_policy{-webkit-font-smoothing:antialiased}#iubenda_policy p{font-size:13px;font-weight:normal;line-height:18px;margin-bottom:9px}#iubenda_policy p small{font-size:11px;color:#bfbfbf}#iubenda_policy h1,#iubenda_policy h2,#iubenda_policy h3,#iubenda_policy h4,#iubenda_policy h5,#iubenda_policy h6{font-weight:bold;color:#59636D}#iubenda_policy h1{margin-bottom:18px;font-size:30px;line-height:2}#iubenda_policy h1 small{font-size:18px}#iubenda_policy h2{font-size:24px;margin-bottom:18px;line-height:1.5}#iubenda_policy h2 small{font-size:14px}#iubenda_policy h3,#iubenda_policy h4,#iubenda_policy h5,#iubenda_policy h6{margin-bottom:9px}#iubenda_policy h3{font-size:18px}#iubenda_policy h3 small{font-size:14px}#iubenda_policy h4{font-size:16px}#iubenda_policy h4 small{font-weight:bold;font-size:13px}#iubenda_policy h5{font-size:13px;padding-top:19px}#iubenda_policy h6{font-size:13px;color:#bfbfbf;text-transform:uppercase}#iubenda_policy ul ul,#iubenda_policy ul ol,#iubenda_policy ol ol,#iubenda_policy ol ul{margin:0}#iubenda_policy ul.styled,#iubenda_policy ul{list-style:disc;padding-top:5px}#iubenda_policy ul.styled li,#iubenda_policy ul li{list-style:disc;line-height:19px;font-size:13px;margin-left:30px;margin-top:2px}#iubenda_policy ol{list-style:decimal}#iubenda_policy ul.unstyled{list-style:none;margin-left:0}#iubenda_policy dl{margin-bottom:18px}#iubenda_policy dl dt,#iubenda_policy dl dd{line-height:18px}#iubenda_policy dl dt{font-weight:bold}#iubenda_policy dl dd{margin-left:9px}#iubenda_policy hr{margin:0 0 19px;border:0;border-bottom:1px solid #eee}#iubenda_policy strong{font-style:inherit;font-weight:bold}#iubenda_policy em{font-style:italic;font-weight:inherit;line-height:inherit}#iubenda_policy .muted{color:#bfbfbf}#iubenda_policy blockquote{margin-bottom:18px;border-left:5px solid #eee;padding-left:15px}#iubenda_policy blockquote p{font-size:14px;font-weight:300;line-height:18px;margin-bottom:0}#iubenda_policy blockquote small{display:block;font-size:12px;font-weight:300;line-height:18px;color:#bfbfbf}#iubenda_policy blockquote small:before{content:'\2014 \00A0'}#iubenda_policy address{display:block;line-height:18px;margin-bottom:18px}#iubenda_policy code,#iubenda_policy pre{padding:0 3px 2px;font-family:Monaco, Andale Mono, Courier New, monospace;font-size:12px;border-radius:3px}#iubenda_policy code{background-color:#fee9cc;color:rgba(0,0,0,0.75);padding:1px 3px}#iubenda_policy pre{background-color:#f5f5f5;display:block;padding:17px;margin:0 0 18px;line-height:18px;font-size:12px;border:1px solid #ccc;border:1px solid rgba(0,0,0,0.15);border-radius:3px;white-space:pre;white-space:pre-wrap;word-wrap:break-word}#iubenda_policy .breadcrumbs{padding:0 0 10px 0;margin-bottom:30px;border-bottom:1px solid #F6F6F6;width:100%}#iubenda_policy .breadcrumbs>li{float:left;filter:alpha(opacity=50);-khtml-opacity:0.5;-moz-opacity:0.5;opacity:0.5}#iubenda_policy .breadcrumbs>li:not(:last-child):after{color:#333B43;padding:0 10px;content:"\203a"}#iubenda_policy .breadcrumbs+.pills,#iubenda_policy .breadcrumbs+.sec_tabs{margin-top:-15px}#iubenda_policy .table{display:table;border-collapse:collapse;padding:0 !important;margin:0}#iubenda_policy .cust_row{display:table-row;margin:0}#iubenda_policy .column{display:table-cell;vertical-align:top;padding:30px}#iubenda_policy .box_primary{border:1px solid #C0C1C1;border-bottom-color:#A8AAAB;-webkit-box-shadow:0 1px 0 #ebebec;box-shadow:0 1px 0 #ebebec;-webkit-box-shadow:0 1px 0 rgba(0,0,0,0.1);box-shadow:0 1px 0 rgba(0,0,0,0.1);background:#FFF}#iubenda_policy .box_content{border-radius:4px;padding:30px}#iubenda_policy .box_content .iub_content{padding:30px}#iubenda_policy .box_content .iub_content>hr{width:686px;margin-left:-30px;margin-right:-30px}#iubenda_policy .box_content .aside{width:191px;padding:30px}#iubenda_policy .box_content .aside.aside-right{border-left:1px solid #DFDFDF}#iubenda_policy .table>.box_content{padding:0}#iubenda_policy .box_10{padding:10px;border-radius:3px;margin-bottom:15px}#iubenda_policy .box_10>h4{margin-bottom:0;font-size:13px}#iubenda_policy .box_10>.w_icon,#iubenda_policy .box_10.expand>.w_icon,#iubenda_policy .box_10>.w_icon.expand-click,#iubenda_policy .box_10.expand>.w_icon.expand-click{padding-left:45px;background-repeat:no-repeat;background-color:transparent;background-position-x:10px;background-position-y:7px;background-position:10px 7px}#iubenda_policy .box_10>.w_icon_16,#iubenda_policy .box_10.expand>.w_icon_16,#iubenda_policy .box_10>.w_icon_16.expand-click,#iubenda_policy .box_10.expand>.w_icon_16.expand-click{padding-left:40px;background-repeat:no-repeat;background-color:transparent;background-position-x:11px;background-position-y:11px;background-position:11px 11px}#iubenda_policy .box_10>.w_icon_24,#iubenda_policy .box_10.expand>.w_icon_24,#iubenda_policy .box_10>.w_icon_24.expand-click,#iubenda_policy .box_10.expand>.w_icon_24.expand-click{padding-left:45px;background-repeat:no-repeat;background-color:transparent;background-position-x:10px;background-position-y:10px;background-position:10px 10px}#iubenda_policy .box_5{padding:5px;border-radius:3px;font-size:11px;margin-bottom:15px}#iubenda_policy .box_5 hr{padding-top:5px;margin:0 -5px 5px -5px;border:0;border-bottom:1px solid #AC3737}#iubenda_policy .box_5.w_icon_16{padding-left:30px;background-repeat:no-repeat;background-position-x:8px;background-position-y:6px;background-position:8px 6px}#iubenda_policy .box_5.w_icon_16 hr{width:100%;padding-left:30px;padding-right:5px;margin-left:-30px;margin-right:-5px}#iubenda_policy .box_5.w_icon_16.red{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAATlBMVEUAAAD%2F%2F%2F8AAAD%2F%2F%2F8AAAAAAAD%2F%2F%2F%2F%2F%2F%2F%2FT09P%2F%2F%2F%2F9%2Ff3Y2Nj9%2Ff39%2Ff3d3d3%2F%2F%2F%2F8%2FPz39%2Ff19fX%2B%2Fv79%2Ff34%2BPj5%2Bfn8%2FPz9%2Ff3%2F%2F%2F8ZO4GEAAAAGXRSTlMAEB0gMDNAUHSAgYSRoaWwsra3weLl5fLyUJhrdwAAAF1JREFUeF6NzUcWhCAAwFAQsIPOWCD3v6gPxLYjy7%2BJKE1Ok%2FxAD%2BMbFIB6wYIxLA%2FUbEJAc8PKHmG9oAOkArq8DICdgXCuLUA7EDkBsd%2BfWALnyXmXoNImpytR0AEwdQcUE5t8VQAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .box_thumb{background:#FFF;-webkit-box-shadow:0 0 1px #a3a3a3, 0 1px 1px #a3a3a3;box-shadow:0 0 1px #a3a3a3, 0 1px 1px #a3a3a3;padding:6px}#iubenda_policy footer{margin-top:17px;padding-top:17px;border-top:1px solid #eee}#iubenda_policy hr{padding-top:15px;margin:0 0 15px 0}#iubenda_policy hr.primary{border:0;border-bottom:1px solid #DFDFDF;-webkit-box-shadow:0 1px 0 #f7f7f7;box-shadow:0 1px 0 #f7f7f7}#iubenda_policy .btn{cursor:pointer;display:inline-block;font-weight:bold;background-color:rgba(0,0,0,0.08);padding:0 20px;line-height:38px;color:#54616B;font-size:13px;border:0;border-radius:4rem;border-collapse:separate;-webkit-transition:0.1s linear all;transition:0.1s linear all}#iubenda_policy .btn:hover{background-position:0 -15px;text-decoration:none}#iubenda_policy .btn:focus{outline:1px dotted #666}#iubenda_policy .btn.primary{color:#fff;background-color:#0073CE}#iubenda_policy .btn:active{-webkit-box-shadow:inset 0 2px 4px rgba(0,0,0,0.25),0 1px 2px rgba(0,0,0,0.05);box-shadow:inset 0 2px 4px rgba(0,0,0,0.25),0 1px 2px rgba(0,0,0,0.05)}#iubenda_policy .btn.disabled{cursor:default;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=65);-khtml-opacity:0.65;-moz-opacity:0.65;opacity:0.65;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy .btn[disabled]{cursor:default;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=65);-khtml-opacity:0.65;-moz-opacity:0.65;opacity:0.65;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy .btn.large{font-size:16px;line-height:normal;padding:0 14px;border-radius:6px}#iubenda_policy .btn.mid_large{padding:0 10px;line-height:32px;font-size:13px}#iubenda_policy .btn.mid{padding:0 10px;line-height:28px;font-size:11px}#iubenda_policy .btn.small{padding:0 8px;line-height:18px;font-size:11px}#iubenda_policy :root .alert-message,#iubenda_policy :root .btn{border-radius:0 \0}#iubenda_policy button.btn::-moz-focus-inner,#iubenda_policy input.btn[type=submit]::-moz-focus-inner{padding:0;border:0}#iubenda_policy .circle{font-size:11px;line-height:18px;width:18px;padding:0;text-align:center;border-radius:11px}#iubenda_policy .circle.small{width:14px;line-height:14px;border-radius:9px;padding:0}#iubenda_policy .blue{color:#fff;background-color:#0073CE}#iubenda_policy .yellow{color:#6D693D;background-color:#FFD24D}#iubenda_policy .red{color:#FFF;background-color:#FF5D4D}#iubenda_policy .red a,#iubenda_policy .red a:hover:not(.btn){color:#FFF}#iubenda_policy .red a{border-bottom-color:rgba(247,247,247,0.3)}#iubenda_policy .red a:hover{border-bottom-color:rgba(247,247,247,0.6)}#iubenda_policy .green{color:#4D6C47;background-color:#F1FFD5}#iubenda_policy .iubgreen{color:#ffffff;background-color:#1CC691}#iubenda_policy .azure{color:#364048;background-color:#D2ECFE}#iubenda_policy .white{color:#54616B;background-color:#F8F8F8}#iubenda_policy .black{color:#FFF;background-color:#333333}#iubenda_policy .trasp{color:#333B43;background-color:#FFFFFF}#iubenda_policy .alert-message{position:relative;padding:7px 15px;margin-bottom:18px;color:#404040;background-color:#eedc94;background-repeat:repeat-x;background-image:-khtml-gradient(linear, left top, left bottom, from(#fceec1), to(#eedc94));background-image:-webkit-gradient(linear, left top, left bottom, from(#fceec1), to(#eedc94));background-image:linear-gradient(to bottom, #fceec1, #eedc94);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#fceec1', endColorstr='#eedc94', GradientType=0);text-shadow:0 -1px 0 rgba(0,0,0,0.25);border-color:#eedc94 #eedc94 #e4c652;border-color:rgba(0,0,0,0.1) rgba(0,0,0,0.1) rgba(0,0,0,0.25);text-shadow:0 1px 0 rgba(255,255,255,0.5);border-width:1px;border-style:solid;border-radius:4px;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,0.25);box-shadow:inset 0 1px 0 rgba(255,255,255,0.25)}#iubenda_policy .alert-message .close{*margin-top:3px}#iubenda_policy .alert-message h5{line-height:18px}#iubenda_policy .alert-message p{margin-bottom:0}#iubenda_policy .alert-message div{margin-top:5px;margin-bottom:2px;line-height:28px}#iubenda_policy .alert-message .btn{-webkit-box-shadow:0 1px 0 rgba(255,255,255,0.25);box-shadow:0 1px 0 rgba(255,255,255,0.25)}#iubenda_policy .alert-message.block-message{background-image:none;background-color:#fdf5d9;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);padding:14px;border-color:#fceec1;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy .alert-message.block-message ul,#iubenda_policy .alert-message.block-message p{margin-right:30px}#iubenda_policy .alert-message.block-message ul{margin-bottom:0}#iubenda_policy .alert-message.block-message li{color:#404040}#iubenda_policy .alert-message.block-message .alert-actions{margin-top:5px}#iubenda_policy .alert-message.block-message.error,#iubenda_policy .alert-message.block-message.success,#iubenda_policy .alert-message.block-message.info{color:#404040;text-shadow:0 1px 0 rgba(255,255,255,0.5)}#iubenda_policy .alert-message.block-message.error{background-color:#fddfde;border-color:#fbc7c6}#iubenda_policy .alert-message.block-message.success{background-color:#d1eed1;border-color:#bfe7bf}#iubenda_policy .alert-message.block-message.info{background-color:#ddf4fb;border-color:#c6edf9}#iubenda_policy .fade{-webkit-transition:opacity 0.15s linear;transition:opacity 0.15s linear;opacity:0}#iubenda_policy .fade.in{opacity:1}#iubenda_policy .expand-click{cursor:pointer;position:relative}#iubenda_policy .box_10.expand .expand-click{margin:-10px;padding:12px 25px 13px 10px}#iubenda_policy .box_10.expand .expand-content{margin-top:10px}#iubenda_policy .box_10.expand .expand-content>*:first-child{margin-top:0;padding-top:0}#iubenda_policy .expand.expanded .expand-click:after,#iubenda_policy .box_10.expand.expanded .expand-click:after{content:"";position:absolute;right:10px;top:19px;border:5px;border-color:transparent;border-style:solid;border-top-color:#333B43}#iubenda_policy .expand .expand-click,#iubenda_policy .box_10.expand .expand-click,#iubenda_policy .expand.expanded .expand-click,#iubenda_policy .box_10.expand.expanded .expand-click{border-bottom:1px dotted #DDD;margin-bottom:10px;-webkit-transition:0.2s linear all;transition:0.2s linear all}#iubenda_policy .expand.collapsed .expand-click{border-bottom:0;margin-bottom:-10px}#iubenda_policy .expand.collapsed .expand-click:after{content:"";position:absolute;right:10px;top:17px;border:5px;border-color:transparent;border-style:solid;border-right-color:#333B43}#iubenda_policy .all-collapsed .expand .expand-click:after{content:"";position:absolute;right:10px;top:17px;border:5px;border-color:transparent;border-style:solid;border-right-color:#333B43}#iubenda_policy .all-collapsed .expand .expand-click{border-bottom:0;margin-bottom:-10px}#iubenda_policy .all-collapsed .expand-content{display:none}html#iubenda_policy,#iubenda_policy body{background-color:#FFF}#iubenda_policy{font-family:"Helvetica Neue", Helvetica, Arial, FreeSans, sans-serif;font-size:13px;font-weight:normal;line-height:18px;color:#59636D}#iubenda_policy body{margin:0}#iubenda_policy .iub_container-fluid{position:relative;min-width:940px;padding-left:20px;padding-right:20px;zoom:1}#iubenda_policy .iub_container-fluid:before,#iubenda_policy .iub_container-fluid:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy .iub_container-fluid:after{clear:both}#iubenda_policy .iub_container-fluid>.sidebar{float:left;width:220px}#iubenda_policy .iub_container-fluid>.iub_content{margin-left:240px}#iubenda_policy a{text-decoration:none;font-weight:bold;border-bottom:1px solid #F6F6F6;color:#333b43}#iubenda_policy a.unstyled{border-bottom:0}#iubenda_policy a:hover:not(.btn){color:#121518;border-bottom-color:#D6D6D6;-webkit-transition:0.1s linear all;transition:0.1s linear all}#iubenda_policy a.no_border,#iubenda_policy a.no_border:hover{border-bottom-width:0}#iubenda_policy .pull-right{float:right}#iubenda_policy .pull-left{float:left}#iubenda_policy .hide{display:none}#iubenda_policy .show{display:block}#iubenda_policy .link_on_dark a{border-bottom-color:rgba(247,247,247,0.3)}#iubenda_policy .link_on_dark a:hover{border-bottom-color:rgba(247,247,247,0.6)}#iubenda_policy [class*="policyicon_"]{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYBAMAAAASWSDLAAAAGFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz9%2BjSc3AAAAB3RSTlMAEEBQgMzQxeXuPgAAADJJREFUGFdjYMAJWEPhIAAPh70cDgoGK6cI5B8Yp6S8TACJk4gkA5RAcBKR9BQLoAUOAATNYYOCulUNAAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_pdt_68{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAKVJREFUeF51jlmWwyAMBGXEboT6%2FqedIZAAJqnfer3QJKpGOrkKakW5noIrAlFA5V0EKL%2B8Iqw1d%2B%2FojflTx4JlNUJGnVe1tOBUfRMZYmjDCDKRINFBglCLnXiltnTClfAtEgACxvHJldHF4xYL3gLq1l1Mgfk5AZtQx%2FYfdroL4TySXFeRWTAQc0%2Fhe0FHbRiicsJGZG3iNgUPiimgYBUHlQP94g9%2BZg8xOTGEFAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .policyicon_purpose_5{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYBAMAAAASWSDLAAAAElBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2BtTDCxAAAABXRSTlMAECBAgLf%2B2%2BsAAABGSURBVBhXY2AAA5ZQBwY4YA0NIJfjCjYHygkNDUTmBGPhgOyFc1iB6pE4wSAOUAGCIxoaiOCYhgYjOKqhQThkyODAAR4OAI98N9LK6tL3AAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_purpose_7{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAINJREFUeF6V0UsOxCAIBmB8tVoZ4f6nnUqaoFUW%2FVeEj0hUMOKM9kE7CBcxr93SuGcCf%2FRZniCmXGVUwZV2M78DgYRXQDaAP0OzIJIB4C%2FaQo%2BTCyK9ISFizimAPyuNACjlKXW6SMF30B9I9YFndRieuZCCHKU0QIU1LDEhrvDrQG6EP%2FDZElAL0vLHAAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_purpose_9{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAQAAABKfvVzAAACC0lEQVQ4y7XSO2gWVhQH8BPxDRG%2BEhurMcSI4GsoPqjkZ6BLwcFFHUQJKqbEwRciDqZDF90cpIsILtZHh0KTIdQMgkTRiIshBoWgTRpbsVaxgqRf4uM4JCHfRzpIwXun8%2Bf%2BuHDOifj%2FxwoD2qek7Qat%2FG9Qr1%2FblLRNv%2FqyqKHCjIgIqw3oGE9mmtlQERGhw4DVERFmNFREhG91uq6gxUspnVdlky5dNqlyXkovtSi4rtPe8JeUaq1yWLN9tkVoklJThK1a7HXISrVSehpSGrXb5woWqFZljZNSOmmtBRapUe0Lu4xKOQZSr0633dejS7chKQ25p0%2BvHn3u6Bt7OQFSeuWG3pI6DbvpZ5dc8WwimwTPbYswx49Sei89sDNCpaoI6%2FyqWA5OmxUR4StF6Z0hX5puvyH%2FOmeeudrLwXfjg1prUCo6FuGyty444W89CpYZKQU%2FmF3ywwvVthtxwpwImz1yzjSdpWBYq2nWuzbWoQgX%2FaPOAd%2Br1O55hDOl4LHdDRXqnPVWehLhlPSNgiURFlof4adJMGC7eRERarRKr32t2qBn9lhlg%2BVq7fDbJDhasp%2BfueW9brOscdULv7vntlselnZpadlKH5fSRYvN16ytdJgT4KBGGzVqtNFmv4yndzWrt8WjqSCNGFZUNOxN2Xq8K6%2FD47Et%2FKg7ajAc9edHgz8ciU9%2BPgBKt4%2FTzlslzAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .policyicon_purpose_10,#iubenda_policy .policyicon_purpose_15{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAKVJREFUeF51jlmWwyAMBGXEboT6%2FqedIZAAJqnfer3QJKpGOrkKakW5noIrAlFA5V0EKL%2B8Iqw1d%2B%2FojflTx4JlNUJGnVe1tOBUfRMZYmjDCDKRINFBglCLnXiltnTClfAtEgACxvHJldHF4xYL3gLq1l1Mgfk5AZtQx%2FYfdroL4TySXFeRWTAQc0%2Fhe0FHbRiicsJGZG3iNgUPiimgYBUHlQP94g9%2BZg8xOTGEFAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .policyicon_purpose_13{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAJ1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz9PhkGkAAAADHRSTlMAECBAUHCQoLDA4PB7ua%2BoAAAAa0lEQVR42p3QQQ6AIAxE0aEIFdr7n1eMxIAOMfEt%2B9sF4IOkYt5YSTKO1Qd6p%2BQP6Zqrvyjd7zdiLJggO5VReajwhR%2FBnDIoDwrhQcAfkhd%2FtQO0KDqf1A0kmEZgDjk2AZPzPoJo6wFEYOsHFFISOn%2BKxfoAAAAASUVORK5CYII%3D)}#iubenda_policy .policyicon_purpose_14{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAMFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2Fjai5RAAAAD3RSTlMAECAwUGBwgJCgsMDQ4PASl6hyAAAAfklEQVR42pXRUQ6EMAgE0MEWW21l7n9btanJWnE3%2Bz4hhCHgq5jKooKD6FJS7OVQebIIROOphlY3dqrsLABidJgg0ZWw0bWBL%2F5vvO%2FIdGVM%2Fh0TMNMx47DwYcVJKgdV0MgwUwSXfA%2F0QY2dKW7CxutHA1lbHMFTavE9qsBvOztlFTRVyS%2BYAAAAAElFTkSuQmCC)}#iubenda_policy .policyicon_purpose_16{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAM1BMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2F10LmwAAAAEHRSTlMAECAwQFBgcICQoLDA0ODwVOCoyAAAAJFJREFUeF6V0NsOAyEIRVE6I4rFwvn%2Fr63N3CR10nQnPK2IUdpbpKmsorJQqOKTl2xeRhDsycMgA7QDGkmfq9cI%2FvNEhGcAO8CowAbAGTEwX1XDKvYNnJM7f78clVqfydOlgwRIG6S1TwDdQEnD3cv1iWw4f54VQ1qfUO5QDDGYVLNCmOQ5O2Ea8R2kP8FWobvefhoT%2FSVCMbAAAAAASUVORK5CYII%3D)}#iubenda_policy .icon_ribbon{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAW0lEQVR42u3OwQkAIQxE0XSWVrazlJpdQdGDC0pQEf7A3ELmibsPV1V9pDM%2FAQAAAAAAAAAAAAAAEAXY1%2BcUwCQnITYD6niL2ASo4z3EaoDKf8qNBQHxArgK8ALKMXCw%2Bim7vwAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .icon_owner{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAAMFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz%2Fjai5RAAAAD3RSTlMAECAwQGBwgJCgsMDQ4PC8YWy5AAAAiElEQVR42o2QwRKFIAhFIcwyRP7%2Fb3uNlkBv0dkw3jODd4AbPHhNC7xAafqjYBRZOzUa0cHmc9IbiZsefIFtiuQ68RS7FUkNnwTWmRewLE9ewSPh73dfCgJbzxkiRxcrDGJhWVxa5MqYr1HzcLSPRo2ojcoZAcyV2F1MzaPoxIqcP4gGkP5BcAIxQBCQ7o5t3AAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .icon_general{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYBAMAAAASWSDLAAAAGFBMVEUAAAA%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz8%2FPz9%2BjSc3AAAAB3RSTlMAEEBQgMzQxeXuPgAAADJJREFUGFdjYMAJWEPhIAAPh70cDgoGK6cI5B8Yp6S8TACJk4gkA5RAcBKR9BQLoAUOAATNYYOCulUNAAAAAElFTkSuQmCC)}#iubenda_policy .icon_temple_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABwklEQVR42s3Wu0vDUBjGYS%2BLsbZSSaWgguAFHFztYEmFbp0E%2FwOrgotQFyetOKiTLqKCWCenbl20S8FFERydBLt1KV7QwUGR4094hQymjYpi4SGH9zvf%2BUgCoQ3GmF%2F1dwNq%2FRzHaUwkEn24lP73rEaL%2FwEcZmEcJexiDyfKrG8P0OG9OIDBrCvPKMuh98sDaApiAmWYj8fiqg%2FjSrWy9gbrDlDzEHIwLi9YRieiWMOrakIPvZ4DKHYhjTsYD%2Be48Kqrdwpdnw1I4RAFbCKHHWxhX%2BtjHGFb2ZbynHoKOiNV7x3YrnWLrmFFWqvm6vH7DmK4ho0l5NGGCialoiyvPbZ6Yn4GOHhCFBsoIQSDOTHKStoTVY%2FjZ0Act7CxiiICqGJaqsqK2mOrJ%2F6VARGs6ZA2ZTNyq6yoPZF%2FNWC0xiOaEq9HNOpnQBIG3djFGcLKFsQoO8UOepQl%2FQyIIKtP9BjSylcwghhWlKWR0N4sIp4D1NCKDgR0DSIEGxbCYikLibvH8voWNWMdD6jiEXe4waOye1GdGntc9Qcso8nrDtoxgEFdIcp81INed7CIBWQw%2F00ZnbH42YAXef4RnfNn%2FyreALybXwSLU3v7AAAAAElFTkSuQmCC)}#iubenda_policy .icon_box_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABv0lEQVR42t3Vz0uTcRzAcUMyWhmWdAgqkKDMiBHt0A%2FYsploddwpO1gk0l%2BQEEQU0iUPgd0LIpCOCh2KkG4GTaI6mqAmWhG0CQ5jfXsdntN4bJPRxS%2B84IFnz%2Ff97Nl4Pg0hhP9qkwT%2BtTKZTCN7uM0qeTrZuc4ltQVs0EqK%2B3xmigc8Z5E39HOI7TUFfHAbJxngNQtM0kdzg5VOp7c4TvKYeeZ4wmXaYgNONHGcW7zjA6Mkqzy%2BZq4zzgxj5DhcGUgxwzSZ9TasEtvFCL%2F4WBm4SKDAPXrZV%2BPGWznFVSYIhMpAliILhEieO5ynMWbjDgZ4xjxlAn%2FiAt0skeMG44TIT8boo51zDPOeEqFSXKAnCrRHd5fgNMN8IrDCFLOUCVB74CsdZBlkL03s5xG%2FCcAGA73M0cIViswyQisn%2BFZPoIdljkWP6AIvKDFIiuV6Al2s8JIciSh0hqNk%2BVHvNwiRNd5ylwNRqKvewNnYv1z0O%2FCQ7xsIFCsDCS4xyhKhwiprhCqmGaIz%2Fm0qxBGu8YoCoYpFntLNwbS3ba3zYDdJhshTohwpMEE%2FbeyoMg%2BqTrQWbvKFSSxDJn5tsqH%2FF0QW2NxzTlYFAAAAAElFTkSuQmCC)}#iubenda_policy .icon_tools_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABdklEQVR42rXVzyuDcRzA8WU3ctOag0RiO5mEg8MKcaJc%2FAlcdxppKPlZdpeTE0dqxZWaaEnh7DShlYuJbG0f78Nz%2BPj2zfM89Wz1qmff5%2FPdu%2B27tpCINNTfJzySyeQGhkPGg7UljBtrEbxDMOkaYCiKJ8QtgR0cGWt9EMe8l8AIBAOWwCGKxtqMCux5CSRQxyW61QtNo4yCEVhWgRzCboFm5CF4xTVuUYUgZQTOVeAZHV4OeRSfEMMFWoxAVt2%2FQtQ14Gzsx43anEWr5Vx61Eza9Qz%2B%2BXw71S09M6hm1v0GVtXmWCMCa2pz3BpgXc1kAg2w1oW0mjnGRJCBOYjhLshAO96MQCroM3hQMzUMBfkOZvEDUU78BFbUxl5LYBdiqPgJbKmNCUtg2xL48PpTMYVvFFDEPdqCDDwi51xHIVi0%2FAGJoew18IJ957oJFWx6CHx5DSygjgPkUULM8i2qGoFTP4ecgaCEMcshh5FFDYIzRGyBhvoF3n%2ByMxzF1ykAAAAASUVORK5CYII%3D)}#iubenda_policy .icon_paper_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABYklEQVR42t3VP0vDQBjH8Tq4SKXiWFwcRHARVyspgq9AOjkoLoKTcymk%2BjKKYDcnO6iLKPgHRJ11aVGkgt2M2IiWlobzKzyB4zBwBGvBwIdc7rnjR8ITLqGU6qm%2FC8hms%2Bo39TWgg0fUUJX7PV7RlVo1Qtsm4Ckhl%2BM4A%2BGY%2BQJ8TCYiLmp1m4AHWbyGa%2BxiFEtQMneIY80RTtCyCahJwDpOsYc0FtHGDS5wbjjDp03AM6aRRhIpTGAbH5jBEJIm208UwMcbmuIFHam34KEZ0tYGNgEeXFEUW9jAKvLYRFHjCs8moIEMZpHRxnNwzJrx3Oj%2Fj2a%2BQbT4b%2BDBjcmz6iK9M6LF76I6UnHY%2Fgc%2BythB2YK%2B1tcC%2Ful54COPMeT0tsMBxsW%2B0dY52VPAe1RAgAoGw7OA8QoUbvVzgPEU7qS2HJ4b33tRQfBTQBcl4wBZgMIlhrX5EVxJbd7YU0JXD%2BipLw8sG8DBrCLzAAAAAElFTkSuQmCC)}#iubenda_policy .icon_man_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABLUlEQVR42t3VsUrDUBSAYaWtSwSp6NAH6CbOVSHZ9QEEBx9AEPc6OAh9Bp0KDg6igqs4tktXFQQnKQiKiNRAp%2BT4C2cImqbXc3Fp4VsazvlpuUmmRORfTUig6BNFURnbeISoB2yhlDPiHvhegF18Qn74wA5KPoE13EFGuEXDFGBwBoeQMQ5QsQSqOHUInGDOEljElUPgEguWwDzOHQJnqFoCszh2CBwhsAQq2EdSsDxFE2XrMV3HS0HgFRs%2B90ENNwWBa9TMgTAMp%2FWR8J6z%2FA2bXo8K%2FRXLuB9xFy%2BZAwwHWMUF4pxArNdWnE%2BRLm2ghS76SMecoj66aOls8CvAl3XsoYNnDCF%2FNNTZju6qZwO93L%2FBLkYvGxggVeIpVYNsoI0nJBBPie5qT8ZL%2FwsLLryq%2FnnTDAAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .icon_keyhole_24{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABIUlEQVR42rXUP0vCQRjA8bIoiAppLmwQEmehSX5RLTb2Huw9RGODLvUCXG0Kp16ALhENNRjRXLRlIeafJOyevkNu14M89%2FPgMx133%2BF4bkZEpkrdHK8oipIoowuHK2QxGxzgkk1cYgD3R9BEAQlzgMOruMA3xOMZuZDAEToQxRkWrYEHOIiiibQ1IBMEOtixBn4mCLSRtwbqIKIGbrFhDRzgA6I4xpw1kMA5ep6LHa6RCh20ddx4Aq%2FYj2OSF1D3BJ6QjCOQwosn8IbtOAK7%2BPQEvlAcf3ghj1zE4J9HrmApJDCPkvLZ3WMtJLCCmjLNLWRCAmk8KkPWxyHMgQLaSmCIk5BJPkVfCYxQxbI10MBQCTjcYcsaeMcIomhhTwtM1S9g12NLa1YPRQAAAABJRU5ErkJggg%3D%3D)}#iubenda_policy .iub_base_container{border-radius:3px;background:#ffffff;color:#6B6B6B;position:relative}#iubenda_policy .iub_base_container>.close{background:transparent url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABcAAAAYCAMAAAAmopZHAAAAw1BMVEUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAB4eHh1dXUAAAAAAAAAAAAAAAAAAABfX18AAAAAAAAAAAAAAAAAAAAAAAA2NjYAAAAAAAArKyvJycne3t7X19eFhYWxsbGVlZWsrKzr6%2BvLy8vJycnv7%2B%2Fp6enS0tLi4uL09PTv7%2B%2F8%2FPz7%2B%2Fv4%2BPj39%2FcAAABPT09fX19vb2%2F%2F%2F%2F9S%2BfXQAAAAPHRSTlMAAgMEBQYHCgsMDQ4PEhMWGRobHB8gIiMkJScoKSs0NT1DRUpMWF5gjpOYmaGjpr%2FIys3S1dnZ7vP09vfFQC13AAAA9ElEQVR42oXQZ6%2BCMBiG4aeCAoqiuPceuPes8P7%2FX6Xn5RgBTbw%2BNO3dpG2KH0RcM5JJQ4uLUE2UnSM9HZ1y4r0TM50z%2FTs7ZuyVSysKWJX8DZHeUsg2zUfpU4qY6gBE8xLtl6YAtAnP79Ij8uSdFxMNsHY8lVK67nPgxc4CisQ8yTxiRaBGPvcvu%2BSrAY1vvQHUv51TByqHz3sPFcCef75zbgOpwZUiroMUoFSX0b6sKgDMzjqc1x2Tvznb2wTzppf1P1q1u7PTq55mXVuFT7Va48X%2BRnTbL8YtizMTRqHdH45Gw367YAgEKHoml8%2FnMroC9gCKfVabzD1q%2BwAAAABJRU5ErkJggg%3D%3D) no-repeat;border:none;display:block;position:absolute;z-index:110;top:-10px;right:-9px;height:24px;width:23px}#iubenda_policy p{line-height:19px;margin:0;padding-top:11px}#iubenda_policy address{margin:0;line-height:inherit;display:inline}#iubenda_policy a{font-weight:normal;border-bottom:1px solid #F0F0F0}#iubenda_policy .iub_content{position:relative;padding:25px 30px;margin:0 auto;border-radius:3px 3px 0 0}#iubenda_policy #wbars{position:relative;overflow-y:auto;overflow-x:hidden}#iubenda_policy #wbars .horizontal{display:none}#iubenda_policy .iub_header{border-bottom:1px dotted #DFDFDF;padding-bottom:25px;position:relative}#iubenda_policy .iub_header p{margin:0;padding:0}#iubenda_policy .iub_header img{display:block;position:absolute;top:5px;right:0}#iubenda_policy h1,#iubenda_policy h2,#iubenda_policy h3{color:#3F3F3F;margin:0}#iubenda_policy h1+p,#iubenda_policy h2+p,#iubenda_policy h3+p{padding-top:5px}#iubenda_policy h1{font-size:19px;font-weight:normal;line-height:23px;margin-bottom:5px}#iubenda_policy h2{font-size:17px;font-weight:bold;line-height:21px;padding-top:21px}#iubenda_policy h3{font-size:13px;line-height:19px;font-weight:bold;padding-top:24px}#iubenda_policy h3+p{padding-top:0}#iubenda_policy .iconed ul li h3{padding-top:10px;color:#615e5e}#iubenda_policy h4{font-size:13px;font-weight:bold;padding-top:19px;margin-bottom:0}#iubenda_policy h4:first-child{padding-top:0}#iubenda_policy ul.for_boxes,#iubenda_policy ul.for_boxes>li,#iubenda_policy ul.unstyled,#iubenda_policy ul.unstyled>li{list-style:none;padding:0;margin:0}#iubenda_policy ul.for_boxes{zoom:1}#iubenda_policy ul.for_boxes:before,#iubenda_policy ul.for_boxes:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy ul.for_boxes:after{clear:both}#iubenda_policy .half_col{float:left;width:50%;zoom:1}#iubenda_policy .half_col:before,#iubenda_policy .half_col:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy .half_col:after{clear:both}#iubenda_policy .half_col:nth-child(2n+1)>*{margin-right:15px}#iubenda_policy .half_col:nth-child(2n)>*{margin-left:15px}#iubenda_policy .half_col+.one_line_col,#iubenda_policy .half_col+.iub_footer{border-top:1px dotted #DFDFDF}#iubenda_policy .one_line_col{zoom:1;float:left;width:100%;border-bottom:1px dotted #DFDFDF}#iubenda_policy .one_line_col:before,#iubenda_policy .one_line_col:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy .one_line_col:after{clear:both}#iubenda_policy .one_line_col>ul.for_boxes>li{float:left;width:50%}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1){clear:left}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:15px}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n){clear:right}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:15px}#iubenda_policy .one_line_col.wide{width:100%}#iubenda_policy .one_line_col.wide>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy .one_line_col.wide>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy .one_line_col.wide>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy ul.normal_list{list-style:disc;display:block;padding-top:11px}#iubenda_policy ul.normal_list li{list-style:disc;float:none;line-height:19px;margin:5px 25px}#iubenda_policy .simple_pp>ul>li{padding-bottom:21px}#iubenda_policy .simple_pp>ul>li>ul .iconed{padding-left:40px;background-repeat:no-repeat;background-color:transparent;background-position-x:2px;background-position-y:26px;background-position:2px 26px}#iubenda_policy .simple_pp .for_boxes>.one_line_col>ul.for_boxes{margin-top:0}#iubenda_policy .legal_pp .one_line_col{float:none;border-top:0;padding-bottom:21px}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes{margin-top:21px}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n+1){clear:left;float:left}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n){float:right;clear:right}#iubenda_policy .legal_pp .definitions{margin-top:21px}#iubenda_policy .legal_pp .definitions .expand-click.w_icon_24{margin-top:-11px;padding:14px 10px 12px 45px;background-repeat:no-repeat;background-color:transparent;background-position-x:5px;background-position-y:0;background-position:5px 0}#iubenda_policy .legal_pp .definitions .expand-content{padding-left:5px;padding-right:5px}#iubenda_policy .wrap p{display:inline-block}#iubenda_policy .iub_footer{clear:both;position:relative;font-size:11px}#iubenda_policy .iub_footer p{font-size:11px;padding:0}#iubenda_policy .iub_content .iub_footer{padding:24px 0}#iubenda_policy .iub_content .iub_footer p{margin:10px 0;clear:both}#iubenda_policy .iub_content .iub_footer .show_comp_link{display:block;float:right}#iubenda_policy .iub_container>.iub_footer{min-height:21px;background-color:#F6F6F6;color:#717171;padding:30px;-webkit-box-shadow:0 -1px 6px #cfcfcf;box-shadow:0 -1px 6px #cfcfcf;border-radius:0 0 3px 3px}#iubenda_policy .iub_container>.iub_footer>.btn{position:absolute;top:25px;right:30px}#iubenda_policy .iub_container>.iub_footer .btn{padding:0px 24px;line-height:29px}#iubenda_policy .iub_container>.iub_footer .button-stack{margin:-4px 0}#iubenda_policy .iub_container>.iub_footer .button-stack .btn+.btn{margin-left:5px}#iubenda_policy .iub_container>.iub_footer img{margin:-4px 3px 0;vertical-align:middle;width:70px;height:25px}#iubenda_policy .wide{width:150px}@media (max-width: 767px){#iubenda_policy .legal_pp .one_line_col,#iubenda_policy .legal_pp .half_col{width:100%}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li,#iubenda_policy .legal_pp .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy .legal_pp .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy .legal_pp .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy .legal_pp .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy .iub_header img{position:static;margin-bottom:12.5px}#iubenda_policy .iub_content>.iub_footer .show_comp_link{position:static;display:inline}#iubenda_policy .iub_container>.iub_footer{padding:20px}#iubenda_policy .iub_container>.iub_footer .btn{top:15px;right:15px}#iubenda_policy .iub_base_container>.close{content:"X";color:#000;font-size:11px;line-height:18px;padding:0;text-align:center;border-radius:30px;display:block;background:#fff url(../design/images/close_big.png) no-repeat;background-position-x:18px;background-position-y:18px;background-position:18px 18px;position:absolute;z-index:110;top:-10px;right:-10px;margin:5px 5px 0 0;height:57px;width:60px;-webkit-box-shadow:0 1px 1px #000000;box-shadow:0 1px 1px #000000}#iubenda_policy .iub_base_container>.close.small{width:14px;line-height:14px;border-radius:9px;padding:0}}@media (max-width: 480px){html#iubenda_policy{padding:0}#iubenda_policy body{padding:0}#iubenda_policy .iub_base_container,#iubenda_policy .iub_container{margin:0}#iubenda_policy .half_col:nth-child(2n+1)>*{margin-right:0}#iubenda_policy .half_col:nth-child(2n)>*{margin-left:0}#iubenda_policy .one_line_col,#iubenda_policy .half_col{width:100%}#iubenda_policy .one_line_col>ul.for_boxes>li,#iubenda_policy .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy .iub_header img{position:static;margin-bottom:12.5px}#iubenda_policy .iub_content>.iub_footer .show_comp_link{position:static;display:inline}#iubenda_policy .iub_container>.iub_footer{padding:10px;text-align:center}#iubenda_policy .iub_container>.iub_footer .btn{position:static;width:auto;display:block;margin:10px auto 0 auto;max-width:200px}#iubenda_policy .iub_container>.iub_footer.in_preview{padding:30px 10px}#iubenda_policy .iub_content{padding-left:20px;padding-right:20px}#iubenda_policy .iub_base_container>.close{content:"X";color:#000;font-size:11px;line-height:18px;padding:0;text-align:center;border-radius:30px;display:block;background:#fff url(../design/images/close_big.png) no-repeat;background-position-x:18px;background-position-y:18px;background-position:18px 18px;position:absolute;z-index:110;top:-10px;right:-10px;margin:5px 5px 0 0;height:57px;width:60px;-webkit-box-shadow:0 1px 1px #000000;box-shadow:0 1px 1px #000000}#iubenda_policy .iub_base_container>.close.small{width:14px;line-height:14px;border-radius:9px;padding:0}}#iubenda_policy.iubenda_fixed_policy .iub_base_container{max-width:800px}#iubenda_policy.iubenda_fixed_policy .iub_container{margin-left:auto;margin-right:auto;zoom:1}#iubenda_policy.iubenda_fixed_policy .iub_container:before,#iubenda_policy.iubenda_fixed_policy .iub_container:after{display:table;content:"";zoom:1;*display:inline}#iubenda_policy.iubenda_fixed_policy .iub_container:after{clear:both}#iubenda_policy.iubenda_fluid_policy #wbars{overflow-y:auto;-webkit-box-shadow:none;box-shadow:none;height:auto}#iubenda_policy.iubenda_fluid_policy .iub_container{margin-top:30px;margin-bottom:30px}#iubenda_policy.iubenda_fluid_policy .half_col:nth-child(2n+1)>*{margin-right:0}#iubenda_policy.iubenda_fluid_policy .half_col:nth-child(2n)>*{margin-left:0}#iubenda_policy.iubenda_fluid_policy .one_line_col,#iubenda_policy.iubenda_fluid_policy .half_col{width:100%}#iubenda_policy.iubenda_fluid_policy .one_line_col>ul.for_boxes>li,#iubenda_policy.iubenda_fluid_policy .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy.iubenda_fluid_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy.iubenda_fluid_policy .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy.iubenda_fluid_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy.iubenda_fluid_policy .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy.iubenda_embed_policy .iub_base_container{background:none}#iubenda_policy.iubenda_embed_policy .iub_container>.iub_footer{-webkit-box-shadow:none;box-shadow:none;border-radius:none}#iubenda_policy.iubenda_embed_policy .expand-click{cursor:default}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .iub_base_container{color:#666}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h2{font-size:24px;padding-top:50px}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h3{color:#444;font-size:20px;padding-top:45px}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h4{font-size:16px;padding-top:40px;color:#555}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h5{font-size:14px;padding-top:35px;margin-bottom:0;color:#666}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy h6{font-size:12px;color:#505050;text-transform:uppercase;padding-top:32px;margin-bottom:0}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions{margin-top:60px !important}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions .expand-content{padding:25px 15px !important}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions .expand-content h4{font-size:15px !important}#iubenda_policy.iubenda_vip_policy.iubenda_terms_policy .definitions:before{content:"";border-top:1px dotted rgba(0,0,0,0.1);display:block;margin:0 -10px;position:relative;top:-45px}#iubenda_policy.iubenda_vip_policy.iubenda_fixed_policy .iub_container{max-width:660px;padding-top:80px}#iubenda_policy.iubenda_vip_policy .iub_base_container{color:#6B6B6B}#iubenda_policy.iubenda_vip_policy p{font-size:14px;line-height:1.6}#iubenda_policy.iubenda_vip_policy .allcaps,#iubenda_policy.iubenda_vip_policy p.allcaps,#iubenda_policy.iubenda_vip_policy ul.allcaps li{font-variant:small-caps !important;font-weight:bold !important;font-size:16px !important;font-family:-apple-system, BlinkMacSystemFont, Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif !important}#iubenda_policy.iubenda_vip_policy ul li{font-size:14px;line-height:1.6}#iubenda_policy.iubenda_vip_policy h1{font-size:30px;color:#141414;line-height:1.6;margin-bottom:60px}#iubenda_policy.iubenda_vip_policy h2{font-size:18px;color:#141414;line-height:1.6;padding-top:50px;padding-bottom:15px}#iubenda_policy.iubenda_vip_policy h3{color:#141414;font-size:16px;line-height:1.6;margin-bottom:10px}#iubenda_policy.iubenda_vip_policy .legal_pp .one_line_col{padding-bottom:50px}#iubenda_policy.iubenda_vip_policy .half_col:nth-child(2n+1)>*{margin-right:0}#iubenda_policy.iubenda_vip_policy .half_col:nth-child(2n)>*{margin-left:0}#iubenda_policy.iubenda_vip_policy .one_line_col,#iubenda_policy.iubenda_vip_policy .half_col{width:100%}#iubenda_policy.iubenda_vip_policy .one_line_col>ul.for_boxes>li,#iubenda_policy.iubenda_vip_policy .half_col>ul.for_boxes>li{clear:both;width:100%}#iubenda_policy.iubenda_vip_policy .one_line_col>ul.for_boxes>li:nth-child(2n+1)>div,#iubenda_policy.iubenda_vip_policy .half_col>ul.for_boxes>li:nth-child(2n+1)>div{margin-right:0}#iubenda_policy.iubenda_vip_policy .one_line_col>ul.for_boxes>li:nth-child(2n)>div,#iubenda_policy.iubenda_vip_policy .half_col>ul.for_boxes>li:nth-child(2n)>div{margin-left:0}#iubenda_policy.iubenda_vip_policy .definitions,#iubenda_policy.iubenda_vip_policy .iub_footer,#iubenda_policy.iubenda_vip_policy .for_boxes{color:#59636D}#iubenda_policy.iubenda_vip_policy .definitions h3,#iubenda_policy.iubenda_vip_policy .iub_footer h3,#iubenda_policy.iubenda_vip_policy .for_boxes h3,#iubenda_policy.iubenda_vip_policy .definitions p,#iubenda_policy.iubenda_vip_policy .iub_footer p,#iubenda_policy.iubenda_vip_policy .for_boxes p,#iubenda_policy.iubenda_vip_policy .definitions li,#iubenda_policy.iubenda_vip_policy .iub_footer li,#iubenda_policy.iubenda_vip_policy .for_boxes li{font-size:13px}#iubenda_policy.iubenda_vip_policy .w_icon_24{background-image:none}#iubenda_policy.iubenda_vip_policy .box_10.expand .expand-click.w_icon_24{padding-left:10px}#iubenda_policy.iubenda_vip_policy .box_primary{border-color:#E0E0E0;border-bottom-color:#D3D3D3;-webkit-box-shadow:none;box-shadow:none}#iubenda_policy.iubenda_vip_policy .box_primary h3{color:#333}#iubenda_policy.iubenda_vip_policy .tc-deactivated h1{font-size:20px;margin-bottom:10px}#iubenda_policy.iubenda_vip_policy .legal_pp .one_line_col{padding-bottom:21px}
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/templates/iubenda/cookie.html` & `django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-{% extends 'base.html' %}
-{% load i18n static compress %}
-
-{% block head_canonical %}
-    <link href="{{ SITE_URL }}{{ request.get_full_path }}" rel="canonical">
-{% endblock head_canonical %}
-
-{% block itemtype %}{% endblock itemtype %}
-
-{% block extra_title %} - Cookie Policy{% endblock extra_title %}
-
-{% block content %}
-<section id="cookie">
-  <div class="wrapper light-wrapper">
-    <div class="container inner">
-      <div class="row">
-        {% if req_cookie %}
-          {% block css %}
-        	{% compress css file iubenda %}
-            <link rel="stylesheet" type="text/css" href="{% static 'iubenda/css/iubenda_policy.css' %}">
-        	{% endcompress %}
-          {% endblock css %}
-
-          {{ req_cookie.content | safe }}
-        {% else %}
-          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}/cookie-policy" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Cookie Policy">Cookie Policy</a>
-
-          {% block js %}
-          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
-          {% endblock js %}
-        {% endif %}
-      </div>
-      <!-- /.row -->
-    </div>
-    <!-- /.container -->
-  </div>
-  <!-- /.wrapper -->
-</section>
-<!-- /#cookie -->
-{% endblock content %}
-
+{% extends 'base.html' %}
+{% load i18n static %}
+
+{% block head_canonical %}
+    <link href="{{ SITE_URL }}{{ request.get_full_path }}" rel="canonical">
+{% endblock head_canonical %}
+
+{% block itemtype %}{% endblock itemtype %}
+
+{% block extra_title %} - Privacy Policy{% endblock extra_title %}
+
+{% block content %}
+<section id="privacy">
+  <div class="wrapper light-wrapper">
+    <div class="container inner">
+      <div class="row">
+        {% if req_privacy %}
+          {% block css %}
+            <link rel="stylesheet" type="text/css" href="{% static 'iubenda/css/iubenda_policy.css' %}">
+          {% endblock css %}
+
+          {{ req_privacy.content | safe }}
+        {% else %}
+          <!-- Could be added as class: "iub-legal-only" -->
+          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Privacy Policy">Privacy Policy</a>
+
+          {% block js %}
+          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
+          {% endblock js %}
+        {% endif %}
+      </div>
+      <!-- /.row -->
+    </div>
+    <!-- /.container -->
+  </div>
+  <!-- /.wrapper -->
+</section>
+<!-- /#privacy -->
+{% endblock content %}
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/templates/iubenda/include-content.html` & `django-iubenda-1.2.6/src/iubenda/templates/iubenda/include-content.html`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-<p class="text-center">
-    <i>
-        <!--Privacy Policy -->
-        <a href="{% url 'privacy' %}" class="iubenda-black no-brand iubenda-noiframe " title="Privacy Policy ">Privacy Policy</a>
-    -
-        <!--Cookie Policy-->
-        <a href="{% url 'cookie' %}" class="iubenda-black no-brand iubenda-noiframe " title="Cookie Policy ">Cookie Policy</a>
-    </i>
-</p>
-
-<!-- JS Cookie Solution -->
-<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>var _iub = _iub || [];_iub.csConfiguration = {"ccpaAcknowledgeOnDisplay":true,"ccpaApplies":true,"consentOnContinuedBrowsing":false,"enableCcpa":true,"floatingPreferencesButtonDisplay":"bottom-left","invalidateConsentWithoutLog":true,"perPurposeConsent":true,"siteId":{{ cx_iubenda.iub_site_id }},"whitelabel":false,"cookiePolicyId":{{ cx_iubenda.iub_policy_id }},"lang":"{{ LANGUAGE_CODE }}", "banner":{ "acceptButtonDisplay":true,"backgroundOverlay":true,"closeButtonRejects":true,"customizeButtonDisplay":true,"explicitWithdrawal":true,"fontSize":"14px","listPurposes":true,"position":"float-center","rejectButtonDisplay":true }};</script>
-
-<!-- JS Iubenda -->
-<script type="text/javascript" src="https://cdn.iubenda.com/cs/ccpa/stub.js"></script>
-<script type="text/javascript" src="https://cdn.iubenda.com/cs/iubenda_cs.js" charset="UTF-8" async></script>
+<p class="text-center">
+    <i>
+        <!--Privacy Policy -->
+        <a href="{% url 'privacy' %}" class="iubenda-black no-brand iubenda-noiframe " title="Privacy Policy ">Privacy Policy</a>
+    -
+        <!--Cookie Policy-->
+        <a href="{% url 'cookie' %}" class="iubenda-black no-brand iubenda-noiframe " title="Cookie Policy ">Cookie Policy</a>
+    </i>
+</p>
+
+<!-- JS Cookie Solution -->
+<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>var _iub = _iub || [];_iub.csConfiguration = {"ccpaAcknowledgeOnDisplay":true,"ccpaApplies":true,"consentOnContinuedBrowsing":false,"enableCcpa":true,"floatingPreferencesButtonDisplay":"bottom-left","invalidateConsentWithoutLog":true,"perPurposeConsent":true,"siteId":{{ cx_iubenda.iub_site_id }},"whitelabel":false,"cookiePolicyId":{{ cx_iubenda.iub_policy_id }},"lang":"{{ LANGUAGE_CODE }}", "banner":{ "acceptButtonDisplay":true,"backgroundOverlay":true,"closeButtonRejects":true,"customizeButtonDisplay":true,"explicitWithdrawal":true,"fontSize":"14px","listPurposes":true,"position":"float-center","rejectButtonDisplay":true }};</script>
+
+<!-- JS Iubenda -->
+<script type="text/javascript" src="https://cdn.iubenda.com/cs/ccpa/stub.js"></script>
+<script type="text/javascript" src="https://cdn.iubenda.com/cs/iubenda_cs.js" charset="UTF-8" async></script>
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/templates/iubenda/privacy.html` & `django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy-compress.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-{% extends 'base.html' %}
-{% load i18n static compress %}
-
-{% block head_canonical %}
-    <link href="{{ SITE_URL }}{{ request.get_full_path }}" rel="canonical">
-{% endblock head_canonical %}
-
-{% block itemtype %}{% endblock itemtype %}
-
-{% block extra_title %} - Privacy Policy{% endblock extra_title %}
-
-{% block content %}
-<section id="privacy">
-  <div class="wrapper light-wrapper">
-    <div class="container inner">
-      <div class="row">
-        {% if req_privacy %}
-          {% block css %}
-        	{% compress css file iubenda %}
-            <link rel="stylesheet" type="text/css" href="{% static 'iubenda/css/iubenda_policy.css' %}">
-        	{% endcompress %}
-          {% endblock css %}
-
-          {{ req_privacy.content | safe }}
-        {% else %}
-          <!-- Could be added as class: "iub-legal-only" -->
-          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Privacy Policy">Privacy Policy</a>
-
-          {% block js %}
-          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
-          {% endblock js %}
-        {% endif %}
-      </div>
-      <!-- /.row -->
-    </div>
-    <!-- /.container -->
-  </div>
-  <!-- /.wrapper -->
-</section>
-<!-- /#privacy -->
-{% endblock content %}
-
+{% extends 'base.html' %}
+{% load i18n static compress %}
+
+{% block head_canonical %}
+    <link href="{{ SITE_URL }}{{ request.get_full_path }}" rel="canonical">
+{% endblock head_canonical %}
+
+{% block itemtype %}{% endblock itemtype %}
+
+{% block extra_title %} - Privacy Policy{% endblock extra_title %}
+
+{% block content %}
+<section id="privacy">
+  <div class="wrapper light-wrapper">
+    <div class="container inner">
+      <div class="row">
+        {% if req_privacy %}
+          {% block css %}
+        	{% compress css file iubenda %}
+            <link rel="stylesheet" type="text/css" href="{% static 'iubenda/css/iubenda_policy.css' %}">
+        	{% endcompress %}
+          {% endblock css %}
+
+          {{ req_privacy.content | safe }}
+        {% else %}
+          <!-- Could be added as class: "iub-legal-only" -->
+          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Privacy Policy">Privacy Policy</a>
+
+          {% block js %}
+          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
+          {% endblock js %}
+        {% endif %}
+      </div>
+      <!-- /.row -->
+    </div>
+    <!-- /.container -->
+  </div>
+  <!-- /.wrapper -->
+</section>
+<!-- /#privacy -->
+{% endblock content %}
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/urls.py` & `django-iubenda-1.2.6/src/iubenda/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-"""example URL Configuration
-
-The `urlpatterns` list routes URLs to views. For more information please see:
-    https://docs.djangoproject.com/en/1.9/topics/http/urls/
-Examples:
-Function views
-    1. Add an import:  from my_app import views
-    2. Add a URL to urlpatterns:  url(r'^$', views.home, name='home')
-Class-based views
-    1. Add an import:  from other_app.views import Home
-    2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
-Including another URLconf
-    1. Add an import:  from blog import urls as blog_urls
-    2. Import the include() function: from django.conf.urls import url, include
-    3. Add a URL to urlpatterns:  url(r'^blog/', include(blog_urls))
-"""
-from django.urls import path
-from .views import cookie, privacy
-
-urlpatterns = [
-    path('privacy-policy/', privacy, name='privacy'),
-    path('cookie-policy/', cookie, name='cookie'),
-]
+"""example URL Configuration
+
+The `urlpatterns` list routes URLs to views. For more information please see:
+    https://docs.djangoproject.com/en/1.9/topics/http/urls/
+Examples:
+Function views
+    1. Add an import:  from my_app import views
+    2. Add a URL to urlpatterns:  url(r'^$', views.home, name='home')
+Class-based views
+    1. Add an import:  from other_app.views import Home
+    2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
+Including another URLconf
+    1. Add an import:  from blog import urls as blog_urls
+    2. Import the include() function: from django.conf.urls import url, include
+    3. Add a URL to urlpatterns:  url(r'^blog/', include(blog_urls))
+"""
+from django.urls import path
+
+from .views import cookie, privacy
+
+urlpatterns = [
+    path("privacy-policy/", privacy, name="privacy"),
+    path("cookie-policy/", cookie, name="cookie"),
+]
```

### Comparing `django-iubenda-0.1.12.dev0/src/iubenda/views.py` & `django-iubenda-1.2.6/src/iubenda/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,85 @@
-from django.contrib import messages
-from django.contrib.sites.models import Site
-from django.core.cache import cache
-from django.views.decorators.http import require_http_methods
-from django.views.decorators.vary import vary_on_headers
-from django.shortcuts import render
-from .models import Iubenda
-import requests
-import json
-
-
-@require_http_methods(["GET"])
-@vary_on_headers('User-Agent', 'Cookie')
-def privacy(request):
-    context = {}
-
-    cache_key = f"api_iubenda_privacy_{request.LANGUAGE_CODE}"
-    context_cache = None
-    try:
-        context_cache = cache.get(cache_key)
-    except Exception as err:
-        context_cache = None
-
-    if context_cache is None:
-        try:
-            iubenda = Iubenda.objects.filter(site=Site.objects.get_current()).values('iub_policy_id').get()
-            r = requests.get(f'https://www.iubenda.com/api/privacy-policy/{iubenda["iub_policy_id"]}', params=request.GET)
-            if r.status_code == 200:
-                context = {"req_privacy": json.loads(r.content)}
-            context_cache = cache.set(cache_key, context, timeout=86400)
-            return render(request, 'iubenda/privacy.html', context)
-        except Exception as err:
-            messages.error(request, err)
-    return render(request, 'iubenda/privacy.html', context_cache)
-
-
-@require_http_methods(["GET"])
-@vary_on_headers('User-Agent', 'Cookie')
-def cookie(request):
-    context = {}
-
-    cache_key = f"api_iubenda_cookie_{request.LANGUAGE_CODE}"
-    context_cache = None
-    try:
-        context_cache = cache.get(cache_key)
-    except Exception as err:
-        context_cache = None
-
-    if context_cache is None:
-        try:
-            iubenda = Iubenda.objects.filter(site=Site.objects.get_current()).values('iub_policy_id').get()
-            r = requests.get(f'https://www.iubenda.com/api/privacy-policy/{iubenda["iub_policy_id"]}/cookie-policy', params=request.GET)
-            if r.status_code == 200:
-                context = {"req_cookie": json.loads(r.content)}
-            context_cache = cache.set(cache_key, context, timeout=86400)
-            return render(request, 'iubenda/cookie.html', context)
-        except Exception as err:
-            messages.error(request, err)
-    return render(request, 'iubenda/cookie.html', context_cache)
-
-
-
+import json
+
+import requests
+from django.conf import settings
+from django.contrib import messages
+from django.contrib.sites.models import Site
+from django.core.cache import cache
+from django.shortcuts import render
+from django.views.decorators.http import require_http_methods
+from django.views.decorators.vary import vary_on_headers
+
+from .models import Iubenda
+
+
+@require_http_methods(["GET"])
+@vary_on_headers("User-Agent", "Cookie")
+def privacy(request):
+    context = {}
+
+    cache_key = f"api_iubenda_privacy_{request.LANGUAGE_CODE}"
+    context_cache = None
+    try:
+        context_cache = cache.get(cache_key)
+    except Exception as err:
+        messages.warning(request, err)
+        context_cache = None
+
+    if context_cache is None:
+        try:
+            iubenda = (
+                Iubenda.objects.filter(site=Site.objects.get_current())
+                .values("iub_policy_id")
+                .get()
+            )
+            r = requests.get(
+                f'https://www.iubenda.com/api/privacy-policy/{iubenda["iub_policy_id"]}',
+                params=request.GET,
+            )
+            if r.status_code == 200:
+                context = {"req_privacy": json.loads(r.content)}
+            context_cache = cache.set(cache_key, context, timeout=86400)
+
+            if getattr(settings, "IUBENDA_USE_COMPRESS", True):
+                return render(request, "iubenda/privacy-compress.html", context)
+            return render(request, "iubenda/privacy.html", context)
+        except Exception as err:
+            messages.error(request, err)
+    return render(request, "iubenda/privacy.html", context_cache)
+
+
+@require_http_methods(["GET"])
+@vary_on_headers("User-Agent", "Cookie")
+def cookie(request):
+    context = {}
+
+    cache_key = f"api_iubenda_cookie_{request.LANGUAGE_CODE}"
+    context_cache = None
+    try:
+        context_cache = cache.get(cache_key)
+    except Exception as err:
+        messages.warning(request, err)
+        context_cache = None
+
+    if context_cache is None:
+        try:
+            iubenda = (
+                Iubenda.objects.filter(site=Site.objects.get_current())
+                .values("iub_policy_id")
+                .get()
+            )
+            r = requests.get(
+                f'https://www.iubenda.com/api/privacy-policy/{iubenda["iub_policy_id"]}/cookie-policy',
+                params=request.GET,
+            )
+            if r.status_code == 200:
+                context = {"req_cookie": json.loads(r.content)}
+
+            cache.set(cache_key, context, timeout=86400)
+            context_cache = cache.get(cache_key)
+
+        except Exception as err:
+            messages.error(request, err)
+    if getattr(settings, "IUBENDA_USE_COMPRESS", True):
+        return render(request, "iubenda/cookie-compress.html", context_cache)
+    return render(request, "iubenda/cookie.html", context_cache)
```

### Comparing `django-iubenda-0.1.12.dev0/tox.ini` & `django-iubenda-1.2.6/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,47 @@
-00000000: 5b74 6f78 5d0d 0a69 736f 6c61 7465 645f  [tox]..isolated_
-00000010: 6275 696c 6420 3d20 5472 7565 0d0a 656e  build = True..en
-00000020: 766c 6973 7420 3d0d 0a20 2020 2070 7933  vlist =..    py3
-00000030: 372d 646a 616e 676f 7b33 327d 0d0a 2020  7-django{32}..  
-00000040: 2020 7079 3338 2d64 6a61 6e67 6f7b 3332    py38-django{32
-00000050: 2c34 307d 0d0a 2020 2020 7079 3339 2d64  ,40}..    py39-d
-00000060: 6a61 6e67 6f7b 3332 2c34 307d 0d0a 2020  jango{32,40}..  
-00000070: 2020 7079 3331 302d 646a 616e 676f 7b33    py310-django{3
-00000080: 322c 3430 7d0d 0a20 2020 2070 7933 3131  2,40}..    py311
-00000090: 2d64 6a61 6e67 6f7b 3332 2c34 307d 0d0a  -django{32,40}..
-000000a0: 0d0a 5b74 6573 7465 6e76 5d0d 0a63 6f6d  ..[testenv]..com
-000000b0: 6d61 6e64 7320 3d20 7079 7468 6f6e 202d  mands = python -
-000000c0: 5720 6572 726f 723a 3a44 6570 7265 6361  W error::Depreca
-000000d0: 7469 6f6e 5761 726e 696e 6720 2d57 2065  tionWarning -W e
-000000e0: 7272 6f72 3a3a 5065 6e64 696e 6744 6570  rror::PendingDep
-000000f0: 7265 6361 7469 6f6e 5761 726e 696e 6720  recationWarning 
-00000100: 2d6d 2063 6f76 6572 6167 6520 7275 6e20  -m coverage run 
-00000110: 2d2d 7061 7261 6c6c 656c 202d 6d20 7079  --parallel -m py
-00000120: 7465 7374 207b 706f 7361 7267 733a 7465  test {posargs:te
-00000130: 7374 737d 0d0a 0d0a 5b74 6573 7465 6e76  sts}....[testenv
-00000140: 3a70 7933 372d 646a 616e 676f 3332 5d0d  :py37-django32].
-00000150: 0a64 6570 7320 3d20 2d72 7265 7175 6972  .deps = -rrequir
-00000160: 656d 656e 7473 2f70 7933 372d 646a 616e  ements/py37-djan
-00000170: 676f 3332 2e74 7874 0d0a 0d0a 5b74 6573  go32.txt....[tes
-00000180: 7465 6e76 3a70 7933 382d 646a 616e 676f  tenv:py38-django
-00000190: 3332 5d0d 0a64 6570 7320 3d20 2d72 7265  32]..deps = -rre
-000001a0: 7175 6972 656d 656e 7473 2f70 7933 382d  quirements/py38-
-000001b0: 646a 616e 676f 3332 2e74 7874 0d0a 0d0a  django32.txt....
-000001c0: 5b74 6573 7465 6e76 3a70 7933 382d 646a  [testenv:py38-dj
-000001d0: 616e 676f 3430 5d0d 0a64 6570 7320 3d20  ango40]..deps = 
-000001e0: 2d72 7265 7175 6972 656d 656e 7473 2f70  -rrequirements/p
-000001f0: 7933 382d 646a 616e 676f 3430 2e74 7874  y38-django40.txt
-00000200: 0d0a 0d0a 5b74 6573 7465 6e76 3a70 7933  ....[testenv:py3
-00000210: 392d 646a 616e 676f 3332 5d0d 0a64 6570  9-django32]..dep
-00000220: 7320 3d20 2d72 7265 7175 6972 656d 656e  s = -rrequiremen
-00000230: 7473 2f70 7933 392d 646a 616e 676f 3332  ts/py39-django32
-00000240: 2e74 7874 0d0a 0d0a 5b74 6573 7465 6e76  .txt....[testenv
-00000250: 3a70 7933 392d 646a 616e 676f 3430 5d0d  :py39-django40].
-00000260: 0a64 6570 7320 3d20 2d72 7265 7175 6972  .deps = -rrequir
-00000270: 656d 656e 7473 2f70 7933 392d 646a 616e  ements/py39-djan
-00000280: 676f 3430 2e74 7874 0d0a 0d0a 5b74 6573  go40.txt....[tes
-00000290: 7465 6e76 3a70 7933 3130 2d64 6a61 6e67  tenv:py310-djang
-000002a0: 6f33 325d 0d0a 6465 7073 203d 202d 7272  o32]..deps = -rr
-000002b0: 6571 7569 7265 6d65 6e74 732f 7079 3331  equirements/py31
-000002c0: 302d 646a 616e 676f 3332 2e74 7874 0d0a  0-django32.txt..
-000002d0: 0d0a 5b74 6573 7465 6e76 3a70 7933 3130  ..[testenv:py310
-000002e0: 2d64 6a61 6e67 6f34 305d 0d0a 6465 7073  -django40]..deps
-000002f0: 203d 202d 7272 6571 7569 7265 6d65 6e74   = -rrequirement
-00000300: 732f 7079 3331 302d 646a 616e 676f 3430  s/py310-django40
-00000310: 2e74 7874 0d0a 0d0a 5b74 6573 7465 6e76  .txt....[testenv
-00000320: 3a70 7933 3131 2d64 6a61 6e67 6f33 325d  :py311-django32]
-00000330: 0d0a 6465 7073 203d 202d 7272 6571 7569  ..deps = -rrequi
-00000340: 7265 6d65 6e74 732f 7079 3331 312d 646a  rements/py311-dj
-00000350: 616e 676f 3332 2e74 7874 0d0a 0d0a 5b74  ango32.txt....[t
-00000360: 6573 7465 6e76 3a70 7933 3131 2d64 6a61  estenv:py311-dja
-00000370: 6e67 6f34 305d 0d0a 6465 7073 203d 202d  ngo40]..deps = -
-00000380: 7272 6571 7569 7265 6d65 6e74 732f 7079  rrequirements/py
-00000390: 3331 312d 646a 616e 676f 3430 2e74 7874  311-django40.txt
-000003a0: 0d0a                                     ..
+00000000: 5b74 6f78 5d0a 6973 6f6c 6174 6564 5f62  [tox].isolated_b
+00000010: 7569 6c64 203d 2054 7275 650a 656e 766c  uild = True.envl
+00000020: 6973 7420 3d0a 2020 2020 7079 7b33 382c  ist =.    py{38,
+00000030: 3339 2c33 3130 2c33 3131 7d2d 646a 616e  39,310,311}-djan
+00000040: 676f 7b33 322c 3432 7d0a 0a5b 7465 7374  go{32,42}..[test
+00000050: 656e 765d 0a63 6f6d 6d61 6e64 7320 3d20  env].commands = 
+00000060: 7079 7468 6f6e 202d 5720 6572 726f 723a  python -W error:
+00000070: 3a44 6570 7265 6361 7469 6f6e 5761 726e  :DeprecationWarn
+00000080: 696e 6720 2d57 2065 7272 6f72 3a3a 5065  ing -W error::Pe
+00000090: 6e64 696e 6744 6570 7265 6361 7469 6f6e  ndingDeprecation
+000000a0: 5761 726e 696e 6720 2d6d 2063 6f76 6572  Warning -m cover
+000000b0: 6167 6520 7275 6e20 2d2d 7061 7261 6c6c  age run --parall
+000000c0: 656c 202d 6d20 7079 7465 7374 207b 706f  el -m pytest {po
+000000d0: 7361 7267 733a 7465 7374 737d 0a0a 5b74  sargs:tests}..[t
+000000e0: 6573 7465 6e76 3a70 7933 382d 646a 616e  estenv:py38-djan
+000000f0: 676f 3332 5d0a 6465 7073 203d 202d 7272  go32].deps = -rr
+00000100: 6571 7569 7265 6d65 6e74 732f 7079 3338  equirements/py38
+00000110: 2d64 6a61 6e67 6f33 322e 7478 740a 0a5b  -django32.txt..[
+00000120: 7465 7374 656e 763a 7079 3338 2d64 6a61  testenv:py38-dja
+00000130: 6e67 6f34 325d 0a64 6570 7320 3d20 2d72  ngo42].deps = -r
+00000140: 7265 7175 6972 656d 656e 7473 2f70 7933  requirements/py3
+00000150: 382d 646a 616e 676f 3432 2e74 7874 0a0a  8-django42.txt..
+00000160: 5b74 6573 7465 6e76 3a70 7933 392d 646a  [testenv:py39-dj
+00000170: 616e 676f 3332 5d0a 6465 7073 203d 202d  ango32].deps = -
+00000180: 7272 6571 7569 7265 6d65 6e74 732f 7079  rrequirements/py
+00000190: 3339 2d64 6a61 6e67 6f33 322e 7478 740a  39-django32.txt.
+000001a0: 0a5b 7465 7374 656e 763a 7079 3339 2d64  .[testenv:py39-d
+000001b0: 6a61 6e67 6f34 325d 0a64 6570 7320 3d20  jango42].deps = 
+000001c0: 2d72 7265 7175 6972 656d 656e 7473 2f70  -rrequirements/p
+000001d0: 7933 392d 646a 616e 676f 3432 2e74 7874  y39-django42.txt
+000001e0: 0a0a 5b74 6573 7465 6e76 3a70 7933 3130  ..[testenv:py310
+000001f0: 2d64 6a61 6e67 6f33 325d 0a64 6570 7320  -django32].deps 
+00000200: 3d20 2d72 7265 7175 6972 656d 656e 7473  = -rrequirements
+00000210: 2f70 7933 3130 2d64 6a61 6e67 6f33 322e  /py310-django32.
+00000220: 7478 740a 0a5b 7465 7374 656e 763a 7079  txt..[testenv:py
+00000230: 3331 302d 646a 616e 676f 3432 5d0a 6465  310-django42].de
+00000240: 7073 203d 202d 7272 6571 7569 7265 6d65  ps = -rrequireme
+00000250: 6e74 732f 7079 3331 302d 646a 616e 676f  nts/py310-django
+00000260: 3432 2e74 7874 0a0a 5b74 6573 7465 6e76  42.txt..[testenv
+00000270: 3a70 7933 3131 2d64 6a61 6e67 6f33 325d  :py311-django32]
+00000280: 0a64 6570 7320 3d20 2d72 7265 7175 6972  .deps = -rrequir
+00000290: 656d 656e 7473 2f70 7933 3131 2d64 6a61  ements/py311-dja
+000002a0: 6e67 6f33 322e 7478 740a 0a5b 7465 7374  ngo32.txt..[test
+000002b0: 656e 763a 7079 3331 312d 646a 616e 676f  env:py311-django
+000002c0: 3432 5d0a 6465 7073 203d 202d 7272 6571  42].deps = -rreq
+000002d0: 7569 7265 6d65 6e74 732f 7079 3331 312d  uirements/py311-
+000002e0: 646a 616e 676f 3432 2e74 7874 0a         django42.txt.
```

