# Comparing `tmp/unigui-1.9.8.tar.gz` & `tmp/unigui-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.8.tar", last modified: Mon Jul 31 08:24:20 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.9.tar", last modified: Thu Aug  3 18:47:43 2023, max compression
```

## Comparing `unigui-1.9.8.tar` & `unigui-1.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     5345 2023-07-31 07:12:00.000000 unigui-1.9.8/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.8/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)     4181 2023-07-28 17:59:21.000000 unigui-1.9.8/unigui/tables.py
--rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.8/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     7796 2023-07-29 16:08:30.000000 unigui-1.9.8/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2669 2023-07-31 07:45:36.000000 unigui-1.9.8/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.8/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.8/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)     2691 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/css/435.30396533.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/css/vendor.f747ec02.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    50532 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/435.ced6eca8.js
--rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/app.353e1981.js
--rw-rw-r--   0 george    (1000) george    (1000)  1445576 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/vendor.8cb03aaa.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.8/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-31 08:24:03.000000 unigui-1.9.8/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    18773 2023-07-31 08:24:20.000000 unigui-1.9.8/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-31 08:24:20.000000 unigui-1.9.8/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18468 2023-07-30 04:54:06.000000 unigui-1.9.8/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.8/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    18773 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.8/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5345 2023-07-31 07:12:00.000000 unigui-1.9.9/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.9/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4181 2023-07-28 17:59:21.000000 unigui-1.9.9/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.9/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7796 2023-07-29 16:08:30.000000 unigui-1.9.9/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2669 2023-07-31 07:45:36.000000 unigui-1.9.9/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.9/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8755 2023-08-03 14:56:50.000000 unigui-1.9.9/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/css/vendor.f747ec02.css
+-rw-rw-r--   0 george    (1000) george    (1000)     2691 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/css/768.30396533.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    50573 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/768.89ad69c0.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1445576 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/vendor.8cb03aaa.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/app.c32942a4.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.9/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      642 2023-08-03 18:47:28.000000 unigui-1.9.9/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18773 2023-08-03 18:47:43.000000 unigui-1.9.9/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-08-03 18:47:43.000000 unigui-1.9.9/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18468 2023-07-30 04:54:06.000000 unigui-1.9.9/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.9/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       63 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18773 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.9/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.8/unigui/guielements.py` & `unigui-1.9.9/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/server.py` & `unigui-1.9.9/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/tables.py` & `unigui-1.9.9/unigui/tables.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/autotest.py` & `unigui-1.9.9/unigui/autotest.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/utils.py` & `unigui-1.9.9/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/reloader.py` & `unigui-1.9.9/unigui/reloader.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/users.py` & `unigui-1.9.9/unigui/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     def load_screen(self, file):
         screen_vars = {
             'icon' : None,
             'prepare' : None,            
             'blocks' : [],
             'header' : config.appname,                        
             'toolbar' : [], 
-            'order' : 0
+            'order' : 0,
+            'reload': config.hot_reload 
         }             
         name = file[:-3]        
         path = f'{screens_dir}{divpath}{file}'                
         spec = importlib.util.spec_from_file_location(name,path)
         module = importlib.util.module_from_spec(spec)        
                 
         module.user = self
```

### Comparing `unigui-1.9.8/unigui/web/favicon.ico` & `unigui-1.9.9/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/css/435.30396533.css` & `unigui-1.9.9/unigui/web/css/768.30396533.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/css/vendor.f747ec02.css` & `unigui-1.9.9/unigui/web/css/vendor.f747ec02.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.9/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.9/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.9/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.9/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.9/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.9/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/js/430.591e9a73.js` & `unigui-1.9.9/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/js/435.ced6eca8.js` & `unigui-1.9.9/unigui/web/js/768.89ad69c0.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [435], {
-        3435: (e, t, a) => {
+    [768], {
+        9768: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => sa
             });
             var s = a(3673),
                 l = a(2323);
             const i = (0, s._)("div", {
                     class: "q-pa-md"
@@ -236,15 +236,15 @@
             function E(e = !1) {
                 for (let t of Object.values(k))
                     if (t.expanding && (!e || f.includes(t.type))) {
                         t.has_recalc = !0;
                         let e = t.$el;
                         if (e.getBoundingClientRect) {
                             let e = t.$el.getBoundingClientRect();
-                            window.innerHeight < e.top + e.height && (t.styleSize = "")
+                            window.innerHeight < e.top + e.height && (t.styleSize = null)
                         }
                     }(0, s.Y3)((() => {
                         requestAnimationFrame((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
                                     K(document.documentElement.scrollWidth > window.innerWidth)
                                 }))
@@ -278,15 +278,15 @@
                         } else if (e.name == t.data.name) {
                         d = t;
                         break
                     }
                     let p = n;
                     p /= o;
                     let m = e || f.includes(t.type) || t.has_recalc,
-                        g = m ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
+                        g = m && !t.only_fixed_elems ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
                         y = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
                     y < 0 && (y = 20);
                     let w = `height: ${y+l}px; ${g}`;
                     w != t.styleSize && (t.styleSize = w), t.has_recalc = !1
                 }
             }
 
@@ -501,15 +501,15 @@
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
             const ee = {
-                    class: "row"
+                    class: "row no-wrap"
                 },
                 te = ["data", "pdata"],
                 ae = {
                     key: 0,
                     class: "row"
                 },
                 se = ["data", "pdata"],
@@ -521,15 +521,15 @@
             function ie(e, t, a, i, n, o) {
                 const d = (0, s.up)("element"),
                     r = (0, s.up)("q-icon"),
                     c = (0, s.up)("q-scroll-area"),
                     h = (0, s.up)("q-card");
                 return (0, s.wg)(), (0, s.j4)(h, {
                     class: "my-card q-ma-xs",
-                    style: (0, l.j5)(e.only_fixed_elems ? e.styleSize : "")
+                    style: (0, l.j5)(e.only_fixed_elems ? e.styleSize : null)
                 }, {
                     default: (0, s.w5)((() => [(0, s._)("div", ee, [e.data.logo ? ((0, s.wg)(), (0, s.j4)(d, {
                         key: 0,
                         class: "q-ma-sm",
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, s.wg)(), (0, s.j4)(r, {
@@ -2147,15 +2147,15 @@
                 name: "block",
                 components: {
                     element: St
                 },
                 data() {
                     return {
                         Dark: je.Z,
-                        styleSize: "",
+                        styleSize: null,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
                         },
@@ -2231,15 +2231,15 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = h.visibility ? S(this) : "", k[this.fullname] = this)
+                        g && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = A ? S(this) : null, k[this.fullname] = this)
                     }
                 }
             });
             var Zt = a(151);
             const $t = (0, U.Z)(zt, [
                     ["render", ie]
                 ]),
@@ -2490,15 +2490,15 @@
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if ("screen" == e.type) z(), this.screen.name != e.name && (D(!1), g || this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
+                        if ("screen" == e.type) z(), this.screen.name != e.name ? (D(!1), g || this.visible(!1)) : e.reload && D(!1), this.screen = e, this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
```

### Comparing `unigui-1.9.8/unigui/web/js/app.353e1981.js` & `unigui-1.9.9/unigui/web/js/app.c32942a4.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(435)]).then(r.bind(r, 3435)),
+                        component: () => Promise.all([r.e(736), r.e(768)]).then(r.bind(r, 9768)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -164,24 +164,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, o) => (r.f[o](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
             430: "591e9a73",
-            435: "ced6eca8"
+            768: "89ad69c0"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            435: "30396533",
-            736: "f747ec02"
+            736: "f747ec02",
+            768: "30396533"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -264,15 +264,15 @@
                 e(o, l, n, a)
             })),
             n = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                435: 1
+                768: 1
             };
             n[e] ? t.push(n[e]) : 0 !== n[e] && r[e] && t.push(n[e] = o(e).then((() => {
                 n[e] = 0
             }), (t => {
                 throw delete n[e], t
             })))
         }
```

### Comparing `unigui-1.9.8/unigui/web/js/vendor.8cb03aaa.js` & `unigui-1.9.9/unigui/web/js/vendor.8cb03aaa.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/js/193.283445be.js` & `unigui-1.9.9/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui/web/index.html` & `unigui-1.9.9/unigui/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.8cb03aaa.js></script><script defer src=js/app.353e1981.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.8cb03aaa.js></script><script defer src=js/app.c32942a4.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.9.8/LICENSE` & `unigui-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/setup.py` & `unigui-1.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.8',      
+      version='1.9.9',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.9.8/PKG-INFO` & `unigui-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.8
+Version: 1.9.9
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.8/README.md` & `unigui-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.9.8/unigui.egg-info/PKG-INFO` & `unigui-1.9.9/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.8
+Version: 1.9.9
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.8/unigui.egg-info/SOURCES.txt` & `unigui-1.9.9/unigui.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/435.30396533.css
+unigui/web/css/768.30396533.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.f747ec02.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -31,10 +31,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/435.ced6eca8.js
-unigui/web/js/app.353e1981.js
+unigui/web/js/768.89ad69c0.js
+unigui/web/js/app.c32942a4.js
 unigui/web/js/vendor.8cb03aaa.js
```

