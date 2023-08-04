# Comparing `tmp/django-errors-2.3.2.tar.gz` & `tmp/django-errors-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-errors-2.3.2.tar", last modified: Sat Jul 29 16:17:48 2023, max compression
+gzip compressed data, was "django-errors-2.3.4.tar", last modified: Fri Aug  4 23:02:46 2023, max compression
```

## Comparing `django-errors-2.3.2.tar` & `django-errors-2.3.4.tar`

### file list

```diff
@@ -1,102 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.664380 django-errors-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 16:17:34.000000 django-errors-2.3.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 16:17:34.000000 django-errors-2.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-29 16:17:34.000000 django-errors-2.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 16:17:34.000000 django-errors-2.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-29 16:17:34.000000 django-errors-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 16:17:34.000000 django-errors-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 16:17:48.664380 django-errors-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-29 16:17:34.000000 django-errors-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-29 16:17:34.000000 django-errors-2.3.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-29 16:17:34.000000 django-errors-2.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29213 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-29 16:17:34.000000 django-errors-2.3.2/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-29 16:17:34.000000 django-errors-2.3.2/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 16:17:48.664380 django-errors-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-29 16:17:34.000000 django-errors-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/cn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/cn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.648379 django-errors-2.3.2/src/django_errors/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/zh_hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/locale/zh_hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.652379 django-errors-2.3.2/src/django_errors/locale/zh_hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/locale/zh_hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/middleware/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.660380 django-errors-2.3.2/src/django_errors/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/405.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-29 16:17:34.000000 django-errors-2.3.2/src/django_errors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.656379 django-errors-2.3.2/src/django_errors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 16:17:48.000000 django-errors-2.3.2/src/django_errors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:48.664380 django-errors-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_locale_it.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/test_errors_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-29 16:17:34.000000 django-errors-2.3.2/tests/views_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 16:17:34.000000 django-errors-2.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.420655 django-errors-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:02:34.000000 django-errors-2.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 23:02:34.000000 django-errors-2.3.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:02:34.000000 django-errors-2.3.4/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-04 23:02:34.000000 django-errors-2.3.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:02:34.000000 django-errors-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-04 23:02:34.000000 django-errors-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-08-04 23:02:46.420655 django-errors-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-04 23:02:34.000000 django-errors-2.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-04 23:02:34.000000 django-errors-2.3.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-04 23:02:34.000000 django-errors-2.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.412655 django-errors-2.3.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 23:02:34.000000 django-errors-2.3.4/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:02:34.000000 django-errors-2.3.4/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-04 23:02:46.420655 django-errors-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-04 23:02:34.000000 django-errors-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.412655 django-errors-2.3.4/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/zh_hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/zh_hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/locale/zh_hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/locale/zh_hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.408655 django-errors-2.3.4/src/django_errors/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-04 23:02:34.000000 django-errors-2.3.4/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.416655 django-errors-2.3.4/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 23:02:46.000000 django-errors-2.3.4/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:46.420655 django-errors-2.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_locale_it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/test_errors_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-04 23:02:34.000000 django-errors-2.3.4/tests/views_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:02:34.000000 django-errors-2.3.4/tox.ini
```

### Comparing `django-errors-2.3.2/.pre-commit-config.yaml` & `django-errors-2.3.4/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,16 @@
   - id: check-case-conflict
   - id: check-json
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-toml
   - id: end-of-file-fixer
   - id: trailing-whitespace
-    exclude: .bumpversion.cfg
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.9.0
+  rev: v3.10.1
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/psf/black
   rev: 23.7.0
   hooks:
   - id: black
@@ -28,21 +27,21 @@
     - black>=22.12.0
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
     args: ["--profile", "black"]
 - repo: https://github.com/PyCQA/flake8
-  rev: 6.0.0
+  rev: 6.1.0
   hooks:
   - id: flake8
     additional_dependencies:
     - flake8-bugbear
     - flake8-comprehensions
     - flake8-tidy-imports
     - flake8-typing-imports
 - repo: https://github.com/mgedmin/check-manifest
   rev: "0.49"
   hooks:
   - id: check-manifest
     args: [--no-build-isolation]
-    additional_dependencies: ["Django>=2.2"]
+    additional_dependencies: ["Django>=3.2"]
```

### Comparing `django-errors-2.3.2/LICENSE` & `django-errors-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/PKG-INFO` & `django-errors-2.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.3.2
+Version: 2.3.4
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yaml)
 
 ## Check Demo Project
 * Browser the demo app on-line on [Heroku](https://django-errors.herokuapp.com/)
 * Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-errors)
 
 ## Requirements
 -   Python 3.8+ supported.
```

### Comparing `django-errors-2.3.2/README.md` & `django-errors-2.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yaml)
 
 ## Check Demo Project
 * Browser the demo app on-line on [Heroku](https://django-errors.herokuapp.com/)
 * Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-errors)
 
 ## Requirements
 -   Python 3.8+ supported.
```

### Comparing `django-errors-2.3.2/mkdocs.yml` & `django-errors-2.3.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/pyproject.toml` & `django-errors-2.3.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -48,7 +48,18 @@
   { name = "Deprecations and Removals", directory = "removal", showcontent = true },
   { name = "Features",                  directory = "feature", showcontent = true },
   { name = "Bug Fixes",                 directory = "bugfix",  showcontent = true },
   { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
   { name = "Improved Documentation",    directory = "doc",     showcontent = true },
   { name = "Trivial Changes",           directory = "trivial", showcontent = false },
 ]
+
+# bump-my-version
+[tool.bumpversion]
+current_version = "2.3.4"
+allow_dirty = true
+
+[[tool.bumpversion.files]]
+filename = "./setup.cfg"
+
+[[tool.bumpversion.files]]
+filename = "./src/django_errors/__init__.py"
```

### Comparing `django-errors-2.3.2/requirements/docs.txt` & `django-errors-2.3.4/requirements/docs.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/docs.txt requirements/docs.in
 #
 certifi==2023.7.22 \
     --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
     --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
@@ -81,17 +81,17 @@
     --hash=sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c \
     --hash=sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918 \
     --hash=sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1 \
     --hash=sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c \
     --hash=sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac \
     --hash=sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa
     # via requests
-click==8.1.5 \
-    --hash=sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367 \
-    --hash=sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548
+click==8.1.6 \
+    --hash=sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd \
+    --hash=sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5
     # via mkdocs
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via mkdocs-material
 ghp-import==2.1.0 \
     --hash=sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619 \
@@ -112,17 +112,17 @@
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
     # via
     #   mkdocs
     #   mkdocs-git-revision-date-plugin
     #   mkdocs-material
-markdown==3.3.7 \
-    --hash=sha256:cbb516f16218e643d8e0a95b309f77eb118cb138d39a4f27851e6a63581db874 \
-    --hash=sha256:f5da449a6e1c989a4cea2631aa8ee67caa5a2ef855d551c88f9e309f4634c621
+markdown==3.4.4 \
+    --hash=sha256:225c6123522495d4119a90b3a3ba31a1e87a70369e03f14799ea9c0d7183a3d6 \
+    --hash=sha256:a4c1b65c0957b4bd9e7d86ddc7b3c9868fb9670660f6f99f6d1bca8954d5a941
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
 markupsafe==2.1.3 \
     --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
     --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
@@ -170,94 +170,104 @@
     --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
     --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
     --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
     --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
     --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
     --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
     --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2
-    # via jinja2
+    # via
+    #   jinja2
+    #   mkdocs
 mergedeep==1.3.4 \
     --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
     --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
     # via mkdocs
-mkdocs==1.4.3 \
-    --hash=sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57 \
-    --hash=sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd
+mkdocs==1.5.2 \
+    --hash=sha256:60a62538519c2e96fe8426654a67ee177350451616118a41596ae7c876bb7eac \
+    --hash=sha256:70d0da09c26cff288852471be03c23f0f521fc15cf16ac89c7a3bfb9ae8d24f9
     # via
-    #   -r docs.in
+    #   -r requirements/docs.in
     #   mkdocs-git-revision-date-plugin
     #   mkdocs-material
 mkdocs-git-revision-date-plugin==0.3.2 \
     --hash=sha256:2e67956cb01823dd2418e2833f3623dee8604cdf223bddd005fe36226a56f6ef
-    # via -r docs.in
-mkdocs-material==9.1.18 \
-    --hash=sha256:5bcf8fb79ac2f253c0ffe93fa181cba87718c6438f459dc4180ac7418cc9a450 \
-    --hash=sha256:981dd39979723d4cda7cfc77bbbe5e54922d5761a7af23fb8ba9edb52f114b13
-    # via -r docs.in
+    # via -r requirements/docs.in
+mkdocs-material==9.1.21 \
+    --hash=sha256:58bb2f11ef240632e176d6f0f7d1cff06be1d11c696a5a1b553b808b4280ed47 \
+    --hash=sha256:71940cdfca84ab296b6362889c25395b1621273fb16c93deda257adb7ff44ec8
+    # via -r requirements/docs.in
 mkdocs-material-extensions==1.1.1 \
     --hash=sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93 \
     --hash=sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945
     # via mkdocs-material
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via mkdocs
+pathspec==0.11.2 \
+    --hash=sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20 \
+    --hash=sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3
+    # via mkdocs
+platformdirs==3.10.0 \
+    --hash=sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d \
+    --hash=sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d
+    # via mkdocs
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via mkdocs-material
 pymdown-extensions==10.1 \
     --hash=sha256:508009b211373058debb8247e168de4cbcb91b1bff7b5e961b2c3e864e00b195 \
     --hash=sha256:ef25dbbae530e8f67575d222b75ff0649b1e841e22c2ae9a20bad9472c2207dc
     # via mkdocs-material
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via ghp-import
-pyyaml==6.0 \
-    --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
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
-    --hash=sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782 \
-    --hash=sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0 \
-    --hash=sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92 \
-    --hash=sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f \
-    --hash=sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2 \
-    --hash=sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc \
-    --hash=sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1 \
-    --hash=sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c \
-    --hash=sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86 \
-    --hash=sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4 \
-    --hash=sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c \
-    --hash=sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34 \
-    --hash=sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b \
-    --hash=sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d \
-    --hash=sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c \
-    --hash=sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb \
-    --hash=sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7 \
-    --hash=sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737 \
-    --hash=sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3 \
-    --hash=sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d \
-    --hash=sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358 \
-    --hash=sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53 \
-    --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
-    --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
-    --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
-    --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
-    --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
-    --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
+pyyaml==6.0.1 \
+    --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
+    --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
+    --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
+    --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
+    --hash=sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595 \
+    --hash=sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62 \
+    --hash=sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98 \
+    --hash=sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696 \
+    --hash=sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d \
+    --hash=sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867 \
+    --hash=sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47 \
+    --hash=sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486 \
+    --hash=sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6 \
+    --hash=sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3 \
+    --hash=sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007 \
+    --hash=sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938 \
+    --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
+    --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
+    --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
+    --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
+    --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
+    --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
+    --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
+    --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
+    --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
+    --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
+    --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
+    --hash=sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924 \
+    --hash=sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34 \
+    --hash=sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43 \
+    --hash=sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859 \
+    --hash=sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673 \
+    --hash=sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a \
+    --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
+    --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
+    --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
+    --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
+    --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
+    --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1 \
     --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
     --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
@@ -360,17 +370,17 @@
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via python-dateutil
 smmap==5.0.0 \
     --hash=sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94 \
     --hash=sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936
     # via gitdb
-urllib3==2.0.3 \
-    --hash=sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1 \
-    --hash=sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825
+urllib3==2.0.4 \
+    --hash=sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11 \
+    --hash=sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4
     # via requests
 watchdog==3.0.0 \
     --hash=sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a \
     --hash=sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100 \
     --hash=sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8 \
     --hash=sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc \
     --hash=sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae \
```

### Comparing `django-errors-2.3.2/requirements/py310-django32.txt` & `django-errors-2.3.4/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/requirements/py310-django42.txt` & `django-errors-2.3.4/requirements/py38-django32.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,22 +66,26 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.3 \
-    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
-    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
+django==3.2.20 \
+    --hash=sha256:a477ab326ae7d8807dc25c186b951ab8c7648a3a23f9497763c37307a2b5ef87 \
+    --hash=sha256:dec2a116787b8e14962014bf78e120bba454135108e1af9e9b91ade7b2964c40
     # via -r requirements/requirements.in
 exceptiongroup==1.1.2 \
     --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
     --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
+    # via pytest-randomly
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
@@ -101,19 +105,27 @@
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
 pytest-randomly==3.13.0 \
     --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
     --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
+pytz==2023.3 \
+    --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
+    --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
+    # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via pytest
 typing-extensions==4.7.1 \
     --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
     --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via asgiref
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
+    # via importlib-metadata
```

### Comparing `django-errors-2.3.2/requirements/py311-django32.txt` & `django-errors-2.3.4/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/requirements/py311-django42.txt` & `django-errors-2.3.4/requirements/py311-django42.txt`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.3 \
-    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
-    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
+django==4.2.4 \
+    --hash=sha256:7e4225ec065e0f354ccf7349a22d209de09cc1c074832be9eb84c51c1799c432 \
+    --hash=sha256:860ae6a138a238fc4f22c99b52f3ead982bb4b1aad8c0122bcd8c8a3a02e409d
     # via -r requirements/requirements.in
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
```

### Comparing `django-errors-2.3.2/requirements/py38-django32.txt` & `django-errors-2.3.4/requirements/py39-django32.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
```

### Comparing `django-errors-2.3.2/requirements/py38-django42.txt` & `django-errors-2.3.4/requirements/py38-django42.txt`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.3 \
-    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
-    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
+django==4.2.4 \
+    --hash=sha256:7e4225ec065e0f354ccf7349a22d209de09cc1c074832be9eb84c51c1799c432 \
+    --hash=sha256:860ae6a138a238fc4f22c99b52f3ead982bb4b1aad8c0122bcd8c8a3a02e409d
     # via -r requirements/requirements.in
 exceptiongroup==1.1.2 \
     --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
     --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
 importlib-metadata==6.8.0 \
     --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
```

### Comparing `django-errors-2.3.2/requirements/py39-django32.txt` & `django-errors-2.3.4/requirements/py39-django42.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py39-django42.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,17 +66,17 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==3.2.20 \
-    --hash=sha256:a477ab326ae7d8807dc25c186b951ab8c7648a3a23f9497763c37307a2b5ef87 \
-    --hash=sha256:dec2a116787b8e14962014bf78e120bba454135108e1af9e9b91ade7b2964c40
+django==4.2.4 \
+    --hash=sha256:7e4225ec065e0f354ccf7349a22d209de09cc1c074832be9eb84c51c1799c432 \
+    --hash=sha256:860ae6a138a238fc4f22c99b52f3ead982bb4b1aad8c0122bcd8c8a3a02e409d
     # via -r requirements/requirements.in
 exceptiongroup==1.1.2 \
     --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
     --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
 importlib-metadata==6.8.0 \
     --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
@@ -105,18 +105,14 @@
     --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
     --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
     # via -r requirements/requirements.in
 pytest-randomly==3.13.0 \
     --hash=sha256:079c78b94693189879fbd7304de4e147304f0811fa96249ea5619f2f1cd33df0 \
     --hash=sha256:e78d898ef4066f89744e5075083aa7fb6f0de07ffd70ca9c4435cda590cf1eac
     # via -r requirements/requirements.in
-pytz==2023.3 \
-    --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
-    --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
-    # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
```

### Comparing `django-errors-2.3.2/requirements/py39-django42.txt` & `django-errors-2.3.4/requirements/py310-django42.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py39-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
 #
 asgiref==3.7.2 \
     --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
     --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
     # via django
 coverage==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
@@ -66,26 +66,22 @@
     --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
     --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/requirements.in
-django==4.2.3 \
-    --hash=sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed \
-    --hash=sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039
+django==4.2.4 \
+    --hash=sha256:7e4225ec065e0f354ccf7349a22d209de09cc1c074832be9eb84c51c1799c432 \
+    --hash=sha256:860ae6a138a238fc4f22c99b52f3ead982bb4b1aad8c0122bcd8c8a3a02e409d
     # via -r requirements/requirements.in
 exceptiongroup==1.1.2 \
     --hash=sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5 \
     --hash=sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f
     # via pytest
-importlib-metadata==6.8.0 \
-    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
-    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
-    # via pytest-randomly
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
@@ -117,11 +113,7 @@
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via pytest
 typing-extensions==4.7.1 \
     --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
     --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via asgiref
-zipp==3.16.2 \
-    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
-    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
-    # via importlib-metadata
```

### Comparing `django-errors-2.3.2/runtests.py` & `django-errors-2.3.4/runtests.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/setup.cfg` & `django-errors-2.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-errors
-version = 2.3.2
+version = 2.3.4
 url = https://github.com/DLRSP/django-errors
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling server errors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-errors-2.3.2/setup.py` & `django-errors-2.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/cn/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/de/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/en/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/es/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/fr/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/it/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/ja/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/lt/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/nl/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/ru/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/zh_hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po` & `django-errors-2.3.4/src/django_errors/locale/zh_hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/middleware/handler.py` & `django-errors-2.3.4/src/django_errors/middleware/handler.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors/views.py` & `django-errors-2.3.4/src/django_errors/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/src/django_errors.egg-info/PKG-INFO` & `django-errors-2.3.4/src/django_errors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 2.3.2
+Version: 2.3.4
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-errors.svg)](https://pypi.python.org/pypi/django_errors)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-errors.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-errors.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-errors/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-errors?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-errors/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-errors/main) [![gitthub.com](https://github.com/DLRSP/django-errors/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-errors/actions/workflows/ci.yaml)
 
 ## Check Demo Project
 * Browser the demo app on-line on [Heroku](https://django-errors.herokuapp.com/)
 * Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-errors)
 
 ## Requirements
 -   Python 3.8+ supported.
```

### Comparing `django-errors-2.3.2/src/django_errors.egg-info/SOURCES.txt` & `django-errors-2.3.4/src/django_errors.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.bumpversion.cfg
 .pre-commit-config.yaml
 CHANGELOG.rst
+CODEOWNERS
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 mkdocs.yml
 pyproject.toml
 runtests.py
@@ -42,15 +42,14 @@
 src/django_errors/locale/lt/LC_MESSAGES/django.po
 src/django_errors/locale/nl/LC_MESSAGES/django.po
 src/django_errors/locale/ru/LC_MESSAGES/django.po
 src/django_errors/locale/zh_hans/LC_MESSAGES/django.po
 src/django_errors/locale/zh_hant/LC_MESSAGES/django.po
 src/django_errors/middleware/__init__.py
 src/django_errors/middleware/handler.py
-src/django_errors/templates/base.html
 src/django_errors/templates/errors/400.html
 src/django_errors/templates/errors/403.html
 src/django_errors/templates/errors/404.html
 src/django_errors/templates/errors/405.html
 src/django_errors/templates/errors/500.html
 tests/__init__.py
 tests/settings.py
```

### Comparing `django-errors-2.3.2/tests/settings.py` & `django-errors-2.3.4/tests/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Test's settings"""
+import os
+
 from django.utils.translation import gettext_noop
 
 DEBUG = False
 
+BASE_DIR = os.path.dirname(os.path.abspath(__file__))
+
 PASSWORD_HASHERS = ["django.contrib.auth.hashers.MD5PasswordHasher"]
 
 SECRET_KEY = "NOTASECRET"
 
 ALLOWED_HOSTS = ["*"]
 
 INSTALLED_APPS = [
@@ -18,15 +22,19 @@
     "django.contrib.messages",
     "django.contrib.staticfiles",
 ]
 
 DATABASES = {"default": {"ENGINE": "django.db.backends.sqlite3"}}
 
 TEMPLATES = [
-    {"BACKEND": "django.template.backends.django.DjangoTemplates", "APP_DIRS": True}
+    {
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "APP_DIRS": True,
+        "DIRS": [os.path.join(BASE_DIR, "templates")],
+    }
 ]
 
 ROOT_URLCONF = "tests.urls"
 
 MIDDLEWARE = (
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
```

### Comparing `django-errors-2.3.2/tests/test_errors.py` & `django-errors-2.3.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/test_errors_exceptions.py` & `django-errors-2.3.4/tests/test_errors_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/test_errors_locale_it.py` & `django-errors-2.3.4/tests/test_errors_locale_it.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/test_errors_standard.py` & `django-errors-2.3.4/tests/test_errors_standard.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/test_errors_templates.py` & `django-errors-2.3.4/tests/test_errors_templates.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/test_errors_urls.py` & `django-errors-2.3.4/tests/test_errors_urls.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/urls.py` & `django-errors-2.3.4/tests/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test's urls view for django-errors"""
 from django.conf.urls.i18n import i18n_patterns
 from django.contrib import admin
 from django.urls import include, path, re_path
 from django.views.i18n import JavaScriptCatalog
 
-from src.django_errors import views as errors_views
+from django_errors import views as errors_views
 
 from . import views, views_exceptions, views_standard, views_templates
 
 urlpatterns = [
     path("", include("django_errors.urls")),
     path("admin/", admin.site.urls),
     path("test-method-only-get/", views.test_view_405_only_get),
```

### Comparing `django-errors-2.3.2/tests/views.py` & `django-errors-2.3.4/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/views_standard.py` & `django-errors-2.3.4/tests/views_standard.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tests/views_templates.py` & `django-errors-2.3.4/tests/views_templates.py`

 * *Files identical despite different names*

### Comparing `django-errors-2.3.2/tox.ini` & `django-errors-2.3.4/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 [tox]
 isolated_build = True
 envlist =
-    py38-django{32,42}
-    py39-django{32,42}
-    py310-django{32,42}
-    py311-django{32,42}
+    py{38,39,310,311}-django{32,42}
 
 [testenv]
 commands = python -W error::DeprecationWarning -W error::PendingDeprecationWarning -m coverage run --parallel -m pytest {posargs:tests}
 
 [testenv:py38-django32]
 deps = -rrequirements/py38-django32.txt
```

