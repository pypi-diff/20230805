# Comparing `tmp/etm-dgraham-5.1.7.tar.gz` & `tmp/etm-dgraham-5.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.1.7.tar", last modified: Fri Jun 23 00:25:30 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.8.tar", last modified: Fri Jun 23 18:33:08 2023, max compression
```

## Comparing `etm-dgraham-5.1.7.tar` & `etm-dgraham-5.1.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.105715 etm-dgraham-5.1.7/
--rw-r--r--   0 dag        (501) staff       (20)     2411 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   132192 2023-06-23 00:25:30.105573 etm-dgraham-5.1.7/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   131280 2023-06-21 13:13:42.000000 etm-dgraham-5.1.7/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.7/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.7/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.097038 etm-dgraham-5.1.7/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.101449 etm-dgraham-5.1.7/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.7/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.7/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.7/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.7/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   287838 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.7/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.7/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   100599 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.103942 etm-dgraham-5.1.7/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   132192 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.7/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.7/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-23 00:25:30.105751 etm-dgraham-5.1.7/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.7/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.104038 etm-dgraham-5.1.7/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.7/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.105106 etm-dgraham-5.1.7/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.7/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.7/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.7/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 18:33:08.567089 etm-dgraham-5.1.8/
+-rw-r--r--   0 dag        (501) staff       (20)     2409 2023-06-23 18:33:00.000000 etm-dgraham-5.1.8/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.8/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132192 2023-06-23 18:33:08.566942 etm-dgraham-5.1.8/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131280 2023-06-21 13:13:42.000000 etm-dgraham-5.1.8/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.8/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.8/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 18:33:08.558951 etm-dgraham-5.1.8/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.8/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.8/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.8/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 18:33:08.562608 etm-dgraham-5.1.8/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.8/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.8/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-23 18:33:00.000000 etm-dgraham-5.1.8/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.8/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.8/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.8/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   288753 2023-06-23 18:33:00.000000 etm-dgraham-5.1.8/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.8/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.8/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100605 2023-06-23 18:33:00.000000 etm-dgraham-5.1.8/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 18:33:08.565297 etm-dgraham-5.1.8/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132192 2023-06-23 18:33:08.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-23 18:33:08.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-23 18:33:08.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-23 18:33:08.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-23 18:33:08.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-23 18:33:08.000000 etm-dgraham-5.1.8/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.8/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.8/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.8/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.8/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.8/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.8/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-23 18:33:08.567122 etm-dgraham-5.1.8/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.8/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 18:33:08.565390 etm-dgraham-5.1.8/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.8/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 18:33:08.566449 etm-dgraham-5.1.8/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.8/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.8/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.8/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.8/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.1.7/CHANGES.txt` & `etm-dgraham-5.1.8/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-Recent tagged changes as of 2023-06-22T20:25:12.409983-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.1.7) Daniel Graham
+Recent tagged changes as of 2023-06-23T14:32:58.480420-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.1.8) Daniel Graham
+    3d22710 2023-06-23 14:32:58 -0400
+    Tagged version 5.1.8.
+
+- 18 hours ago (tag: 5.1.7) Daniel Graham
     fe31c71 2023-06-22 20:25:12 -0400
     Tagged version 5.1.7.
 
-- 30 hours ago (tag: 5.1.6) Daniel Graham
+- 2 days ago (tag: 5.1.6) Daniel Graham
     9c70c17 2023-06-21 14:33:46 -0400
     Tagged version 5.1.6.
 
-- 35 hours ago (tag: 5.1.5) Daniel Graham
+- 2 days ago (tag: 5.1.5) Daniel Graham
     17d91e2 2023-06-21 09:13:39 -0400
     Tagged version 5.1.5.
 
-- 3 days ago (tag: 5.1.4) Daniel Graham
+- 4 days ago (tag: 5.1.4) Daniel Graham
     84421ec 2023-06-19 13:40:16 -0400
     Tagged version 5.1.4.
 
-- 3 days ago (tag: 5.1.3) Daniel Graham
+- 4 days ago (tag: 5.1.3) Daniel Graham
     c776097 2023-06-19 11:40:16 -0400
     Tagged version 5.1.3.
 
 - 4 days ago (tag: 5.1.2) Daniel Graham
     3483b69 2023-06-19 05:51:42 -0400
     Tagged version 5.1.2.
 
@@ -28,40 +32,40 @@
     Tagged version 5.1.1.
 
 - 5 days ago (tag: 5.1.0) Daniel Graham
     ece86e8 2023-06-18 07:28:25 -0400
     Tagged version 5.1.0. Added ability to display completion history
     for tasks including skipped instead of finished instances.
 
-- 5 days ago (tag: 5.0.12) Daniel Graham
+- 6 days ago (tag: 5.0.12) Daniel Graham
     c42576c 2023-06-17 08:57:03 -0400
     Tagged version 5.0.12.
 
 - 6 days ago (tag: 5.0.11) Daniel Graham
     e9228d2 2023-06-17 05:19:31 -0400
     Tagged version 5.0.11.
 
 - 6 days ago (tag: 5.0.10) Daniel Graham
     2e1f579 2023-06-17 05:05:32 -0400
     Tagged version 5.0.10.
 
-- 7 days ago (tag: 5.0.9) Daniel Graham
+- 8 days ago (tag: 5.0.9) Daniel Graham
     7f30e8b 2023-06-15 10:14:19 -0400
     Tagged version 5.0.9.
 
-- 9 days ago (tag: 5.0.8) Daniel Graham
+- 10 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
 - 2 weeks ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
 
-- 2 weeks ago (tag: 5.0.6) Daniel Graham
+- 3 weeks ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
 - 3 weeks ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
@@ -72,11 +76,7 @@
 - 3 weeks ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
 - 3 weeks ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
-
-- 3 weeks ago (tag: 5.0.1) Daniel Graham
-    b30f0ed 2023-06-04 12:47:15 -0400
-    Tagged version 5.0.1.
```

### Comparing `etm-dgraham-5.1.7/PKG-INFO` & `etm-dgraham-5.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.7
+Version: 5.1.8
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.7/README.md` & `etm-dgraham-5.1.8/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/bump.py` & `etm-dgraham-5.1.8/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/docs/index_konnections.md` & `etm-dgraham-5.1.8/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/docs/index_usedtime.md` & `etm-dgraham-5.1.8/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/docs/multiple_timers.md` & `etm-dgraham-5.1.8/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm/__main__.py` & `etm-dgraham-5.1.8/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm/data.py` & `etm-dgraham-5.1.8/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm/ical.py` & `etm-dgraham-5.1.8/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm/make_examples.py` & `etm-dgraham-5.1.8/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm/model.py` & `etm-dgraham-5.1.8/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -852,24 +852,26 @@
                 #     save_item = True
 
         else:
             # no jobs
             if 's' in self.item_hsh:
                 if 'r' in self.item_hsh:
                     nxt = get_next_due(self.item_hsh, completed_datetime, completion_entry.end)
+                    # logger.debug(f"nxt: {nxt}")
                     if nxt:
                         for i in range(len(self.item_hsh['r'])):
                             if 'c' in self.item_hsh['r'][i] and self.item_hsh['r'][i]['c'] > 0:
                                 self.item_hsh['r'][i]['c'] -= 1
                                 break
                         self.item_hsh['s'] = nxt
 
                         self.item_hsh.setdefault('h', []).append(completion_entry)
                         save_item = True
                     else:  # finished last instance
+                        # logger.debug(f"not nxt, finished last instance")
                         self.item_hsh['f'] = completion_entry
                         save_item = True
 
                 elif '+' in self.item_hsh:
                     # simple repetition
                     tmp = [self.item_hsh['s']] + self.item_hsh['+']
                     tmp = [date_to_datetime(x) for x in tmp]
@@ -1018,15 +1020,15 @@
         self.item_hsh = {'created': created}
         cur_hsh = {}
         cur_key = None
         msg = []
         for pos, (k, v) in self.pos_hsh.items():
             obj = self.object_hsh.get((k, v))
             if obj is None:
-                logger.debug(f"got None for {k}, {v}")
+                # logger.debug(f"got None for {k}, {v}")
                 msg.append(f"bad entry for {k}: {v}")
                 return msg
                 # continue
             elif k in ['a', 'u', 'n', 't', 'k']:
                 self.item_hsh.setdefault(k, []).append(obj)
             elif k in ['rr', 'jj']:
                 if cur_hsh:
@@ -1955,28 +1957,33 @@
     end = obj.end
     neg = start > end
     if neg:
         diff = start - end
     else:
         diff = end - start
     until = []
+    weeks = diff.in_weeks()
     days = diff.remaining_days
     hours = diff.hours
     minutes = diff.minutes
     if neg:
         until.append("-")
     else:
         until.append("+")
+    tmp = []
+    if weeks:
+        until.append(f"{weeks}w")
     if days:
         until.append(f"{days}d")
     if hours:
         until.append(f"{hours}h")
     if minutes:
         until.append(f"{minutes}m")
-    return "".join(until)
+    # keep the sign and the 2 most significant
+    return "".join(until[:3])
 
 
 def format_duration_list(obj_lst):
     try:
         return ", ".join([format_duration(x) for x in obj_lst])
     except Exception as e:
         logger.error(f"{obj_lst}: {e}")
@@ -3046,47 +3053,51 @@
         item_id = res[0]
 
         if not (item_id and item_id in self.id2relevant):
             return ''
         showing = "Completion History"
         item = DBITEM.get(doc_id=item_id)
 
-        if not (item['itemtype'] == '-' and ('r' in item or '+' in item)):
-            return showing, "not a repeating task"
-        if 'h' not in item:
+        # if not (item['itemtype'] == '-' and ('r' in item or '+' in item)):
+        #     return showing, "not a repeating task"
+        if 'h' not in item and 'f' not in item:
             return showing, "there is no history of completions"
 
         relevant = self.id2relevant.get(item_id)
         res = []
         skip = item.get('o', 'k') == 's'
-        for c in item['h']:
+        if 'f' in item:
+            per = item['f']
+            res.append((per.end, f" {fmt_period(per)}", FINISHED_CHAR))
+        for c in item.get('h', []):
             if skip and c.start == c.end + ONEMIN:
                 res.append((c.end, "", SKIPPED_CHAR))
             else:
                 # due at 12am, change the effective due date to 12am of the following day
                 per = pendulum.period(c.start, c.end + DAY)
-                res.append((c.end, f" ({fmt_period(per)})", FINISHED_CHAR))
+                res.append((c.end, f" {fmt_period(per)}", FINISHED_CHAR))
         res.sort() # pendulum.DateTime obj as first component
         if len(res) > num:
             showing = f"Completion History: last {num} of {len(res)}"
             res = res[-num:]
         else:
             showing = f"Completion History"
         relevant = res[-1][0]
         details = f"{item['itemtype']} {item['summary']}"
 
         pairs = [f"{x[2]} {format_datetime(x[0])[1]}{x[1]}" for x in res]
         starting = format_datetime(relevant.date())[1]
 
         ps = f"\n\nSkipped instances are marked with a {SKIPPED_CHAR}." if skip else "\n"
-        pss = """
-Datetimes at which an instance was due are
-listed together with the period (+/-) from
-the completion until the due datetime in
-parentheses.
+        pss = f"""
+Completed instances are marked with a {FINISHED_CHAR}
+and listed by due datetimes followed
+by the period by which the completion
+datetime preceded (+) or followed (-)
+the due datetime.
 """
 
         return  showing, f"through {starting} for\n{details}:\n  " + "\n  ".join(pairs) + ps + pss
 
     def touch(self, row):
         res = self.get_row_details(row)
         if not res:
@@ -4797,19 +4808,25 @@
     lofh = item.get('r')
     if not lofh:
         return ''
     rset = rruleset()
     overdue = item.get('o', 'k') # make 'k' the default for 'o'
     start = item['s']
     dtstart = date_to_datetime(item['s'])
+    # logger.debug(f"done: {done}, due: {due}, dtstart: {dtstart}")
     if due > dtstart:
         # we've finished a between instance
+        # logger.debug(f"between, returning dtstart: {dtstart}")
         return dtstart
     # we're finishing the oldest instance
+    h = [x.end for x in item.get('h', [])]
+    h.sort()
+
     due = dtstart if not due else due
+
     if overdue == 'k':
         aft = due
         inc = False
     elif overdue == 'r':
         aft = done
         dtstart = done
         inc = False
@@ -4830,30 +4847,38 @@
         kwd['dtstart'] = dtstart
         try:
             rset.rrule(rrule(freq, **kwd))
         except Exception as e:
             logger.error(f"error processing {hsh}: {e}")
             return []
 
-    if '-' in item:
-        for dt in item['-']:
-            rset.exdate(dt)
-
-    if '+' in item:
-        for dt in item['+']:
-            rset.rdate(dt)
-    nxt_rset = rset.after(aft, inc)
+    plus = item.get('+', [])
+    hist = [x.end for x in item.get('h', [])]
+    minus = item.get('-', [])
+    minus_hist = hist + minus
+
+    plus_not_minus = list(set(plus) - set(minus_hist))
+    minus_not_plus = list(set(minus_hist) - set(plus))
+
+    for dt in minus_not_plus:
+        rset.exdate(date_to_datetime(dt))
+
+    for dt in plus_not_minus:
+        rset.rdate(date_to_datetime(dt))
+
+    nxt_rset = rset.after(date_to_datetime(aft), inc)
     if nxt_rset:
         nxt = pendulum.instance(nxt_rset)
         if using_dates:
             nxt = nxt.date()
     else:
         nxt = None
     return nxt
 
+
 def date_to_datetime(dt, hour=0, minute=0):
     if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
         dt= pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=hour, minute=minute, tz='local')
     return dt
 
 
 def item_instances(item, aft_dt, bef_dt=1, honor_skip=True):
```

### Comparing `etm-dgraham-5.1.7/etm/options.py` & `etm-dgraham-5.1.8/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm/report.py` & `etm-dgraham-5.1.8/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm/view.py` & `etm-dgraham-5.1.8/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1423,17 +1423,17 @@
                 current_datetime = status_time(now)
                 today = now.format("YYYYMMDD")
 
                 if updates_interval and minutes % updates_interval == 0:
                     loop = asyncio.get_event_loop()
                     asyncio.ensure_future(updates_loop(loop))
 
-                if minutes % 5 == 0:
-                    loop = asyncio.get_event_loop()
-                    asyncio.ensure_future(refresh_loop(loop))
+                # if minutes % 5 == 0:
+                #     loop = asyncio.get_event_loop()
+                #     asyncio.ensure_future(refresh_loop(loop))
 
                 if today != current_today:
                     loop = asyncio.get_event_loop()
                     asyncio.ensure_future(new_day(loop))
 
             asyncio.ensure_future(save_timers())
             if dataview.active_view == 'timers':
```

### Comparing `etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.8/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.7
+Version: 5.1.8
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.8/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.8/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etmlogo.png` & `etm-dgraham-5.1.8/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etmlogo_small.png` & `etm-dgraham-5.1.8/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/etmview_agenda.png` & `etm-dgraham-5.1.8/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/namedcolors.py` & `etm-dgraham-5.1.8/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/new.png` & `etm-dgraham-5.1.8/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/setup.py` & `etm-dgraham-5.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/test/test_parser.py` & `etm-dgraham-5.1.8/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.8/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/utilities/etm_in` & `etm-dgraham-5.1.8/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/utilities/inbasket` & `etm-dgraham-5.1.8/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.7/utilities/open_in_mutt` & `etm-dgraham-5.1.8/utilities/open_in_mutt`

 * *Files identical despite different names*

