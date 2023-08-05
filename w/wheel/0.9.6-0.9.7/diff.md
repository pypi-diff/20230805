# Comparing `tmp/wheel-0.9.6.tar.gz` & `tmp/wheel-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wheel-0.9.6.tar", last modified: Thu Sep 20 01:47:16 2012, max compression
+gzip compressed data, was "dist/wheel-0.9.7.tar", last modified: Thu Sep 20 15:53:31 2012, max compression
```

## Comparing `wheel-0.9.6.tar` & `wheel-0.9.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      445 2012-09-20 01:47:16.000000 wheel-0.9.6/setup.cfg
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     5438 2012-09-20 01:47:16.000000 wheel-0.9.6/PKG-INFO
--rwxrwxr-x   0 dholth    (1000) dholth    (1000)     1076 2012-09-20 01:47:06.000000 wheel-0.9.6/wheeldemo.sh
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     1570 2012-09-20 01:47:06.000000 wheel-0.9.6/setup.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      186 2012-09-20 01:47:06.000000 wheel-0.9.6/entry_points.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     1456 2012-09-20 01:47:06.000000 wheel-0.9.6/README.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      114 2012-09-20 01:47:06.000000 wheel-0.9.6/MANIFEST.in
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     1120 2012-09-20 01:47:06.000000 wheel-0.9.6/LICENSE.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     2241 2012-09-20 01:47:06.000000 wheel-0.9.6/CHANGES.txt
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)        6 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/top_level.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)       98 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/requires.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)        1 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/not-zip-safe
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      186 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/entry_points.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)        1 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/dependency_links.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      861 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/SOURCES.txt
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     5438 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel.egg-info/PKG-INFO
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/
--rwxrwxr-x   0 dholth    (1000) dholth    (1000)     6147 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/wininst2wheel.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     6232 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/util.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     1225 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/pkginfo.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     3281 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/keys.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)    14473 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/install.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)    25363 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/eggnames.txt
--rwxrwxr-x   0 dholth    (1000) dholth    (1000)     2237 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/egg2wheel.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      541 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/decorator.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)    15401 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/bdist_wheel.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     1559 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/archive.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      403 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/__main__.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)        2 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/__init__.py
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/tool/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     6493 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/tool/__init__.py
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/test/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     2005 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/test/test_wheelfile.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     1676 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/test/test_install.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     3014 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/test/__init__.py
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/test/simple.dist/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      383 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/test/simple.dist/setup.py
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/test/simple.dist/simpledist/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/test/simple.dist/simpledist/__init__.py
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/test/complex.dist/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)      390 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/test/complex.dist/setup.py
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/test/complex.dist/complexdist/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/test/complex.dist/complexdist/__init__.py
-drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 01:47:16.000000 wheel-0.9.6/wheel/signatures/
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     1692 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/signatures/ed25519py.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     6755 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/signatures/djbec.py
--rw-rw-r--   0 dholth    (1000) dholth    (1000)     3191 2012-09-20 01:47:06.000000 wheel-0.9.6/wheel/signatures/__init__.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      445 2012-09-20 15:53:31.000000 wheel-0.9.7/setup.cfg
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     5608 2012-09-20 15:53:31.000000 wheel-0.9.7/PKG-INFO
+-rwxrwxr-x   0 dholth    (1000) dholth    (1000)     1076 2012-09-20 15:53:22.000000 wheel-0.9.7/wheeldemo.sh
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     1570 2012-09-20 15:53:22.000000 wheel-0.9.7/setup.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      186 2012-09-20 15:53:22.000000 wheel-0.9.7/entry_points.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     1456 2012-09-20 15:53:22.000000 wheel-0.9.7/README.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      114 2012-09-20 15:53:22.000000 wheel-0.9.7/MANIFEST.in
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     1120 2012-09-20 15:53:22.000000 wheel-0.9.7/LICENSE.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     2371 2012-09-20 15:53:22.000000 wheel-0.9.7/CHANGES.txt
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)        6 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/top_level.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)       98 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/requires.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)        1 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/not-zip-safe
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      186 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/entry_points.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)        1 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/dependency_links.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      861 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/SOURCES.txt
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     5608 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel.egg-info/PKG-INFO
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/
+-rwxrwxr-x   0 dholth    (1000) dholth    (1000)     6147 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/wininst2wheel.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     6421 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/util.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     1225 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/pkginfo.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     3281 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/keys.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)    14473 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/install.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)    25363 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/eggnames.txt
+-rwxrwxr-x   0 dholth    (1000) dholth    (1000)     2237 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/egg2wheel.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      541 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/decorator.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)    15401 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/bdist_wheel.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     1559 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/archive.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      403 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/__main__.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)        2 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/__init__.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/tool/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     6493 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/tool/__init__.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/test/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     2005 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/test/test_wheelfile.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     1676 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/test/test_install.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     3014 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/test/__init__.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/test/simple.dist/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      383 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/test/simple.dist/setup.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/test/simple.dist/simpledist/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/test/simple.dist/simpledist/__init__.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/test/complex.dist/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)      390 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/test/complex.dist/setup.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/test/complex.dist/complexdist/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/test/complex.dist/complexdist/__init__.py
+drwxrwxr-x   0 dholth    (1000) dholth    (1000)        0 2012-09-20 15:53:31.000000 wheel-0.9.7/wheel/signatures/
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     1692 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/signatures/ed25519py.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     6755 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/signatures/djbec.py
+-rw-rw-r--   0 dholth    (1000) dholth    (1000)     3191 2012-09-20 15:53:22.000000 wheel-0.9.7/wheel/signatures/__init__.py
```

### Comparing `wheel-0.9.6/PKG-INFO` & `wheel-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wheel
-Version: 0.9.6
+Version: 0.9.7
 Summary: A built-package format for Python.
 Home-page: http://bitbucket.org/dholth/wheel/
 Author: Daniel Holth
 Author-email: dholth@fastmail.fm
 License: MIT
 Description: 
         Wheel
@@ -39,14 +39,19 @@
         
         Unlike .egg, wheel will be a fully-documented standard at the binary level
         that is truly easy to install even if you do not want to use the reference
         implementation.
         
         
         
+        0.9.7
+        =====
+        - Only import dirspec when needed. dirspec is only needed to find the
+          configuration for keygen/signing operations.
+        
         0.9.6
         =====
         - requires-dist from setup.cfg overwrites any requirements from setup.py
           Care must be taken that the requirements are the same in both cases,
           or just always install from wheel.
         - drop dirspec requirement on win32
         - improved command line utility, adds 'wheel convert [egg or wininst]' to
```

### Comparing `wheel-0.9.6/wheeldemo.sh` & `wheel-0.9.7/wheeldemo.sh`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/setup.py` & `wheel-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 CHANGES = codecs.open(os.path.join(here, 'CHANGES.txt'), encoding='utf8').read()
 
 tool_reqs = ['keyring']
 if sys.platform != 'win32':
     tool_reqs.append('dirspec')
 
 setup(name='wheel',
-      version='0.9.6',
+      version='0.9.7',
       description='A built-package format for Python.',
       long_description=README + '\n\n' +  CHANGES,
       classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
```

### Comparing `wheel-0.9.6/README.txt` & `wheel-0.9.7/README.txt`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/LICENSE.txt` & `wheel-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/CHANGES.txt` & `wheel-0.9.7/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.9.7
+=====
+- Only import dirspec when needed. dirspec is only needed to find the
+  configuration for keygen/signing operations.
+
 0.9.6
 =====
 - requires-dist from setup.cfg overwrites any requirements from setup.py
   Care must be taken that the requirements are the same in both cases,
   or just always install from wheel.
 - drop dirspec requirement on win32
 - improved command line utility, adds 'wheel convert [egg or wininst]' to
```

### Comparing `wheel-0.9.6/wheel.egg-info/SOURCES.txt` & `wheel-0.9.7/wheel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel.egg-info/PKG-INFO` & `wheel-0.9.7/wheel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wheel
-Version: 0.9.6
+Version: 0.9.7
 Summary: A built-package format for Python.
 Home-page: http://bitbucket.org/dholth/wheel/
 Author: Daniel Holth
 Author-email: dholth@fastmail.fm
 License: MIT
 Description: 
         Wheel
@@ -39,14 +39,19 @@
         
         Unlike .egg, wheel will be a fully-documented standard at the binary level
         that is truly easy to install even if you do not want to use the reference
         implementation.
         
         
         
+        0.9.7
+        =====
+        - Only import dirspec when needed. dirspec is only needed to find the
+          configuration for keygen/signing operations.
+        
         0.9.6
         =====
         - requires-dist from setup.cfg overwrites any requirements from setup.py
           Care must be taken that the requirements are the same in both cases,
           or just always install from wheel.
         - drop dirspec requirement on win32
         - improved command line utility, adds 'wheel convert [egg or wininst]' to
```

### Comparing `wheel-0.9.6/wheel/wininst2wheel.py` & `wheel-0.9.7/wheel/wininst2wheel.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/util.py` & `wheel-0.9.7/wheel/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,8 +203,14 @@
         ids = ["CSIDL_LOCAL_APPDATA", "CSIDL_COMMON_APPDATA"]
         for id in ids:
             base = get_path(id)
             path = os.path.join(base, *resource)
             if os.path.exists(path):
                 yield path
 else:
-    from dirspec.basedir import load_config_paths, save_config_path
+    def save_config_path(*resource):
+        import dirspec.basedir
+        return dirspec.basedir.save_config_path(*resource)
+    def load_config_paths(*resource):
+        import dirspec.basedir
+        return dirspec.basedir.load_config_paths(*resource)
+
```

### Comparing `wheel-0.9.6/wheel/pkginfo.py` & `wheel-0.9.7/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/keys.py` & `wheel-0.9.7/wheel/keys.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/install.py` & `wheel-0.9.7/wheel/install.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/eggnames.txt` & `wheel-0.9.7/wheel/eggnames.txt`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/egg2wheel.py` & `wheel-0.9.7/wheel/egg2wheel.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/decorator.py` & `wheel-0.9.7/wheel/decorator.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/bdist_wheel.py` & `wheel-0.9.7/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/archive.py` & `wheel-0.9.7/wheel/archive.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/tool/__init__.py` & `wheel-0.9.7/wheel/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/test/test_wheelfile.py` & `wheel-0.9.7/wheel/test/test_wheelfile.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/test/test_install.py` & `wheel-0.9.7/wheel/test/test_install.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/test/__init__.py` & `wheel-0.9.7/wheel/test/__init__.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/signatures/ed25519py.py` & `wheel-0.9.7/wheel/signatures/ed25519py.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/signatures/djbec.py` & `wheel-0.9.7/wheel/signatures/djbec.py`

 * *Files identical despite different names*

### Comparing `wheel-0.9.6/wheel/signatures/__init__.py` & `wheel-0.9.7/wheel/signatures/__init__.py`

 * *Files identical despite different names*

