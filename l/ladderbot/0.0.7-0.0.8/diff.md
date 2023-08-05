# Comparing `tmp/ladderbot-0.0.7.tar.gz` & `tmp/ladderbot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladderbot-0.0.7.tar", last modified: Sat Aug  5 18:53:42 2023, max compression
+gzip compressed data, was "ladderbot-0.0.8.tar", last modified: Sat Aug  5 18:57:29 2023, max compression
```

## Comparing `ladderbot-0.0.7.tar` & `ladderbot-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 18:53:42.306031 ladderbot-0.0.7/
--rw-rw-rw-   0        0        0    35802 2023-08-05 17:26:33.000000 ladderbot-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      530 2023-08-05 18:53:42.305032 ladderbot-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       32 2023-08-05 17:23:37.000000 ladderbot-0.0.7/README.md
--rw-rw-rw-   0        0        0      631 2023-08-05 18:53:03.000000 ladderbot-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 18:53:42.306031 ladderbot-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 18:53:42.260950 ladderbot-0.0.7/src/
--rw-rw-rw-   0        0        0       44 2023-08-05 18:52:21.000000 ladderbot-0.0.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 18:53:42.274114 ladderbot-0.0.7/src/ladderbot/
--rw-rw-rw-   0        0        0        0 2023-08-05 18:20:34.000000 ladderbot-0.0.7/src/ladderbot/__init__.py
--rw-rw-rw-   0        0        0    53173 2023-08-05 18:26:32.000000 ladderbot-0.0.7/src/ladderbot/controllers.py
--rw-rw-rw-   0        0        0      661 2023-08-01 15:46:39.000000 ladderbot-0.0.7/src/ladderbot/creds.py
--rw-rw-rw-   0        0        0     1251 2023-08-05 18:26:53.000000 ladderbot-0.0.7/src/ladderbot/html_creator.py
--rw-rw-rw-   0        0        0     4600 2023-07-29 19:13:10.000000 ladderbot-0.0.7/src/ladderbot/items.py
--rw-rw-rw-   0        0        0     9349 2023-07-29 19:33:34.000000 ladderbot-0.0.7/src/ladderbot/mappings.py
--rw-rw-rw-   0        0        0     4865 2023-08-05 18:51:17.000000 ladderbot-0.0.7/src/ladderbot/run.py
-drwxrwxrwx   0        0        0        0 2023-08-05 18:53:42.300045 ladderbot-0.0.7/src/ladderbot.egg-info/
--rw-rw-rw-   0        0        0      530 2023-08-05 18:53:42.000000 ladderbot-0.0.7/src/ladderbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-08-05 18:53:42.000000 ladderbot-0.0.7/src/ladderbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 18:53:42.000000 ladderbot-0.0.7/src/ladderbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-08-05 18:53:42.000000 ladderbot-0.0.7/src/ladderbot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-08-05 18:53:42.000000 ladderbot-0.0.7/src/ladderbot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 18:53:42.303041 ladderbot-0.0.7/src/resources/
--rw-rw-rw-   0        0        0     2167 2023-07-29 18:57:30.000000 ladderbot-0.0.7/src/resources/update.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:57:29.435025 ladderbot-0.0.8/
+-rw-rw-rw-   0        0        0    35802 2023-08-05 17:26:33.000000 ladderbot-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      530 2023-08-05 18:57:29.434054 ladderbot-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2023-08-05 17:23:37.000000 ladderbot-0.0.8/README.md
+-rw-rw-rw-   0        0        0      628 2023-08-05 18:57:07.000000 ladderbot-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 18:57:29.435025 ladderbot-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 18:57:29.399891 ladderbot-0.0.8/src/
+-rw-rw-rw-   0        0        0       44 2023-08-05 18:52:21.000000 ladderbot-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:57:29.410146 ladderbot-0.0.8/src/ladderbot/
+-rw-rw-rw-   0        0        0        0 2023-08-05 18:20:34.000000 ladderbot-0.0.8/src/ladderbot/__init__.py
+-rw-rw-rw-   0        0        0    53173 2023-08-05 18:26:32.000000 ladderbot-0.0.8/src/ladderbot/controllers.py
+-rw-rw-rw-   0        0        0      661 2023-08-01 15:46:39.000000 ladderbot-0.0.8/src/ladderbot/creds.py
+-rw-rw-rw-   0        0        0     1251 2023-08-05 18:26:53.000000 ladderbot-0.0.8/src/ladderbot/html_creator.py
+-rw-rw-rw-   0        0        0     4600 2023-07-29 19:13:10.000000 ladderbot-0.0.8/src/ladderbot/items.py
+-rw-rw-rw-   0        0        0     9349 2023-07-29 19:33:34.000000 ladderbot-0.0.8/src/ladderbot/mappings.py
+-rw-rw-rw-   0        0        0     4865 2023-08-05 18:51:17.000000 ladderbot-0.0.8/src/ladderbot/run.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:57:29.431031 ladderbot-0.0.8/src/ladderbot.egg-info/
+-rw-rw-rw-   0        0        0      530 2023-08-05 18:57:29.000000 ladderbot-0.0.8/src/ladderbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-08-05 18:57:29.000000 ladderbot-0.0.8/src/ladderbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:57:29.000000 ladderbot-0.0.8/src/ladderbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-05 18:57:29.000000 ladderbot-0.0.8/src/ladderbot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-05 18:57:29.000000 ladderbot-0.0.8/src/ladderbot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 18:57:29.432037 ladderbot-0.0.8/src/resources/
+-rw-rw-rw-   0        0        0     2167 2023-07-29 18:57:30.000000 ladderbot-0.0.8/src/resources/update.py
```

### Comparing `ladderbot-0.0.7/LICENSE` & `ladderbot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.7/PKG-INFO` & `ladderbot-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladderbot
-Version: 0.0.7
+Version: 0.0.8
 Summary: game automation
 Author-email: ch7cken <ch7cken@proton.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ladderbot-0.0.7/pyproject.toml` & `ladderbot-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ladderbot"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="ch7cken", email="ch7cken@proton.me" },
 ]
 description = "game automation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,8 +18,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
 
 [project.scripts]
-ladderbot = "ladderbot:launch"
+ladderbot = "ladderbot:run"
```

### Comparing `ladderbot-0.0.7/src/ladderbot/controllers.py` & `ladderbot-0.0.8/src/ladderbot/controllers.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.7/src/ladderbot/creds.py` & `ladderbot-0.0.8/src/ladderbot/creds.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.7/src/ladderbot/html_creator.py` & `ladderbot-0.0.8/src/ladderbot/html_creator.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.7/src/ladderbot/items.py` & `ladderbot-0.0.8/src/ladderbot/items.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.7/src/ladderbot/mappings.py` & `ladderbot-0.0.8/src/ladderbot/mappings.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.7/src/ladderbot/run.py` & `ladderbot-0.0.8/src/ladderbot/run.py`

 * *Files identical despite different names*

### Comparing `ladderbot-0.0.7/src/ladderbot.egg-info/PKG-INFO` & `ladderbot-0.0.8/src/ladderbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladderbot
-Version: 0.0.7
+Version: 0.0.8
 Summary: game automation
 Author-email: ch7cken <ch7cken@proton.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ladderbot-0.0.7/src/resources/update.py` & `ladderbot-0.0.8/src/resources/update.py`

 * *Files identical despite different names*

