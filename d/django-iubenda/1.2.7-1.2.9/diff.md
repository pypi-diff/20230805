# Comparing `tmp/django-iubenda-1.2.7.tar.gz` & `tmp/django-iubenda-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-1.2.7.tar", last modified: Fri Aug  4 23:17:08 2023, max compression
+gzip compressed data, was "django-iubenda-1.2.9.tar", last modified: Fri Aug  4 23:39:47 2023, max compression
```

## Comparing `django-iubenda-1.2.7.tar` & `django-iubenda-1.2.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.091691 django-iubenda-1.2.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.079691 django-iubenda-1.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/django_iubenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 23:17:08.000000 django-iubenda-1.2.7/src/django_iubenda.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/iubenda/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/iubenda/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/fixtures/data.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.095691 django-iubenda-1.2.7/src/iubenda/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.099691 django-iubenda-1.2.7/src/iubenda/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/sitemaps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/static/iubenda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.099691 django-iubenda-1.2.7/src/iubenda/static/iubenda/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_badge.css
--rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_policy.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.083691 django-iubenda-1.2.7/src/iubenda/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.099691 django-iubenda-1.2.7/src/iubenda/templates/iubenda/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie-compress.html
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie.html
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/include-content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy-compress.html
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/src/iubenda/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/fixtures/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:17:08.103691 django-iubenda-1.2.7/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/test_iubenda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/test_iubenda_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/test_iubenda_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:16:55.000000 django-iubenda-1.2.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.383698 django-iubenda-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-04 23:39:47.383698 django-iubenda-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.375698 django-iubenda-1.2.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-04 23:39:47.383698 django-iubenda-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.371698 django-iubenda-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.379698 django-iubenda-1.2.9/src/django_iubenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-04 23:39:47.000000 django-iubenda-1.2.9/src/django_iubenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-04 23:39:47.000000 django-iubenda-1.2.9/src/django_iubenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:39:47.000000 django-iubenda-1.2.9/src/django_iubenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 23:39:47.000000 django-iubenda-1.2.9/src/django_iubenda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 23:39:47.000000 django-iubenda-1.2.9/src/django_iubenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 23:39:47.000000 django-iubenda-1.2.9/src/django_iubenda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.379698 django-iubenda-1.2.9/src/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.379698 django-iubenda-1.2.9/src/iubenda/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/fixtures/data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.371698 django-iubenda-1.2.9/src/iubenda/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.371698 django-iubenda-1.2.9/src/iubenda/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.379698 django-iubenda-1.2.9/src/iubenda/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.379698 django-iubenda-1.2.9/src/iubenda/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.371698 django-iubenda-1.2.9/src/iubenda/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.371698 django-iubenda-1.2.9/src/iubenda/static/iubenda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.379698 django-iubenda-1.2.9/src/iubenda/static/iubenda/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/static/iubenda/css/iubenda_badge.css
+-rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/static/iubenda/css/iubenda_policy.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.371698 django-iubenda-1.2.9/src/iubenda/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.379698 django-iubenda-1.2.9/src/iubenda/templates/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/templates/iubenda/cookie-compress.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/templates/iubenda/cookie.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/templates/iubenda/include-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/templates/iubenda/privacy-compress.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/templates/iubenda/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/src/iubenda/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.383698 django-iubenda-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.383698 django-iubenda-1.2.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/fixtures/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 23:39:47.383698 django-iubenda-1.2.9/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/test_iubenda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/test_iubenda_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/test_iubenda_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 23:39:19.000000 django-iubenda-1.2.9/tox.ini
```

### Comparing `django-iubenda-1.2.7/.pre-commit-config.yaml` & `django-iubenda-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/LICENSE` & `django-iubenda-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/PKG-INFO` & `django-iubenda-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.2.7
+Version: 1.2.9
 Summary: Django application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,iubenda,privacy,cookie
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-iubenda-1.2.7/README.md` & `django-iubenda-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/mkdocs.yml` & `django-iubenda-1.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/pyproject.toml` & `django-iubenda-1.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
   { name = "Improved Documentation",    directory = "doc",     showcontent = true },
   { name = "Trivial Changes",           directory = "trivial", showcontent = false },
 ]
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "1.2.7"
+current_version = "1.2.9"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
 
 [[tool.bumpversion.files]]
 filename = "./src/iubenda/__init__.py"
```

### Comparing `django-iubenda-1.2.7/requirements/docs.txt` & `django-iubenda-1.2.9/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py310-django32.txt` & `django-iubenda-1.2.9/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py310-django42.txt` & `django-iubenda-1.2.9/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py311-django32.txt` & `django-iubenda-1.2.9/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py311-django42.txt` & `django-iubenda-1.2.9/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py38-django32.txt` & `django-iubenda-1.2.9/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py38-django42.txt` & `django-iubenda-1.2.9/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py39-django32.txt` & `django-iubenda-1.2.9/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/requirements/py39-django42.txt` & `django-iubenda-1.2.9/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/runtests.py` & `django-iubenda-1.2.9/runtests.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/setup.cfg` & `django-iubenda-1.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-iubenda
-version = 1.2.7
+version = 1.2.9
 url = https://github.com/DLRSP/django-iubenda
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling privacy and cookie policies configured with Iubenda.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-iubenda-1.2.7/setup.py` & `django-iubenda-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/django_iubenda.egg-info/PKG-INFO` & `django-iubenda-1.2.9/src/django_iubenda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.2.7
+Version: 1.2.9
 Summary: Django application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,iubenda,privacy,cookie
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-iubenda-1.2.7/src/django_iubenda.egg-info/SOURCES.txt` & `django-iubenda-1.2.9/src/django_iubenda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/context_processors.py` & `django-iubenda-1.2.9/src/iubenda/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/locale/it/LC_MESSAGES/django.po` & `django-iubenda-1.2.9/src/iubenda/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/migrations/0001_initial.py` & `django-iubenda-1.2.9/src/iubenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/models.py` & `django-iubenda-1.2.9/src/iubenda/models.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_badge.css` & `django-iubenda-1.2.9/src/iubenda/static/iubenda/css/iubenda_badge.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/static/iubenda/css/iubenda_policy.css` & `django-iubenda-1.2.9/src/iubenda/static/iubenda/css/iubenda_policy.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie-compress.html` & `django-iubenda-1.2.9/src/iubenda/templates/iubenda/cookie-compress.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/templates/iubenda/cookie.html` & `django-iubenda-1.2.9/src/iubenda/templates/iubenda/cookie.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/templates/iubenda/include-content.html` & `django-iubenda-1.2.9/src/iubenda/templates/iubenda/include-content.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy-compress.html` & `django-iubenda-1.2.9/src/iubenda/templates/iubenda/privacy-compress.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/templates/iubenda/privacy.html` & `django-iubenda-1.2.9/src/iubenda/templates/iubenda/privacy.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/urls.py` & `django-iubenda-1.2.9/src/iubenda/urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/src/iubenda/views.py` & `django-iubenda-1.2.9/src/iubenda/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,18 @@
                 f'https://www.iubenda.com/api/privacy-policy/{iubenda["iub_policy_id"]}',
                 params=request.GET,
             )
             if r.status_code == 200:
                 context = {"req_privacy": json.loads(r.content)}
             context_cache = cache.set(cache_key, context, timeout=86400)
 
-            if getattr(settings, "IUBENDA_USE_COMPRESS", True):
-                return render(request, "iubenda/privacy-compress.html", context)
-            return render(request, "iubenda/privacy.html", context)
         except Exception as err:
             messages.error(request, err)
+    if getattr(settings, "IUBENDA_USE_COMPRESS", True):
+        return render(request, "iubenda/privacy-compress.html", context_cache)
     return render(request, "iubenda/privacy.html", context_cache)
 
 
 @require_http_methods(["GET"])
 @vary_on_headers("User-Agent", "Cookie")
 def cookie(request):
     context = {}
```

### Comparing `django-iubenda-1.2.7/tests/settings.py` & `django-iubenda-1.2.9/tests/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
     "django.contrib.sites",
+    "django.contrib.sitemaps",
     "compressor",
     "iubenda",
 ]
 
 DATABASES = {"default": {"ENGINE": "django.db.backends.sqlite3"}}
 
 TEMPLATES = [
```

### Comparing `django-iubenda-1.2.7/tests/test_iubenda_template.py` & `django-iubenda-1.2.9/tests/test_iubenda_template.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.2.7/tests/test_iubenda_urls.py` & `django-iubenda-1.2.9/tests/test_iubenda_urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,21 @@
         """Set up common assets for tests"""
         LOGGER.debug("Tests setUp")
 
     def tearDown(self):
         """Remove Test Data"""
         LOGGER.debug("Tests tearDown")
 
+    def test_sitemap(self):
+        """Test that render sitemap.xml."""
+        LOGGER.debug("Render Sitemap")
+        response = self.client.get("/it/sitemap.xml", follow=True)
+        LOGGER.debug(response)
+        self.assertEqual(200, response.status_code)
+
     def test_privacy_urls(self):
         """Test that render Privacy page."""
         LOGGER.debug("Render Privacy page")
         response = self.client.get("/privacy-policy/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(200, response.status_code)
```

### Comparing `django-iubenda-1.2.7/tox.ini` & `django-iubenda-1.2.9/tox.ini`

 * *Files identical despite different names*

