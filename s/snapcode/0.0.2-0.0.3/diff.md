# Comparing `tmp/snapcode-0.0.2.tar.gz` & `tmp/snapcode-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapcode-0.0.2.tar", last modified: Tue Aug  1 13:50:16 2023, max compression
+gzip compressed data, was "snapcode-0.0.3.tar", last modified: Sat Aug  5 05:53:55 2023, max compression
```

## Comparing `snapcode-0.0.2.tar` & `snapcode-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:50:16.693863 snapcode-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 13:50:03.000000 snapcode-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 13:50:16.693863 snapcode-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 13:50:03.000000 snapcode-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 13:50:16.693863 snapcode-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-01 13:50:03.000000 snapcode-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:50:16.693863 snapcode-0.0.2/snapcode/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-01 13:50:03.000000 snapcode-0.0.2/snapcode/snapcode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:50:16.693863 snapcode-0.0.2/snapcode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 13:50:16.000000 snapcode-0.0.2/snapcode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-01 13:50:16.000000 snapcode-0.0.2/snapcode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:50:16.000000 snapcode-0.0.2/snapcode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:50:16.000000 snapcode-0.0.2/snapcode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 13:50:16.000000 snapcode-0.0.2/snapcode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 13:50:16.000000 snapcode-0.0.2/snapcode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 05:53:55.109038 snapcode-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 05:53:46.000000 snapcode-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-05 05:53:55.109038 snapcode-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-05 05:53:46.000000 snapcode-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-05 05:53:55.109038 snapcode-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-05 05:53:46.000000 snapcode-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 05:53:55.105038 snapcode-0.0.3/snapcode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-05 05:53:46.000000 snapcode-0.0.3/snapcode/snapcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 05:53:55.109038 snapcode-0.0.3/snapcode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-05 05:53:55.000000 snapcode-0.0.3/snapcode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-05 05:53:55.000000 snapcode-0.0.3/snapcode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 05:53:55.000000 snapcode-0.0.3/snapcode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 05:53:55.000000 snapcode-0.0.3/snapcode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-05 05:53:55.000000 snapcode-0.0.3/snapcode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 05:53:55.000000 snapcode-0.0.3/snapcode.egg-info/top_level.txt
```

### Comparing `snapcode-0.0.2/LICENSE` & `snapcode-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snapcode-0.0.2/PKG-INFO` & `snapcode-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapcode
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extract code blocks from screenshots and images
 Home-page: https://github.com/Vishnunkumar/snapcode/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: codesnap,nlp,cv,transformers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `snapcode-0.0.2/setup.py` & `snapcode-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   'transformers',
   'pytesseract'
 ]
 
 
 setuptools.setup(
     name="snapcode",
-    version="0.0.2",
+    version="0.0.3",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract code blocks from screenshots and images",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/snapcode/',
     packages=[
```

### Comparing `snapcode-0.0.2/snapcode/snapcode.py` & `snapcode-0.0.3/snapcode/snapcode.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 class CodeSnap:
   def __init__(self, image_path):
 
     self.image_path = image_path
   
   def loadmodel(self):
-    
-    tokenizer = AutoTokenizer.from_pretrained("vishnun/codenlbert-sm")
-    model = AutoModelForSequenceClassification.from_pretrained("vishnun/codenlbert-sm")
+
+    model_id = "vishnun/codenlbert-tiny"
+    tokenizer = AutoTokenizer.from_pretrained(model_id)
+    model = AutoModelForSequenceClassification.from_pretrained(model_id)
 
     return tokenizer, model
 
   def retrievecode(self):
 
     ocr_list = [x for x in pytesseract.image_to_string(self.image_path).split("\n") if x != '']
     tokenizer, model = self.loadmodel()
```

### Comparing `snapcode-0.0.2/snapcode.egg-info/PKG-INFO` & `snapcode-0.0.3/snapcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapcode
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extract code blocks from screenshots and images
 Home-page: https://github.com/Vishnunkumar/snapcode/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: codesnap,nlp,cv,transformers
 Classifier: Development Status :: 3 - Alpha
```

