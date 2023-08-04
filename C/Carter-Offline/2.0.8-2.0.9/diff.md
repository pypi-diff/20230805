# Comparing `tmp/Carter-Offline-2.0.8.tar.gz` & `tmp/Carter-Offline-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.8.tar", last modified: Fri Aug  4 22:43:54 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.9.tar", last modified: Fri Aug  4 23:22:27 2023, max compression
```

## Comparing `Carter-Offline-2.0.8.tar` & `Carter-Offline-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/CarterOffline/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-04 22:19:13.000000 Carter-Offline-2.0.8/CarterOffline/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/CarterOffline/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      895 2023-08-04 22:43:17.000000 Carter-Offline-2.0.8/CarterOffline/main.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/Carter_Offline.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      387 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       30 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       14 2023-08-04 22:43:54.000000 Carter-Offline-2.0.8/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-08-04 22:18:30.000000 Carter-Offline-2.0.8/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1708 2023-08-04 22:34:49.000000 Carter-Offline-2.0.8/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-04 22:43:54.452653 Carter-Offline-2.0.8/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1328 2023-08-04 22:43:27.000000 Carter-Offline-2.0.8/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 23:22:27.700483 Carter-Offline-2.0.9/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 23:22:27.700483 Carter-Offline-2.0.9/CarterOffline/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 23:22:27.700483 Carter-Offline-2.0.9/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.9/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.9/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-04 22:19:13.000000 Carter-Offline-2.0.9/CarterOffline/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-08-04 22:18:30.000000 Carter-Offline-2.0.9/CarterOffline/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1194 2023-08-04 23:22:05.000000 Carter-Offline-2.0.9/CarterOffline/main.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 23:22:27.700483 Carter-Offline-2.0.9/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2102 2023-08-04 23:22:27.000000 Carter-Offline-2.0.9/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      387 2023-08-04 23:22:27.000000 Carter-Offline-2.0.9/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-04 23:22:27.000000 Carter-Offline-2.0.9/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       30 2023-08-04 23:22:27.000000 Carter-Offline-2.0.9/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       14 2023-08-04 23:22:27.000000 Carter-Offline-2.0.9/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-08-04 22:18:30.000000 Carter-Offline-2.0.9/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2102 2023-08-04 23:22:27.700483 Carter-Offline-2.0.9/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1715 2023-08-04 23:03:18.000000 Carter-Offline-2.0.9/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-04 23:22:27.700483 Carter-Offline-2.0.9/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1328 2023-08-04 23:22:19.000000 Carter-Offline-2.0.9/setup.py
```

### Comparing `Carter-Offline-2.0.8/CarterOffline/main.py` & `Carter-Offline-2.0.9/CarterOffline/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,13 +10,22 @@
         carter = Carter(self.CarterAPI)
         response = carter.say(input_string, User)
         thesaurus_file_path = "thesaurus.json"
         matcher = IntentMatcher(self.intents_file_path, thesaurus_file_path)
         intent_class, sim = matcher.pattern_compare(input_string)
         intents = matcher.train()
 
-        intent_class.setdefault("patterns", []).append(input_string)
-        intent_class.setdefault("responses", []).append(response.output_text)
-        with open(self.intents_file_path, 'w') as json_file:
+        if intent_class:
+                target_class.setdefault("patterns", []).append(original)
+                target_class.setdefault("responses", []).append(ResponseOutput)
+        else:
+                new_class = {
+                        "tag": User,
+                        "patterns": [sentence],
+                        "responses": [ResponseOutput]
+                        }
+                intents['intents'].append(new_class)
+
+        with open(f"{self.intents_file_path}", 'w') as json_file:
             json.dump(intents, json_file, indent=4, separators=(',', ': '))
 
         return response.output_text
```

### Comparing `Carter-Offline-2.0.8/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.9/Carter_Offline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.8
+Version: 2.0.9
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 
 This is based on an older version of Janex (release 0.0.5.beta, specifically), and so it may not include the latest features from there unless explicitly added in.
 
 See also:
 
 ```
 https://github.com/LazyLyrics/carter-py
-https://github.com/Cipher58/Janex
+https://github.com/Cipher58/Janex-Python
 ```
 
 <h3> How to use </h3>
 
 <h5> Adding to your project </h5>
 
 Firstly, you'll need to install the library using the Python pip package manager.
```

### Comparing `Carter-Offline-2.0.8/LICENSE` & `Carter-Offline-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.8/PKG-INFO` & `Carter-Offline-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.8
+Version: 2.0.9
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 
 This is based on an older version of Janex (release 0.0.5.beta, specifically), and so it may not include the latest features from there unless explicitly added in.
 
 See also:
 
 ```
 https://github.com/LazyLyrics/carter-py
-https://github.com/Cipher58/Janex
+https://github.com/Cipher58/Janex-Python
 ```
 
 <h3> How to use </h3>
 
 <h5> Adding to your project </h5>
 
 Firstly, you'll need to install the library using the Python pip package manager.
```

### Comparing `Carter-Offline-2.0.8/README.md` & `Carter-Offline-2.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This is based on an older version of Janex (release 0.0.5.beta, specifically), and so it may not include the latest features from there unless explicitly added in.
 
 See also:
 
 ```
 https://github.com/LazyLyrics/carter-py
-https://github.com/Cipher58/Janex
+https://github.com/Cipher58/Janex-Python
 ```
 
 <h3> How to use </h3>
 
 <h5> Adding to your project </h5>
 
 Firstly, you'll need to install the library using the Python pip package manager.
```

### Comparing `Carter-Offline-2.0.8/setup.py` & `Carter-Offline-2.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.8",
+    version="2.0.9",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

