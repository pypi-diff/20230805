# Comparing `tmp/PySiglent_SSA3000x-0.2.tar.gz` & `tmp/PySiglent_SSA3000x-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySiglent_SSA3000x-0.2.tar", last modified: Sat Jul  1 16:47:32 2023, max compression
+gzip compressed data, was "PySiglent_SSA3000x-0.3.tar", last modified: Sat Aug  5 12:59:51 2023, max compression
```

## Comparing `PySiglent_SSA3000x-0.2.tar` & `PySiglent_SSA3000x-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 16:47:31.986064 PySiglent_SSA3000x-0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.2/LICENSE
--rw-rw-rw-   0        0        0      413 2023-07-01 16:47:31.984063 PySiglent_SSA3000x-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-01 16:47:31.943064 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/
--rw-rw-rw-   0        0        0    26168 2023-07-01 16:45:44.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/PySiglent_SSA3000x.py
--rw-rw-rw-   0        0        0       54 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:47:31.978065 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/
--rw-rw-rw-   0        0        0      413 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 16:47:31.987065 PySiglent_SSA3000x-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-06-25 20:19:33.000000 PySiglent_SSA3000x-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:59:51.276339 PySiglent_SSA3000x-0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.3/LICENSE
+-rw-rw-rw-   0        0        0      413 2023-08-05 12:59:51.276339 PySiglent_SSA3000x-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 12:59:51.266784 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/
+-rw-rw-rw-   0        0        0    26295 2023-08-05 12:59:14.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/PySiglent_SSA3000x.py
+-rw-rw-rw-   0        0        0       54 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:59:51.274307 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/
+-rw-rw-rw-   0        0        0      413 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-05 12:59:51.000000 PySiglent_SSA3000x-0.3/PySiglent_SSA3000x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 12:59:51.277346 PySiglent_SSA3000x-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-06-25 20:19:33.000000 PySiglent_SSA3000x-0.3/setup.py
```

### Comparing `PySiglent_SSA3000x-0.2/LICENSE` & `PySiglent_SSA3000x-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/PySiglent_SSA3000x.py` & `PySiglent_SSA3000x-0.3/PySiglent_SSA3000x/PySiglent_SSA3000x.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,23 +264,26 @@
             raise self.Exceptions.ConnectionError
 
     def close(self):
         """close connection"""
         self.interface.close()
 
     def _set_get(self, cmd: str, val=None):
-        if val is None:
-            cmd += '?'
-            val = self.query(cmd)
-            print(f'response ->{val}')
-            return val
+        if self.connected:
+            if val is None:
+                cmd += '?'
+                val = self.query(cmd)
+                print(f'response ->{val}')
+                return val
+            else:
+                cmd += f' {val}'
+                self.write(cmd)
+                return val
         else:
-            cmd += f' {val}'
-            self.write(cmd)
-            return val
+            raise self.Exceptions.NotConnected
     
     def _string_to_bool(val:str):
         if val in ('1', 'ON'):
             return True
         return False
     
     # custom fuinctions ---------------
```

### Comparing `PySiglent_SSA3000x-0.2/setup.py` & `PySiglent_SSA3000x-0.3/setup.py`

 * *Files identical despite different names*

