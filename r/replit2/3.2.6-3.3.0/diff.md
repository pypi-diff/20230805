# Comparing `tmp/replit2-3.2.6.tar.gz` & `tmp/replit2-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit2-3.2.6.tar", max compression
+gzip compressed data, was "replit2-3.3.0.tar", max compression
```

## Comparing `replit2-3.2.6.tar` & `replit2-3.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      720 2023-06-30 06:56:03.231081 replit2-3.2.6/LICENSE
--rw-r--r--   0        0        0      675 2023-06-30 08:26:36.601237 replit2-3.2.6/README.md
--rw-r--r--   0        0        0     1280 2023-06-30 09:15:49.673801 replit2-3.2.6/pyproject.toml
--rw-r--r--   0        0        0      410 2023-06-30 06:56:03.247081 replit2-3.2.6/src/replit2/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-30 06:56:03.247081 replit2-3.2.6/src/replit2/__main__.py
--rw-r--r--   0        0        0      171 2023-06-30 06:56:03.247081 replit2-3.2.6/src/replit2/audio/Makefile
--rw-r--r--   0        0        0    13226 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/audio/__init__.py
--rw-r--r--   0        0        0     1848 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/audio/test.py
--rw-r--r--   0        0        0     3687 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/audio/types.py
--rw-r--r--   0        0        0      426 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/database/__init__.py
--rw-r--r--   0        0        0    22058 2023-06-30 09:14:25.629222 replit2-3.2.6/src/replit2/database/database.py
--rw-r--r--   0        0        0      361 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/database/default_db.py
--rw-r--r--   0        0        0     2239 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/database/server.py
--rw-r--r--   0        0        0       33 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/api/__init__.py
--rw-r--r--   0        0        0     5198 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/api/client_pb2.py
--rw-r--r--   0        0        0        0 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/api/features/__init__.py
--rw-r--r--   0        0        0     1516 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/api/features/features_pb2.py
--rw-r--r--   0        0        0        0 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/api/repl/__init__.py
--rw-r--r--   0        0        0     3031 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/api/repl/repl_pb2.py
--rw-r--r--   0        0        0     3563 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/goval/api/signing_pb2.py
--rw-r--r--   0        0        0      135 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/identity/__init__.py
--rw-r--r--   0        0        0      159 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/identity/exceptions.py
--rw-r--r--   0        0        0     9156 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/identity/verify.py
--rw-r--r--   0        0        0     2466 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/info.py
--rw-r--r--   0        0        0      352 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/web/__init__.py
--rw-r--r--   0        0        0     2589 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/web/app.py
--rw-r--r--   0        0        0     3329 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/web/user.py
--rw-r--r--   0        0        0     8552 2023-06-30 06:56:03.251081 replit2-3.2.6/src/replit2/web/utils.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 replit2-3.2.6/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-30 06:56:03.231081 replit2-3.3.0/LICENSE
+-rw-r--r--   0        0        0      675 2023-06-30 08:26:36.601237 replit2-3.3.0/README.md
+-rw-r--r--   0        0        0     1280 2023-08-05 06:43:14.694110 replit2-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0      410 2023-06-30 06:56:03.247081 replit2-3.3.0/src/replit2/__init__.py
+-rw-r--r--   0        0        0     2868 2023-06-30 06:56:03.247081 replit2-3.3.0/src/replit2/__main__.py
+-rw-r--r--   0        0        0      171 2023-06-30 06:56:03.247081 replit2-3.3.0/src/replit2/audio/Makefile
+-rw-r--r--   0        0        0    13226 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/audio/__init__.py
+-rw-r--r--   0        0        0     1848 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/audio/test.py
+-rw-r--r--   0        0        0     3687 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/audio/types.py
+-rw-r--r--   0        0        0      426 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/database/__init__.py
+-rw-r--r--   0        0        0    22052 2023-08-05 06:40:22.688885 replit2-3.3.0/src/replit2/database/database.py
+-rw-r--r--   0        0        0      361 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/database/default_db.py
+-rw-r--r--   0        0        0     2239 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/database/server.py
+-rw-r--r--   0        0        0       33 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/api/__init__.py
+-rw-r--r--   0        0        0     5198 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/api/client_pb2.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/api/features/__init__.py
+-rw-r--r--   0        0        0     1516 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/api/features/features_pb2.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/api/repl/__init__.py
+-rw-r--r--   0        0        0     3031 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/api/repl/repl_pb2.py
+-rw-r--r--   0        0        0     3563 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/goval/api/signing_pb2.py
+-rw-r--r--   0        0        0      135 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/identity/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/identity/exceptions.py
+-rw-r--r--   0        0        0     9156 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/identity/verify.py
+-rw-r--r--   0        0        0     2466 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/info.py
+-rw-r--r--   0        0        0      352 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/web/__init__.py
+-rw-r--r--   0        0        0     2589 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/web/app.py
+-rw-r--r--   0        0        0     3329 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/web/user.py
+-rw-r--r--   0        0        0     8552 2023-06-30 06:56:03.251081 replit2-3.3.0/src/replit2/web/utils.py
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 replit2-3.3.0/PKG-INFO
```

### Comparing `replit2-3.2.6/LICENSE` & `replit2-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/README.md` & `replit2-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/pyproject.toml` & `replit2-3.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit2"
-version = "3.2.6"
+version = "3.3.0"
 description = "A library for interacting with features of repl.it"
 authors = ["Repl.it <contact@repl.it>", "mat <pypi@matdoes.dev>", "kennethreitz <me@kennethreitz.org>", "Scoder12 <pypi@scoder12.ml>", "AllAwesome497", "python660", ]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/py660/repl.it"
 homepage = "https://github.com/py660/repl.it"
 documentation = "https://replit-py.readthedocs.org/"
```

### Comparing `replit2-3.2.6/src/replit2/__main__.py` & `replit2-3.3.0/src/replit2/__main__.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/audio/__init__.py` & `replit2-3.3.0/src/replit2/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/audio/test.py` & `replit2-3.3.0/src/replit2/audio/test.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/audio/types.py` & `replit2-3.3.0/src/replit2/audio/types.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/database/database.py` & `replit2-3.3.0/src/replit2/database/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 class AsyncDatabase:
     """Async interface for Repl.it Database."""
 
     __slots__ = ("backup_loc", "backup_mode", "db_url", "sess")
 
-    def __init__(self, db_url: str, backup: str=".config/db_backup.json", backup_mode: int=-1) -> None:
+    def __init__(self, db_url: str, backup: str="db_backup.json", backup_mode: int=-1) -> None:
         """Initialize database. You shouldn't have to do this manually.
 
         Args:
             db_url      (str): Database url to use.
             backup      (str): Location of DB backups.
             backup_mode (int): DB backup mode (-1 to disable, 0 for on_modify).
         """
@@ -444,17 +444,17 @@
 class Database(abc.MutableMapping):
     """Dictionary-like interface for Repl.it Database.
 
     This interface will coerce all values everything to and from JSON. If you
     don't want this, use AsyncDatabase instead.
     """
 
-    __slots__ = ("backup_loc", "backup_mode", "db_url", "sess")
+    __slots__ = ("backup_loc", "backup_mode", "db_url", "sess", "backup_thread")
 
-    def __init__(self, db_url: str, backup: str=".config/db_backup.json", backup_mode: int=-1) -> None:
+    def __init__(self, db_url: str, backup: str="db_backup.json", backup_mode: int=-1) -> None:
         """Initialize database. You shouldn't have to do this manually.
 
         Args:
             db_url      (str): Database url to use.
             backup      (str): Location of DB backups.
             backup_mode (int): DB backup mode (-1 to disable, 0 for on_modify, n [positive integer] for recurring backup every n seconds).
         """
@@ -652,15 +652,15 @@
             None: None
         """
         ret = {}
         keys = self.keys()
         for i in keys:
             ret[i] = self.get_raw(i)
   
-        print("ret:", ret)
+        #print("ret:", ret)
         with open(self.backup_loc, 'w') as fout:
             json.dump(ret, fout)
 
     def load_backup(self, location: str="") -> None:
         """Overwrites the current DB with the data stored in the specified file
         
         Returns:
@@ -688,14 +688,14 @@
         self.sess.close()
 
 
 class DatabaseStarter():
     def __init__(self, db_url: str=""):
         self.db_url = db_url
 
-    def start(self, backup: str=".config/db_backup.json", backup_mode: int=-1, warn=True):
+    def start(self, backup: str="db_backup.json", backup_mode: int=-1, warn=True):
         if self.db_url:
             return Database(db_url=self.db_url, backup=backup, backup_mode=backup_mode)
         else:
             if warn:
                 print("Replit DB is currently running in ephemeral mode, and will not save upon exiting.")
             return dict()
```

### Comparing `replit2-3.2.6/src/replit2/database/server.py` & `replit2-3.3.0/src/replit2/database/server.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/goval/api/client_pb2.py` & `replit2-3.3.0/src/replit2/goval/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/goval/api/features/features_pb2.py` & `replit2-3.3.0/src/replit2/goval/api/features/features_pb2.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/goval/api/repl/repl_pb2.py` & `replit2-3.3.0/src/replit2/goval/api/repl/repl_pb2.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/goval/api/signing_pb2.py` & `replit2-3.3.0/src/replit2/goval/api/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/identity/verify.py` & `replit2-3.3.0/src/replit2/identity/verify.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/info.py` & `replit2-3.3.0/src/replit2/info.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/web/app.py` & `replit2-3.3.0/src/replit2/web/app.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/web/user.py` & `replit2-3.3.0/src/replit2/web/user.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/src/replit2/web/utils.py` & `replit2-3.3.0/src/replit2/web/utils.py`

 * *Files identical despite different names*

### Comparing `replit2-3.2.6/PKG-INFO` & `replit2-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit2
-Version: 3.2.6
+Version: 3.3.0
 Summary: A library for interacting with features of repl.it
 Home-page: https://github.com/py660/repl.it
 License: ISC
 Author: Repl.it
 Author-email: contact@repl.it
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
```

