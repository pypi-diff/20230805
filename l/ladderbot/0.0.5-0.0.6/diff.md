# Comparing `tmp/ladderbot-0.0.5.tar.gz` & `tmp/ladderbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladderbot-0.0.5.tar", last modified: Sat Aug  5 18:36:10 2023, max compression
+gzip compressed data, was "ladderbot-0.0.6.tar", last modified: Sat Aug  5 18:43:03 2023, max compression
```

## Comparing `ladderbot-0.0.5.tar` & `ladderbot-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 18:36:10.047053 ladderbot-0.0.5/
--rw-rw-rw-   0        0        0    35802 2023-08-05 17:26:33.000000 ladderbot-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      530 2023-08-05 18:36:10.046037 ladderbot-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       32 2023-08-05 17:23:37.000000 ladderbot-0.0.5/README.md
--rw-rw-rw-   0        0        0      578 2023-08-05 18:35:47.000000 ladderbot-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 18:36:10.047053 ladderbot-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 18:36:10.014126 ladderbot-0.0.5/src/
--rw-rw-rw-   0        0        0       25 2023-08-05 18:24:12.000000 ladderbot-0.0.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 18:36:10.028883 ladderbot-0.0.5/src/ladderbot/
--rw-rw-rw-   0        0        0        0 2023-08-05 18:20:34.000000 ladderbot-0.0.5/src/ladderbot/__init__.py
--rw-rw-rw-   0        0        0       10 2023-08-05 18:35:29.000000 ladderbot-0.0.5/src/ladderbot/__main__.py
--rw-rw-rw-   0        0        0    53173 2023-08-05 18:26:32.000000 ladderbot-0.0.5/src/ladderbot/controllers.py
--rw-rw-rw-   0        0        0      661 2023-08-01 15:46:39.000000 ladderbot-0.0.5/src/ladderbot/creds.py
--rw-rw-rw-   0        0        0     1251 2023-08-05 18:26:53.000000 ladderbot-0.0.5/src/ladderbot/html_creator.py
--rw-rw-rw-   0        0        0     4600 2023-07-29 19:13:10.000000 ladderbot-0.0.5/src/ladderbot/items.py
--rw-rw-rw-   0        0        0     9349 2023-07-29 19:33:34.000000 ladderbot-0.0.5/src/ladderbot/mappings.py
--rw-rw-rw-   0        0        0     4865 2023-08-05 18:26:01.000000 ladderbot-0.0.5/src/ladderbot/run.py
-drwxrwxrwx   0        0        0        0 2023-08-05 18:36:10.041911 ladderbot-0.0.5/src/ladderbot.egg-info/
--rw-rw-rw-   0        0        0      530 2023-08-05 18:36:09.000000 ladderbot-0.0.5/src/ladderbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-08-05 18:36:09.000000 ladderbot-0.0.5/src/ladderbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 18:36:09.000000 ladderbot-0.0.5/src/ladderbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-08-05 18:36:09.000000 ladderbot-0.0.5/src/ladderbot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 18:36:10.043902 ladderbot-0.0.5/src/resources/
--rw-rw-rw-   0        0        0     2167 2023-07-29 18:57:30.000000 ladderbot-0.0.5/src/resources/update.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:03.624773 ladderbot-0.0.6/
+-rw-rw-rw-   0        0        0    35802 2023-08-05 17:26:33.000000 ladderbot-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      530 2023-08-05 18:43:03.623774 ladderbot-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2023-08-05 17:23:37.000000 ladderbot-0.0.6/README.md
+-rw-rw-rw-   0        0        0      578 2023-08-05 18:41:45.000000 ladderbot-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 18:43:03.624773 ladderbot-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:03.591833 ladderbot-0.0.6/src/
+-rw-rw-rw-   0        0        0       25 2023-08-05 18:24:12.000000 ladderbot-0.0.6/src/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-08-05 18:41:16.000000 ladderbot-0.0.6/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:03.602833 ladderbot-0.0.6/src/ladderbot/
+-rw-rw-rw-   0        0        0        0 2023-08-05 18:20:34.000000 ladderbot-0.0.6/src/ladderbot/__init__.py
+-rw-rw-rw-   0        0        0       10 2023-08-05 18:35:29.000000 ladderbot-0.0.6/src/ladderbot/__main__.py
+-rw-rw-rw-   0        0        0    53173 2023-08-05 18:26:32.000000 ladderbot-0.0.6/src/ladderbot/controllers.py
+-rw-rw-rw-   0        0        0      661 2023-08-01 15:46:39.000000 ladderbot-0.0.6/src/ladderbot/creds.py
+-rw-rw-rw-   0        0        0     1251 2023-08-05 18:26:53.000000 ladderbot-0.0.6/src/ladderbot/html_creator.py
+-rw-rw-rw-   0        0        0     4600 2023-07-29 19:13:10.000000 ladderbot-0.0.6/src/ladderbot/items.py
+-rw-rw-rw-   0        0        0     9349 2023-07-29 19:33:34.000000 ladderbot-0.0.6/src/ladderbot/mappings.py
+-rw-rw-rw-   0        0        0     4865 2023-08-05 18:26:01.000000 ladderbot-0.0.6/src/ladderbot/run.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:03.620780 ladderbot-0.0.6/src/ladderbot.egg-info/
+-rw-rw-rw-   0        0        0      530 2023-08-05 18:43:03.000000 ladderbot-0.0.6/src/ladderbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-08-05 18:43:03.000000 ladderbot-0.0.6/src/ladderbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:43:03.000000 ladderbot-0.0.6/src/ladderbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-08-05 18:43:03.000000 ladderbot-0.0.6/src/ladderbot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 18:43:03.621780 ladderbot-0.0.6/src/resources/
+-rw-rw-rw-   0        0        0     2167 2023-07-29 18:57:30.000000 ladderbot-0.0.6/src/resources/update.py
```

### Comparing `ladderbot-0.0.5/LICENSE` & `ladderbot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.5/PKG-INFO` & `ladderbot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladderbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: game automation
 Author-email: ch7cken <ch7cken@proton.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ladderbot-0.0.5/pyproject.toml` & `ladderbot-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ladderbot"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="ch7cken", email="ch7cken@proton.me" },
 ]
 description = "game automation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ladderbot-0.0.5/src/ladderbot/controllers.py` & `ladderbot-0.0.6/src/ladderbot/controllers.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.5/src/ladderbot/creds.py` & `ladderbot-0.0.6/src/ladderbot/creds.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.5/src/ladderbot/html_creator.py` & `ladderbot-0.0.6/src/ladderbot/html_creator.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.5/src/ladderbot/items.py` & `ladderbot-0.0.6/src/ladderbot/items.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.5/src/ladderbot/mappings.py` & `ladderbot-0.0.6/src/ladderbot/mappings.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.5/src/ladderbot/run.py` & `ladderbot-0.0.6/src/ladderbot/run.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.5/src/ladderbot.egg-info/PKG-INFO` & `ladderbot-0.0.6/src/ladderbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladderbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: game automation
 Author-email: ch7cken <ch7cken@proton.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ladderbot-0.0.5/src/resources/update.py` & `ladderbot-0.0.6/src/resources/update.py`

 * *Files identical despite different names*

