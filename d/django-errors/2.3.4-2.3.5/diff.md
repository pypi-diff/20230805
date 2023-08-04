# Comparing `tmp/django-errors-2.3.4.tar.gz` & `tmp/django-errors-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-errors-2.3.4.tar", last modified: Fri Aug  4 23:02:46 2023, max compression
+gzip compressed data, was "django-errors-2.3.5.tar", last modified: Fri Aug  4 23:16:59 2023, max compression
```

## Comparing `django-errors-2.3.4.tar` & `django-errors-2.3.5.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.420655 django-errors-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:02:34.000000 django-errors-2.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 23:02:34.000000 django-errors-2.3.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:02:34.000000 django-errors-2.3.4/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-04 23:02:34.000000 django-errors-2.3.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:02:34.000000 django-errors-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-04 23:02:34.000000 django-errors-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-08-04 23:02:46.420655 django-errors-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-04 23:02:34.000000 django-errors-2.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-04 23:02:34.000000 django-errors-2.3.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-04 23:02:34.000000 django-errors-2.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.412655 django-errors-2.3.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:02:34.000000 django-errors-2.3.4/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-04 23:02:46.420655 django-errors-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-04 23:02:34.000000 django-errors-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.412655 django-errors-2.3.4/src/django_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/cn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/cn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/zh_hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/zh_hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/zh_hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/zh_hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/middleware/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/405.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.420655 django-errors-2.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_locale_it.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:02:34.000000 django-errors-2.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.620355 django-errors-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:16:38.000000 django-errors-2.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 23:16:38.000000 django-errors-2.3.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:16:38.000000 django-errors-2.3.5/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-04 23:16:38.000000 django-errors-2.3.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:16:38.000000 django-errors-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-04 23:16:38.000000 django-errors-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-08-04 23:16:59.620355 django-errors-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-04 23:16:38.000000 django-errors-2.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-04 23:16:38.000000 django-errors-2.3.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-04 23:16:38.000000 django-errors-2.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 23:16:38.000000 django-errors-2.3.5/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:16:38.000000 django-errors-2.3.5/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-04 23:16:59.620355 django-errors-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-04 23:16:38.000000 django-errors-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.608355 django-errors-2.3.5/src/django_errors/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/src/django_errors/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/src/django_errors/locale/zh_hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/zh_hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/src/django_errors/locale/zh_hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/locale/zh_hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.612355 django-errors-2.3.5/src/django_errors/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-04 23:16:38.000000 django-errors-2.3.5/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.616355 django-errors-2.3.5/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-08-04 23:16:59.000000 django-errors-2.3.5/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-04 23:16:59.000000 django-errors-2.3.5/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:16:59.000000 django-errors-2.3.5/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:16:59.000000 django-errors-2.3.5/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:16:59.000000 django-errors-2.3.5/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 23:16:59.000000 django-errors-2.3.5/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.620355 django-errors-2.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:59.620355 django-errors-2.3.5/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/test_errors_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/test_errors_locale_it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/test_errors_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/test_errors_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/test_errors_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/views_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/views_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-04 23:16:38.000000 django-errors-2.3.5/tests/views_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:16:38.000000 django-errors-2.3.5/tox.ini
```

### Comparing `django-errors-2.3.4/.pre-commit-config.yaml` & `django-errors-2.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/LICENSE` & `django-errors-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/PKG-INFO` & `django-errors-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.3.4
+Version: 2.3.5
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-2.3.4/README.md` & `django-errors-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/mkdocs.yml` & `django-errors-2.3.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/pyproject.toml` & `django-errors-2.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
   { name = "Improved Documentation",    directory = "doc",     showcontent = true },
   { name = "Trivial Changes",           directory = "trivial", showcontent = false },
 ]
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "2.3.4"
+current_version = "2.3.5"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
 
 [[tool.bumpversion.files]]
 filename = "./src/django_errors/__init__.py"
```

### Comparing `django-errors-2.3.4/requirements/docs.txt` & `django-errors-2.3.5/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py310-django32.txt` & `django-errors-2.3.5/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py310-django42.txt` & `django-errors-2.3.5/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py311-django32.txt` & `django-errors-2.3.5/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py311-django42.txt` & `django-errors-2.3.5/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py38-django32.txt` & `django-errors-2.3.5/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py38-django42.txt` & `django-errors-2.3.5/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py39-django32.txt` & `django-errors-2.3.5/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/requirements/py39-django42.txt` & `django-errors-2.3.5/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/runtests.py` & `django-errors-2.3.5/runtests.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/setup.cfg` & `django-errors-2.3.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-errors
-version = 2.3.4
+version = 2.3.5
 url = https://github.com/DLRSP/django-errors
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling server errors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-errors-2.3.4/setup.py` & `django-errors-2.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/cn/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/de/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/en/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/es/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/fr/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/it/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/ja/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/lt/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/nl/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/ru/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po` & `django-errors-2.3.5/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/middleware/handler.py` & `django-errors-2.3.5/src/django_errors/middleware/handler.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors/views.py` & `django-errors-2.3.5/src/django_errors/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/src/django_errors.egg-info/PKG-INFO` & `django-errors-2.3.5/src/django_errors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.3.4
+Version: 2.3.5
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-2.3.4/src/django_errors.egg-info/SOURCES.txt` & `django-errors-2.3.5/src/django_errors.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -59,8 +59,9 @@
 tests/test_errors_standard.py
 tests/test_errors_templates.py
 tests/test_errors_urls.py
 tests/urls.py
 tests/views.py
 tests/views_exceptions.py
 tests/views_standard.py
-tests/views_templates.py
+tests/views_templates.py
+tests/templates/base.html
```

### Comparing `django-errors-2.3.4/tests/settings.py` & `django-errors-2.3.5/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/test_errors.py` & `django-errors-2.3.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/test_errors_exceptions.py` & `django-errors-2.3.5/tests/test_errors_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/test_errors_locale_it.py` & `django-errors-2.3.5/tests/test_errors_locale_it.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/test_errors_standard.py` & `django-errors-2.3.5/tests/test_errors_standard.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/test_errors_templates.py` & `django-errors-2.3.5/tests/test_errors_templates.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/test_errors_urls.py` & `django-errors-2.3.5/tests/test_errors_urls.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/urls.py` & `django-errors-2.3.5/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/views.py` & `django-errors-2.3.5/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/views_standard.py` & `django-errors-2.3.5/tests/views_standard.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tests/views_templates.py` & `django-errors-2.3.5/tests/views_templates.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.4/tox.ini` & `django-errors-2.3.5/tox.ini`

 * *Files identical despite different names*

