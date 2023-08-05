# Comparing `tmp/bforce-0.3.tar.gz` & `tmp/bforce-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bforce-0.3.tar", last modified: Wed Aug  2 08:28:19 2023, max compression
+gzip compressed data, was "bforce-0.4.tar", last modified: Sat Aug  5 08:52:18 2023, max compression
```

## Comparing `bforce-0.3.tar` & `bforce-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-02 08:28:19.538977 bforce-0.3/
--rw-r--r--   0 voidful    (501) staff       (20)      129 2023-08-02 08:28:19.537990 bforce-0.3/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)     1738 2023-07-30 22:15:47.000000 bforce-0.3/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-02 08:28:19.531785 bforce-0.3/bforce/
--rw-r--r--   0 voidful    (501) staff       (20)       19 2023-07-30 22:03:29.000000 bforce-0.3/bforce/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)       44 2023-07-30 21:58:35.000000 bforce-0.3/bforce/exceptions.py
--rw-r--r--   0 voidful    (501) staff       (20)     3716 2023-08-02 08:26:32.000000 bforce-0.3/bforce/main.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-02 08:28:19.537459 bforce-0.3/bforce.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)      129 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      193 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)        7 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/top_level.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-08-02 08:28:19.539127 bforce-0.3/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)      122 2023-08-02 08:26:46.000000 bforce-0.3/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-05 08:52:18.732628 bforce-0.4/
+-rw-r--r--   0 voidful    (501) staff       (20)      129 2023-08-05 08:52:18.731980 bforce-0.4/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)     1738 2023-07-30 22:15:47.000000 bforce-0.4/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-05 08:52:18.724688 bforce-0.4/bforce/
+-rw-r--r--   0 voidful    (501) staff       (20)       19 2023-07-30 22:03:29.000000 bforce-0.4/bforce/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)       44 2023-07-30 21:58:35.000000 bforce-0.4/bforce/exceptions.py
+-rw-r--r--   0 voidful    (501) staff       (20)     3233 2023-08-05 08:49:59.000000 bforce-0.4/bforce/main.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-05 08:52:18.731088 bforce-0.4/bforce.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)      129 2023-08-05 08:52:18.000000 bforce-0.4/bforce.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      193 2023-08-05 08:52:18.000000 bforce-0.4/bforce.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2023-08-05 08:52:18.000000 bforce-0.4/bforce.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        7 2023-08-05 08:52:18.000000 bforce-0.4/bforce.egg-info/top_level.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2023-08-05 08:52:18.732731 bforce-0.4/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)      122 2023-08-05 08:51:04.000000 bforce-0.4/setup.py
```

### Comparing `bforce-0.3/README.md` & `bforce-0.4/README.md`

 * *Files identical despite different names*

### Comparing `bforce-0.3/bforce/main.py` & `bforce-0.4/bforce/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import json
-import os
 import pickle
 import threading
-import uuid
+import os
+import atexit
 from functools import wraps
-
+import hashlib
+import json
 from .exceptions import TimeoutException
 
 
 def timeout_retries(seconds, max_retries=3):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
@@ -39,72 +39,59 @@
             raise TimeoutException(f"Function {func.__name__} exceeded maximum retries")
 
         return wrapper
 
     return decorator
 
 
-def clear_cache(cache_dir="cache"):
-    if os.path.exists(cache_dir):
-        for filename in os.listdir(cache_dir):
-            file_path = os.path.join(cache_dir, filename)
-            os.remove(file_path)
-
+def make_cache_key(func, args, kwargs):
+    func_name = pickle.dumps(func.__name__)
+    args_data = pickle.dumps(args)
+    kwargs_data = pickle.dumps(kwargs)
+    key = func_name + args_data + kwargs_data
+    return hashlib.sha256(key).hexdigest()
+
+class CacheResult:
+    def __init__(self, cache_dir="cache"):
+        self.cache_dir = cache_dir
+        if not os.path.exists(cache_dir):
+            os.makedirs(cache_dir)
+        self.cache = self.load_cache(cache_dir)
+        atexit.register(self.save_all)  # Save cache when program exits
 
-def save_cache(cache_key, cache_value, cache_dir="cache"):
-    if not os.path.exists(cache_dir):
-        os.makedirs(cache_dir)
-    try:
-        file_path = os.path.join(cache_dir, f"{uuid.uuid4().hex}.json")
-        with open(file_path, "w") as f:
-            json.dump((cache_key, cache_value), f)
-    except TypeError:  # If data is not JSON serializable, use pickle
-        file_path = os.path.join(cache_dir, f"{uuid.uuid4().hex}.pkl")
-        with open(file_path, "wb") as f:
-            pickle.dump((cache_key, cache_value), f)
-    return file_path
-
-
-def load_cache(cache_dir="cache"):
-    if not os.path.exists(cache_dir):
-        return {}
-    cache = {}
-    for filename in os.listdir(cache_dir):
-        file_path = os.path.join(cache_dir, filename)
+    def save_cache(self, cache_key, cache_value):
         try:
+            self.cache[cache_key] = dict(cache_value)
+        except TypeError:  # If data is not serializable
+            self.cache[cache_key] = cache_value
+
+    def save_all(self):
+        for cache_key, cache_value in self.cache.items():
+            file_path = os.path.join(self.cache_dir, f"{cache_key}.json")
+            with open(file_path, "w") as f:
+                json.dump(cache_value, f)
+
+    def load_cache(self, cache_dir):
+        if not os.path.exists(cache_dir):
+            return {}
+        cache = {}
+        for filename in os.listdir(cache_dir):
+            file_path = os.path.join(cache_dir, filename)
             if filename.endswith('.json'):
                 with open(file_path, "r") as f:
-                    cache_key, cache_value = json.load(f)
-            elif filename.endswith('.pkl'):
-                with open(file_path, "rb") as f:
-                    cache_key, cache_value = pickle.load(f)
-            else:
-                continue
-            cache[cache_key] = cache_value
-        except (json.JSONDecodeError, ValueError, pickle.UnpicklingError) as e:
-            print(f"Error in file: {file_path}. Skipping this file.")
-            print(f"Error message: {e}")
-            with open(file_path, "r") as f:
-                print(f"Content: {f.read()}")
-    return cache
-
+                    cache_value = json.load(f)
+                cache_key = filename.split(".")[0]  # Remove the extension
+                cache[cache_key] = cache_value
+        return cache
 
-def cache_result(cache_dir="cache"):
-    def decorator(func):
+    def __call__(self, func):
         @wraps(func)
         def wrapper(*args, **kwargs):
-            # Load cache
-            cache = load_cache(cache_dir)
-            # Create a key based on function name and arguments
-            cache_key = f"{func.__name__}_{args}_{kwargs}"
-            if cache_key in cache:
-                # print(f"Loaded result from cache for function: {func.__name__} with args: {args} and kwargs: {kwargs}")
-                return cache[cache_key]
+            cache_key = make_cache_key(func, args, kwargs)
+            if cache_key in self.cache:
+                return self.cache[cache_key]
             else:
                 result = func(*args, **kwargs)
-                # Save result to cache
-                save_cache(cache_key, result, cache_dir)
+                self.save_cache(cache_key, result)
                 return result
 
-        return wrapper
-
-    return decorator
+        return wrapper
```

