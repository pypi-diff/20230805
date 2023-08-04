# Comparing `tmp/Carter-Offline-2.0.6.tar.gz` & `tmp/Carter-Offline-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.6.tar", last modified: Tue Jul 18 18:31:44 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.7.tar", last modified: Fri Aug  4 22:36:47 2023, max compression
```

## Comparing `Carter-Offline-2.0.6.tar` & `Carter-Offline-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.410636 Carter-Offline-2.0.6/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.400371 Carter-Offline-2.0.6/CarterOffline/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.401682 Carter-Offline-2.0.6/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.6/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.6/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)       20 2023-07-18 18:26:41.000000 Carter-Offline-2.0.6/CarterOffline/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.6/CarterOffline/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)    10343 2023-07-18 18:26:48.000000 Carter-Offline-2.0.6/CarterOffline/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.409987 Carter-Offline-2.0.6/Carter_Offline.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     2092 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      576 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.6/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     2092 2023-07-18 18:31:44.410483 Carter-Offline-2.0.6/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.6/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-18 18:31:44.410708 Carter-Offline-2.0.6/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1322 2023-07-18 18:30:19.000000 Carter-Offline-2.0.6/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/CarterOffline/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-04 22:19:13.000000 Carter-Offline-2.0.7/CarterOffline/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/CarterOffline/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      889 2023-08-04 22:33:09.000000 Carter-Offline-2.0.7/CarterOffline/main.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      387 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       30 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       14 2023-08-04 22:36:47.000000 Carter-Offline-2.0.7/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-08-04 22:18:30.000000 Carter-Offline-2.0.7/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2095 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1708 2023-08-04 22:34:49.000000 Carter-Offline-2.0.7/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-04 22:36:47.982785 Carter-Offline-2.0.7/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1328 2023-08-04 22:36:40.000000 Carter-Offline-2.0.7/setup.py
```

### Comparing `Carter-Offline-2.0.6/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.7/Carter_Offline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.6
+Version: 2.0.7
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -62,12 +62,12 @@
 ```
 
 <h5>Speak to your agent</h5>
 
 Here is the simple bit of code that sends the message to your Carter agent using the Carter-Py library, and then uses the Janex code to classify it, and save it to your intents file.
 
 ```
-ResponseOutput = SendToCarter(CarterAPI, input_string, User)
+ResponseOutput = CarterOffline.SendToCarter(input_string, User)
 
 print(ResponseOutput)
 
 ```
```

### Comparing `Carter-Offline-2.0.6/LICENSE` & `Carter-Offline-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.6/PKG-INFO` & `Carter-Offline-2.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.6
+Version: 2.0.7
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -62,12 +62,12 @@
 ```
 
 <h5>Speak to your agent</h5>
 
 Here is the simple bit of code that sends the message to your Carter agent using the Carter-Py library, and then uses the Janex code to classify it, and save it to your intents file.
 
 ```
-ResponseOutput = SendToCarter(CarterAPI, input_string, User)
+ResponseOutput = CarterOffline.SendToCarter(input_string, User)
 
 print(ResponseOutput)
 
 ```
```

### Comparing `Carter-Offline-2.0.6/README.md` & `Carter-Offline-2.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -49,12 +49,12 @@
 ```
 
 <h5>Speak to your agent</h5>
 
 Here is the simple bit of code that sends the message to your Carter agent using the Carter-Py library, and then uses the Janex code to classify it, and save it to your intents file.
 
 ```
-ResponseOutput = SendToCarter(CarterAPI, input_string, User)
+ResponseOutput = CarterOffline.SendToCarter(input_string, User)
 
 print(ResponseOutput)
 
 ```
```

### Comparing `Carter-Offline-2.0.6/setup.py` & `Carter-Offline-2.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.6",
+    version="2.0.7",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
@@ -33,17 +33,17 @@
     packages=setuptools.find_packages(),
 
 
     #if module has dependencies i.e. if your package rely on other package at pypi.org
     # then you must add there, in order to download every requirement of package
 
     install_requires=[
-          "numpy",
-        "torch",
         "carter-py",
+        "Janex",
+        "CipherProgram",
         ],
 
 
     license="Lily 1.0",
 
     # classifiers like program is suitable for python3, just leave as it is.
     classifiers=[
```

