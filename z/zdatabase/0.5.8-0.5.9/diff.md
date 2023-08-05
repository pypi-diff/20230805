# Comparing `tmp/zdatabase-0.5.8.tar.gz` & `tmp/zdatabase-0.5.9.tar.gz`

## Comparing `zdatabase-0.5.8.tar` & `zdatabase-0.5.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.8/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 zdatabase-0.5.8/src/zdatabase/model.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 zdatabase-0.5.8/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.8/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.8/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.9/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 zdatabase-0.5.9/src/zdatabase/model.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 zdatabase-0.5.9/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.9/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.9/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.5.9/PKG-INFO
```

### Comparing `zdatabase-0.5.8/src/zdatabase/__init__.py` & `zdatabase-0.5.9/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.8/src/zdatabase/model.py` & `zdatabase-0.5.9/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.8/src/zdatabase/utility.py` & `zdatabase-0.5.9/src/zdatabase/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,25 +91,25 @@
     def add_(cls, data):
         obj = cls.new(data)
         obj.add_one()
         return obj
 
     @classmethod
     def add(cls, data, sync=True):
-        if hasattr(cls, 'schema'):
-            validate(instance=data, schema=cls.schema)
+        if hasattr(cls, '__schema__'):
+            validate(instance=data, schema=cls.__schema__)
         obj = cls.add_(data)
         if sync:
             cls.commit()
         return obj
 
     @classmethod
     def save(cls, primary_key, data):
-        if hasattr(cls, 'schema'):
-            validate(instance=data, schema=cls.schema)
+        if hasattr(cls, '__schema__'):
+            validate(instance=data, schema=cls.__schema__)
         obj = cls.get(primary_key)
         obj.update(data)
         cls.commit()
 
     @classmethod
     def get(cls, primary_key):
         return cls.query.get(primary_key)
```

### Comparing `zdatabase-0.5.8/LICENSE` & `zdatabase-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.8/pyproject.toml` & `zdatabase-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.5.8/PKG-INFO` & `zdatabase-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.5.8
+Version: 0.5.9
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

