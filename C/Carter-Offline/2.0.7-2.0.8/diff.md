# Comparing `tmp/Carter-Offline-2.0.7.tar.gz` & `tmp/Carter-Offline-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.7.tar", last modified: Fri Aug  4 22:36:47 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.8.tar", last modified: Fri Aug  4 22:43:54 2023, max compression
```

## Comparing `Carter-Offline-2.0.7.tar` & `Carter-Offline-2.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/CarterOffline/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-04 22:19:13.000000 Carter-Offline-2.0.7/CarterOffline/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/CarterOffline/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      889 2023-08-04 22:33:09.000000 Carter-Offline-2.0.7/CarterOffline/main.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/Carter_Offline.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      387 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       30 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       14 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1708 2023-08-04 22:34:49.000000 Carter-Offline-2.0.7/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1328 2023-08-04 22:36:40.000000 Carter-Offline-2.0.7/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/CarterOffline/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-04 22:19:13.000000 Carter-Offline-2.0.8/CarterOffline/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/CarterOffline/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      895 2023-08-04 22:43:17.000000 Carter-Offline-2.0.8/CarterOffline/main.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      387 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       30 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       14 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1708 2023-08-04 22:34:49.000000 Carter-Offline-2.0.8/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1328 2023-08-04 22:43:27.000000 Carter-Offline-2.0.8/setup.py
```

### Comparing `Carter-Offline-2.0.7/CarterOffline/main.py` & `Carter-Offline-2.0.8/CarterOffline/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from carterpy import Carter
 
 class CarterOffline:
     def __init__(self, intents_file_path, CarterAPI):
         self.intents_file_path = intents_file_path
         self.CarterAPI = CarterAPI
 
-    def SendToCarter(input_string, User):
+    def SendToCarter(self, input_string, User):
         carter = Carter(self.CarterAPI)
         response = carter.say(input_string, User)
         thesaurus_file_path = "thesaurus.json"
         matcher = IntentMatcher(self.intents_file_path, thesaurus_file_path)
         intent_class, sim = matcher.pattern_compare(input_string)
         intents = matcher.train()
```

### Comparing `Carter-Offline-2.0.7/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.8/Carter_Offline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.7
+Version: 2.0.8
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.7/LICENSE` & `Carter-Offline-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.7/PKG-INFO` & `Carter-Offline-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.7
+Version: 2.0.8
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.7/README.md` & `Carter-Offline-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.7/setup.py` & `Carter-Offline-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.7",
+    version="2.0.8",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

