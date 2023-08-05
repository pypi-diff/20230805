# Comparing `tmp/hardbrake-0.1.1.tar.gz` & `tmp/hardbrake-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardbrake-0.1.1.tar", last modified: Wed Apr 12 14:57:17 2023, max compression
+gzip compressed data, was "hardbrake-0.1.2.tar", last modified: Sat Aug  5 21:00:31 2023, max compression
```

## Comparing `hardbrake-0.1.1.tar` & `hardbrake-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:57:17.214648 hardbrake-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-12 14:56:42.000000 hardbrake-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 14:57:17.214648 hardbrake-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      940 2023-04-12 14:56:42.000000 hardbrake-0.1.1/README.md
--rwxr-xr-x   0 root         (0) root         (0)      517 2023-04-12 14:56:42.000000 hardbrake-0.1.1/hardbrake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:57:17.210648 hardbrake-0.1.1/hardbrake.egg-info/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      340 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-04-12 14:56:42.000000 hardbrake-0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 14:57:17.214648 hardbrake-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      502 2023-04-12 14:56:42.000000 hardbrake-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:57:17.214648 hardbrake-0.1.1/src/
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/app.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/event.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/file.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/loader.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/logger.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/manager.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/prompts.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 21:00:31.082325 hardbrake-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-08-05 20:59:48.000000 hardbrake-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      199 2023-08-05 21:00:31.082325 hardbrake-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      940 2023-08-05 20:59:48.000000 hardbrake-0.1.2/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      517 2023-08-05 20:59:48.000000 hardbrake-0.1.2/hardbrake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 21:00:31.078325 hardbrake-0.1.2/hardbrake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-08-05 21:00:31.000000 hardbrake-0.1.2/hardbrake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      340 2023-08-05 21:00:31.000000 hardbrake-0.1.2/hardbrake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 21:00:31.000000 hardbrake-0.1.2/hardbrake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-08-05 21:00:31.000000 hardbrake-0.1.2/hardbrake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-05 21:00:31.000000 hardbrake-0.1.2/hardbrake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-08-05 20:59:48.000000 hardbrake-0.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 21:00:31.082325 hardbrake-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      502 2023-08-05 20:59:48.000000 hardbrake-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 21:00:31.082325 hardbrake-0.1.2/src/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/app.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/event.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/file.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/loader.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/prompts.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-08-05 20:59:48.000000 hardbrake-0.1.2/src/utils.py
```

### Comparing `hardbrake-0.1.1/LICENSE` & `hardbrake-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/README.md` & `hardbrake-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/hardbrake` & `hardbrake-0.1.2/hardbrake`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/src/app.py` & `hardbrake-0.1.2/src/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 traceback.install()
 
 
 def main():
   try:
     try:
       utils.verify_installation("HandBrakeCLI")
-      logger.success("HandBrakeCLI is installed")
+      logger.success("HandBrakeCLI found")
+      utils.verify_installation("ranger")
+      logger.success("ranger found")
     except Exception as e:
       logger.error(e.args[0])
       return
 
     happy = False
     original_files = file.select_files()
```

### Comparing `hardbrake-0.1.1/src/event.py` & `hardbrake-0.1.2/src/event.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/src/file.py` & `hardbrake-0.1.2/src/file.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/src/loader.py` & `hardbrake-0.1.2/src/loader.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/src/manager.py` & `hardbrake-0.1.2/src/manager.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/src/prompts.py` & `hardbrake-0.1.2/src/prompts.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.1/src/utils.py` & `hardbrake-0.1.2/src/utils.py`

 * *Files identical despite different names*

