# Comparing `tmp/license_scanner-0.1.3.tar.gz` & `tmp/license_scanner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_scanner-0.1.3.tar", last modified: Wed Jul 26 18:22:13 2023, max compression
+gzip compressed data, was "license_scanner-0.2.0.tar", last modified: Sat Aug  5 11:49:01 2023, max compression
```

## Comparing `license_scanner-0.1.3.tar` & `license_scanner-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.897564 license_scanner-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 18:22:03.000000 license_scanner-0.1.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-26 18:22:03.000000 license_scanner-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 18:22:13.897564 license_scanner-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 18:22:03.000000 license_scanner-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.893564 license_scanner-0.1.3/license_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/get_all_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.897564 license_scanner-0.1.3/license_scanner/parse_license/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/parse_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/parse_license/licenses_synonyms.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 18:22:03.000000 license_scanner-0.1.3/license_scanner/parse_license/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:13.897564 license_scanner-0.1.3/license_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 18:22:13.000000 license_scanner-0.1.3/license_scanner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 18:22:03.000000 license_scanner-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-26 18:22:13.897564 license_scanner-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-26 18:22:03.000000 license_scanner-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:01.665816 license_scanner-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-05 11:48:42.000000 license_scanner-0.2.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-05 11:48:42.000000 license_scanner-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-05 11:49:01.665816 license_scanner-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-05 11:48:42.000000 license_scanner-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:01.657816 license_scanner-0.2.0/license_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-05 11:48:42.000000 license_scanner-0.2.0/license_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-05 11:48:42.000000 license_scanner-0.2.0/license_scanner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-05 11:48:42.000000 license_scanner-0.2.0/license_scanner/get_all_licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:01.661816 license_scanner-0.2.0/license_scanner/parse_license/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-05 11:48:42.000000 license_scanner-0.2.0/license_scanner/parse_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-08-05 11:48:42.000000 license_scanner-0.2.0/license_scanner/parse_license/licenses_synonyms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-05 11:48:42.000000 license_scanner-0.2.0/license_scanner/parse_license/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:01.661816 license_scanner-0.2.0/license_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-05 11:49:01.000000 license_scanner-0.2.0/license_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-05 11:49:01.000000 license_scanner-0.2.0/license_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:49:01.000000 license_scanner-0.2.0/license_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-05 11:49:01.000000 license_scanner-0.2.0/license_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:48:48.000000 license_scanner-0.2.0/license_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 11:49:01.000000 license_scanner-0.2.0/license_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-05 11:49:01.000000 license_scanner-0.2.0/license_scanner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-05 11:48:42.000000 license_scanner-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-05 11:48:42.000000 license_scanner-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-05 11:49:01.665816 license_scanner-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-05 11:48:42.000000 license_scanner-0.2.0/setup.py
```

### Comparing `license_scanner-0.1.3/license_scanner/get_all_licenses.py` & `license_scanner-0.2.0/license_scanner/get_all_licenses.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#%%
+# %%
 from pkg_resources import working_set
-from .parse_license import parse_license
+from license_scanner.parse_license import parse_license
 
 
 def get_all_licenses():
     all_licenses = {}
     for key in working_set.normalized_to_canonical_keys:
         """
         The metadata of a package is stored in "metadata" or "PKG-INFO"
```

### Comparing `license_scanner-0.1.3/license_scanner/parse_license/licenses_synonyms.py` & `license_scanner-0.2.0/license_scanner/parse_license/licenses_synonyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,18 @@
     "gnu affero general public license v3": gnu_affero_v3,
     "gnu affero general public license v3.0": gnu_affero_v3,
     "gnu affero general public license, version 3": gnu_affero_v3,
     "gnu affero gpl 3.0": gnu_affero_v3,
     "gnu affero general public license v3 or later (agplv3+)": gnu_affero_v3,
     "gnu library or lesser general public license (lgpl)": gnu_lesser_public_license,
     "gnu lesser general public license v2 (lgplv2)": gnu_lesser_public_license_v2,
+    "gnu lesser general public license v2": gnu_lesser_public_license_v2,
     "lgpl-2.1-only": gnu_lesser_public_license_v2,
     "gnu lesser general public license v3 (lgplv3)": gnu_lesser_public_license_v3,
+    "gnu lesser general public license v3": gnu_lesser_public_license_v3,
     "lgpl, see also license.txt": gnu_lesser_public_license,
     "lgpl-2.1 license": gnu_lesser_public_license_v2,
     "lgpl-3.0": gnu_lesser_public_license_v3,
     "https://www.gnu.org/licenses/lgpl.html": gnu_lesser_public_license_v3,
     "lgpl-3.0 license": gnu_lesser_public_license_v3,
     "gnu lesser general public license version 3, 29 june 2007  copyright (c) 2007 free software foundation, inc. <https://fsf.org/> everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.   this version of the gnu lesser general public licen": gnu_lesser_public_license_v3,
     "gnu lesser general public license v2 or later (lgplv2+)": gnu_lesser_public_license_v2,
```

### Comparing `license_scanner-0.1.3/license_scanner/parse_license/main.py` & `license_scanner-0.2.0/license_scanner/parse_license/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from .licenses_synonyms import LICENSES_SYNONYMS
+from license_scanner.parse_license.licenses_synonyms import LICENSES_SYNONYMS
 
 current_loc = os.path.dirname(os.path.realpath(__file__))
 
 
 def remove_trailing_whitespace(string: str):
     if string.endswith((" ", "\t", "\n", "\r")):
         return remove_trailing_whitespace(string[:-1])
```

### Comparing `license_scanner-0.1.3/setup.cfg` & `license_scanner-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.3
+current_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `license_scanner-0.1.3/setup.py` & `license_scanner-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     keywords="license_scanner",
     name="license_scanner",
     packages=find_packages(include=["license_scanner*"], exclude=["docs*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/wagenrace/license_scanner",
-    version="0.1.3",
+    version="0.2.0",
     zip_safe=False,
 )
```

