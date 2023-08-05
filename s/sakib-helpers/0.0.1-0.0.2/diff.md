# Comparing `tmp/sakib_helpers-0.0.1.tar.gz` & `tmp/sakib_helpers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakib_helpers-0.0.1.tar", last modified: Thu Aug  3 03:30:35 2023, max compression
+gzip compressed data, was "sakib_helpers-0.0.2.tar", last modified: Sat Aug  5 02:55:31 2023, max compression
```

## Comparing `sakib_helpers-0.0.1.tar` & `sakib_helpers-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 03:30:35.192925 sakib_helpers-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-08-02 02:13:53.000000 sakib_helpers-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1619 2023-08-03 03:30:35.177304 sakib_helpers-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      956 2023-08-02 02:13:35.000000 sakib_helpers-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 03:30:35.114774 sakib_helpers-0.0.1/sakib_helpers/
--rw-rw-rw-   0        0        0        0 2023-08-02 02:03:25.000000 sakib_helpers-0.0.1/sakib_helpers/__init__.py
--rw-rw-rw-   0        0        0      205 2023-08-02 02:12:47.000000 sakib_helpers-0.0.1/sakib_helpers/filters.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:30:35.177304 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/
--rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/__init__.py
--rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/admin.py
--rw-rw-rw-   0        0        0      170 2023-08-03 03:08:38.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:30:35.177304 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/migrations/
--rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-08-03 03:08:38.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/models.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:30:35.177304 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/templatetags/
--rw-rw-rw-   0        0        0        0 2023-08-03 03:11:05.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/templatetags/__init__.py
--rw-rw-rw-   0        0        0      357 2023-08-03 03:15:10.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/templatetags/sakib_helpers.py
--rw-rw-rw-   0        0        0       63 2023-08-03 03:08:38.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/tests.py
--rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.1/sakib_helpers/sakib_helpers_app/views.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:30:35.161649 sakib_helpers-0.0.1/sakib_helpers.egg-info/
--rw-rw-rw-   0        0        0     1619 2023-08-03 03:30:34.000000 sakib_helpers-0.0.1/sakib_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-08-03 03:30:34.000000 sakib_helpers-0.0.1/sakib_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 03:30:34.000000 sakib_helpers-0.0.1/sakib_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 03:30:34.000000 sakib_helpers-0.0.1/sakib_helpers.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-08-03 03:30:34.000000 sakib_helpers-0.0.1/sakib_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-03 03:30:34.000000 sakib_helpers-0.0.1/sakib_helpers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 03:30:35.192925 sakib_helpers-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3067 2023-08-03 03:30:29.000000 sakib_helpers-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-08-02 02:13:53.000000 sakib_helpers-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1619 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2023-08-02 02:13:35.000000 sakib_helpers-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.351030 sakib_helpers-0.0.2/sakib_helpers/
+-rw-rw-rw-   0        0        0        0 2023-08-02 02:03:25.000000 sakib_helpers-0.0.2/sakib_helpers/__init__.py
+-rw-rw-rw-   0        0        0      205 2023-08-02 02:12:47.000000 sakib_helpers-0.0.2/sakib_helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.398323 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/
+-rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/admin.py
+-rw-rw-rw-   0        0        0      184 2023-08-05 02:52:34.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/migrations/
+-rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/models.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-08-03 03:11:05.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-08-03 03:15:10.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/templatetags/sakib_helpers.py
+-rw-rw-rw-   0        0        0       63 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/tests.py
+-rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/views.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.392311 sakib_helpers-0.0.2/sakib_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1619 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3121 2023-08-05 02:55:24.000000 sakib_helpers-0.0.2/setup.py
```

### Comparing `sakib_helpers-0.0.1/LICENSE` & `sakib_helpers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sakib_helpers-0.0.1/PKG-INFO` & `sakib_helpers-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakib_helpers
-Version: 0.0.1
+Version: 0.0.2
 Summary: python helper functions/methods
 Home-page: https://w3code.tech
 Author: Sakib Malik
 Author-email: maliksakib347@gmail.com
 Project-URL: Docs, https://w3code.tech
 Keywords: arithmetic,math,mathematics,python tutorial
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sakib_helpers-0.0.1/README.md` & `sakib_helpers-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sakib_helpers-0.0.1/sakib_helpers.egg-info/PKG-INFO` & `sakib_helpers-0.0.2/sakib_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakib-helpers
-Version: 0.0.1
+Version: 0.0.2
 Summary: python helper functions/methods
 Home-page: https://w3code.tech
 Author: Sakib Malik
 Author-email: maliksakib347@gmail.com
 Project-URL: Docs, https://w3code.tech
 Keywords: arithmetic,math,mathematics,python tutorial
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sakib_helpers-0.0.1/sakib_helpers.egg-info/SOURCES.txt` & `sakib_helpers-0.0.2/sakib_helpers.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 README.md
 setup.py
 sakib_helpers/__init__.py
-sakib_helpers/filters.py
+sakib_helpers/helpers.py
 sakib_helpers.egg-info/PKG-INFO
 sakib_helpers.egg-info/SOURCES.txt
 sakib_helpers.egg-info/dependency_links.txt
 sakib_helpers.egg-info/not-zip-safe
 sakib_helpers.egg-info/requires.txt
 sakib_helpers.egg-info/top_level.txt
 sakib_helpers/sakib_helpers_app/__init__.py
```

### Comparing `sakib_helpers-0.0.1/setup.py` & `sakib_helpers-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from io import open
 
 
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 6)
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'python helper functions/methods'
 LONG_DESCRIPTION = 'In this package have more helpful packages used in django and python. This package is developed by sakib malik.'
 
 
 def read(f):
     return open(f, 'r', encoding='utf-8').read()
 
@@ -50,19 +50,21 @@
     os.system("python setup.py sdist bdist_wheel")
     if os.system("twine check dist/*"):
         print("twine check failed. Packages might be outdated.")
         print("Try using `pip install -U twine wheel`.\nExiting.")
         sys.exit()
     os.system("twine upload dist/*")
     print("You probably want to also tag the version now:")
-    print("  git tag -a %s -m 'version %s'" % (VERSION, VERSION))
-    print("  git push --tags")
+    print("git push")
     shutil.rmtree('dist')
     shutil.rmtree('build')
     shutil.rmtree('sakib_helpers.egg-info')
+    # os.system("git add *")
+    # os.system(f"git commit -m 'New Version = {VERSION} released' ")
+    # os.system("git push")
     sys.exit()
 
 
 # Setting up
 setup(
     name="sakib_helpers",
     version=VERSION,
```

