# Comparing `tmp/thunno2-2.2.8.tar.gz` & `tmp/thunno2-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.2.8.tar", last modified: Sat Jul 22 10:24:23 2023, max compression
+gzip compressed data, was "thunno2-2.2.9.tar", last modified: Mon Jul 24 15:58:09 2023, max compression
```

## Comparing `thunno2-2.2.8.tar` & `thunno2-2.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 10:24:23.052973 thunno2-2.2.8/
--rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 10:24:23.052860 thunno2-2.2.8/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-22 10:24:23.053003 thunno2-2.2.8/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.8/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 10:24:23.052172 thunno2-2.2.8/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.8/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.8/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.8/thunno2/canvas.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.8/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.8/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.8/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.8/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.8/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    58811 2023-07-13 18:38:48.000000 thunno2-2.2.8/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    34295 2023-07-22 09:41:31.000000 thunno2-2.2.8/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    26469 2023-07-22 09:41:31.000000 thunno2-2.2.8/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.8/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    86420 2023-07-13 18:37:15.000000 thunno2-2.2.8/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.8/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-22 10:23:46.000000 thunno2-2.2.8/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 10:24:23.052698 thunno2-2.2.8/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 10:24:23.000000 thunno2-2.2.8/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-22 10:24:23.000000 thunno2-2.2.8/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-22 10:24:23.000000 thunno2-2.2.8/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       53 2023-07-22 10:24:23.000000 thunno2-2.2.8/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-22 10:24:23.000000 thunno2-2.2.8/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-24 15:58:09.052392 thunno2-2.2.9/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-24 15:58:09.052286 thunno2-2.2.9/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-24 15:58:09.052421 thunno2-2.2.9/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.9/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-24 15:58:09.051589 thunno2-2.2.9/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.9/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.9/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.9/thunno2/canvas.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.9/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.9/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.9/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.9/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-07-23 09:35:39.000000 thunno2-2.2.9/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    58819 2023-07-24 15:56:45.000000 thunno2-2.2.9/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    34295 2023-07-22 09:41:31.000000 thunno2-2.2.9/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    26469 2023-07-22 09:41:31.000000 thunno2-2.2.9/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.9/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    86420 2023-07-13 18:37:15.000000 thunno2-2.2.9/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.9/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-24 15:57:14.000000 thunno2-2.2.9/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-24 15:58:09.052121 thunno2-2.2.9/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-24 15:58:09.000000 thunno2-2.2.9/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-24 15:58:09.000000 thunno2-2.2.9/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-24 15:58:09.000000 thunno2-2.2.9/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       53 2023-07-24 15:58:09.000000 thunno2-2.2.9/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-24 15:58:09.000000 thunno2-2.2.9/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.2.8/PKG-INFO` & `thunno2-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.8
+Version: 2.2.9
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.8.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.9.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
 Keywords: golfing,code-golf,language
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `thunno2-2.2.8/setup.py` & `thunno2-2.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/autoexplanation.py` & `thunno2-2.2.9/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/canvas.py` & `thunno2-2.2.9/thunno2/canvas.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/codepage.py` & `thunno2-2.2.9/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/commands.py` & `thunno2-2.2.9/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/constants.py` & `thunno2-2.2.9/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/dictionary.py` & `thunno2-2.2.9/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/flags.py` & `thunno2-2.2.9/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/helpers.py` & `thunno2-2.2.9/thunno2/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
     return wrapper
 
 
 def safe_max_len(*lsts):
     m = 0
     for lst in lsts:
-        if isinstance(lst, list):
+        if isinstance(lst, (list, str)):
             if len(lst) > m:
                 m = len(lst)
     return m
 
 
 def first_non_none(l):
     for i in l:
@@ -2689,15 +2689,15 @@
     return dump(digits(n))
 
 
 def centre_list(x):
     l = [*map(str, x)]
     if not l:
         return ""
-    max_len = safe_max_len(l)
+    max_len = max(map(len, l))
     return newline_join([*map(lambda s, m=max_len: s.center(m), l)])
 
 
 @convert_all_to_string
 def brackets_are_balanced(s):
     brackets = dict(chunk_wrap_2("()[]{}<>"))
     l = []
```

### Comparing `thunno2-2.2.8/thunno2/interpreter.py` & `thunno2-2.2.9/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/lexer.py` & `thunno2-2.2.9/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/run.py` & `thunno2-2.2.9/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/tests.py` & `thunno2-2.2.9/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2/tokens.py` & `thunno2-2.2.9/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.8/thunno2.egg-info/PKG-INFO` & `thunno2-2.2.9/thunno2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.8
+Version: 2.2.9
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.8.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.9.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
 Keywords: golfing,code-golf,language
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

