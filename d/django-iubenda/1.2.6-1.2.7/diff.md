# Comparing `tmp/django-iubenda-1.2.6.tar.gz` & `tmp/django-iubenda-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-1.2.6.tar", last modified: Fri Aug  4 23:01:08 2023, max compression
+gzip compressed data, was "django-iubenda-1.2.7.tar", last modified: Fri Aug  4 23:17:08 2023, max compression
```

## Comparing `django-iubenda-1.2.6.tar` & `django-iubenda-1.2.7.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.712355 django-iubenda-1.2.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-04 23:01:08.720355 django-iubenda-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.712355 django-iubenda-1.2.6/src/django_iubenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 23:01:08.000000 django-iubenda-1.2.6/src/django_iubenda.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/fixtures/data.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/sitemaps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/static/iubenda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/static/iubenda/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_badge.css
--rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_policy.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.708355 django-iubenda-1.2.6/src/iubenda/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/src/iubenda/templates/iubenda/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/cookie-compress.html
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/cookie.html
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/include-content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy-compress.html
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/src/iubenda/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:01:08.716355 django-iubenda-1.2.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/fixtures/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/test_iubenda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/test_iubenda_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/test_iubenda_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:00:55.000000 django-iubenda-1.2.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.091691 django-iubenda-1.2.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.079691 django-iubenda-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/django_iubenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/iubenda/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/fixtures/data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/iubenda/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.099691 django-iubenda-1.2.7/src/iubenda/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/static/iubenda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.099691 django-iubenda-1.2.7/src/iubenda/static/iubenda/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_badge.css
+-rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_policy.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.099691 django-iubenda-1.2.7/src/iubenda/templates/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie-compress.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/include-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy-compress.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/fixtures/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/test_iubenda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/test_iubenda_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/test_iubenda_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tox.ini
```

### Comparing `django-iubenda-1.2.6/.pre-commit-config.yaml` & `django-iubenda-1.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/LICENSE` & `django-iubenda-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/PKG-INFO` & `django-iubenda-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.2.6
+Version: 1.2.7
 Summary: Django application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,iubenda,privacy,cookie
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-iubenda.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-iubenda?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/main) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
 
 ## Compliance for websites and apps
 Click [here](http://iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda
 [![Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/dlrspapi)
 
 
 ## Check Demo Project
```

### Comparing `django-iubenda-1.2.6/README.md` & `django-iubenda-1.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-iubenda.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-iubenda?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/main) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
 
 ## Compliance for websites and apps
 Click [here](http://iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda
 [![Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/dlrspapi)
 
 
 ## Check Demo Project
```

#### html2text {}

```diff
@@ -8,41 +8,41 @@
 (https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/
 pypi/django-iubenda) [![PyPi downloads](https://img.shields.io/pypi/dw/django-
 iubenda.svg)](https://pypi.python.org/pypi/django-iubenda) [![PyPi downloads]
 (https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/
 pypi/django-iubenda) ## GitHub ![GitHub release](https://img.shields.io/github/
 tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/
 release/DLRSP/django-iubenda.svg) ## Test [![codecov.io](https://codecov.io/
-github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/
-github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://
-results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://
-results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [!
-[gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/
-ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/
-ci.yaml) ## Compliance for websites and apps Click [here](http://
-iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda [!
-[Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://
-iubenda.refr.cc/dlrspapi) ## Check Demo Project * Check the demo repo on
-[GitHub](https://github.com/DLRSP/example/tree/django-iubenda) ## Requirements
-- Python +3.8 supported. - Django +3.2 supported. ## Setup 1. Install from
-**pip**: ```shell pip install django-iubenda ``` 2. Modify `settings.py` by
-adding the app to `INSTALLED_APPS`: ```python INSTALLED_APPS =
-( "modeltranslation", # ... "iubenda", # ... ) ``` 3. Modify `settings.py` by
-adding the app's context processor to `TEMPLATES`: ```python TEMPLATES = [ { #
-... "OPTIONS": { "context_processors": [ # ...
-"iubenda.context_processors.iubenda", # ... ], }, }, ] ``` 4. Be sure the
-Django's Locale middleware is enabled inside `settings.py`: ```python
-MIDDLEWARE = ( # ... "django.middleware.locale.LocaleMiddleware", # ... ) ```
-5. Modify `url.py` by adding the app's urls to `urlpatterns`: ```python
-urlpatterns += [ path("", include("iubenda.urls")), ] ``` 6. Modify `url.py` by
-adding the app's sitemaps to `sitemaps`: ```python from iubenda.sitemaps import
-PrivacySitemap, CookieSitemap sitemaps = { # ... "privacy": PrivacySitemap,
-"cookie": CookieSitemap, # ... } ``` 7. Be sure the variable `LANGUAGE_CODE` is
-available for HTML templates: ```html {% load i18n %} {% get_current_language
-as LANGUAGE_CODE %} ``` 8. Modify your project's template to add privacy and
+github/DLRSP/django-iubenda/coverage.svg?branch=main)](https://codecov.io/
+github/DLRSP/django-iubenda?branch=main) [![pre-commit.ci status](https://
+results.pre-commit.ci/badge/github/DLRSP/django-iubenda/main.svg)](https://
+results.pre-commit.ci/latest/github/DLRSP/django-iubenda/main) [![gitthub.com]
+(https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)]
+(https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml) ##
+Compliance for websites and apps Click [here](http://iubenda.refr.cc/dlrspapi)
+and get 10% discount on first year at Iubenda [![Iubenda](https://
+cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/
+dlrspapi) ## Check Demo Project * Check the demo repo on [GitHub](https://
+github.com/DLRSP/example/tree/django-iubenda) ## Requirements - Python +3.8
+supported. - Django +3.2 supported. ## Setup 1. Install from **pip**: ```shell
+pip install django-iubenda ``` 2. Modify `settings.py` by adding the app to
+`INSTALLED_APPS`: ```python INSTALLED_APPS = ( "modeltranslation", # ...
+"iubenda", # ... ) ``` 3. Modify `settings.py` by adding the app's context
+processor to `TEMPLATES`: ```python TEMPLATES = [ { # ... "OPTIONS":
+{ "context_processors": [ # ... "iubenda.context_processors.iubenda", # ... ],
+}, }, ] ``` 4. Be sure the Django's Locale middleware is enabled inside
+`settings.py`: ```python MIDDLEWARE = ( # ...
+"django.middleware.locale.LocaleMiddleware", # ... ) ``` 5. Modify `url.py` by
+adding the app's urls to `urlpatterns`: ```python urlpatterns += [ path("",
+include("iubenda.urls")), ] ``` 6. Modify `url.py` by adding the app's sitemaps
+to `sitemaps`: ```python from iubenda.sitemaps import PrivacySitemap,
+CookieSitemap sitemaps = { # ... "privacy": PrivacySitemap, "cookie":
+CookieSitemap, # ... } ``` 7. Be sure the variable `LANGUAGE_CODE` is available
+for HTML templates: ```html {% load i18n %} {% get_current_language as
+LANGUAGE_CODE %} ``` 8. Modify your project's template to add privacy and
 cookie policies. For example inside the `footer.html` add following code:
 ```html {% if not debug %} {% block iubenda %}{% include "iubenda/include-
 content.html" %}{% endblock iubenda %} {% endif %} ``` ## Optional ### Content
 Security Policy If Content Security Policy are implemented in your server and
 inline scripts are disabled, the variable `IUBENDA_CSP_NONCE` can be set with
 nonce tag will be inserted script's nonce. ```html
 % if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}> ``` Inside
```

### Comparing `django-iubenda-1.2.6/mkdocs.yml` & `django-iubenda-1.2.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/pyproject.toml` & `django-iubenda-1.2.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
   { name = "Improved Documentation",    directory = "doc",     showcontent = true },
   { name = "Trivial Changes",           directory = "trivial", showcontent = false },
 ]
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "1.2.6"
+current_version = "1.2.7"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
 
 [[tool.bumpversion.files]]
 filename = "./src/iubenda/__init__.py"
```

### Comparing `django-iubenda-1.2.6/requirements/docs.txt` & `django-iubenda-1.2.7/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py310-django32.txt` & `django-iubenda-1.2.7/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py310-django42.txt` & `django-iubenda-1.2.7/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py311-django32.txt` & `django-iubenda-1.2.7/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py311-django42.txt` & `django-iubenda-1.2.7/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py38-django32.txt` & `django-iubenda-1.2.7/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py38-django42.txt` & `django-iubenda-1.2.7/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py39-django32.txt` & `django-iubenda-1.2.7/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/requirements/py39-django42.txt` & `django-iubenda-1.2.7/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/runtests.py` & `django-iubenda-1.2.7/runtests.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/setup.cfg` & `django-iubenda-1.2.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-iubenda
-version = 1.2.6
+version = 1.2.7
 url = https://github.com/DLRSP/django-iubenda
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling privacy and cookie policies configured with Iubenda.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-iubenda-1.2.6/setup.py` & `django-iubenda-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/django_iubenda.egg-info/PKG-INFO` & `django-iubenda-1.2.7/src/django_iubenda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.2.6
+Version: 1.2.7
 Summary: Django application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,iubenda,privacy,cookie
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 [![PyPi python version](https://img.shields.io/pypi/pyversions/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dm/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dw/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 [![PyPi downloads](https://img.shields.io/pypi/dd/django-iubenda.svg)](https://pypi.python.org/pypi/django-iubenda)
 
 ## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-iubenda.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-iubenda.svg)
 
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-iubenda?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/master) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-iubenda/coverage.svg?branch=main)](https://codecov.io/github/DLRSP/django-iubenda?branch=main) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-iubenda/main.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-iubenda/main) [![gitthub.com](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml/badge.svg)](https://github.com/DLRSP/django-iubenda/actions/workflows/ci.yaml)
 
 ## Compliance for websites and apps
 Click [here](http://iubenda.refr.cc/dlrspapi) and get 10% discount on first year at Iubenda
 [![Iubenda](https://cdn.filestackcontent.com/kTEmy2XBQJiiEy0ULvg0)](http://iubenda.refr.cc/dlrspapi)
 
 
 ## Check Demo Project
```

### Comparing `django-iubenda-1.2.6/src/django_iubenda.egg-info/SOURCES.txt` & `django-iubenda-1.2.7/src/django_iubenda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,8 +50,9 @@
 tests/__init__.py
 tests/settings.py
 tests/test_iubenda.py
 tests/test_iubenda_template.py
 tests/test_iubenda_urls.py
 tests/urls.py
 tests/views.py
-tests/fixtures/data.json
+tests/fixtures/data.json
+tests/templates/base.html
```

### Comparing `django-iubenda-1.2.6/src/iubenda/context_processors.py` & `django-iubenda-1.2.7/src/iubenda/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/locale/it/LC_MESSAGES/django.po` & `django-iubenda-1.2.7/src/iubenda/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/migrations/0001_initial.py` & `django-iubenda-1.2.7/src/iubenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/models.py` & `django-iubenda-1.2.7/src/iubenda/models.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_badge.css` & `django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_badge.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/static/iubenda/css/iubenda_policy.css` & `django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_policy.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/templates/iubenda/cookie-compress.html` & `django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie-compress.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/templates/iubenda/cookie.html` & `django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/templates/iubenda/include-content.html` & `django-iubenda-1.2.7/src/iubenda/templates/iubenda/include-content.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy-compress.html` & `django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy-compress.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/templates/iubenda/privacy.html` & `django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/urls.py` & `django-iubenda-1.2.7/src/iubenda/urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/src/iubenda/views.py` & `django-iubenda-1.2.7/src/iubenda/views.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/tests/settings.py` & `django-iubenda-1.2.7/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/tests/test_iubenda_template.py` & `django-iubenda-1.2.7/tests/test_iubenda_template.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/tests/test_iubenda_urls.py` & `django-iubenda-1.2.7/tests/test_iubenda_urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.6/tox.ini` & `django-iubenda-1.2.7/tox.ini`

 * *Files identical despite different names*

