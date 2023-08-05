# Comparing `tmp/sr.comp.http-1.8.0.tar.gz` & `tmp/sr.comp.http-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sr.comp.http-1.8.0.tar", last modified: Tue Mar 28 21:29:02 2023, max compression
+gzip compressed data, was "dist/sr.comp.http-1.8.1.tar", last modified: Sat Aug  5 16:21:28 2023, max compression
```

## Comparing `sr.comp.http-1.8.0.tar` & `sr.comp.http-1.8.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3620 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1130 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2117 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr/comp/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr/comp/http/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/escaping_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/json_encoder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/logging-stdout.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)      365 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/logging-syslog.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3213 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5184 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/query_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12022 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-03-28 21:28:53.000000 sr.comp.http-1.8.0/sr/comp/http/update.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3620 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      943 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/sr.comp.http.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/venv/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-28 21:29:02.000000 sr.comp.http-1.8.0/venv/bin/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      615 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2html.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      737 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      814 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      637 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2man.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      803 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1741 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      622 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      658 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      894 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      623 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      691 2023-03-28 21:29:00.000000 sr.comp.http-1.8.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3644 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      405 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2117 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr/comp/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr/comp/http/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      426 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/escaping_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/json_encoder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/logging-stdout.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      365 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/logging-syslog.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3213 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5184 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/query_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12162 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/update.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3644 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      943 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/venv/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/venv/bin/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      625 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2html.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      747 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2html4.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2html5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      824 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2latex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      647 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2man.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      813 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2odt.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      619 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      632 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      668 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2s5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      904 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      633 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2xml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      701 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rstpep2html.py
```

### Comparing `sr.comp.http-1.8.0/PKG-INFO` & `sr.comp.http-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 1.2
 Name: sr.comp.http
-Version: 1.8.0
+Version: 1.8.1
 Summary: HTTP API for Student Robotics Competition Software
 Home-page: https://github.com/PeterJCLaw/srcomp-http
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp-http.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp-http
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/srcomp-http/issues
 Description: SR Comp HTTP
         ============
         
         |Build Status| |Docs Status|
         
         A HTTP interface around `SRComp <https://github.com/PeterJCLaw/srcomp/wiki/SRComp>`__,
-        the fifth round of `Student Robotics <http://srobo.org>`__ competition
+        the fifth round of `Student Robotics <https://studentrobotics.org>`__ competition
         software.
         
         This repository provides a JSON API to accessing information about the
         state of the competition. It is a lightweight
-        `Flask <http://flask.pocoo.org/>`__ application wrapping the
+        `Flask <https://palletsprojects.com/p/flask/>`__ application wrapping the
         `SRComp <https://github.com/PeterJCLaw/srcomp>`__ python
         APIs to the competition state.
         
         Usage
         -----
         
         **Install**:
```

### Comparing `sr.comp.http-1.8.0/README.rst` & `sr.comp.http-1.8.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 SR Comp HTTP
 ============
 
 |Build Status| |Docs Status|
 
 A HTTP interface around `SRComp <https://github.com/PeterJCLaw/srcomp/wiki/SRComp>`__,
-the fifth round of `Student Robotics <http://srobo.org>`__ competition
+the fifth round of `Student Robotics <https://studentrobotics.org>`__ competition
 software.
 
 This repository provides a JSON API to accessing information about the
 state of the competition. It is a lightweight
-`Flask <http://flask.pocoo.org/>`__ application wrapping the
+`Flask <https://palletsprojects.com/p/flask/>`__ application wrapping the
 `SRComp <https://github.com/PeterJCLaw/srcomp>`__ python
 APIs to the competition state.
 
 Usage
 -----
 
 **Install**:
```

### Comparing `sr.comp.http-1.8.0/setup.cfg` & `sr.comp.http-1.8.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 default_section = THIRDPARTY
 known_first_party = sr.comp
 extra_standard_library = typing_extensions
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [mypy]
 warn_unused_configs = True
+show_column_numbers = True
 show_error_codes = True
 enable_error_code = ignore-without-code
 exclude = tests/dummy/scoring/
 warn_incomplete_stub = True
 warn_unused_ignores = True
 warn_redundant_casts = True
 no_implicit_optional = True
```

### Comparing `sr.comp.http-1.8.0/setup.py` & `sr.comp.http-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_namespace_packages, setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='sr.comp.http',
-    version='1.8.0',
+    version='1.8.1',
     url='https://github.com/PeterJCLaw/srcomp-http',
     project_urls={
         'Documentation': 'https://srcomp-http.readthedocs.org/',
         'Code': 'https://github.com/PeterJCLaw/srcomp-http',
         'Issue tracker': 'https://github.com/PeterJCLaw/srcomp-http/issues',
     },
     packages=find_namespace_packages(exclude=('tests',)),
```

### Comparing `sr.comp.http-1.8.0/sr/comp/http/__main__.py` & `sr.comp.http-1.8.1/sr/comp/http/__main__.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/sr/comp/http/config.py` & `sr.comp.http-1.8.1/sr/comp/http/config.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/sr/comp/http/json_encoder.py` & `sr.comp.http-1.8.1/sr/comp/http/json_encoder.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/sr/comp/http/manager.py` & `sr.comp.http-1.8.1/sr/comp/http/manager.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/sr/comp/http/query_utils.py` & `sr.comp.http-1.8.1/sr/comp/http/query_utils.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/sr/comp/http/server.py` & `sr.comp.http-1.8.1/sr/comp/http/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,19 +271,22 @@
             match_json_info(comp, match)
             for match in slots.values()
         )
 
     def parse_date(string: str) -> datetime.datetime:
         if ' ' in string:
             raise errors.BadRequest(
-                'Date string should not contain spaces. '
+                "Date string should not contain spaces. "
                 "Did you pass in a '+'?",
             )
         else:
-            return dateutil.parser.parse(string)
+            when = dateutil.parser.parse(string)
+            if when.tzinfo is None:
+                raise errors.BadRequest("Date string must include a timezone.")
+            return when
 
     filters: Any = [  # TODO: re-work this to get checking
         ('type', MatchType, lambda x: x['type']),
         ('arena', str, lambda x: x['arena']),
         ('num', int, lambda x: x['num']),
         ('game_start_time', parse_date, lambda x: x['times']['game']['start']),
         ('game_end_time', parse_date, lambda x: x['times']['game']['end']),
```

### Comparing `sr.comp.http-1.8.0/sr/comp/http/update.py` & `sr.comp.http-1.8.1/sr/comp/http/update.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/sr.comp.http.egg-info/PKG-INFO` & `sr.comp.http-1.8.1/sr.comp.http.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 1.2
 Name: sr.comp.http
-Version: 1.8.0
+Version: 1.8.1
 Summary: HTTP API for Student Robotics Competition Software
 Home-page: https://github.com/PeterJCLaw/srcomp-http
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp-http.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp-http
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/srcomp-http/issues
 Description: SR Comp HTTP
         ============
         
         |Build Status| |Docs Status|
         
         A HTTP interface around `SRComp <https://github.com/PeterJCLaw/srcomp/wiki/SRComp>`__,
-        the fifth round of `Student Robotics <http://srobo.org>`__ competition
+        the fifth round of `Student Robotics <https://studentrobotics.org>`__ competition
         software.
         
         This repository provides a JSON API to accessing information about the
         state of the competition. It is a lightweight
-        `Flask <http://flask.pocoo.org/>`__ application wrapping the
+        `Flask <https://palletsprojects.com/p/flask/>`__ application wrapping the
         `SRComp <https://github.com/PeterJCLaw/srcomp>`__ python
         APIs to the competition state.
         
         Usage
         -----
         
         **Install**:
```

### Comparing `sr.comp.http-1.8.0/sr.comp.http.egg-info/SOURCES.txt` & `sr.comp.http-1.8.1/sr.comp.http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2html.py` & `sr.comp.http-1.8.1/venv/bin/rst2html.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2html.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2html.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates (X)HTML documents from standalone reStructuredText '
                'sources.  ' + default_description)
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2html4.py` & `sr.comp.http-1.8.1/venv/bin/rst2html4.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2html4.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2html4.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing (X)HTML.
 
 The output conforms to XHTML 1.0 transitional
 and almost to HTML 4.01 transitional (except for closing empty tags).
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates (X)HTML documents from standalone reStructuredText '
                'sources.  ' + default_description)
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2html5.py` & `sr.comp.http-1.8.1/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2latex.py` & `sr.comp.http-1.8.1/venv/bin/rst2latex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2latex.py 8956 2022-01-20 10:11:44Z milde $
+# $Id: rst2latex.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing LaTeX.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline
 
 description = ('Generates LaTeX documents from standalone reStructuredText '
                'sources. '
                'Reads from <source> (default is stdin) and writes to '
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2man.py` & `sr.comp.http-1.8.1/venv/bin/rst2man.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 This module provides a simple command line interface that uses the
 man page writer to output from ReStructuredText source.
 """
 
 import locale
 try:
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 from docutils.writers import manpage
 
 description = ("Generates plain unix manual documents.  "
                + default_description)
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2odt.py` & `sr.comp.http-1.8.1/venv/bin/rst2odt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2odt.py 8994 2022-01-29 16:28:17Z milde $
+# $Id: rst2odt.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Dave Kuhlman <dkuhlman@rexx.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 A front end to the Docutils Publisher, producing OpenOffice documents.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline_to_binary, default_description
 from docutils.writers.odf_odt import Writer, Reader
 
 
 description = ('Generates OpenDocument/OpenOffice/ODF documents from '
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2pseudoxml.py` & `sr.comp.http-1.8.1/venv/bin/rst2pseudoxml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2pseudoxml.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2pseudoxml.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing pseudo-XML.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates pseudo-XML from standalone reStructuredText '
                'sources (for testing purposes).  ' + default_description)
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2s5.py` & `sr.comp.http-1.8.1/venv/bin/rst2s5.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2s5.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2s5.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Chris Liechti <cliechti@gmx.net>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML slides using
 the S5 template system.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates S5 (X)HTML slideshow documents from standalone '
                'reStructuredText sources.  ' + default_description)
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2xetex.py` & `sr.comp.http-1.8.1/venv/bin/rst2xetex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2xetex.py 8956 2022-01-20 10:11:44Z milde $
+# $Id: rst2xetex.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Guenter Milde
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing Lua/XeLaTeX code.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline
 
 description = ('Generates LaTeX documents from standalone reStructuredText '
                'sources for compilation with the Unicode-aware TeX variants '
                'XeLaTeX or LuaLaTeX. '
```

### Comparing `sr.comp.http-1.8.0/venv/bin/rst2xml.py` & `sr.comp.http-1.8.1/venv/bin/rstpep2html.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2xml.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rstpep2html.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
-A minimal front end to the Docutils Publisher, producing Docutils XML.
+A minimal front end to the Docutils Publisher, producing HTML from PEP
+(Python Enhancement Proposal) documents.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
-description = ('Generates Docutils-native XML from standalone '
-               'reStructuredText sources.  ' + default_description)
+description = ('Generates (X)HTML from reStructuredText-format PEP files.  '
+               + default_description)
 
-publish_cmdline(writer_name='xml', description=description)
+publish_cmdline(reader_name='pep', writer_name='pep_html',
+                description=description)
```

