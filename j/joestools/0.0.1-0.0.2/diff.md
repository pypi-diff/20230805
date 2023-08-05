# Comparing `tmp/joestools-0.0.1.tar.gz` & `tmp/joestools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joestools-0.0.1.tar", last modified: Thu Aug  3 21:23:46 2023, max compression
+gzip compressed data, was "joestools-0.0.2.tar", last modified: Sat Aug  5 19:54:11 2023, max compression
```

## Comparing `joestools-0.0.1.tar` & `joestools-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jochen    (1000) jochen    (1000)        0 2023-08-03 21:23:46.450147 joestools-0.0.1/
--rw-rw-r--   0 jochen    (1000) jochen    (1000)    35131 2023-01-24 23:34:06.000000 joestools-0.0.1/LICENSE
--rw-rw-r--   0 jochen    (1000) jochen    (1000)      471 2023-08-03 21:23:46.450147 joestools-0.0.1/PKG-INFO
--rw-rw-r--   0 jochen    (1000) jochen    (1000)      100 2023-01-24 23:32:23.000000 joestools-0.0.1/README.md
--rw-rw-r--   0 jochen    (1000) jochen    (1000)      935 2023-08-03 21:23:36.000000 joestools-0.0.1/pyproject.toml
--rw-rw-r--   0 jochen    (1000) jochen    (1000)       38 2023-08-03 21:23:46.450147 joestools-0.0.1/setup.cfg
-drwxrwxr-x   0 jochen    (1000) jochen    (1000)        0 2023-08-03 21:23:46.450147 joestools-0.0.1/src/
--rw-rw-r--   0 jochen    (1000) jochen    (1000)    14591 2023-02-20 20:30:03.000000 joestools-0.0.1/src/controlhue2.py
-drwxrwxr-x   0 jochen    (1000) jochen    (1000)        0 2023-08-03 21:23:46.450147 joestools-0.0.1/src/joestools/
--rw-rw-r--   0 jochen    (1000) jochen    (1000)        0 2023-01-19 14:27:46.000000 joestools-0.0.1/src/joestools/__init__.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)    14901 2023-05-19 09:17:52.000000 joestools-0.0.1/src/joestools/ccu_jack.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)    12934 2023-07-30 14:39:36.000000 joestools-0.0.1/src/joestools/common.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)     8392 2023-08-01 11:14:38.000000 joestools-0.0.1/src/joestools/credauth.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)    18544 2023-05-29 21:05:38.000000 joestools-0.0.1/src/joestools/fhem_con.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)    14648 2023-05-18 23:12:22.000000 joestools-0.0.1/src/joestools/hue.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)    10281 2023-02-21 20:50:22.000000 joestools-0.0.1/src/joestools/knx.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)     6314 2023-05-18 23:17:30.000000 joestools-0.0.1/src/joestools/lancom.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)     7905 2023-08-03 21:10:31.000000 joestools-0.0.1/src/joestools/misc.py
--rw-rw-r--   0 jochen    (1000) jochen    (1000)     7088 2023-08-01 13:03:48.000000 joestools-0.0.1/src/joestools/msh.py
-drwxrwxr-x   0 jochen    (1000) jochen    (1000)        0 2023-08-03 21:23:46.450147 joestools-0.0.1/src/joestools.egg-info/
--rw-rw-r--   0 jochen    (1000) jochen    (1000)      471 2023-08-03 21:23:46.000000 joestools-0.0.1/src/joestools.egg-info/PKG-INFO
--rw-rw-r--   0 jochen    (1000) jochen    (1000)      472 2023-08-03 21:23:46.000000 joestools-0.0.1/src/joestools.egg-info/SOURCES.txt
--rw-rw-r--   0 jochen    (1000) jochen    (1000)        1 2023-08-03 21:23:46.000000 joestools-0.0.1/src/joestools.egg-info/dependency_links.txt
--rw-rw-r--   0 jochen    (1000) jochen    (1000)      243 2023-08-03 21:23:46.000000 joestools-0.0.1/src/joestools.egg-info/requires.txt
--rw-rw-r--   0 jochen    (1000) jochen    (1000)       22 2023-08-03 21:23:46.000000 joestools-0.0.1/src/joestools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:54:11.494451 joestools-0.0.2/
+-rw-rw-r--   0 root         (0) root         (0)    35131 2023-01-24 23:34:06.000000 joestools-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      471 2023-08-05 19:54:11.494451 joestools-0.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      100 2023-01-24 23:32:23.000000 joestools-0.0.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      934 2023-08-05 19:54:00.000000 joestools-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 19:54:11.494451 joestools-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:54:11.490451 joestools-0.0.2/src/
+-rw-rw-r--   0 root         (0) root         (0)    14591 2023-02-20 20:30:03.000000 joestools-0.0.2/src/controlhue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:54:11.494451 joestools-0.0.2/src/joestools/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-01-19 14:27:46.000000 joestools-0.0.2/src/joestools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14901 2023-05-19 09:17:52.000000 joestools-0.0.2/src/joestools/ccu_jack.py
+-rw-rw-r--   0 root         (0) root         (0)    12934 2023-07-30 14:39:36.000000 joestools-0.0.2/src/joestools/common.py
+-rw-rw-r--   0 root         (0) root         (0)     8392 2023-08-01 11:14:38.000000 joestools-0.0.2/src/joestools/credauth.py
+-rw-rw-r--   0 root         (0) root         (0)    18544 2023-05-29 21:05:38.000000 joestools-0.0.2/src/joestools/fhem_con.py
+-rw-rw-r--   0 root         (0) root         (0)    14648 2023-05-18 23:12:22.000000 joestools-0.0.2/src/joestools/hue.py
+-rw-rw-r--   0 root         (0) root         (0)    10281 2023-02-21 20:50:22.000000 joestools-0.0.2/src/joestools/knx.py
+-rw-rw-r--   0 root         (0) root         (0)     6314 2023-05-18 23:17:30.000000 joestools-0.0.2/src/joestools/lancom.py
+-rw-rw-r--   0 root         (0) root         (0)     7905 2023-08-03 21:10:31.000000 joestools-0.0.2/src/joestools/misc.py
+-rw-rw-r--   0 root         (0) root         (0)     7088 2023-08-01 13:03:48.000000 joestools-0.0.2/src/joestools/msh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:54:11.494451 joestools-0.0.2/src/joestools.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      471 2023-08-05 19:54:11.000000 joestools-0.0.2/src/joestools.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      472 2023-08-05 19:54:11.000000 joestools-0.0.2/src/joestools.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-08-05 19:54:11.000000 joestools-0.0.2/src/joestools.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      242 2023-08-05 19:54:11.000000 joestools-0.0.2/src/joestools.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-08-05 19:54:11.000000 joestools-0.0.2/src/joestools.egg-info/top_level.txt
```

### Comparing `joestools-0.0.1/LICENSE` & `joestools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/pyproject.toml` & `joestools-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joestools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jochen Mälzer", email="mishki@mishki.de" },
 ]
 description = "Tools for my home automation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,15 +19,15 @@
 dependencies = [
     "beautifulsoup4 == 4.12.2",
     "fhem == 0.6.5",
     "Flask==2.2.2",
     "Flask-HTTPAuth==4.7.0",
     "itsdangerous==2.1.2",
     "Jinja2==3.1.2",
-    "lxml==4.9.20",
+    "lxml==4.9.2",
     "mysql-connector-python==8.0.32",
     "platformdirs==2.6.2",
     "requests==2.28.2",
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "Werkzeug==2.2.2",
 ]
```

### Comparing `joestools-0.0.1/src/controlhue2.py` & `joestools-0.0.2/src/controlhue2.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/ccu_jack.py` & `joestools-0.0.2/src/joestools/ccu_jack.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/common.py` & `joestools-0.0.2/src/joestools/common.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/credauth.py` & `joestools-0.0.2/src/joestools/credauth.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/fhem_con.py` & `joestools-0.0.2/src/joestools/fhem_con.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/hue.py` & `joestools-0.0.2/src/joestools/hue.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/knx.py` & `joestools-0.0.2/src/joestools/knx.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/lancom.py` & `joestools-0.0.2/src/joestools/lancom.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/misc.py` & `joestools-0.0.2/src/joestools/misc.py`

 * *Files identical despite different names*

### Comparing `joestools-0.0.1/src/joestools/msh.py` & `joestools-0.0.2/src/joestools/msh.py`

 * *Files identical despite different names*

