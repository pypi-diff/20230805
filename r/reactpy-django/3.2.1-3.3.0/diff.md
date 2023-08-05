# Comparing `tmp/reactpy_django-3.2.1.tar.gz` & `tmp/reactpy_django-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_django-3.2.1.tar", last modified: Thu Jun 29 20:01:08 2023, max compression
+gzip compressed data, was "reactpy_django-3.3.0.tar", last modified: Sat Aug  5 07:52:46 2023, max compression
```

## Comparing `reactpy_django-3.2.1.tar` & `reactpy_django-3.3.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/http/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/http/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/reactpy_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/static/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django/static/reactpy_django/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/reactpy_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/templates/reactpy/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/templates/reactpy/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/templatetags/reactpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/websocket/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/websocket/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:01:01.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/http/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/http/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0004_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/reactpy_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/static/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django/static/reactpy_django/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/reactpy_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/templates/reactpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/templates/reactpy/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/templatetags/reactpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/websocket/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/websocket/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:52:39.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/top_level.txt
```

### Comparing `reactpy_django-3.2.1/LICENSE` & `reactpy_django-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/PKG-INFO` & `reactpy_django-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy_django
-Version: 3.2.1
+Version: 3.3.0
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -12,19 +12,19 @@
 Platform: Windows
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="https://raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/reactpy-logo-square.svg" align="left" height="45"/> ReactPy Django
 
 <!--badge-start-->
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: reactpy_django Version: 3.2.1 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy_django Version: 3.3.0 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Environment ::
-Web Environment Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Environment ::
+Web Environment Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE # [https://raw.githubusercontent.com/reactive-python/
 reactpy/main/branding/svg/reactpy-logo-square.svg] ReactPy Django
 [https://github.com/reactive-python/reactpy-django/workflows/Test/
 badge.svg?event=push] [https://img.shields.io/pypi/v/reactpy-
 django.svg?label=PyPI] [https://img.shields.io/badge/License-MIT-purple.svg]
 [https://img.shields.io/
 website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-
```

### Comparing `reactpy_django-3.2.1/README.md` & `reactpy_django-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/setup.py` & `reactpy_django-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 from logging import StreamHandler, getLogger
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.develop import develop
 from setuptools.command.sdist import sdist
 
-
 if sys.platform == "win32":
     from subprocess import list2cmdline
 else:
 
     def list2cmdline(cmd_list):
         return " ".join(map(pipes.quote, cmd_list))
 
 
-log = getLogger()
+log = getLogger()  # noqa: F811
 log.addHandler(StreamHandler(sys.stdout))
 
 
 # -----------------------------------------------------------------------------
 # Basic Constants
 # -----------------------------------------------------------------------------
 
@@ -43,15 +42,15 @@
 # -----------------------------------------------------------------------------
 # Package Definition
 # -----------------------------------------------------------------------------
 
 
 package = {
     "name": name,
-    "python_requires": ">=3.8",
+    "python_requires": ">=3.9",
     "packages": find_packages(str(src_dir)),
     "package_dir": {"": "src"},
     "description": "Control the web with Python",
     "author": "Ryan Morshead",
     "author_email": "ryan.morshead@gmail.com",
     "url": "https://github.com/reactive-python/reactpy-django",
     "license": "MIT",
@@ -62,17 +61,17 @@
     "classifiers": [
         "Framework :: Django",
         "Framework :: Django :: 4.0",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Topic :: Multimedia :: Graphics",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Environment :: Web Environment",
     ],
 }
 
 
 # -----------------------------------------------------------------------------
 # Library Version
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django/components.py` & `reactpy_django-3.3.0/src/reactpy_django/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,15 +206,14 @@
     abs_path = find(static_path)
     if not abs_path:
         raise FileNotFoundError(
             f"Could not find static file {static_path} within Django's static files."
         )
 
     # Fetch the file from cache, if available
-    # Cache is preferrable to `use_memo` due to multiprocessing capabilities
     last_modified_time = os.stat(abs_path).st_mtime
     cache_key = f"reactpy_django:static_contents:{static_path}"
     file_contents = caches[REACTPY_CACHE].get(
         cache_key, version=int(last_modified_time)
     )
     if file_contents is None:
         with open(abs_path, encoding="utf-8") as static_file:
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django/config.py` & `reactpy_django-3.3.0/src/reactpy_django/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from reactpy_django.types import (
     AsyncPostprocessor,
     SyncPostprocessor,
     ViewComponentIframe,
 )
 from reactpy_django.utils import import_dotted_path
 
-
-# Not user configurable settings
+# Non-configurable values
 REACTPY_DEBUG_MODE.set_current(getattr(settings, "DEBUG"))
 REACTPY_REGISTERED_COMPONENTS: dict[str, ComponentConstructor] = {}
+REACTPY_FAILED_COMPONENTS: set[str] = set()
 REACTPY_VIEW_COMPONENT_IFRAMES: dict[str, ViewComponentIframe] = {}
 
 
 # Configurable through Django settings.py
 REACTPY_WEBSOCKET_URL = getattr(
     settings,
     "REACTPY_WEBSOCKET_URL",
@@ -37,21 +37,29 @@
     DEFAULT_CACHE_ALIAS,
 )
 REACTPY_DATABASE: str = getattr(
     settings,
     "REACTPY_DATABASE",
     DEFAULT_DB_ALIAS,
 )
+_default_query_postprocessor = getattr(
+    settings,
+    "REACTPY_DEFAULT_QUERY_POSTPROCESSOR",
+    None,
+)
 REACTPY_DEFAULT_QUERY_POSTPROCESSOR: AsyncPostprocessor | SyncPostprocessor | None = (
     import_dotted_path(
-        getattr(
-            settings,
-            "REACTPY_DEFAULT_QUERY_POSTPROCESSOR",
-            "reactpy_django.utils.django_query_postprocessor",
-        )
+        _default_query_postprocessor
+        if isinstance(_default_query_postprocessor, str)
+        else "reactpy_django.utils.django_query_postprocessor",
     )
 )
 REACTPY_AUTH_BACKEND: str | None = getattr(
     settings,
     "REACTPY_AUTH_BACKEND",
     None,
 )
+REACTPY_BACKHAUL_THREAD: bool = getattr(
+    settings,
+    "REACTPY_BACKHAUL_THREAD",
+    True,
+)
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django/decorators.py` & `reactpy_django-3.3.0/src/reactpy_django/decorators.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/src/reactpy_django/hooks.py` & `reactpy_django-3.3.0/src/reactpy_django/hooks.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/src/reactpy_django/http/views.py` & `reactpy_django-3.3.0/src/reactpy_django/http/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 
 async def web_modules_file(request: HttpRequest, file: str) -> HttpResponse:
     """Gets JavaScript required for ReactPy modules at runtime. These modules are
     returned from cache if available."""
     from reactpy_django.config import REACTPY_CACHE
 
     web_modules_dir = REACTPY_WEB_MODULES_DIR.current
-    path = os.path.abspath(web_modules_dir.joinpath(*file.split("/")))
+    path = os.path.abspath(web_modules_dir.joinpath(file))
 
     # Prevent attempts to walk outside of the web modules dir
     if str(web_modules_dir) != os.path.commonpath((path, web_modules_dir)):
         raise SuspiciousOperation(
             "Attempt to access a directory outside of REACTPY_WEB_MODULES_DIR."
         )
 
     # Fetch the file from cache, if available
     last_modified_time = os.stat(path).st_mtime
-    cache_key = create_cache_key("web_module", str(path).lstrip(str(web_modules_dir)))
-    response = await caches[REACTPY_CACHE].aget(
+    cache_key = create_cache_key("web_modules", path)
+    file_contents = await caches[REACTPY_CACHE].aget(
         cache_key, version=int(last_modified_time)
     )
-    if response is None:
+    if file_contents is None:
         async with async_open(path, "r") as fp:
-            response = HttpResponse(await fp.read(), content_type="text/javascript")
+            file_contents = await fp.read()
         await caches[REACTPY_CACHE].adelete(cache_key)
         await caches[REACTPY_CACHE].aset(
-            cache_key, response, timeout=None, version=int(last_modified_time)
+            cache_key, file_contents, timeout=604800, version=int(last_modified_time)
         )
-    return response
+    return HttpResponse(file_contents, content_type="text/javascript")
 
 
 async def view_to_component_iframe(
     request: HttpRequest, view_path: str
 ) -> HttpResponse:
     """Returns a view that was registered by view_to_component.
     This view is intended to be used as iframe, for compatibility purposes."""
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django/migrations/0001_initial.py` & `reactpy_django-3.3.0/src/reactpy_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py` & `reactpy_django-3.3.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/src/reactpy_django/static/reactpy_django/client.js` & `reactpy_django-3.3.0/src/reactpy_django/static/reactpy_django/client.js`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/src/reactpy_django/templates/reactpy/component.html` & `reactpy_django-3.3.0/src/reactpy_django/templates/reactpy/component.html`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/src/reactpy_django/templatetags/reactpy.py` & `reactpy_django-3.3.0/src/reactpy_django/templatetags/reactpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import dill as pickle
 from django import template
 from django.urls import reverse
 
 from reactpy_django import models
 from reactpy_django.config import (
-    REACTPY_DATABASE,
     REACTPY_DEBUG_MODE,
     REACTPY_RECONNECT_MAX,
     REACTPY_WEBSOCKET_URL,
 )
 from reactpy_django.exceptions import ComponentDoesNotExistError, ComponentParamError
 from reactpy_django.types import ComponentParamData
 from reactpy_django.utils import (
@@ -69,15 +68,15 @@
     # This will be fetched by the websocket consumer later
     try:
         check_component_args(component, *args, **kwargs)
         if func_has_args(component):
             params = ComponentParamData(args, kwargs)
             model = models.ComponentSession(uuid=uuid, params=pickle.dumps(params))
             model.full_clean()
-            model.save(using=REACTPY_DATABASE)
+            model.save()
 
     except Exception as e:
         if isinstance(e, ComponentParamError):
             _logger.error(str(e))
         else:
             _logger.exception(
                 "An unknown error has occurred while saving component params for '%s'.",
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django/types.py` & `reactpy_django-3.3.0/src/reactpy_django/types.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.1/src/reactpy_django/utils.py` & `reactpy_django-3.3.0/src/reactpy_django/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from __future__ import annotations
 
 import contextlib
 import inspect
 import logging
 import os
 import re
-from datetime import datetime, timedelta
+from datetime import timedelta
 from fnmatch import fnmatch
 from importlib import import_module
 from inspect import iscoroutinefunction
 from typing import Any, Callable, Sequence
 
 from channels.db import database_sync_to_async
-from django.core.cache import caches
 from django.db.models import ManyToManyField, ManyToOneRel, prefetch_related_objects
 from django.db.models.base import Model
 from django.db.models.query import QuerySet
 from django.http import HttpRequest, HttpResponse
 from django.template import engines
 from django.utils import timezone
 from django.utils.encoding import smart_str
 from django.views import View
 
 from reactpy_django.exceptions import ComponentDoesNotExistError, ComponentParamError
 
-
 _logger = logging.getLogger(__name__)
 _component_tag = r"(?P<tag>component)"
 _component_path = r"(?P<path>\"[^\"'\s]+\"|'[^\"'\s]+')"
 _component_kwargs = r"(?P<kwargs>[\s\S]*?)"
 COMMENT_REGEX = re.compile(r"<!--[\s\S]*?-->")
 COMPONENT_REGEX = re.compile(
     r"{%\s*"
@@ -84,22 +82,26 @@
     return response
 
 
 def _register_component(dotted_path: str) -> Callable:
     """Adds a component to the mapping of registered components.
     This should only be called on startup to maintain synchronization during mulitprocessing.
     """
-    from reactpy_django.config import REACTPY_REGISTERED_COMPONENTS
+    from reactpy_django.config import (
+        REACTPY_FAILED_COMPONENTS,
+        REACTPY_REGISTERED_COMPONENTS,
+    )
 
     if dotted_path in REACTPY_REGISTERED_COMPONENTS:
         return REACTPY_REGISTERED_COMPONENTS[dotted_path]
 
     try:
         REACTPY_REGISTERED_COMPONENTS[dotted_path] = import_dotted_path(dotted_path)
     except AttributeError as e:
+        REACTPY_FAILED_COMPONENTS.add(dotted_path)
         raise ComponentDoesNotExistError(
             f"Error while fetching '{dotted_path}'. {(str(e).capitalize())}."
         ) from e
     _logger.debug("ReactPy has registered component %s", dotted_path)
     return REACTPY_REGISTERED_COMPONENTS[dotted_path]
 
 
@@ -262,15 +264,15 @@
     # `Model` instances
     elif isinstance(data, Model):
         prefetch_fields: list[str] = []
         for field in data._meta.get_fields():
             # Force the query to execute
             getattr(data, field.name, None)
 
-            if many_to_one and type(field) == ManyToOneRel:
+            if many_to_one and type(field) == ManyToOneRel:  # noqa: #E721
                 prefetch_fields.append(field.related_name or f"{field.name}_set")
 
             elif many_to_many and isinstance(field, ManyToManyField):
                 prefetch_fields.append(field.name)
 
         if prefetch_fields:
             prefetch_related_objects([data], *prefetch_fields)
@@ -328,49 +330,30 @@
 
     return f"reactpy_django:{':'.join(str(arg) for arg in args)}"
 
 
 def db_cleanup(immediate: bool = False):
     """Deletes expired component sessions from the database.
     This function may be expanded in the future to include additional cleanup tasks."""
-    from .config import (
-        REACTPY_CACHE,
-        REACTPY_DATABASE,
-        REACTPY_DEBUG_MODE,
-        REACTPY_RECONNECT_MAX,
-    )
-    from .models import ComponentSession
+    from .config import REACTPY_DEBUG_MODE, REACTPY_RECONNECT_MAX
+    from .models import ComponentSession, Config
 
-    clean_started_at = datetime.now()
-    cache_key: str = create_cache_key("last_cleaned")
-    now_str: str = datetime.strftime(timezone.now(), DATE_FORMAT)
-    cleaned_at_str: str = caches[REACTPY_CACHE].get(cache_key)
-    cleaned_at: datetime = timezone.make_aware(
-        datetime.strptime(cleaned_at_str or now_str, DATE_FORMAT)
-    )
+    config = Config.load()
+    start_time = timezone.now()
+    cleaned_at = config.cleaned_at
     clean_needed_by = cleaned_at + timedelta(seconds=REACTPY_RECONNECT_MAX)
-    expires_by: datetime = timezone.now() - timedelta(seconds=REACTPY_RECONNECT_MAX)
-
-    # Component params exist in the DB, but we don't know when they were last cleaned
-    if not cleaned_at_str and ComponentSession.objects.using(REACTPY_DATABASE).all():
-        _logger.warning(
-            "ReactPy has detected component sessions in the database, "
-            "but no timestamp was found in cache. This may indicate that "
-            "the cache has been cleared."
-        )
 
     # Delete expired component parameters
-    # Use timestamps in cache (`cleaned_at_str`) as a no-dependency rate limiter
-    if immediate or not cleaned_at_str or timezone.now() >= clean_needed_by:
-        ComponentSession.objects.using(REACTPY_DATABASE).filter(
-            last_accessed__lte=expires_by
-        ).delete()
-        caches[REACTPY_CACHE].set(cache_key, now_str, timeout=None)
+    if immediate or timezone.now() >= clean_needed_by:
+        expiration_date = timezone.now() - timedelta(seconds=REACTPY_RECONNECT_MAX)
+        ComponentSession.objects.filter(last_accessed__lte=expiration_date).delete()
+        config.cleaned_at = timezone.now()
+        config.save()
 
     # Check if cleaning took abnormally long
-    clean_duration = datetime.now() - clean_started_at
+    clean_duration = timezone.now() - start_time
     if REACTPY_DEBUG_MODE and clean_duration.total_seconds() > 1:
         _logger.warning(
             "ReactPy has taken %s seconds to clean up expired component sessions. "
             "This may indicate a performance issue with your system, cache, or database.",
             clean_duration.total_seconds(),
         )
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django/websocket/consumer.py` & `reactpy_django-3.3.0/src/reactpy_django/websocket/consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Anything used to construct a websocket endpoint"""
+
 from __future__ import annotations
 
 import asyncio
+import contextlib
 import logging
+from concurrent.futures import Future
 from datetime import timedelta
+from threading import Thread
 from typing import Any, MutableMapping, Sequence
 
 import dill as pickle
 from channels.auth import login
 from channels.db import database_sync_to_async
 from channels.generic.websocket import AsyncJsonWebsocketConsumer
 from django.utils import timezone
@@ -15,83 +19,109 @@
 from reactpy.backend.types import Connection, Location
 from reactpy.core.layout import Layout
 from reactpy.core.serve import serve_layout
 
 from reactpy_django.types import ComponentParamData, ComponentWebsocket
 from reactpy_django.utils import db_cleanup, func_has_args
 
-
 _logger = logging.getLogger(__name__)
+backhaul_loop = asyncio.new_event_loop()
+
+
+def start_backhaul_loop():
+    """Starts the asyncio event loop that will perform component rendering tasks."""
+    asyncio.set_event_loop(backhaul_loop)
+    backhaul_loop.run_forever()
+
+
+backhaul_thread = Thread(target=start_backhaul_loop, daemon=True)
 
 
 class ReactpyAsyncWebsocketConsumer(AsyncJsonWebsocketConsumer):
     """Communicates with the browser to perform actions on-demand."""
 
     async def connect(self) -> None:
         """The browser has connected."""
+        from reactpy_django.config import REACTPY_AUTH_BACKEND, REACTPY_BACKHAUL_THREAD
+
         await super().connect()
 
         # Authenticate the user, if possible
-        from reactpy_django.config import REACTPY_AUTH_BACKEND
-
         user: Any = self.scope.get("user")
         if user and user.is_authenticated:
             try:
                 await login(self.scope, user, backend=REACTPY_AUTH_BACKEND)
             except Exception:
-                _logger.exception("ReactPy websocket authentication has failed!")
+                await asyncio.to_thread(
+                    _logger.exception, "ReactPy websocket authentication has failed!"
+                )
         elif user is None:
-            _logger.debug(
+            await asyncio.to_thread(
+                _logger.debug,
                 "ReactPy websocket is missing AuthMiddlewareStack! "
-                "Users will not be accessible within `use_scope` or `use_websocket`!"
+                "Users will not be accessible within `use_scope` or `use_websocket`!",
             )
 
         # Save the session, if possible
         if self.scope.get("session"):
             try:
                 await database_sync_to_async(self.scope["session"].save)()
             except Exception:
-                _logger.exception("ReactPy has failed to save scope['session']!")
+                await asyncio.to_thread(
+                    _logger.exception, "ReactPy has failed to save scope['session']!"
+                )
         else:
-            _logger.debug(
+            await asyncio.to_thread(
+                _logger.debug,
                 "ReactPy websocket is missing SessionMiddlewareStack! "
-                "Sessions will not be accessible within `use_scope` or `use_websocket`!"
+                "Sessions will not be accessible within `use_scope` or `use_websocket`!",
             )
 
-        # Start allowing component renders
-        self._reactpy_dispatcher_future = asyncio.ensure_future(
-            self._run_dispatch_loop()
-        )
+        # Start the component dispatcher
+        self.dispatcher: Future | asyncio.Task
+        self.threaded = REACTPY_BACKHAUL_THREAD
+        if self.threaded:
+            if not backhaul_thread.is_alive():
+                await asyncio.to_thread(
+                    _logger.debug, "Starting ReactPy backhaul thread."
+                )
+                backhaul_thread.start()
+            self.dispatcher = asyncio.run_coroutine_threadsafe(
+                self.run_dispatcher(), backhaul_loop
+            )
+        else:
+            self.dispatcher = asyncio.create_task(self.run_dispatcher())
 
     async def disconnect(self, code: int) -> None:
         """The browser has disconnected."""
-        if self._reactpy_dispatcher_future.done():
-            await self._reactpy_dispatcher_future
-        else:
-            self._reactpy_dispatcher_future.cancel()
+        self.dispatcher.cancel()
         await super().disconnect(code)
 
     async def receive_json(self, content: Any, **_) -> None:
-        """Receive a message from the browser. Typically messages are event signals."""
-        await self._reactpy_recv_queue.put(content)
+        """Receive a message from the browser. Typically, messages are event signals."""
+        if self.threaded:
+            asyncio.run_coroutine_threadsafe(
+                self.recv_queue.put(content), backhaul_loop
+            )
+        else:
+            await self.recv_queue.put(content)
 
-    async def _run_dispatch_loop(self):
+    async def run_dispatcher(self):
         """Runs the main loop that performs component rendering tasks."""
         from reactpy_django import models
         from reactpy_django.config import (
-            REACTPY_DATABASE,
             REACTPY_RECONNECT_MAX,
             REACTPY_REGISTERED_COMPONENTS,
         )
 
         scope = self.scope
         dotted_path = scope["url_route"]["kwargs"]["dotted_path"]
         uuid = scope["url_route"]["kwargs"]["uuid"]
         search = scope["query_string"].decode()
-        self._reactpy_recv_queue: asyncio.Queue = asyncio.Queue()
+        self.recv_queue: asyncio.Queue = asyncio.Queue()
         connection = Connection(  # For `use_connection`
             scope=scope,
             location=Location(
                 pathname=scope["path"],
                 search=f"?{search}" if (search and (search != "undefined")) else "",
             ),
             carrier=ComponentWebsocket(self.close, self.disconnect, dotted_path),
@@ -100,62 +130,60 @@
         component_args: Sequence[Any] = ()
         component_kwargs: MutableMapping[str, Any] = {}
 
         # Verify the component has already been registered
         try:
             component_constructor = REACTPY_REGISTERED_COMPONENTS[dotted_path]
         except KeyError:
-            _logger.warning(
-                f"Attempt to access invalid ReactPy component: {dotted_path!r}"
+            await asyncio.to_thread(
+                _logger.warning,
+                f"Attempt to access invalid ReactPy component: {dotted_path!r}",
             )
             return
 
         # Fetch the component's args/kwargs from the database, if needed
         try:
             if func_has_args(component_constructor):
                 try:
                     # Always clean up expired entries first
                     await database_sync_to_async(db_cleanup, thread_sensitive=False)()
 
                     # Get the queries from a DB
-                    params_query = await models.ComponentSession.objects.using(
-                        REACTPY_DATABASE
-                    ).aget(
+                    params_query = await models.ComponentSession.objects.aget(
                         uuid=uuid,
                         last_accessed__gt=now
                         - timedelta(seconds=REACTPY_RECONNECT_MAX),
                     )
                     params_query.last_accessed = timezone.now()
                     await database_sync_to_async(
                         params_query.save, thread_sensitive=False
                     )()
                 except models.ComponentSession.DoesNotExist:
-                    _logger.warning(
+                    await asyncio.to_thread(
+                        _logger.warning,
                         f"Component session for '{dotted_path}:{uuid}' not found. The "
-                        "session may have already expired beyond REACTPY_RECONNECT_MAX."
+                        "session may have already expired beyond REACTPY_RECONNECT_MAX.",
                     )
                     return
                 component_params: ComponentParamData = pickle.loads(params_query.params)
                 component_args = component_params.args
                 component_kwargs = component_params.kwargs
 
             # Generate the initial component instance
             component_instance = component_constructor(
                 *component_args, **component_kwargs
             )
         except Exception:
-            _logger.exception(
+            await asyncio.to_thread(
+                _logger.exception,
                 f"Failed to construct component {component_constructor} "
-                f"with parameters {component_kwargs}"
+                f"with parameters {component_kwargs}",
             )
             return
 
         # Start the ReactPy component rendering loop
-        try:
+        with contextlib.suppress(Exception):
             await serve_layout(
                 Layout(ConnectionContext(component_instance, value=connection)),
                 self.send_json,
-                self._reactpy_recv_queue.get,
+                self.recv_queue.get,
             )
-        except Exception:
-            await self.close()
-            raise
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django.egg-info/PKG-INFO` & `reactpy_django-3.3.0/src/reactpy_django.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-django
-Version: 3.2.1
+Version: 3.3.0
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -12,19 +12,19 @@
 Platform: Windows
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="https://raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/reactpy-logo-square.svg" align="left" height="45"/> ReactPy Django
 
 <!--badge-start-->
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: reactpy-django Version: 3.2.1 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy-django Version: 3.3.0 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Environment ::
-Web Environment Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Environment ::
+Web Environment Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE # [https://raw.githubusercontent.com/reactive-python/
 reactpy/main/branding/svg/reactpy-logo-square.svg] ReactPy Django
 [https://github.com/reactive-python/reactpy-django/workflows/Test/
 badge.svg?event=push] [https://img.shields.io/pypi/v/reactpy-
 django.svg?label=PyPI] [https://img.shields.io/badge/License-MIT-purple.svg]
 [https://img.shields.io/
 website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-
```

### Comparing `reactpy_django-3.2.1/src/reactpy_django.egg-info/SOURCES.txt` & `reactpy_django-3.3.0/src/reactpy_django.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/reactpy_django/__init__.py
 src/reactpy_django/apps.py
+src/reactpy_django/checks.py
 src/reactpy_django/components.py
 src/reactpy_django/config.py
+src/reactpy_django/database.py
 src/reactpy_django/decorators.py
 src/reactpy_django/exceptions.py
 src/reactpy_django/hooks.py
 src/reactpy_django/models.py
 src/reactpy_django/py.typed
 src/reactpy_django/types.py
 src/reactpy_django/utils.py
@@ -23,14 +25,15 @@
 src/reactpy_django.egg-info/top_level.txt
 src/reactpy_django/http/__init__.py
 src/reactpy_django/http/urls.py
 src/reactpy_django/http/views.py
 src/reactpy_django/migrations/0001_initial.py
 src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
 src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
+src/reactpy_django/migrations/0004_config.py
 src/reactpy_django/migrations/__init__.py
 src/reactpy_django/static/reactpy_django/client.js
 src/reactpy_django/templates/reactpy/component.html
 src/reactpy_django/templatetags/__init__.py
 src/reactpy_django/templatetags/reactpy.py
 src/reactpy_django/websocket/__init__.py
 src/reactpy_django/websocket/consumer.py
```

