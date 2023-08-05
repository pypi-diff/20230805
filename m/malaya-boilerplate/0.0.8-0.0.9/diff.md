# Comparing `tmp/malaya-boilerplate-0.0.8.tar.gz` & `tmp/malaya-boilerplate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/malaya-boilerplate/malaya-boilerplate/dist/tmpfj0gx5j0/malaya-boilerplate-0.0.8.tar", last modified: Sat Jul 10 06:33:53 2021, max compression
+gzip compressed data, was "/home/runner/work/malaya-boilerplate/malaya-boilerplate/dist/tmpty04ma4v/malaya-boilerplate-0.0.9.tar", last modified: Wed Jul 14 16:12:56 2021, max compression
```

## Comparing `malaya-boilerplate-0.0.8.tar` & `malaya-boilerplate-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      655 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3426 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/malaya_boilerplate/
--rw-r--r--   0 runner    (1001) docker     (116)      134 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/malaya_boilerplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7599 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/malaya_boilerplate/backblaze.py
--rw-r--r--   0 runner    (1001) docker     (116)    12124 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/malaya_boilerplate/frozen_graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     7388 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/malaya_boilerplate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/malaya_boilerplate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      655 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/malaya_boilerplate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      376 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/malaya_boilerplate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/malaya_boilerplate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/malaya_boilerplate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/malaya_boilerplate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-07-10 06:33:53.000000 malaya-boilerplate-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      980 2021-07-10 06:33:46.000000 malaya-boilerplate-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1072 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      655 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3426 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/malaya_boilerplate/
+-rw-r--r--   0 runner    (1001) docker     (116)      134 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/malaya_boilerplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7649 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/malaya_boilerplate/backblaze.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12124 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/malaya_boilerplate/frozen_graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7388 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/malaya_boilerplate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/malaya_boilerplate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      655 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/malaya_boilerplate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      376 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/malaya_boilerplate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/malaya_boilerplate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/malaya_boilerplate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/malaya_boilerplate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       68 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-07-14 16:12:56.000000 malaya-boilerplate-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      980 2021-07-14 16:12:49.000000 malaya-boilerplate-0.0.9/setup.py
```

### Comparing `malaya-boilerplate-0.0.8/LICENSE` & `malaya-boilerplate-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `malaya-boilerplate-0.0.8/PKG-INFO` & `malaya-boilerplate-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malaya-boilerplate
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tensorflow freeze graph optimization and boilerplates to share among Malaya projects.
 Home-page: https://github.com/huseinzol05/malaya-boilerplate
 Author: huseinzol05
 Author-email: husein.zol05@gmail.com
 License: MIT
 Download-URL: https://github.com/huseinzol05/malaya-boilerplate/archive/master.zip
 Keywords: nlp,bm
```

### Comparing `malaya-boilerplate-0.0.8/README.md` & `malaya-boilerplate-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `malaya-boilerplate-0.0.8/malaya_boilerplate/backblaze.py` & `malaya-boilerplate-0.0.9/malaya_boilerplate/backblaze.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 ):
     model = path
     keys = keys.copy()
     keys['version'] = 'version'
 
     if quantized:
         path = os.path.join(module, f'{path}-quantized')
-        quantized_path = os.path.join(path, 'model.pb')
+        quantized_path = os.path.join(path, 'model.pb').replace('\\', '/')
         if not check_file_cloud(quantized_path)[0]:
             raise Exception(
                 f'Quantized model for `{os.path.join(module, model)}` is not available, please load normal model.'
             )
         logging.warning('Load quantized model will cause accuracy drop.')
     else:
         path = os.path.join(module, path)
@@ -122,36 +122,38 @@
     for key, value in keys.items():
         if '/' in value:
             f_local = os.path.join(path_local, value.split('/')[-1])
             f_cloud = value
         else:
             f_local = os.path.join(path_local, value)
             f_cloud = os.path.join(path, value)
+            f_cloud = f_cloud.replace('\\', '/')
         files_local[key] = f_local
         files_cloud[key] = f_cloud
     if validate:
         download = False
         version = files_local['version']
         latest = str(
             max(
                 [check_file_cloud(item)[1] for key, item in files_cloud.items()]
             )
         )
         if os.path.isfile(version):
             with open(version) as fopen:
-                if latest not in fopen.read():
-                    p = os.path.dirname(version)
-                    print(f'Found old version in {p}, deleting..')
-                    _delete_folder(p)
-                    download = True
-                else:
-                    for key, item in files_local.items():
-                        if not os.path.exists(item):
-                            download = True
-                            break
+                v = fopen.read()
+            if latest not in v:
+                p = os.path.dirname(version)
+                print(f'Found old version in {p}, deleting..')
+                _delete_folder(p)
+                download = True
+            else:
+                for key, item in files_local.items():
+                    if not os.path.exists(item):
+                        download = True
+                        break
         else:
             download = True
 
         if download:
             versions = []
             for key, item in files_local.items():
                 if 'version' in key:
```

### Comparing `malaya-boilerplate-0.0.8/malaya_boilerplate/frozen_graph.py` & `malaya-boilerplate-0.0.9/malaya_boilerplate/frozen_graph.py`

 * *Files identical despite different names*

### Comparing `malaya-boilerplate-0.0.8/malaya_boilerplate/utils.py` & `malaya-boilerplate-0.0.9/malaya_boilerplate/utils.py`

 * *Files identical despite different names*

### Comparing `malaya-boilerplate-0.0.8/malaya_boilerplate.egg-info/PKG-INFO` & `malaya-boilerplate-0.0.9/malaya_boilerplate.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malaya-boilerplate
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tensorflow freeze graph optimization and boilerplates to share among Malaya projects.
 Home-page: https://github.com/huseinzol05/malaya-boilerplate
 Author: huseinzol05
 Author-email: husein.zol05@gmail.com
 License: MIT
 Download-URL: https://github.com/huseinzol05/malaya-boilerplate/archive/master.zip
 Keywords: nlp,bm
```

### Comparing `malaya-boilerplate-0.0.8/setup.py` & `malaya-boilerplate-0.0.9/setup.py`

 * *Files identical despite different names*

