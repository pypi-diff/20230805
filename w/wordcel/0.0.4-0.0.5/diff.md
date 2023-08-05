# Comparing `tmp/wordcel-0.0.4.tar.gz` & `tmp/wordcel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordcel-0.0.4.tar", max compression
+gzip compressed data, was "wordcel-0.0.5.tar", max compression
```

## Comparing `wordcel-0.0.4.tar` & `wordcel-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-25 01:08:30.881980 wordcel-0.0.4/LICENSE
--rw-r--r--   0        0        0     2783 2023-07-25 21:14:13.262827 wordcel-0.0.4/README.md
--rw-r--r--   0        0        0      333 2023-08-01 23:21:25.768810 wordcel-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 00:46:00.681902 wordcel-0.0.4/wordcel/__init__.py
--rw-r--r--   0        0        0     2537 2023-08-01 23:21:15.363512 wordcel-0.0.4/wordcel/featurize.py
--rw-r--r--   0        0        0     1042 2023-07-25 00:48:13.299968 wordcel-0.0.4/wordcel/llm_providers.py
--rw-r--r--   0        0        0     3603 1970-01-01 00:00:00.000000 wordcel-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-25 01:08:30.881980 wordcel-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2783 2023-07-25 21:14:13.262827 wordcel-0.0.5/README.md
+-rw-r--r--   0        0        0      333 2023-08-04 23:08:27.219262 wordcel-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 00:46:00.681902 wordcel-0.0.5/wordcel/__init__.py
+-rw-r--r--   0        0        0     2407 2023-08-04 23:13:05.610363 wordcel-0.0.5/wordcel/featurize.py
+-rw-r--r--   0        0        0     1042 2023-07-25 00:48:13.299968 wordcel-0.0.5/wordcel/llm_providers.py
+-rw-r--r--   0        0        0     3603 1970-01-01 00:00:00.000000 wordcel-0.0.5/PKG-INFO
```

### Comparing `wordcel-0.0.4/LICENSE` & `wordcel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.4/README.md` & `wordcel-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.4/wordcel/featurize.py` & `wordcel-0.0.5/wordcel/featurize.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,23 +31,21 @@
 
     if cache_folder and not os.path.exists(cache_folder):
         os.makedirs(cache_folder)
 
     if id_column is None:
         id_column = df.index.name if df.index.name else "index"
 
-    # Hash the user function. This is used to generate a unique identifier
-    # for each cached file, and avoid collisions.
-    hashed_user_fn = str(hash(user_function))
+    user_fn_name = user_function.__name__ 
 
     def process_text_with_caching(text, identifier):
         if cache_folder:
             # Check if result is already cached
             identifier = str(identifier).replace("/", "_")
-            cache_file = os.path.join(cache_folder, f"{identifier}_{hashed_user_fn}.json")
+            cache_file = os.path.join(cache_folder, f"{identifier}_{user_fn_name}.json")
             if os.path.exists(cache_file):
                 with open(cache_file, "r") as f:
                     return json.load(f)
 
         result = user_function(text)
 
         if cache_folder:
```

### Comparing `wordcel-0.0.4/wordcel/llm_providers.py` & `wordcel-0.0.5/wordcel/llm_providers.py`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.4/PKG-INFO` & `wordcel-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordcel
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create text-based features from large language models
 Author: Andrew Han
 Author-email: handrew11@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

