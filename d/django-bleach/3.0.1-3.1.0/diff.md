# Comparing `tmp/django-bleach-3.0.1.tar.gz` & `tmp/django-bleach-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bleach-3.0.1.tar", last modified: Wed Oct 12 00:33:56 2022, max compression
+gzip compressed data, was "django-bleach-3.1.0.tar", last modified: Sat Aug  5 01:36:15 2023, max compression
```

## Comparing `django-bleach-3.0.1.tar` & `django-bleach-3.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2022-10-12 00:33:48.000000 django-bleach-3.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-12 00:33:48.000000 django-bleach-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-12 00:33:48.000000 django-bleach-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7748 2022-10-12 00:33:56.935078 django-bleach-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6491 2022-10-12 00:33:48.000000 django-bleach-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/django_bleach/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/django_bleach/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/templatetags/bleach_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/django_bleach/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8538 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/tests/test_modelformfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     4647 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-10-12 00:33:48.000000 django-bleach-3.0.1/django_bleach/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/django_bleach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7748 2022-10-12 00:33:56.000000 django-bleach-3.0.1/django_bleach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-10-12 00:33:56.000000 django-bleach-3.0.1/django_bleach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 00:33:56.000000 django-bleach-3.0.1/django_bleach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-12 00:33:56.000000 django-bleach-3.0.1/django_bleach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-12 00:33:56.000000 django-bleach-3.0.1/django_bleach.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-12 00:33:48.000000 django-bleach-3.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-10-12 00:33:48.000000 django-bleach-3.0.1/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-12 00:33:48.000000 django-bleach-3.0.1/docs/setup.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2953 2022-10-12 00:33:48.000000 django-bleach-3.0.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-12 00:33:48.000000 django-bleach-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-10-12 00:33:56.939078 django-bleach-3.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3441 2022-10-12 00:33:48.000000 django-bleach-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/testproject/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1741 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/forms.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1040 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/testproject/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1797 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:33:56.935078 django-bleach-3.0.1/testproject/templates/
--rwxr-xr-x   0 runner    (1001) docker     (121)      351 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/templates/model_form.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      175 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      921 2022-10-12 00:33:48.000000 django-bleach-3.0.1/testproject/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.158605 django-bleach-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-05 01:36:02.000000 django-bleach-3.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-05 01:36:02.000000 django-bleach-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-05 01:36:02.000000 django-bleach-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-08-05 01:36:15.158605 django-bleach-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-08-05 01:36:02.000000 django-bleach-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.154605 django-bleach-3.1.0/django_bleach/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.154605 django-bleach-3.1.0/django_bleach/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/templatetags/bleach_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.154605 django-bleach-3.1.0/django_bleach/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/tests/test_modelformfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-05 01:36:02.000000 django-bleach-3.1.0/django_bleach/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.154605 django-bleach-3.1.0/django_bleach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-08-05 01:36:15.000000 django-bleach-3.1.0/django_bleach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-05 01:36:15.000000 django-bleach-3.1.0/django_bleach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:36:15.000000 django-bleach-3.1.0/django_bleach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-05 01:36:15.000000 django-bleach-3.1.0/django_bleach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-05 01:36:15.000000 django-bleach-3.1.0/django_bleach.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.158605 django-bleach-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-05 01:36:02.000000 django-bleach-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-05 01:36:02.000000 django-bleach-3.1.0/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-05 01:36:02.000000 django-bleach-3.1.0/docs/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-05 01:36:02.000000 django-bleach-3.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-05 01:36:02.000000 django-bleach-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-05 01:36:15.162605 django-bleach-3.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2833 2023-08-05 01:36:02.000000 django-bleach-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.158605 django-bleach-3.1.0/testproject/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.158605 django-bleach-3.1.0/testproject/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:36:15.158605 django-bleach-3.1.0/testproject/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/templates/model_form.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      175 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-08-05 01:36:02.000000 django-bleach-3.1.0/testproject/views.py
```

### Comparing `django-bleach-3.0.1/CHANGELOG.md` & `django-bleach-3.1.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Change Log
 ==========
 
 This document records all notable changes to [django-bleach](https://github.com/marksweb/django-bleach).
 This project adheres to [Semantic Versioning](https://semver.org/).
 
-[unreleased](https://github.com/marksweb/django-bleach/compare/3.0.1...master) changes
+[unreleased](https://github.com/marksweb/django-bleach/compare/3.1.0...master) changes
 -------------------------------------------------------------------------------------
 
+Version 3.1.0
+=============
+**05-08-2023**
+
+* Added support for django 4.2
+* Added support for python 3.12
+* Revamp package for easier maintenance
+
+
 Version 3.0.1
 =============
 **11-10-2022**
 
 * Added support for django 4.1
 
 Version 3.0.0
```

### Comparing `django-bleach-3.0.1/LICENSE` & `django-bleach-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/PKG-INFO` & `django-bleach-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bleach
-Version: 3.0.1
+Version: 3.1.0
 Summary: Easily use bleach with Django models and templates
 Home-page: https://github.com/marksweb/django-bleach
 Author: Tim Heap
 Maintainer: Mark Walker
 Maintainer-email: theshow+django-bleach@gmail.com
 License: MIT
 Project-URL: Documentation, https://django-bleach.readthedocs.io/
@@ -16,17 +16,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 django-bleach - Bleach and sanitise user HTML
 =============================================
```

### Comparing `django-bleach-3.0.1/README.rst` & `django-bleach-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/django_bleach/forms.py` & `django-bleach-3.1.0/django_bleach/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,76 @@
+from importlib import import_module
+
+import bleach
+from bleach.css_sanitizer import CSSSanitizer
 from django import forms
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.safestring import mark_safe
 
-import bleach
-import warnings
-from bleach.css_sanitizer import CSSSanitizer
-from importlib import import_module
-
 from django_bleach.utils import get_bleach_default_options
 
 
 def load_widget(path):
-    """ Load custom widget for the form field """
+    """Load custom widget for the form field"""
     i = path.rfind(".")
-    module, attr = path[:i], path[i + 1:]
+    module, attr = path[:i], path[i + 1 :]
     try:
         mod = import_module(module)
     except (ImportError, ValueError) as e:
         error_message = "Error importing widget for BleachField %s: '%s'"
-        raise ImproperlyConfigured(error_message % (path, e))
+        raise ImproperlyConfigured(error_message % (path, e)) from e
 
     try:
         cls = getattr(mod, attr)
-    except AttributeError:
+    except AttributeError as e:
         raise ImproperlyConfigured(
             f"Module '{module}' does not define a '{attr}' widget"
-        )
+        ) from e
 
     return cls
 
 
 def get_default_widget():
-    """ Get the default widget or the widget defined in settings """
+    """Get the default widget or the widget defined in settings"""
     default_widget = forms.Textarea
     if hasattr(settings, "BLEACH_DEFAULT_WIDGET"):
         default_widget = load_widget(settings.BLEACH_DEFAULT_WIDGET)
     return default_widget
 
 
 class BleachField(forms.CharField):
-    """ Bleach form field """
-    empty_values = [None, "", [], (), {}]
+    """Bleach form field"""
 
-    def __init__(self, allowed_tags=None, allowed_attributes=None,
-                 allowed_styles=None, allowed_protocols=None,
-                 strip_comments=None, strip_tags=None, css_sanitizer=None, *args, **kwargs):
+    empty_values = [None, "", [], (), {}]
 
+    def __init__(
+        self,
+        allowed_tags=None,
+        allowed_attributes=None,
+        allowed_styles=None,
+        allowed_protocols=None,
+        strip_comments=None,
+        strip_tags=None,
+        css_sanitizer=None,
+        *args,
+        **kwargs,
+    ):
         self.widget = get_default_widget()
 
         super().__init__(*args, **kwargs)
 
         self.bleach_options = get_bleach_default_options()
 
         if allowed_tags is not None:
             self.bleach_options["tags"] = allowed_tags
         if allowed_attributes is not None:
             self.bleach_options["attributes"] = allowed_attributes
-        if allowed_styles is not None:
-            warnings.warn(
-                "allowed_styles will be deprecated, use css_sanitizer instead",
-                DeprecationWarning
-            )
-
-            if css_sanitizer:
-                warnings.warn("allowed_styles argument is ignored since css_sanitizer is favoured over allowed_styles")
-            self.bleach_options["css_sanitizer"] = CSSSanitizer(allowed_css_properties=allowed_styles)
+        if allowed_styles:
+            css_sanitizer = CSSSanitizer(allowed_css_properties=allowed_styles)
         if css_sanitizer is not None:
             self.bleach_options["css_sanitizer"] = css_sanitizer
         if allowed_protocols is not None:
             self.bleach_options["protocols"] = allowed_protocols
         if strip_tags is not None:
             self.bleach_options["strip"] = strip_tags
         if strip_comments is not None:
```

### Comparing `django-bleach-3.0.1/django_bleach/models.py` & `django-bleach-3.1.0/django_bleach/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,66 @@
-from django.db import models
-from django.utils.safestring import mark_safe
-
-import warnings
 from bleach import clean
 from bleach.css_sanitizer import CSSSanitizer
+from django.db import models
+from django.utils.safestring import mark_safe
 
 from . import forms
 from .utils import get_bleach_default_options
 
 
 class BleachField(models.TextField):
-    def __init__(self, allowed_tags=None, allowed_attributes=None,
-                 allowed_styles=None, allowed_protocols=None,
-                 strip_tags=None, strip_comments=None, css_sanitizer=None, *args, **kwargs):
-
+    def __init__(
+        self,
+        allowed_tags=None,
+        allowed_attributes=None,
+        allowed_styles=None,
+        allowed_protocols=None,
+        strip_tags=None,
+        strip_comments=None,
+        css_sanitizer=None,
+        *args,
+        **kwargs,
+    ):
         super().__init__(*args, **kwargs)
 
         self.bleach_kwargs = get_bleach_default_options()
 
         if allowed_tags:
             self.bleach_kwargs["tags"] = allowed_tags
         if allowed_attributes:
             self.bleach_kwargs["attributes"] = allowed_attributes
         if allowed_styles:
-            warnings.warn(
-                "allowed_styles will be deprecated, use css_sanitizer instead",
-                DeprecationWarning
-            )
-            if css_sanitizer:
-                warnings.warn("allowed_styles argument is ignored since css_sanitizer is favoured over allowed_styles")
-            self.bleach_kwargs["css_sanitizer"] = CSSSanitizer(allowed_css_properties=allowed_styles)
+            css_sanitizer = CSSSanitizer(allowed_css_properties=allowed_styles)
         if css_sanitizer:
             self.bleach_kwargs["css_sanitizer"] = css_sanitizer
         if allowed_protocols:
             self.bleach_kwargs["protocols"] = allowed_protocols
         if strip_tags:
             self.bleach_kwargs["strip"] = strip_tags
         if strip_comments:
             self.bleach_kwargs["strip_comments"] = strip_comments
 
     def formfield(self, form_class=forms.BleachField, **kwargs):
-        """ Makes the field for a ModelForm """
+        """Makes the field for a ModelForm"""
 
         # If field doesn't have any choices add kwargs expected by BleachField.
         if not self.choices:
             kwargs.setdefault("widget", forms.get_default_widget())
-            kwargs.update({
-                "max_length": self.max_length,
-                "allowed_tags": self.bleach_kwargs.get("tags"),
-                "allowed_attributes": self.bleach_kwargs.get("attributes"),
-                "css_sanitizer": self.bleach_kwargs.get("css_sanitizer"),
-                "allowed_protocols": self.bleach_kwargs.get("protocols"),
-                "strip_tags": self.bleach_kwargs.get("strip"),
-                "strip_comments": self.bleach_kwargs.get("strip_comments"),
-                "required": not self.blank,
-            })
+            kwargs.update(
+                {
+                    "max_length": self.max_length,
+                    "allowed_tags": self.bleach_kwargs.get("tags"),
+                    "allowed_attributes": self.bleach_kwargs.get("attributes"),
+                    "css_sanitizer": self.bleach_kwargs.get("css_sanitizer"),
+                    "allowed_protocols": self.bleach_kwargs.get("protocols"),
+                    "strip_tags": self.bleach_kwargs.get("strip"),
+                    "strip_comments": self.bleach_kwargs.get("strip_comments"),
+                    "required": not self.blank,
+                }
+            )
 
         return super().formfield(form_class=form_class, **kwargs)
 
     def pre_save(self, model_instance, add):
         data = getattr(model_instance, self.attname)
         if data is None:
             return data
```

### Comparing `django-bleach-3.0.1/django_bleach/templatetags/bleach_tags.py` & `django-bleach-3.1.0/django_bleach/templatetags/bleach_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
+import bleach
 from django import template
 from django.utils.safestring import mark_safe
 
-import bleach
-
 from django_bleach.utils import get_bleach_default_options
 
-
 register = template.Library()
 
 
 @register.filter(name="bleach")
 def bleach_value(value, tags=None):
     if value is None:
         return None
```

### Comparing `django-bleach-3.0.1/django_bleach/tests/test_forms.py` & `django-bleach-3.1.0/django_bleach/tests/test_forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,233 +1,209 @@
+from bleach.css_sanitizer import CSSSanitizer
 from django import forms
 from django.test import TestCase, override_settings
 from django.utils.safestring import SafeString
 
-from bleach.css_sanitizer import CSSSanitizer
-
 from django_bleach.forms import BleachField
 from testproject.constants import (
     ALLOWED_ATTRIBUTES,
     ALLOWED_CSS_PROPERTIES,
     ALLOWED_PROTOCOLS,
     ALLOWED_STYLES,
     ALLOWED_TAGS,
 )
 from testproject.forms import BleachForm, CustomBleachWidget
 
 
 class TestBleachField(TestCase):
-
     def test_empty(self):
-        """ Test that the empty_value arg is returned for any input empty value """
-        for requested_empty_value in ('', None):
+        """
+        Test that the empty_value arg is returned for any input empty value
+        """
+        for requested_empty_value in ("", None):
             field = BleachField(empty_value=requested_empty_value)
             for empty_value in field.empty_values:
-                self.assertEqual(field.to_python(empty_value), requested_empty_value)
+                self.assertEqual(
+                    field.to_python(empty_value), requested_empty_value
+                )
 
     def test_return_type(self):
-        """ Test bleached values are SafeString objects """
+        """Test bleached values are SafeString objects"""
         field = BleachField()
         self.assertIsInstance(field.to_python("some text"), SafeString)
 
-    def test_deprecation_allowed_styles(self):
-        with self.assertWarns(DeprecationWarning):
-            BleachField(allowed_styles=ALLOWED_STYLES)
-
-    def test_prefer_css_sanitizer_over_allowed_styles(self):
-        with self.assertWarnsMessage(
-            UserWarning,
-            "allowed_styles argument is ignored since css_sanitizer is favoured over allowed_styles"
-        ):
-            field = BleachField(
-                allowed_styles=['color', 'text-align'],
-                css_sanitizer=CSSSanitizer(allowed_css_properties=ALLOWED_CSS_PROPERTIES)
-            )
-            self.assertIsInstance(field.bleach_options["css_sanitizer"], CSSSanitizer)
-            self.assertEqual(field.bleach_options["css_sanitizer"].allowed_css_properties, ALLOWED_CSS_PROPERTIES)
-
     def test_bleaching(self):
-        """ Test values are bleached """
+        """Test values are bleached"""
         test_data = {
-            'no_tags': "<h1>Heading</h1>",
-            'no_strip': "<h1>Heading</h1>",
-            'bleach_strip': "<!-- script here -->"
-                            "<script>alert(\"Hello World\")</script>",
-            'bleach_attrs': "<a href=\"https://www.google.com\" "
-                            "target=\"_blank\">google.com</a>",
-            'bleach_css_sanitizer': "<li style=\"color: white\">item</li>",
+            "no_tags": "<h1>Heading</h1>",
+            "no_strip": "<h1>Heading</h1>",
+            "bleach_strip": "<!-- script here -->"
+            '<script>alert("Hello World")</script>',
+            "bleach_attrs": '<a href="https://www.google.com" '
+            'target="_blank">google.com</a>',
+            "bleach_css_sanitizer": '<li style="color: white">item</li>',
         }
         form = BleachForm(data=test_data)
         form.is_valid()
+        self.assertEqual(form.cleaned_data["no_tags"], "Heading")
         self.assertEqual(
-            form.cleaned_data['no_tags'], 'Heading'
-        )
-        self.assertEqual(
-            form.cleaned_data['no_strip'],
-            '&lt;h1&gt;Heading&lt;/h1&gt;'
+            form.cleaned_data["no_strip"], "&lt;h1&gt;Heading&lt;/h1&gt;"
         )
         self.assertEqual(
-            form.cleaned_data['bleach_strip'],
-            'alert("Hello World")'
+            form.cleaned_data["bleach_strip"], 'alert("Hello World")'
         )
         self.assertEqual(
-            form.cleaned_data['bleach_attrs'],
-            '<a href="https://www.google.com">google.com</a>'
+            form.cleaned_data["bleach_attrs"],
+            '<a href="https://www.google.com">google.com</a>',
         )
         self.assertNotEqual(
-            form.cleaned_data['bleach_css_sanitizer'],
-            test_data['bleach_css_sanitizer']
+            form.cleaned_data["bleach_css_sanitizer"],
+            test_data["bleach_css_sanitizer"],
         )
 
     def test_tags(self):
-        """ Test allowed tags are rendered"""
+        """Test allowed tags are rendered"""
         test_data = {
-            'no_tags': "<p>No tags here</p>",
-            'no_strip': "No tags here",
-            'bleach_strip': "<ul><li>one</li><li>two</li></ul>",
-            'bleach_attrs': "<a href=\"https://www.google.com\" "
-                            "title=\"Google\">google.com</a>",
-            'bleach_css_sanitizer': "<li style=\"color: white;\">item</li>"
+            "no_tags": "<p>No tags here</p>",
+            "no_strip": "No tags here",
+            "bleach_strip": "<ul><li>one</li><li>two</li></ul>",
+            "bleach_attrs": '<a href="https://www.google.com" '
+            'title="Google">google.com</a>',
+            "bleach_css_sanitizer": '<li style="color: white;">item</li>',
         }
         form = BleachForm(data=test_data)
         form.is_valid()
-        self.assertEqual(form.cleaned_data['no_tags'], "No tags here")
-        self.assertEqual(form.cleaned_data['no_strip'], "No tags here")
+        self.assertEqual(form.cleaned_data["no_tags"], "No tags here")
+        self.assertEqual(form.cleaned_data["no_strip"], "No tags here")
 
         self.assertEqual(
-            form.cleaned_data['bleach_strip'],
-            test_data['bleach_strip']
+            form.cleaned_data["bleach_strip"], test_data["bleach_strip"]
         )
         self.assertEqual(
-            form.cleaned_data['bleach_attrs'],
-            test_data['bleach_attrs']
+            form.cleaned_data["bleach_attrs"], test_data["bleach_attrs"]
         )
         self.assertEqual(
-            form.cleaned_data['bleach_css_sanitizer'],
-            test_data['bleach_css_sanitizer']
+            form.cleaned_data["bleach_css_sanitizer"],
+            test_data["bleach_css_sanitizer"],
         )
 
     def test_attrs(self):
-        """ Test allowed attributes are rendered """
-        list_html = "<ul class=\"our-list\">" \
-                    "<li class=\"list-item\">one</li>" \
-                    "<li>two</li>" \
-                    "</ul>"
+        """Test allowed attributes are rendered"""
+        list_html = (
+            '<ul class="our-list">'
+            '<li class="list-item">one</li>'
+            "<li>two</li>"
+            "</ul>"
+        )
         test_data = {
-            'no_strip': "",
-            'no_tags': list_html,
-            'bleach_strip': list_html,
-            'bleach_attrs': list_html,
-            'bleach_css_sanitizer': list_html
+            "no_strip": "",
+            "no_tags": list_html,
+            "bleach_strip": list_html,
+            "bleach_attrs": list_html,
+            "bleach_css_sanitizer": list_html,
         }
         form = BleachForm(data=test_data)
         form.is_valid()
-        self.assertEqual(form.cleaned_data['no_tags'], '\none\ntwo')
+        self.assertEqual(form.cleaned_data["no_tags"], "\none\ntwo")
 
         self.assertEqual(
-            form.cleaned_data['bleach_strip'],
-            '<ul><li>one</li><li>two</li></ul>'
+            form.cleaned_data["bleach_strip"],
+            "<ul><li>one</li><li>two</li></ul>",
         )
         self.assertEqual(
-            form.cleaned_data['bleach_attrs'],
-            test_data['bleach_strip']
+            form.cleaned_data["bleach_attrs"], test_data["bleach_strip"]
         )
         self.assertEqual(
-            form.cleaned_data['bleach_css_sanitizer'],
-            '<ul><li>one</li><li>two</li></ul>'
+            form.cleaned_data["bleach_css_sanitizer"],
+            "<ul><li>one</li><li>two</li></ul>",
         )
 
 
-@override_settings(BLEACH_DEFAULT_WIDGET='testproject.forms.CustomBleachWidget')
+@override_settings(
+    BLEACH_DEFAULT_WIDGET="testproject.forms.CustomBleachWidget"
+)
 class TestCustomWidget(TestCase):
-
     def setUp(self):
         class CustomForm(forms.Form):
             # Define form inside function with overridden settings so
             # get_default_widget() sees the modified setting.
             no_tags = BleachField(
-                max_length=100,
-                strip_tags=True,
-                allowed_tags=[]
+                max_length=100, strip_tags=True, allowed_tags=[]
             )
             no_strip = BleachField(
-                max_length=100,
-                allowed_tags=None,
-                allowed_attributes=None
+                max_length=100, allowed_tags=None, allowed_attributes=None
             )
             bleach_strip = BleachField(
                 max_length=100,
                 strip_comments=True,
                 strip_tags=True,
-                allowed_tags=ALLOWED_TAGS
+                allowed_tags=ALLOWED_TAGS,
             )
             bleach_attrs = BleachField(
                 max_length=100,
                 strip_tags=False,
                 allowed_tags=ALLOWED_TAGS,
                 allowed_protocols=ALLOWED_PROTOCOLS,
-                allowed_attributes=ALLOWED_ATTRIBUTES
+                allowed_attributes=ALLOWED_ATTRIBUTES,
             )
             bleach_styles = BleachField(
                 max_length=100,
                 strip_tags=False,
-                allowed_attributes=['style'],
+                allowed_attributes=["style"],
                 allowed_tags=ALLOWED_TAGS,
-                allowed_styles=ALLOWED_STYLES
+                allowed_styles=ALLOWED_STYLES,
             )
             bleach_css_sanitizer = BleachField(
                 max_length=100,
                 strip_tags=False,
-                allowed_attributes=['style'],
+                allowed_attributes=["style"],
                 allowed_tags=ALLOWED_TAGS,
-                css_sanitizer=CSSSanitizer(allowed_css_properties=ALLOWED_CSS_PROPERTIES)
+                css_sanitizer=CSSSanitizer(
+                    allowed_css_properties=ALLOWED_CSS_PROPERTIES
+                ),
             )
+
         self.CustomForm = CustomForm
 
     def test_custom_widget_type(self):
-        """ Test widget class matches BLEACH_DEFAULT_WIDGET """
+        """Test widget class matches BLEACH_DEFAULT_WIDGET"""
         for field in self.CustomForm().fields.values():
             self.assertIsInstance(field.widget, CustomBleachWidget)
 
     def test_custom_widget_bleaches_content(self):
         """
         Test input is bleached according to config while using a custom
         widget
         """
         test_data = {
-            'no_tags': '<h1>Heading</h1>',
-            'no_strip': '<h1>Heading</h1>',
-            'bleach_strip': '<!-- script here -->'
-                            '<script>alert("Hello World")</script>',
-            'bleach_attrs': (
+            "no_tags": "<h1>Heading</h1>",
+            "no_strip": "<h1>Heading</h1>",
+            "bleach_strip": "<!-- script here -->"
+            '<script>alert("Hello World")</script>',
+            "bleach_attrs": (
                 '<a href="http://www.google.com" '
                 'target="_blank">google.com</a>'
                 '<a href="https://www.google.com">google.com</a>'
             ),
-            'bleach_styles': '<li style="color: white">item</li>',
-            'bleach_css_sanitizer': '<li style="color: white">item</li>'
+            "bleach_styles": '<li style="color: white">item</li>',
+            "bleach_css_sanitizer": '<li style="color: white">item</li>',
         }
         form = self.CustomForm(data=test_data)
         form.is_valid()
+        self.assertEqual(form.cleaned_data["no_tags"], "Heading")
         self.assertEqual(
-            form.cleaned_data['no_tags'], 'Heading'
-        )
-        self.assertEqual(
-            form.cleaned_data['no_strip'],
-            '&lt;h1&gt;Heading&lt;/h1&gt;'
+            form.cleaned_data["no_strip"], "&lt;h1&gt;Heading&lt;/h1&gt;"
         )
         self.assertEqual(
-            form.cleaned_data['bleach_strip'],
-            'alert("Hello World")'
+            form.cleaned_data["bleach_strip"], 'alert("Hello World")'
         )
         self.assertEqual(
-            form.cleaned_data['bleach_attrs'],
-            '<a>google.com</a><a href="https://www.google.com">google.com</a>'
+            form.cleaned_data["bleach_attrs"],
+            '<a>google.com</a><a href="https://www.google.com">google.com</a>',
         )
         self.assertNotEqual(
-            form.cleaned_data['bleach_styles'],
-            test_data['bleach_styles']
+            form.cleaned_data["bleach_styles"], test_data["bleach_styles"]
         )
         self.assertNotEqual(
-            form.cleaned_data['bleach_css_sanitizer'],
-            test_data['bleach_css_sanitizer']
+            form.cleaned_data["bleach_css_sanitizer"],
+            test_data["bleach_css_sanitizer"],
         )
```

### Comparing `django-bleach-3.0.1/django_bleach/tests/test_modelformfield.py` & `django-bleach-3.1.0/django_bleach/tests/test_modelformfield.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,72 +7,73 @@
 
 from .test_models import BleachContent
 
 
 class BleachContentModelForm(forms.ModelForm):
     class Meta:
         model = BleachContent
-        fields = '__all__'
+        fields = "__all__"
 
 
 class TestModelFormField(TestCase):
-
     def setUp(self):
         model_form = BleachContentModelForm()
-        self.form_field = model_form.fields['content']
-        self.choice_form_field = model_form.fields['choice']
-        self.blank_field_form_field = model_form.fields['blank_field']
-        self.model_field = BleachContent()._meta.get_field('content')
+        self.form_field = model_form.fields["content"]
+        self.choice_form_field = model_form.fields["choice"]
+        self.blank_field_form_field = model_form.fields["blank_field"]
+        self.model_field = BleachContent()._meta.get_field("content")
 
     def test_formfield_type(self):
         """
         Check content's form field is instance of BleachField
         """
         self.assertIsInstance(self.form_field, bleach_forms.BleachField)
 
     def test_default_widget_type(self):
         """
         Widget class is Textarea when BLEACH_DEFAULT_WIDGET is not set.
         """
-        form = forms.modelform_factory(Person, fields='__all__')()
+        form = forms.modelform_factory(Person, fields="__all__")()
         self.assertIsInstance(
-            form.fields['biography'].widget, forms.Textarea,
+            form.fields["biography"].widget,
+            forms.Textarea,
         )
 
     @override_settings(
-        BLEACH_DEFAULT_WIDGET='testproject.forms.CustomBleachWidget'
+        BLEACH_DEFAULT_WIDGET="testproject.forms.CustomBleachWidget"
     )
     def test_custom_widget_type(self):
         """
         Widget class matches BLEACH_DEFAULT_WIDGET setting.
         """
-        form = forms.modelform_factory(Person, fields='__all__')()
+        form = forms.modelform_factory(Person, fields="__all__")()
         self.assertIsInstance(
-            form.fields['biography'].widget, CustomBleachWidget
+            form.fields["biography"].widget, CustomBleachWidget
         )
 
     @override_settings(
-        BLEACH_DEFAULT_WIDGET='testproject.forms.CustomBleachWidget'
+        BLEACH_DEFAULT_WIDGET="testproject.forms.CustomBleachWidget"
     )
     def test_widget_override(self):
         """
         Widget class matches widget class specified in overrides.
         """
         form = forms.modelform_factory(
             Person,
-            fields='__all__',
+            fields="__all__",
             widgets={"biography": CustomBleachWidget},
         )()
         self.assertIsInstance(
-            form.fields['biography'].widget, CustomBleachWidget
+            form.fields["biography"].widget, CustomBleachWidget
         )
 
     def test_same_allowed_args(self):
         """
-        Check model and form's allowed arguments (tags, attributes, ...) are same
+        Check model and form's allowed arguments (tags, attributes, ...)
+        are the same
         """
         form_allowed_args: dict = self.form_field.bleach_options
         model_allowed_args: dict = self.model_field.bleach_kwargs
 
         self.assertEqual(model_allowed_args, form_allowed_args)
 
     def test_with_choices(self):
@@ -98,24 +99,23 @@
 class CustomBleachedFormField(bleach_forms.BleachField):
     ...
 
 
 class OverriddenBleachContentModelForm(forms.ModelForm):
     class Meta:
         model = BleachContent
-        fields = '__all__'
+        fields = "__all__"
         field_classes = {
             "content": CustomBleachedFormField,
         }
 
 
 class TestModelFormFieldOverrides(TestCase):
-
     def setUp(self):
         model_form = OverriddenBleachContentModelForm()
-        self.form_field = model_form.fields['content']
+        self.form_field = model_form.fields["content"]
 
     def test_formfield_type(self):
         """
         Check content's form field is instance of CustomBleachedFormField.
         """
         self.assertIsInstance(self.form_field, CustomBleachedFormField)
```

### Comparing `django-bleach-3.0.1/django_bleach/tests/test_settings.py` & `django-bleach-3.1.0/django_bleach/tests/test_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,92 @@
+from unittest.mock import patch
+
+from bleach.css_sanitizer import CSSSanitizer
 from django.core.exceptions import ImproperlyConfigured
 from django.forms import Textarea
 from django.test import TestCase, override_settings
 
-from bleach.css_sanitizer import CSSSanitizer
-from unittest.mock import patch
-
 from django_bleach.forms import get_default_widget
 from django_bleach.utils import get_bleach_default_options
-from testproject.constants import ALLOWED_ATTRIBUTES, ALLOWED_CSS_PROPERTIES, ALLOWED_PROTOCOLS, ALLOWED_TAGS
+from testproject.constants import (
+    ALLOWED_ATTRIBUTES,
+    ALLOWED_CSS_PROPERTIES,
+    ALLOWED_PROTOCOLS,
+    ALLOWED_TAGS,
+)
 from testproject.forms import CustomBleachWidget
 
 
 class TestBleachOptions(TestCase):
-
-    @patch('django_bleach.utils.settings',
-           BLEACH_ALLOWED_ATTRIBUTES=ALLOWED_ATTRIBUTES)
+    @patch(
+        "django_bleach.utils.settings",
+        BLEACH_ALLOWED_ATTRIBUTES=ALLOWED_ATTRIBUTES,
+    )
     def test_custom_attrs(self, settings):
         bleach_args = get_bleach_default_options()
-        self.assertEqual(bleach_args['attributes'], ALLOWED_ATTRIBUTES)
+        self.assertEqual(bleach_args["attributes"], ALLOWED_ATTRIBUTES)
 
-    @patch('django_bleach.utils.settings',
-           BLEACH_ALLOWED_PROTOCOLS=ALLOWED_PROTOCOLS)
+    @patch(
+        "django_bleach.utils.settings",
+        BLEACH_ALLOWED_PROTOCOLS=ALLOWED_PROTOCOLS,
+    )
     def test_custom_proto(self, settings):
         bleach_args = get_bleach_default_options()
-        self.assertEqual(bleach_args['protocols'], ALLOWED_PROTOCOLS)
+        self.assertEqual(bleach_args["protocols"], ALLOWED_PROTOCOLS)
 
-    @patch('django_bleach.utils.settings',
-           BLEACH_ALLOWED_STYLES=ALLOWED_CSS_PROPERTIES)
+    @patch(
+        "django_bleach.utils.settings",
+        BLEACH_ALLOWED_STYLES=ALLOWED_CSS_PROPERTIES,
+    )
     def test_custom_styles(self, settings):
         bleach_args = get_bleach_default_options()
-        self.assertIsInstance(bleach_args['css_sanitizer'], CSSSanitizer)
-        self.assertEqual(bleach_args['css_sanitizer'].allowed_css_properties, ALLOWED_CSS_PROPERTIES)
+        self.assertIsInstance(bleach_args["css_sanitizer"], CSSSanitizer)
+        self.assertEqual(
+            bleach_args["css_sanitizer"].allowed_css_properties,
+            ALLOWED_CSS_PROPERTIES,
+        )
 
-    @patch('django_bleach.utils.settings', BLEACH_ALLOWED_TAGS=ALLOWED_TAGS)
+    @patch("django_bleach.utils.settings", BLEACH_ALLOWED_TAGS=ALLOWED_TAGS)
     def test_custom_tags(self, settings):
         bleach_args = get_bleach_default_options()
-        self.assertEqual(bleach_args['tags'], ALLOWED_TAGS)
+        self.assertEqual(bleach_args["tags"], ALLOWED_TAGS)
 
-    @patch('django_bleach.utils.settings', BLEACH_STRIP_TAGS=True)
+    @patch("django_bleach.utils.settings", BLEACH_STRIP_TAGS=True)
     def test_strip_tags(self, settings):
         bleach_args = get_bleach_default_options()
-        self.assertEqual(bleach_args['strip'], True)
+        self.assertEqual(bleach_args["strip"], True)
 
-    @patch('django_bleach.utils.settings', BLEACH_STRIP_COMMENTS=True)
+    @patch("django_bleach.utils.settings", BLEACH_STRIP_COMMENTS=True)
     def test_strip_comments(self, settings):
         bleach_args = get_bleach_default_options()
-        self.assertEqual(bleach_args['strip_comments'], True)
+        self.assertEqual(bleach_args["strip_comments"], True)
 
 
 class TestDefaultWidget(TestCase):
-    """ Test form field widgets """
+    """Test form field widgets"""
 
-    @override_settings(BLEACH_DEFAULT_WIDGET='django.forms.widgets.Textarea')
+    @override_settings(BLEACH_DEFAULT_WIDGET="django.forms.widgets.Textarea")
     def test_default_widget(self):
         self.assertEqual(get_default_widget(), Textarea)
 
-    @patch('django_bleach.forms.settings',
-           BLEACH_DEFAULT_WIDGET='testproject.forms.CustomBleachWidget')
+    @patch(
+        "django_bleach.forms.settings",
+        BLEACH_DEFAULT_WIDGET="testproject.forms.CustomBleachWidget",
+    )
     def test_custom_widget(self, settings):
         self.assertEqual(get_default_widget(), CustomBleachWidget)
 
-    @patch('django_bleach.forms.settings',
-           BLEACH_DEFAULT_WIDGET='testproject.forms.NoneExistentWidget')
+    @patch(
+        "django_bleach.forms.settings",
+        BLEACH_DEFAULT_WIDGET="testproject.forms.NoneExistentWidget",
+    )
     def test_attribute_err(self, settings):
         with self.assertRaises(ImproperlyConfigured):
             get_default_widget()
 
-    @patch('django_bleach.forms.settings',
-           BLEACH_DEFAULT_WIDGET='testproject.forms2.CustomBleachWidget')
+    @patch(
+        "django_bleach.forms.settings",
+        BLEACH_DEFAULT_WIDGET="testproject.forms2.CustomBleachWidget",
+    )
     def test_import_err(self, settings):
         with self.assertRaises(ImproperlyConfigured):
             get_default_widget()
```

### Comparing `django-bleach-3.0.1/django_bleach/tests/test_templatetags.py` & `django-bleach-3.1.0/django_bleach/tests/test_templatetags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,68 @@
 from django.template import Context, Template
 from django.test import TestCase
 
 
 class TestBleachTemplates(TestCase):
-    """ Test template tags """
+    """Test template tags"""
 
     def test_bleaching(self):
-        """ Test that unsafe tags are sanitised """
+        """Test that unsafe tags are sanitised"""
         context = Context(
-            {'some_unsafe_content': '<script>alert("Hello World!")</script>'},
+            {"some_unsafe_content": '<script>alert("Hello World!")</script>'},
         )
         template_to_render = Template(
-            '{% load bleach_tags %}'
-            '{{ some_unsafe_content|bleach }}'
+            "{% load bleach_tags %}" "{{ some_unsafe_content|bleach }}"
         )
         rendered_template = template_to_render.render(context)
         self.assertInHTML(
             '&lt;script&gt;alert("Hello World!")&lt;/script&gt;',
-            rendered_template
+            rendered_template,
         )
 
     def test_bleaching_none(self):
-        """ Test that None is handled properly as an input """
-        context = Context(
-            {'none_value': None}
-        )
+        """Test that None is handled properly as an input"""
+        context = Context({"none_value": None})
         template_to_render = Template(
-            '{% load bleach_tags %}'
-            '{{ none_value|bleach }}'
+            "{% load bleach_tags %}" "{{ none_value|bleach }}"
         )
         rendered_template = template_to_render.render(context)
-        self.assertEqual(
-            'None',
-            rendered_template
-        )
+        self.assertEqual("None", rendered_template)
 
     def test_bleaching_tags(self):
-        """ Test provided tags are kept """
+        """Test provided tags are kept"""
         context = Context(
-            {'some_unsafe_content': '<script>alert("Hello World!")</script>'}
+            {"some_unsafe_content": '<script>alert("Hello World!")</script>'}
         )
         template_to_render = Template(
-            '{% load bleach_tags %}'
+            "{% load bleach_tags %}"
             '{{ some_unsafe_content|bleach:"script" }}'
         )
         rendered_template = template_to_render.render(context)
         self.assertInHTML(
             '<script>alert("Hello World!")</script>', rendered_template
         )
 
     def test_linkify(self):
-        """ Test bleach linkify """
-        url = 'www.google.com'
-        context = Context({'link_this': url})
+        """Test bleach linkify"""
+        url = "www.google.com"
+        context = Context({"link_this": url})
         template_to_render = Template(
-            '{% load bleach_tags %}'
-            '{{ link_this|bleach_linkify|safe }}'
+            "{% load bleach_tags %}" "{{ link_this|bleach_linkify|safe }}"
         )
         rendered_template = template_to_render.render(context)
         self.assertInHTML(
             '<a href="http://{0}" rel="nofollow">{0}</a>'.format(url),
-            rendered_template
+            rendered_template,
         )
 
     def test_linkify_none(self):
-        """ Test bleach linkify with None as an input """
-        context = Context({'none_value': None})
+        """Test bleach linkify with None as an input"""
+        context = Context({"none_value": None})
         template_to_render = Template(
-            '{% load bleach_tags %}'
-            '{{ none_value|bleach_linkify }}'
+            "{% load bleach_tags %}" "{{ none_value|bleach_linkify }}"
         )
         rendered_template = template_to_render.render(context)
         self.assertEqual(
-            'None',
+            "None",
             rendered_template,
         )
```

### Comparing `django-bleach-3.0.1/django_bleach/utils.py` & `django-bleach-3.1.0/django_bleach/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from django.conf import settings
-
 from bleach.css_sanitizer import CSSSanitizer
+from django.conf import settings
 
 
 def get_bleach_default_options():
     bleach_args = {}
     bleach_settings = {
         "BLEACH_ALLOWED_TAGS": "tags",
         "BLEACH_ALLOWED_ATTRIBUTES": "attributes",
         "BLEACH_ALLOWED_STYLES": "css_sanitizer",
         "BLEACH_STRIP_TAGS": "strip",
         "BLEACH_STRIP_COMMENTS": "strip_comments",
-        "BLEACH_ALLOWED_PROTOCOLS": "protocols"
+        "BLEACH_ALLOWED_PROTOCOLS": "protocols",
     }
 
     for setting, kwarg in bleach_settings.items():
         if hasattr(settings, setting):
             attr = getattr(settings, setting)
             if setting == "BLEACH_ALLOWED_STYLES":
                 attr = CSSSanitizer(allowed_css_properties=attr)
```

### Comparing `django-bleach-3.0.1/django_bleach.egg-info/PKG-INFO` & `django-bleach-3.1.0/django_bleach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bleach
-Version: 3.0.1
+Version: 3.1.0
 Summary: Easily use bleach with Django models and templates
 Home-page: https://github.com/marksweb/django-bleach
 Author: Tim Heap
 Maintainer: Mark Walker
 Maintainer-email: theshow+django-bleach@gmail.com
 License: MIT
 Project-URL: Documentation, https://django-bleach.readthedocs.io/
@@ -16,17 +16,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 django-bleach - Bleach and sanitise user HTML
 =============================================
```

### Comparing `django-bleach-3.0.1/django_bleach.egg-info/SOURCES.txt` & `django-bleach-3.1.0/django_bleach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/docs/index.rst` & `django-bleach-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/docs/settings.rst` & `django-bleach-3.1.0/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/docs/setup.rst` & `django-bleach-3.1.0/docs/setup.rst`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/docs/usage.rst` & `django-bleach-3.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/testproject/forms.py` & `django-bleach-3.1.0/testproject/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,62 +10,57 @@
     ALLOWED_STYLES,
     ALLOWED_TAGS,
 )
 from testproject.models import Person
 
 
 class CustomBleachWidget(forms.Textarea):
-
     def __init__(self, attrs=None):
-        default_attrs = {'rows': 15, 'cols': 60}
+        default_attrs = {"rows": 15, "cols": 60}
         default_attrs.update(attrs or {})
         super().__init__(attrs=default_attrs)
 
 
 class BleachForm(forms.Form):
-    """ Form for testing BleachField """
-    no_tags = BleachField(
-        max_length=100,
-        strip_tags=True,
-        allowed_tags=[]
-    )
+    """Form for testing BleachField"""
+
+    no_tags = BleachField(max_length=100, strip_tags=True, allowed_tags=[])
 
     no_strip = BleachField(
-        max_length=100,
-        allowed_tags=None,
-        allowed_attributes=None
+        max_length=100, allowed_tags=None, allowed_attributes=None
     )
 
     bleach_strip = BleachField(
         max_length=100,
         strip_comments=True,
         strip_tags=True,
-        allowed_tags=ALLOWED_TAGS
+        allowed_tags=ALLOWED_TAGS,
     )
     bleach_attrs = BleachField(
         max_length=100,
         strip_tags=False,
         allowed_tags=ALLOWED_TAGS,
         allowed_protocols=ALLOWED_PROTOCOLS,
-        allowed_attributes=ALLOWED_ATTRIBUTES
+        allowed_attributes=ALLOWED_ATTRIBUTES,
     )
     bleach_styles = BleachField(
         max_length=100,
         strip_tags=False,
-        allowed_attributes=['style'],
+        allowed_attributes=["style"],
         allowed_tags=ALLOWED_TAGS,
-        allowed_styles=ALLOWED_STYLES
+        allowed_styles=ALLOWED_STYLES,
     )
     bleach_css_sanitizer = BleachField(
         max_length=100,
         strip_tags=False,
-        allowed_attributes=['style'],
+        allowed_attributes=["style"],
         allowed_tags=ALLOWED_TAGS,
-        css_sanitizer=CSSSanitizer(allowed_css_properties=ALLOWED_CSS_PROPERTIES)
+        css_sanitizer=CSSSanitizer(
+            allowed_css_properties=ALLOWED_CSS_PROPERTIES
+        ),
     )
 
 
 class PersonForm(forms.ModelForm):
-
     class Meta:
         model = Person
-        fields = '__all__'
+        fields = "__all__"
```

### Comparing `django-bleach-3.0.1/testproject/manage.py` & `django-bleach-3.1.0/testproject/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 #!/usr/bin/env python
 import sys
 import os
+
 try:
     from django.core.management import execute_manager
+
     OLD_DJANGO = True
 except ImportError:
     from django.core.management import execute_from_command_line
+
     OLD_DJANGO = False
 
 if OLD_DJANGO:
     try:
         import settings  # Assumed to be in the same directory.
     except ImportError:
         sys.stderr.write(
             "Error: Can't find the file 'settings.py' in the directory containing %r. "
             "It appears you've customized things.\nYou'll have to run django-admin.py, "
             "passing it your settings module.\n(If the file settings.py does indeed exist, "
             "it's causing an ImportError somehow.)\n" % __file__
         )
         sys.exit(1)
 
-BASEDIR = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+BASEDIR = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.insert(0, BASEDIR)
 
 if __name__ == "__main__":
     os.environ["DJANGO_SETTINGS_MODULE"] = "testproject.settings"
     if OLD_DJANGO:
         execute_manager(settings)
     else:
```

### Comparing `django-bleach-3.0.1/testproject/migrations/0001_initial.py` & `django-bleach-3.1.0/testproject/migrations/0001_initial.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 # Generated by Django 3.2.4 on 2021-06-15 12:39
 
 from django.db import migrations, models
 import django_bleach.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
-            name='Person',
+            name="Person",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=20)),
-                ('biography', django_bleach.models.BleachField(max_length=100, verbose_name='Person biography')),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("name", models.CharField(max_length=20)),
+                (
+                    "biography",
+                    django_bleach.models.BleachField(
+                        max_length=100, verbose_name="Person biography"
+                    ),
+                ),
             ],
         ),
     ]
```

### Comparing `django-bleach-3.0.1/testproject/requirements.txt` & `django-bleach-3.1.0/testproject/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile
 #
 alabaster==0.7.12
     # via sphinx
-asgiref==3.4.1
+asgiref==3.6.0
     # via django
 attrs==21.4.0
     # via
     #   flake8-bugbear
     #   flake8-eradicate
 babel==2.9.1
     # via sphinx
 bleach==5.0.0
     # via -r requirements.in
-certifi==2021.10.8
+certifi==2022.12.7
     # via requests
 charset-normalizer==2.0.10
     # via requests
 click==8.0.3
     # via pip-tools
 coverage==6.2
     # via -r requirements.in
-django==4.0.7
+django==4.1.9
     # via -r requirements.in
 docutils==0.17.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
 eradicate==2.0.0
     # via flake8-eradicate
@@ -83,15 +83,15 @@
     # via -r requirements.in
 pip-tools==6.4.0
     # via -r requirements.in
 pycodestyle==2.8.0
     # via flake8
 pyflakes==2.4.0
     # via flake8
-pygments==2.11.2
+pygments==2.15.0
     # via sphinx
 pyparsing==3.0.6
     # via packaging
 pytz==2021.3
     # via babel
 requests==2.27.1
     # via sphinx
@@ -113,21 +113,21 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
 tomli==2.0.0
     # via pep517
 urllib3==1.26.7
     # via requests
 webencodings==0.5.1
     # via bleach
-wheel==0.37.1
+wheel==0.38.1
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `django-bleach-3.0.1/testproject/settings.py` & `django-bleach-3.1.0/testproject/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,72 +2,69 @@
 import sys
 
 
 SITE_ID = 1
 
 PROJECT_PATH = os.path.abspath(os.path.dirname(__file__))
 
-PYTHON_VERSION = '%s.%s' % sys.version_info[:2]
+PYTHON_VERSION = "%s.%s" % sys.version_info[:2]
 
 
 DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': os.path.join(PROJECT_PATH, 'django-bleach.db')
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": os.path.join(PROJECT_PATH, "django-bleach.db"),
     }
 }
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
 DATABASE_SUPPORTS_TRANSACTIONS = True
 
 INSTALLED_APPS = [
-    'django.contrib.auth',
-    'django.contrib.admin',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.sites',
-    'django.contrib.messages',
-
-    'django_bleach',
-    'testproject'
+    "django.contrib.auth",
+    "django.contrib.admin",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.sites",
+    "django.contrib.messages",
+    "django_bleach",
+    "testproject",
 ]
 
 LANGUAGE_CODE = "en"
 
-LANGUAGES = (
-    ('en', 'English'),
-)
+LANGUAGES = (("en", "English"),)
 
-ROOT_URLCONF = 'testproject.urls'
+ROOT_URLCONF = "testproject.urls"
 
 DEBUG = True
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'debug': False,
-            'context_processors': (
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "debug": False,
+            "context_processors": (
                 "django.contrib.auth.context_processors.auth",
                 "django.template.context_processors.debug",
                 "django.template.context_processors.i18n",
                 "django.template.context_processors.media",
                 "django.template.context_processors.request",
                 "django.template.context_processors.static",
                 "django.template.context_processors.tz",
-                "django.contrib.messages.context_processors.messages"
-            )
+                "django.contrib.messages.context_processors.messages",
+            ),
         },
-        'DIRS': ('templates', )
+        "DIRS": ("templates",),
     },
 ]
 
 USE_TZ = True
-SECRET_KEY = 'blah'
+SECRET_KEY = "blah"
 
 MIDDLEWARE = (
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware'
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
 )
 
 # BLEACH_DEFAULT_WIDGET = 'testproject.forms.CustomBleachWidget'
```

### Comparing `django-bleach-3.0.1/testproject/templates/model_form.html` & `django-bleach-3.1.0/testproject/templates/model_form.html`

 * *Files identical despite different names*

### Comparing `django-bleach-3.0.1/testproject/views.py` & `django-bleach-3.1.0/testproject/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,35 @@
 from .models import Person
 
 
 def home(request):
     if request.POST:
         form = BleachForm(request.POST)
         if form.is_valid():
-            return HttpResponseRedirect(request.path + '?ok')
+            return HttpResponseRedirect(request.path + "?ok")
     else:
         form = BleachForm()
 
-    return render(request, 'home.html', {'form': form})
+    return render(request, "home.html", {"form": form})
 
 
 def model_form(request):
-
     if request.POST:
         form = PersonForm(request.POST)
         if form.is_valid():
             form.save()
-            return HttpResponseRedirect('?ok')
+            return HttpResponseRedirect("?ok")
     else:
         form = PersonForm()
         try:
             people = list(Person.objects.all())
         except OperationalError:
             people = []
 
-        return render(request, 'model_form.html', {
-            'form': form,
-            'people': people,
-        })
+        return render(
+            request,
+            "model_form.html",
+            {
+                "form": form,
+                "people": people,
+            },
+        )
```

