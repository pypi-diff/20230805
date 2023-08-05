# Comparing `tmp/glinski-0.0.0.tar.gz` & `tmp/glinski-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glinski-0.0.0.tar", last modified: Tue Aug  1 12:18:56 2023, max compression
+gzip compressed data, was "glinski-0.0.1.tar", last modified: Sat Aug  5 15:29:14 2023, max compression
```

## Comparing `glinski-0.0.0.tar` & `glinski-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:18:56.570011 glinski-0.0.0/
--rwxrwxr-x   0 jo        (1000) jo        (1000)     1065 2023-08-01 11:39:32.000000 glinski-0.0.0/LICENSE
--rw-rw-r--   0 jo        (1000) jo        (1000)     1444 2023-08-01 12:18:56.570011 glinski-0.0.0/PKG-INFO
--rwxrwxrwx   0 jo        (1000) jo        (1000)      474 2023-08-01 11:36:30.000000 glinski-0.0.0/pyproject.toml
--rwxrwxrwx   0 jo        (1000) jo        (1000)       38 2023-08-01 12:18:56.570011 glinski-0.0.0/setup.cfg
-drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:18:56.570011 glinski-0.0.0/src/
-drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:18:56.570011 glinski-0.0.0/src/glinski/
--rw-rw-r--   0 jo        (1000) jo        (1000)        2 2023-08-01 12:18:01.000000 glinski-0.0.0/src/glinski/__init__.py
-drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:18:56.570011 glinski-0.0.0/src/glinski.egg-info/
--rw-rw-r--   0 jo        (1000) jo        (1000)     1444 2023-08-01 12:18:56.000000 glinski-0.0.0/src/glinski.egg-info/PKG-INFO
--rw-rw-r--   0 jo        (1000) jo        (1000)      196 2023-08-01 12:18:56.000000 glinski-0.0.0/src/glinski.egg-info/SOURCES.txt
--rw-rw-r--   0 jo        (1000) jo        (1000)        1 2023-08-01 12:18:56.000000 glinski-0.0.0/src/glinski.egg-info/dependency_links.txt
--rw-rw-r--   0 jo        (1000) jo        (1000)        8 2023-08-01 12:18:56.000000 glinski-0.0.0/src/glinski.egg-info/top_level.txt
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-05 15:29:14.217697 glinski-0.0.1/
+-rwxrwxr-x   0 jo        (1000) jo        (1000)     1065 2023-08-01 11:39:32.000000 glinski-0.0.1/LICENSE
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1444 2023-08-05 15:29:14.217697 glinski-0.0.1/PKG-INFO
+-rw-rw-r--   0 jo        (1000) jo        (1000)       10 2023-08-05 15:19:03.000000 glinski-0.0.1/README.md
+-rwxrwxrwx   0 jo        (1000) jo        (1000)      474 2023-08-05 15:22:21.000000 glinski-0.0.1/pyproject.toml
+-rwxrwxrwx   0 jo        (1000) jo        (1000)       38 2023-08-05 15:29:14.217697 glinski-0.0.1/setup.cfg
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-05 15:29:14.213697 glinski-0.0.1/src/
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-05 15:29:14.217697 glinski-0.0.1/src/glinski/
+-rw-rw-r--   0 jo        (1000) jo        (1000)        2 2023-08-05 15:07:22.000000 glinski-0.0.1/src/glinski/__init__.py
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-05 15:29:14.217697 glinski-0.0.1/src/glinski.egg-info/
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1444 2023-08-05 15:29:14.000000 glinski-0.0.1/src/glinski.egg-info/PKG-INFO
+-rw-rw-r--   0 jo        (1000) jo        (1000)      206 2023-08-05 15:29:14.000000 glinski-0.0.1/src/glinski.egg-info/SOURCES.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)        1 2023-08-05 15:29:14.000000 glinski-0.0.1/src/glinski.egg-info/dependency_links.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)        8 2023-08-05 15:29:14.000000 glinski-0.0.1/src/glinski.egg-info/top_level.txt
```

### Comparing `glinski-0.0.0/LICENSE` & `glinski-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glinski-0.0.0/PKG-INFO` & `glinski-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glinski
-Version: 0.0.0
+Version: 0.0.1
 Summary: glinski
 Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
 License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `glinski-0.0.0/src/glinski.egg-info/PKG-INFO` & `glinski-0.0.1/src/glinski.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glinski
-Version: 0.0.0
+Version: 0.0.1
 Summary: glinski
 Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
 License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

