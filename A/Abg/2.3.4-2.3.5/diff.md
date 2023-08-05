# Comparing `tmp/Abg-2.3.4.tar.gz` & `tmp/Abg-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-2.3.4.tar", last modified: Sat Jul 22 08:39:36 2023, max compression
+gzip compressed data, was "Abg-2.3.5.tar", last modified: Sat Aug  5 11:22:05 2023, max compression
```

## Comparing `Abg-2.3.4.tar` & `Abg-2.3.5.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.591057 Abg-2.3.4/
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      322 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/__init__.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      415 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/config.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/helpers/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      855 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/__init__.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3710 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/get_user.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3184 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/helpers.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1596 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/http_helper.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2589 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/human_read.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     7351 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/msg_types.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1279 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/parser.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2533 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/pyro_progress.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2834 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/ratelimit.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5335 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/string.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/inline/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      274 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/__init__.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     6105 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/inline_keyboard.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4267 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/inline_pagination_keyboard.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1487 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/reply_keyboard.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      105 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/__init__.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/bound/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       29 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/bound/__init__.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    12057 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/bound/message.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/decorators/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      140 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/__init__.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    13150 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/adminsOnly.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4398 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/on_cb.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5327 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/on_cmd.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3675 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/utils.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/listen/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       55 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/listen/__init__.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    12016 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/listen/listen.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      776 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/listen/utils.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.591057 Abg-2.3.4/Abg/patch/methods/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      127 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/__init__.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2172 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/edit_message_text.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1713 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/send_as_file.py
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2933 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/send_message.py
-drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg.egg-info/
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5745 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/PKG-INFO
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1007 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/SOURCES.txt
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        1 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/dependency_links.txt
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        1 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/not-zip-safe
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        4 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/top_level.txt
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5745 2023-07-22 08:39:36.591057 Abg-2.3.4/PKG-INFO
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3088 2023-07-22 08:39:01.000000 Abg-2.3.4/README.md
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       38 2023-07-22 08:39:36.591057 Abg-2.3.4/setup.cfg
--rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3045 2023-07-22 08:39:01.000000 Abg-2.3.4/setup.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.126148 Abg-2.3.5/
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.118148 Abg-2.3.5/Abg/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      322 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      419 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/config.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.122148 Abg-2.3.5/Abg/helpers/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      855 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3710 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/get_user.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3184 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/helpers.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1596 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/http_helper.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2589 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/human_read.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     7351 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/msg_types.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1279 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/parser.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2533 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/pyro_progress.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2834 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/ratelimit.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5335 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/helpers/string.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.122148 Abg-2.3.5/Abg/inline/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      274 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/inline/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     6105 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/inline/inline_keyboard.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4267 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/inline/inline_pagination_keyboard.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1487 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/inline/reply_keyboard.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.122148 Abg-2.3.5/Abg/patch/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      105 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/__init__.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.122148 Abg-2.3.5/Abg/patch/bound/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       29 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/bound/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    12480 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/bound/message.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.122148 Abg-2.3.5/Abg/patch/decorators/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      140 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/decorators/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    13432 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/decorators/adminsOnly.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4398 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/decorators/on_cb.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5587 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/decorators/on_cmd.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3583 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/decorators/utils.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.122148 Abg-2.3.5/Abg/patch/listen/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       55 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/listen/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    12016 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/listen/listen.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      776 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/listen/utils.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.126148 Abg-2.3.5/Abg/patch/methods/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      127 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/methods/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2172 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/methods/edit_message_text.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1713 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/methods/send_as_file.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2989 2023-08-05 11:21:43.000000 Abg-2.3.5/Abg/patch/methods/send_message.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-08-05 11:22:05.118148 Abg-2.3.5/Abg.egg-info/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4888 2023-08-05 11:22:05.000000 Abg-2.3.5/Abg.egg-info/PKG-INFO
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1041 2023-08-05 11:22:05.000000 Abg-2.3.5/Abg.egg-info/SOURCES.txt
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        1 2023-08-05 11:22:05.000000 Abg-2.3.5/Abg.egg-info/dependency_links.txt
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        1 2023-08-05 11:22:05.000000 Abg-2.3.5/Abg.egg-info/not-zip-safe
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       31 2023-08-05 11:22:05.000000 Abg-2.3.5/Abg.egg-info/requires.txt
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        4 2023-08-05 11:22:05.000000 Abg-2.3.5/Abg.egg-info/top_level.txt
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1067 2023-08-05 11:21:43.000000 Abg-2.3.5/LICENSE
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4888 2023-08-05 11:22:05.126148 Abg-2.3.5/PKG-INFO
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3088 2023-08-05 11:21:43.000000 Abg-2.3.5/README.md
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       38 2023-08-05 11:22:05.126148 Abg-2.3.5/setup.cfg
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3072 2023-08-05 11:21:43.000000 Abg-2.3.5/setup.py
```

### Comparing `Abg-2.3.4/Abg/helpers/__init__.py` & `Abg-2.3.5/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/get_user.py` & `Abg-2.3.5/Abg/helpers/get_user.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/helpers.py` & `Abg-2.3.5/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/http_helper.py` & `Abg-2.3.5/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/human_read.py` & `Abg-2.3.5/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/msg_types.py` & `Abg-2.3.5/Abg/helpers/msg_types.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/parser.py` & `Abg-2.3.5/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/pyro_progress.py` & `Abg-2.3.5/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/ratelimit.py` & `Abg-2.3.5/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/helpers/string.py` & `Abg-2.3.5/Abg/helpers/string.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/inline/inline_keyboard.py` & `Abg-2.3.5/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/inline/inline_pagination_keyboard.py` & `Abg-2.3.5/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/inline/reply_keyboard.py` & `Abg-2.3.5/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/patch/bound/message.py` & `Abg-2.3.5/Abg/patch/bound/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     ChatWriteForbidden,
     FloodWait,
     MessageAuthorRequired,
     MessageDeleteForbidden,
     MessageIdInvalid,
     MessageNotModified,
     MessageTooLong,
+    RightForbidden,
+    SlowmodeWait,
 )
 from pyrogram.types import Message
 
 LOGGER = getLogger(__name__)
 
 Message.input = property(
     lambda m: m.text[m.text.find(m.command[0]) + len(m.command[0]) + 1 :]
@@ -84,19 +86,23 @@
         if del_in == 0:
             return msg
         await asleep(del_in)
         return bool(await msg.delete_msg())
     except FloodWait as e:
         await asleep(e.value)
         return await reply_text(self, text, *args, **kwargs)
+    except RightForbidden:
+        return await reply_text(
+            "ʙᴏᴛ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴇɴᴏᴜɢʜ ʀɪɢʜᴛs ᴛᴏ ᴘᴇʀғᴏʀᴍᴇᴅ ᴛʜɪs ᴀᴄᴛɪᴏɴ "
+        )
     # except TopicClosed:
     # return
-    except (ChatWriteForbidden, ChatAdminRequired):
+    except (SlowmodeWait, ChatWriteForbidden):
         LOGGER.info(
-            f"Leaving from {self.chat.title} [{self.chat.id}] because doesn't have admin permission."
+            f"Leaving from {self.chat.title} [{self.chat.id}] because doesn't have admin/Write permission."
         )
         return await self.chat.leave()
 
 
 async def edit_text(
     self, text: str, del_in: int = 0, *args, **kwargs
 ) -> Union["Message", bool]:
@@ -133,15 +139,17 @@
         return bool(await msg.delete_msg())
     except FloodWait as e:
         LOGGER.warning(str(e))
         await asleep(e.value)
         return await edit_text(self, text, *args, **kwargs)
     except MessageNotModified:
         return False
-    except (ChatWriteForbidden, ChatAdminRequired):
+    except RightForbidden:
+        return await reply_text("ʙᴏᴛ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴇɴᴏᴜɢʜ ʀɪɢʜᴛs ᴛᴏ ᴘᴇʀғᴏʀᴍᴇᴅ ᴛʜɪs ᴀᴄᴛɪᴏɴ")
+    except (SlowmodeWait, ChatWriteForbidden):
         LOGGER.info(
             f"Leaving from {self.chat.title} [{self.chat.id}] because doesn't have admin permission."
         )
         return await self.chat.leave()
     except (MessageAuthorRequired, MessageIdInvalid):
         return await reply_text(self, text=text, *args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Abg-2.3.4/Abg/patch/decorators/adminsOnly.py` & `Abg-2.3.5/Abg/patch/decorators/adminsOnly.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     self, CallbackQuery: pyrogram.types.CallbackQuery
 ):
     if int(
         f"{CallbackQuery.message.chat.id}{CallbackQuery.data.split('.')[1]}"
     ) not in set(ANON.keys()):
         try:
             await CallbackQuery.message.edit_text("ʙᴜᴛᴛᴏɴ ʜᴀs ʙᴇᴇɴ ᴇxᴘɪʀᴇᴅ.")
-        except pyrogram.types.RPCError:
-            with contextlib.suppress(pyrogram.types.RPCError):
+        except pyrogram.errors.RPCError:
+            with contextlib.suppress(pyrogram.errors.RPCError):
                 await CallbackQuery.message.delete()
         return
     cb = ANON.pop(
         int(f"{CallbackQuery.message.chat.id}{CallbackQuery.data.split('.')[1]}")
     )
     member = await CallbackQuery.message.chat.get_member(CallbackQuery.from_user.id)
     if member.status not in (
@@ -79,14 +79,15 @@
     Args:
         permissions (str, optional): permission type to check. Defaults to None.
         is_bot (bool, optional): If bot can perform the action. Defaults to False.
         is_user (bool, optional): If user can perform the action. Defaults to False.
         is_both (bool, optional): If both user and bot can perform the action. Defaults to False.
         only_owner (bool, optional): If only owner can perform the action. Defaults to False. (It's Chat Owner)
         only_dev (bool, optional): if only dev users can perform the operation. Defaults to False.
+        ex: `@app.adminsOnly(permissions="..", is_both=True)`
     """
 
     def decorator(func):
         @wraps(func)
         async def wrapper(
             abg: Client, message: Union[CallbackQuery, Message], *args, **kwargs
         ):
@@ -127,17 +128,19 @@
                     "ʏᴏᴜ'ʀᴇ ᴀɴ ᴀɴᴏɴʏᴍᴏᴜs ᴀᴅᴍɪɴ, ᴄʟɪᴄᴋ ᴏɴ ᴛʜᴇ ʙᴜᴛᴛᴏɴ ʙᴇʟᴏᴡ ᴛᴏ ᴘʀᴏᴠᴇ ʏᴏᴜʀ ɪᴅᴇɴᴛɪᴛʏ",
                     reply_markup=keyboard,
                 )
 
             try:
                 bot = await chat.get_member(abg.me.id)
                 user = await chat.get_member(message.from_user.id)
+            except pyrogram.errors.exceptions.forbidden_403.ChatAdminRequired:
+                return await sender(f"ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ")
             except UserNotParticipant:
                 return await sender(
-                    f"ᴜsᴇʀ: {message.from_user.id} ɴᴏᴛ ᴍᴀᴍʙᴇʀ ᴏғ ᴛʜɪs ᴄʜᴀᴛ."
+                    f"ᴜsᴇʀ: {message.from_user.first_name} ɴᴏᴛ ᴍᴇᴍʙᴇʀ ᴏғ ᴛʜɪs ᴄʜᴀᴛ."
                 )
             except BaseException as e:
                 return await handle_error(e, msg)
 
             if only_owner:
                 if user.status == ChatMemberStatus.OWNER:
                     return await func(abg, message, *args, **kwargs)
```

### Comparing `Abg-2.3.4/Abg/patch/decorators/on_cb.py` & `Abg-2.3.5/Abg/patch/decorators/on_cb.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/patch/decorators/on_cmd.py` & `Abg-2.3.5/Abg/patch/decorators/on_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import asyncio
+import traceback
 import typing
 from logging import getLogger
 
 import pyrogram
 from pyrogram import Client
-from pyrogram.errors import FloodWait, Forbidden, SlowmodeWait
+from pyrogram.errors import FloodWait, Forbidden, RPCError, SlowmodeWait
 from pyrogram.methods import Decorators
 
-from .utils import handle_error
+from Abg.config import Config
 
-HANDLER = ["/", "!", "~", ".", "+", "*", "$", " @"]
+from .utils import handle_error
 
+HANDLER = Config.HANDLER
 LOGGER = getLogger(__name__)
 
 
 def command(
     self,
-    command: typing.Union[str, list],
+    cmd: typing.Union[str, list],
     is_disabled: typing.Union[bool, bool] = False,
     pm_only: typing.Union[bool, bool] = False,
     group_only: typing.Union[bool, bool] = False,
     self_admin: typing.Union[bool, bool] = False,
     self_only: typing.Union[bool, bool] = False,
     handler: typing.Optional[list] = None,
-    filter: typing.Union[pyrogram.filters.Filter, pyrogram.filters.Filter] = None,
+    filtercmd: typing.Union[pyrogram.filters.Filter, pyrogram.filters.Filter] = None,
     *args,
     **kwargs,
 ):
     """
     ### `@Client.on_cmd`
     - A decorater to Register Commands in simple way and manage errors in that Function itself, alternative for `@pyrogram.Client.on_message(pyrogram.filters.command('command'))`
     - Parameters:
-    - command (str || list):
+    - cmd (str || list):
         - The command to be handled for a function
 
     - group_only (bool) **optional**:
         - If True, the command will only executed in Groups only, By Default False.
 
     - pm_only (bool) **optional**:
         - If True, the command will only executed in Private Messages only, By Default False.
@@ -45,50 +47,49 @@
 
     - handler (list) **optional**:
         - If set, the command will be handled by the specified Handler, By Default `Config.HANDLERS`.
 
     - self_admin (bool) **optional**:
         - If True, the command will only executeed if the Bot is Admin in the Chat, By Default False
 
-    - filter (`~pyrogram.filters`) **optional**:
+    - filtercmd (`~pyrogram.filters`) **optional**:
         - Pyrogram Filters, hope you know about this, for Advaced usage. Use `and` for seaperating filters.
 
     #### Example
     .. code-block:: python
         import pyrogram
 
-        app = pyrogram.Client()
+        app = pyrogram.Client(..)
 
         @app.on_cmd("start", is_disabled=False, group_only=False, pm_only=False, self_admin=False, self_only=False, pyrogram.filters.chat("777000") and pyrogram.filters.text)
         async def start(abg: Client, message):
             await message.reply_text(f"Hello {message.from_user.mention}")
     """
     if handler is None:
         handler = HANDLER
-    if filter:
+    if filtercmd:
         if self_only:
-            filter = (
-                pyrogram.filters.command(command, prefixes=handler)
-                & filter
+            filtercmd = (
+                pyrogram.filters.command(cmd, prefixes=handler)
+                & filtercmd
                 & pyrogram.filters.me
             )
         else:
-            filter = (
-                pyrogram.filters.command(command, prefixes=handler)
-                & filter
+            filtercmd = (
+                pyrogram.filters.command(cmd, prefixes=handler)
+                & filtercmd
                 & pyrogram.filters.me
             )
     else:
         if self_only:
-            filter = (
-                pyrogram.filters.command(command, prefixes=handler)
-                & pyrogram.filters.me
+            filtercmd = (
+                pyrogram.filters.command(cmd, prefixes=handler) & pyrogram.filters.me
             )
         else:
-            filter = pyrogram.filters.command(command, prefixes=handler)
+            filtercmd = pyrogram.filters.command(cmd, prefixes=handler)
 
     def wrapper(func):
         async def decorator(abg: Client, message: pyrogram.types.Message):
             if is_disabled:
                 return await message.reply_text(
                     "sᴏʀʀʏ, ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ʜᴀs ʙᴇᴇɴ ᴅɪsᴀʙʟᴇᴅ ʙʏ ᴏᴡɴᴇʀ."
                 )
@@ -112,24 +113,28 @@
             if pm_only and message.chat.type != pyrogram.enums.ChatType.PRIVATE:
                 return await message.reply_text("ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ ʙᴇ ᴜsᴇᴅ ɪɴ ᴘᴍs ᴏɴʟʏ.")
             try:
                 await func(abg, message)
             except FloodWait as fw:
                 LOGGER.warning(str(fw))
                 await asyncio.sleep(fw.value)
+                LOGGER.info("Sleeping for {fw.value}, Due to flood")
             except (Forbidden, SlowmodeWait):
                 LOGGER.info(
                     f"Leaving chat : {message.chat.title} [{message.chat.id}], because doesn't have write permission."
                 )
-                return await abg.leave_chat(message.chat.id)
+                return await message.chat.leave()
+            except RPCError as err:
+                LOGGER.exception(traceback.format_exc())
+                return await message.reply_text(f"ᴇʀʀᴏʀ ғᴏᴜɴᴅ:\n{err}")
             except BaseException as e:
                 return await handle_error(e, message)
 
         self.add_handler(
-            pyrogram.handlers.MessageHandler(callback=decorator, filters=filter)
+            pyrogram.handlers.MessageHandler(callback=decorator, filters=filtercmd)
         )
         return decorator
 
     return wrapper
 
 
 Decorators.on_cmd = command
```

### Comparing `Abg-2.3.4/Abg/patch/decorators/utils.py` & `Abg-2.3.5/Abg/patch/decorators/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,29 @@
 import traceback
 import typing
 from datetime import datetime
 
 import pyrogram
 from pyrogram import filters
 from pyrogram.errors import MessageDeleteForbidden
+from pytz import timezone
 
 from Abg.config import Config
 
 LOGGER = logging.getLogger(__name__)
-log_chat = Config.OWNER_ID if Config.LOGGER_ID is None else Config.LOGGER_ID
+TIME_ZONE = Config.TIME_ZONE
+LOG = Config.LOGGER_ID
 
 data = {}
 
 
+class StopPropagation(Exception):
+    """Exception that raised to stop propagating an event"""
+
+
 async def task(msg, warn=False, sec=None):
     if warn:
         user = msg.from_user or msg.sender_chat
         ids = await msg.reply_msg(
             f"sᴏʀʀʏ {user.mention if msg.from_user else msg.sender_chat.title} , ʏᴏᴜ ᴍᴜsᴛ ᴡᴀɪᴛ ғᴏʀ {sec}s ʙᴇғᴏʀᴇ ᴜsɪɴɢ ᴛʜɪs ғᴇᴀᴛᴜʀᴇ ᴀɢᴀɪɴ.."
         )
         try:
@@ -56,41 +62,37 @@
             data.update({user_id: {"timestamp": msg.date.timestamp(), "warned": False}})
             return True
 
     return filters.create(___, data=sec)
 
 
 async def handle_error(
-    _, m: typing.Union[pyrogram.types.Message, pyrogram.types.CallbackQuery]
+    error, m: typing.Union[pyrogram.types.Message, pyrogram.types.CallbackQuery]
 ):
-    day = datetime.now()
-    tgl_now = datetime.now()
+    day = datetime.now(timezone(TIME_ZONE))
+    tgl_now = datetime.now(timezone(TIME_ZONE))
     cap_day = f"{day.strftime('%A')}, {tgl_now.strftime('%d %B %Y %H:%M:%S')}"
     f_errname = f"crash_{tgl_now.strftime('%d %B %Y')}.txt"
     LOGGER.error(traceback.format_exc())
     with open(f_errname, "w+", encoding="utf-8") as log:
         log.write(traceback.format_exc())
         log.close()
-    if isinstance(m, pyrogram.types.Message):
+    if isinstance(m, pyrogram.types.CallbackQuery):
         with contextlib.suppress(Exception):
-            await m.reply_text(
-                "ᴇʀʀᴏʀ ғᴏᴜɴᴅ ᴡʜɪʟᴇ ᴘʀᴏᴄᴇssɪɴɢ ʏᴏᴜʀ ᴄᴏᴍᴍᴀɴᴅ.\nsᴏʀʀʏ ғᴏʀ ɪɴᴄᴏɴᴠᴇɴɪᴇɴᴄᴇ"
-            )
-            await m._client.send_document(
-                log_chat,
+            await m.message.delete()
+            await m.message.reply_text("ᴇʀʀᴏʀ ғᴏᴜɴᴅ:\nsᴏʀʀʏ ғᴏʀ ɪɴᴄᴏɴᴠᴇɴɪᴇɴᴄᴇ")
+            await m.message._client.send_document(
+                int(LOG),
                 f_errname,
                 caption=f"ᴄʀᴀsʜ ʀᴇᴘᴏʀᴛ ᴏғ ᴛʜɪs ʙᴏᴛ\n{cap_day}",
             )
-    if isinstance(m, pyrogram.types.CallbackQuery):
+    else:
         with contextlib.suppress(Exception):
-            await m.message.delete()
-            await m.message.reply_text(
-                "ᴇʀʀᴏʀ ғᴏᴜɴᴅ ᴡʜɪʟᴇ ᴘʀᴏᴄᴇssɪɴɢ ʏᴏᴜʀ ᴄᴏᴍᴍᴀɴᴅ.\nsᴏʀʀʏ ғᴏʀ ɪɴᴄᴏɴᴠᴇɴɪᴇɴᴄᴇ"
-            )
-            await m.message._client.send_document(
-                log_chat,
+            await m.reply_text("ᴇʀʀᴏʀ ғᴏᴜɴᴅ:\nsᴏʀʀʏ ғᴏʀ ɪɴᴄᴏɴᴠᴇɴɪᴇɴᴄᴇ")
+            await m._client.send_document(
+                int(LOG),
                 f_errname,
                 caption=f"ᴄʀᴀsʜ ʀᴇᴘᴏʀᴛ ᴏғ ᴛʜɪs ʙᴏᴛ\n{cap_day}",
             )
     if os.path.exists(f_errname):
         os.remove(f_errname)
     return True
```

### Comparing `Abg-2.3.4/Abg/patch/listen/listen.py` & `Abg-2.3.5/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/patch/listen/utils.py` & `Abg-2.3.5/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/patch/methods/edit_message_text.py` & `Abg-2.3.5/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/patch/methods/send_as_file.py` & `Abg-2.3.5/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/Abg/patch/methods/send_message.py` & `Abg-2.3.5/Abg/patch/methods/send_message.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 from typing import Union
 
 from pyrogram import Client
 from pyrogram.types import Message
 
 
 async def send_message(
-    self, chat_id: Union[int, str], text: str, del_in: int = 0, *args, **kwargs
+    self,
+    chat_id: Union[int, str],
+    text: str,
+    del_in: int = 0,
+    message_thread_id: int = None,
+    *args,
+    **kwargs
 ) -> Union["Message", bool]:
     """\nSend text messages.
     Example:
             @userge.send_message(chat_id=12345, text='test')
     Parameters:
         chat_id (``int`` | ``str``):
             Unique identifier (int) or username (str) of the target chat.
@@ -18,17 +24,17 @@
             you can simply use "me" or "self".
             For a contact that exists in your Telegram address book
             you can use his phone number (str).
         text (``str``):
             Text of the message to be sent.
         del_in (``int``):
             Time in Seconds for delete that message.
-        log (``bool`` | ``str``, *optional*):
-            If ``True``, the message will be forwarded to the log channel.
-            If ``str``, the logger name will be updated.
+        message_thread_id (``int``, *optional*):
+                Unique identifier for the target message thread (topic) of the forum.
+                for forum supergroups only.
         parse_mode (:obj:`enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
             Pass "markdown" or "md" to enable Markdown-style parsing only.
             Pass "html" to enable HTML-style parsing only.
             Pass None to completely disable style parsing.
         entities (List of :obj:`~pyrogram.types.MessageEntity`):
```

### Comparing `Abg-2.3.4/Abg.egg-info/PKG-INFO` & `Abg-2.3.5/Abg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,21 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3.4
+Version: 2.3.5
 Summary: add-on for Pyrogram || Telegram bot helpers || Easy botting
 Home-page: https://github.com/Abishnoi69/Abg
+Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
-Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
-Description: <p align="center">
-        <b> ABG </b>
-        </p>
-        
-        <p align="center"><a href="https://pepy.tech/project/abg"> <img src="https://static.pepy.tech/personalized-badge/abg?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads" width="169" height="29.69"/></a></p>
-        
-        ### Requirements 
-        
-        - Python 3.7 ᴏʀ higher.
-        - A [ᴛᴇʟᴇɢʀᴀᴍ ᴀᴘɪ ᴋᴇʏ](https://docs.pyrogram.org/intro/setup#api-keys).
-        - ᴀʙɢ [ᴄᴏɴғɪɢ](https://github.com/Abishnoi69/Abg#configuratoins).
-        
-        ### Installing :
-        
-        ```bash
-        pip install -U Abg
-        ```
-        #### sᴇᴛᴜᴘ
-        ```python
-        from pyrogram import filters, Client
-        from pyrogram.types import CallbackQuery, Message
-        from Abg import patch  # type : ignore
-        from Abg.helpers import ikb
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("myinfo")
-        Resultdef my_info(self: Client, ctx: Message):
-            if not ctx.from_user:
-                return
-            name = await ctx.chat.ask("Type Your Name")
-            age = await ctx.chat.ask("Type your age")
-            add = await ctx.chat.ask("Type your address")
-            # you can also use : ctx.reply_text(...)
-            await self.send_msg(
-                chat_id=ctx.chat.id,
-                text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
-                reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
-            )
-        
-        # callback 
-        @app.on_cb("hello")
-        async def hello(c: Client, q: CallbackQuery):
-            await q.answer("Hello From Abg", show_alert=True)
-        
-          app.run()
-        ```
-        >
-        #### ᴜsᴇʀ/ʙᴏᴛ ʀɪɢʜᴛs 
-        
-        ```python
-        from Abg import patch  # all patch
-        from pyrogram.types import Message
-        from pyrogram import Client
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("del", group_only=True)
-        @app.adminsOnly(permissions="can_delete_messages", is_both=True)
-        async def del_msg(c: Client, m: Message):
-            if m.reply_to_message:
-                await m.delete()
-                await c.delete_messages(
-                    chat_id=m.chat.id,
-                    message_ids=m.reply_to_message.id,
-                )
-            else:
-                await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
-            return
-          
-          app.run()
-        ```
-        
-        
-        >
-        ### keyboard's
-        
-        ```python
-        from Abg.inline import InlineKeyboard, InlineButton
-        
-        
-        keyboard = InlineKeyboard(row_width=3)
-        keyboard.add(
-            InlineButton('1', 'inline_keyboard:1'),
-            InlineButton('2', 'inline_keyboard:2'),
-            InlineButton('3', 'inline_keyboard:3'),
-            InlineButton('4', 'inline_keyboard:4'),
-            InlineButton('5', 'inline_keyboard:5'),
-            InlineButton('6', 'inline_keyboard:6'),
-            InlineButton('7', 'inline_keyboard:7')
-        )
-        ```
-        
-        #### ʀᴇsᴜʟᴛ
-        
-        <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
-        
-        ━━━━━━━━━━━━━━━━━━━━
-        ### Configuratoins
-        ```
-        OWNER_ID = ʏᴏᴜʀ ᴛᴇʟᴇɢʀᴀᴍ ɪᴅ.
-        DEV_USERS = ʙᴏᴛ ᴅᴇᴠs ɪᴅ. (ʏᴏᴜ ᴄᴀɴ ᴀᴅᴅ ᴀ ʟɪsᴛ : 1 2 3)
-        LOGGER_ID = ʏᴏᴜʀ ᴘʀɪᴠᴀᴛᴇ ɢʀᴏᴜᴘ/ᴄʜᴀɴɴᴇʟ ɪᴅ. (ʜᴇʀᴇ ʙᴏᴛ sᴇɴᴅ ʟᴏɢs)
-        ```
-        ━━━━━━━━━━━━━━━━━━━━ 
-        
-        
 Keywords: add-on pyrogram bots telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch https
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -138,7 +30,115 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+<b> ABG </b>
+</p>
+
+<p align="center"><a href="https://pepy.tech/project/abg"> <img src="https://static.pepy.tech/personalized-badge/abg?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads" width="169" height="29.69"/></a></p>
+
+### Requirements 
+
+- Python 3.7 ᴏʀ higher.
+- A [ᴛᴇʟᴇɢʀᴀᴍ ᴀᴘɪ ᴋᴇʏ](https://docs.pyrogram.org/intro/setup#api-keys).
+- ᴀʙɢ [ᴄᴏɴғɪɢ](https://github.com/Abishnoi69/Abg#configuratoins).
+
+### Installing :
+
+```bash
+pip install -U Abg
+```
+#### sᴇᴛᴜᴘ
+```python
+from pyrogram import filters, Client
+from pyrogram.types import CallbackQuery, Message
+from Abg import patch  # type : ignore
+from Abg.helpers import ikb
+
+app = Client("my_account")
+
+@app.on_cmd("myinfo")
+Resultdef my_info(self: Client, ctx: Message):
+    if not ctx.from_user:
+        return
+    name = await ctx.chat.ask("Type Your Name")
+    age = await ctx.chat.ask("Type your age")
+    add = await ctx.chat.ask("Type your address")
+    # you can also use : ctx.reply_text(...)
+    await self.send_msg(
+        chat_id=ctx.chat.id,
+        text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+        reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
+    )
+
+# callback 
+@app.on_cb("hello")
+async def hello(c: Client, q: CallbackQuery):
+    await q.answer("Hello From Abg", show_alert=True)
+
+  app.run()
+```
+>
+#### ᴜsᴇʀ/ʙᴏᴛ ʀɪɢʜᴛs 
+
+```python
+from Abg import patch  # all patch
+from pyrogram.types import Message
+from pyrogram import Client
+
+app = Client("my_account")
+
+@app.on_cmd("del", group_only=True)
+@app.adminsOnly(permissions="can_delete_messages", is_both=True)
+async def del_msg(c: Client, m: Message):
+    if m.reply_to_message:
+        await m.delete()
+        await c.delete_messages(
+            chat_id=m.chat.id,
+            message_ids=m.reply_to_message.id,
+        )
+    else:
+        await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
+    return
+  
+  app.run()
+```
+
+
+>
+### keyboard's
+
+```python
+from Abg.inline import InlineKeyboard, InlineButton
+
+
+keyboard = InlineKeyboard(row_width=3)
+keyboard.add(
+    InlineButton('1', 'inline_keyboard:1'),
+    InlineButton('2', 'inline_keyboard:2'),
+    InlineButton('3', 'inline_keyboard:3'),
+    InlineButton('4', 'inline_keyboard:4'),
+    InlineButton('5', 'inline_keyboard:5'),
+    InlineButton('6', 'inline_keyboard:6'),
+    InlineButton('7', 'inline_keyboard:7')
+)
+```
+
+#### ʀᴇsᴜʟᴛ
+
+<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+
+━━━━━━━━━━━━━━━━━━━━
+### Configuratoins
+```
+OWNER_ID = ʏᴏᴜʀ ᴛᴇʟᴇɢʀᴀᴍ ɪᴅ.
+DEV_USERS = ʙᴏᴛ ᴅᴇᴠs ɪᴅ. (ʏᴏᴜ ᴄᴀɴ ᴀᴅᴅ ᴀ ʟɪsᴛ : 1 2 3)
+LOGGER_ID = ʏᴏᴜʀ ᴘʀɪᴠᴀᴛᴇ ɢʀᴏᴜᴘ/ᴄʜᴀɴɴᴇʟ ɪᴅ. (ʜᴇʀᴇ ʙᴏᴛ sᴇɴᴅ ʟᴏɢs)
+```
+━━━━━━━━━━━━━━━━━━━━ 
+
```

#### html2text {}

```diff
@@ -1,14 +1,31 @@
-Metadata-Version: 2.1 Name: Abg Version: 2.3.4 Summary: add-on for Pyrogram ||
+Metadata-Version: 2.1 Name: Abg Version: 2.3.5 Summary: add-on for Pyrogram ||
 Telegram bot helpers || Easy botting Home-page: https://github.com/Abishnoi69/
-Abg Author: Abishnoi Author-email: Abishnoi69@Abg.org License: MIT Download-
-URL: https://github.com/Abishnoi69/Abg/releases/latest Project-URL: Tracker,
+Abg Download-URL: https://github.com/Abishnoi69/Abg/releases/latest Author:
+Abishnoi Author-email: Abishnoi69@Abg.org License: MIT Project-URL: Tracker,
 https://github.com/Abishnoi69/Abg/issues Project-URL: Community, https://t.me/
 Abgpy Project-URL: Source, https://github.com/Abishnoi69/Abg Project-URL:
-Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce Description:
+Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce Keywords:
+add-on pyrogram bots telegram bot chat messenger mtproto api client library
+python conversation keyboard userbot patch https Classifier: Development Status
+:: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation Classifier: Programming Language :: Python
+:: Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
+Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Libraries :: Application Frameworks Requires-Python: ~=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE
                                       ABG
                  [https://static.pepy.tech/personalized-badge/
 abg?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads]
 ### Requirements - Python 3.7 á´Ê higher. - A [á´á´Êá´É¢Êá´á´ á´á´Éª
 á´á´Ê](https://docs.pyrogram.org/intro/setup#api-keys). - á´ÊÉ¢
 [á´á´É´ÒÉªÉ¢](https://github.com/Abishnoi69/Abg#configuratoins). ###
 Installing : ```bash pip install -U Abg ``` #### sá´á´á´á´ ```python from
@@ -38,25 +55,8 @@
 'inline_keyboard:7') ) ``` #### Êá´sá´Êá´
 [add_inline_button]
 ââââââââââââââââââââ ### Configuratoins
 ``` OWNER_ID = Êá´á´Ê á´á´Êá´É¢Êá´á´ Éªá´. DEV_USERS = Êá´á´
 á´á´á´ s Éªá´. (Êá´á´ á´á´É´ á´á´á´ á´ ÊÉªsá´ : 1 2 3) LOGGER_ID
 = Êá´á´Ê á´ÊÉªá´ á´á´á´ É¢Êá´á´á´/á´Êá´É´É´á´Ê Éªá´.
 (Êá´Êá´ Êá´á´ sá´É´á´ Êá´É¢s) ```
-ââââââââââââââââââââ Keywords: add-on
-pyrogram bots telegram bot chat messenger mtproto api client library python
-conversation keyboard userbot patch https Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: Implementation Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown
+ââââââââââââââââââââ
```

### Comparing `Abg-2.3.4/Abg.egg-info/SOURCES.txt` & `Abg-2.3.5/Abg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+LICENSE
 README.md
 setup.py
 Abg/__init__.py
 Abg/config.py
 Abg.egg-info/PKG-INFO
 Abg.egg-info/SOURCES.txt
 Abg.egg-info/dependency_links.txt
 Abg.egg-info/not-zip-safe
+Abg.egg-info/requires.txt
 Abg.egg-info/top_level.txt
 Abg/helpers/__init__.py
 Abg/helpers/get_user.py
 Abg/helpers/helpers.py
 Abg/helpers/http_helper.py
 Abg/helpers/human_read.py
 Abg/helpers/msg_types.py
```

### Comparing `Abg-2.3.4/PKG-INFO` & `Abg-2.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,21 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3.4
+Version: 2.3.5
 Summary: add-on for Pyrogram || Telegram bot helpers || Easy botting
 Home-page: https://github.com/Abishnoi69/Abg
+Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
-Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
-Description: <p align="center">
-        <b> ABG </b>
-        </p>
-        
-        <p align="center"><a href="https://pepy.tech/project/abg"> <img src="https://static.pepy.tech/personalized-badge/abg?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads" width="169" height="29.69"/></a></p>
-        
-        ### Requirements 
-        
-        - Python 3.7 ᴏʀ higher.
-        - A [ᴛᴇʟᴇɢʀᴀᴍ ᴀᴘɪ ᴋᴇʏ](https://docs.pyrogram.org/intro/setup#api-keys).
-        - ᴀʙɢ [ᴄᴏɴғɪɢ](https://github.com/Abishnoi69/Abg#configuratoins).
-        
-        ### Installing :
-        
-        ```bash
-        pip install -U Abg
-        ```
-        #### sᴇᴛᴜᴘ
-        ```python
-        from pyrogram import filters, Client
-        from pyrogram.types import CallbackQuery, Message
-        from Abg import patch  # type : ignore
-        from Abg.helpers import ikb
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("myinfo")
-        Resultdef my_info(self: Client, ctx: Message):
-            if not ctx.from_user:
-                return
-            name = await ctx.chat.ask("Type Your Name")
-            age = await ctx.chat.ask("Type your age")
-            add = await ctx.chat.ask("Type your address")
-            # you can also use : ctx.reply_text(...)
-            await self.send_msg(
-                chat_id=ctx.chat.id,
-                text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
-                reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
-            )
-        
-        # callback 
-        @app.on_cb("hello")
-        async def hello(c: Client, q: CallbackQuery):
-            await q.answer("Hello From Abg", show_alert=True)
-        
-          app.run()
-        ```
-        >
-        #### ᴜsᴇʀ/ʙᴏᴛ ʀɪɢʜᴛs 
-        
-        ```python
-        from Abg import patch  # all patch
-        from pyrogram.types import Message
-        from pyrogram import Client
-        
-        app = Client("my_account")
-        
-        @app.on_cmd("del", group_only=True)
-        @app.adminsOnly(permissions="can_delete_messages", is_both=True)
-        async def del_msg(c: Client, m: Message):
-            if m.reply_to_message:
-                await m.delete()
-                await c.delete_messages(
-                    chat_id=m.chat.id,
-                    message_ids=m.reply_to_message.id,
-                )
-            else:
-                await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
-            return
-          
-          app.run()
-        ```
-        
-        
-        >
-        ### keyboard's
-        
-        ```python
-        from Abg.inline import InlineKeyboard, InlineButton
-        
-        
-        keyboard = InlineKeyboard(row_width=3)
-        keyboard.add(
-            InlineButton('1', 'inline_keyboard:1'),
-            InlineButton('2', 'inline_keyboard:2'),
-            InlineButton('3', 'inline_keyboard:3'),
-            InlineButton('4', 'inline_keyboard:4'),
-            InlineButton('5', 'inline_keyboard:5'),
-            InlineButton('6', 'inline_keyboard:6'),
-            InlineButton('7', 'inline_keyboard:7')
-        )
-        ```
-        
-        #### ʀᴇsᴜʟᴛ
-        
-        <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
-        
-        ━━━━━━━━━━━━━━━━━━━━
-        ### Configuratoins
-        ```
-        OWNER_ID = ʏᴏᴜʀ ᴛᴇʟᴇɢʀᴀᴍ ɪᴅ.
-        DEV_USERS = ʙᴏᴛ ᴅᴇᴠs ɪᴅ. (ʏᴏᴜ ᴄᴀɴ ᴀᴅᴅ ᴀ ʟɪsᴛ : 1 2 3)
-        LOGGER_ID = ʏᴏᴜʀ ᴘʀɪᴠᴀᴛᴇ ɢʀᴏᴜᴘ/ᴄʜᴀɴɴᴇʟ ɪᴅ. (ʜᴇʀᴇ ʙᴏᴛ sᴇɴᴅ ʟᴏɢs)
-        ```
-        ━━━━━━━━━━━━━━━━━━━━ 
-        
-        
 Keywords: add-on pyrogram bots telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch https
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -138,7 +30,115 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+<b> ABG </b>
+</p>
+
+<p align="center"><a href="https://pepy.tech/project/abg"> <img src="https://static.pepy.tech/personalized-badge/abg?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads" width="169" height="29.69"/></a></p>
+
+### Requirements 
+
+- Python 3.7 ᴏʀ higher.
+- A [ᴛᴇʟᴇɢʀᴀᴍ ᴀᴘɪ ᴋᴇʏ](https://docs.pyrogram.org/intro/setup#api-keys).
+- ᴀʙɢ [ᴄᴏɴғɪɢ](https://github.com/Abishnoi69/Abg#configuratoins).
+
+### Installing :
+
+```bash
+pip install -U Abg
+```
+#### sᴇᴛᴜᴘ
+```python
+from pyrogram import filters, Client
+from pyrogram.types import CallbackQuery, Message
+from Abg import patch  # type : ignore
+from Abg.helpers import ikb
+
+app = Client("my_account")
+
+@app.on_cmd("myinfo")
+Resultdef my_info(self: Client, ctx: Message):
+    if not ctx.from_user:
+        return
+    name = await ctx.chat.ask("Type Your Name")
+    age = await ctx.chat.ask("Type your age")
+    add = await ctx.chat.ask("Type your address")
+    # you can also use : ctx.reply_text(...)
+    await self.send_msg(
+        chat_id=ctx.chat.id,
+        text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+        reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
+    )
+
+# callback 
+@app.on_cb("hello")
+async def hello(c: Client, q: CallbackQuery):
+    await q.answer("Hello From Abg", show_alert=True)
+
+  app.run()
+```
+>
+#### ᴜsᴇʀ/ʙᴏᴛ ʀɪɢʜᴛs 
+
+```python
+from Abg import patch  # all patch
+from pyrogram.types import Message
+from pyrogram import Client
+
+app = Client("my_account")
+
+@app.on_cmd("del", group_only=True)
+@app.adminsOnly(permissions="can_delete_messages", is_both=True)
+async def del_msg(c: Client, m: Message):
+    if m.reply_to_message:
+        await m.delete()
+        await c.delete_messages(
+            chat_id=m.chat.id,
+            message_ids=m.reply_to_message.id,
+        )
+    else:
+        await m.reply_text(text="ᴡʜᴀᴛ ᴅᴏ ʏᴏᴜ ᴡᴀɴɴᴀ ᴅᴇʟᴇᴛᴇ?")
+    return
+  
+  app.run()
+```
+
+
+>
+### keyboard's
+
+```python
+from Abg.inline import InlineKeyboard, InlineButton
+
+
+keyboard = InlineKeyboard(row_width=3)
+keyboard.add(
+    InlineButton('1', 'inline_keyboard:1'),
+    InlineButton('2', 'inline_keyboard:2'),
+    InlineButton('3', 'inline_keyboard:3'),
+    InlineButton('4', 'inline_keyboard:4'),
+    InlineButton('5', 'inline_keyboard:5'),
+    InlineButton('6', 'inline_keyboard:6'),
+    InlineButton('7', 'inline_keyboard:7')
+)
+```
+
+#### ʀᴇsᴜʟᴛ
+
+<p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
+
+━━━━━━━━━━━━━━━━━━━━
+### Configuratoins
+```
+OWNER_ID = ʏᴏᴜʀ ᴛᴇʟᴇɢʀᴀᴍ ɪᴅ.
+DEV_USERS = ʙᴏᴛ ᴅᴇᴠs ɪᴅ. (ʏᴏᴜ ᴄᴀɴ ᴀᴅᴅ ᴀ ʟɪsᴛ : 1 2 3)
+LOGGER_ID = ʏᴏᴜʀ ᴘʀɪᴠᴀᴛᴇ ɢʀᴏᴜᴘ/ᴄʜᴀɴɴᴇʟ ɪᴅ. (ʜᴇʀᴇ ʙᴏᴛ sᴇɴᴅ ʟᴏɢs)
+```
+━━━━━━━━━━━━━━━━━━━━ 
+
```

#### html2text {}

```diff
@@ -1,14 +1,31 @@
-Metadata-Version: 2.1 Name: Abg Version: 2.3.4 Summary: add-on for Pyrogram ||
+Metadata-Version: 2.1 Name: Abg Version: 2.3.5 Summary: add-on for Pyrogram ||
 Telegram bot helpers || Easy botting Home-page: https://github.com/Abishnoi69/
-Abg Author: Abishnoi Author-email: Abishnoi69@Abg.org License: MIT Download-
-URL: https://github.com/Abishnoi69/Abg/releases/latest Project-URL: Tracker,
+Abg Download-URL: https://github.com/Abishnoi69/Abg/releases/latest Author:
+Abishnoi Author-email: Abishnoi69@Abg.org License: MIT Project-URL: Tracker,
 https://github.com/Abishnoi69/Abg/issues Project-URL: Community, https://t.me/
 Abgpy Project-URL: Source, https://github.com/Abishnoi69/Abg Project-URL:
-Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce Description:
+Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce Keywords:
+add-on pyrogram bots telegram bot chat messenger mtproto api client library
+python conversation keyboard userbot patch https Classifier: Development Status
+:: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation Classifier: Programming Language :: Python
+:: Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Internet Classifier: Topic ::
+Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Libraries :: Application Frameworks Requires-Python: ~=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE
                                       ABG
                  [https://static.pepy.tech/personalized-badge/
 abg?period=total&units=international_system&left_color=black&right_color=black&left_text=Downloads]
 ### Requirements - Python 3.7 á´Ê higher. - A [á´á´Êá´É¢Êá´á´ á´á´Éª
 á´á´Ê](https://docs.pyrogram.org/intro/setup#api-keys). - á´ÊÉ¢
 [á´á´É´ÒÉªÉ¢](https://github.com/Abishnoi69/Abg#configuratoins). ###
 Installing : ```bash pip install -U Abg ``` #### sá´á´á´á´ ```python from
@@ -38,25 +55,8 @@
 'inline_keyboard:7') ) ``` #### Êá´sá´Êá´
 [add_inline_button]
 ââââââââââââââââââââ ### Configuratoins
 ``` OWNER_ID = Êá´á´Ê á´á´Êá´É¢Êá´á´ Éªá´. DEV_USERS = Êá´á´
 á´á´á´ s Éªá´. (Êá´á´ á´á´É´ á´á´á´ á´ ÊÉªsá´ : 1 2 3) LOGGER_ID
 = Êá´á´Ê á´ÊÉªá´ á´á´á´ É¢Êá´á´á´/á´Êá´É´É´á´Ê Éªá´.
 (Êá´Êá´ Êá´á´ sá´É´á´ Êá´É¢s) ```
-ââââââââââââââââââââ Keywords: add-on
-pyrogram bots telegram bot chat messenger mtproto api client library python
-conversation keyboard userbot patch https Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: Implementation Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown
+ââââââââââââââââââââ
```

### Comparing `Abg-2.3.4/README.md` & `Abg-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `Abg-2.3.4/setup.py` & `Abg-2.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     requires = f.read().splitlines()
 """
 
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="2.3.4",
+    version="2.3.5",
     description="add-on for Pyrogram || Telegram bot helpers || Easy botting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69/Abg",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi",
     author_email="Abishnoi69@Abg.org",
@@ -68,9 +68,9 @@
         "Tracker": "https://github.com/Abishnoi69/Abg/issues",
         "Community": "https://t.me/Abgpy",
         "Source": "https://github.com/Abishnoi69/Abg",
         "Documentation": "https://github.com/Abishnoi69/Abg/tree/master/doce",
     },
     python_requires="~=3.7",
     zip_safe=False,
-    # install_requires=requires,
+    install_requires=["pytz>=2023.3", "cachetools>=5.3.1"],
 )
```

