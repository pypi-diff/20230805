# Comparing `tmp/pyvlc-1.0.0.tar.gz` & `tmp/pyvlc-1.0.1.tar.gz`

## Comparing `pyvlc-1.0.0.tar` & `pyvlc-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyvlc-1.0.0/src/PyVLC/__init__.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyvlc-1.0.0/src/PyVLC/pyvlc.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyvlc-1.0.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyvlc-1.0.0/LICENSE
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pyvlc-1.0.0/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pyvlc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pyvlc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyvlc-1.0.1/src/PyVLC/PyVLC.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyvlc-1.0.1/src/PyVLC/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyvlc-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyvlc-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pyvlc-1.0.1/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pyvlc-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 pyvlc-1.0.1/PKG-INFO
```

### Comparing `pyvlc-1.0.0/src/PyVLC/pyvlc.py` & `pyvlc-1.0.1/src/PyVLC/PyVLC.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import telnetlib3
 import asyncio
 from getpass import getpass
 
-class pyvlc:
+class PyVLC:
     def __init__(self, host="localhost", port=4212):
         self.host = host
         self.port = port
         self.buffer = ""
 
     async def connect(self):
         try:
```

### Comparing `pyvlc-1.0.0/LICENSE` & `pyvlc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvlc-1.0.0/pyproject.toml` & `pyvlc-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","telnetlib3","asyncio"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyVLC"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Harshit Bhardwaj", email="htg4920@gmail.com" },
 ]
 description = "A python package that utilizes telnetlib3 and asyncio to communicate with VLC Media Player"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

