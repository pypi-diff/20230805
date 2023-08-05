# Comparing `tmp/find-ff-601.tar.gz` & `tmp/find-ff-603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find-ff-601.tar", last modified: Sat Aug 21 11:56:18 2021, max compression
+gzip compressed data, was "find-ff-603.tar", last modified: Sat Aug  5 13:16:21 2023, max compression
```

## Comparing `find-ff-601.tar` & `find-ff-603.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.093301 find-ff-601/
--rw-r--r--   0 lars      (1000) lars      (1000)    35149 2020-05-08 05:04:20.000000 find-ff-601/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)     3198 2021-08-21 11:56:18.093301 find-ff-601/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     2459 2021-04-07 09:17:57.000000 find-ff-601/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.086634 find-ff-601/bin/
--rwxr-xr-x   0 lars      (1000) lars      (1000)     1506 2020-06-30 06:38:14.000000 find-ff-601/bin/ff
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.086634 find-ff-601/ff/
--rw-r--r--   0 lars      (1000) lars      (1000)      966 2020-06-30 06:38:14.000000 find-ff-601/ff/__init__.py
--rw-r--r--   0 lars      (1000) lars      (1000)      951 2020-10-03 06:47:48.000000 find-ff-601/ff/__main__.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.086634 find-ff-601/find_ff.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     3198 2021-08-21 11:56:17.000000 find-ff-601/find_ff.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      946 2021-08-21 11:56:17.000000 find-ff-601/find_ff.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2021-08-21 11:56:17.000000 find-ff-601/find_ff.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       23 2021-08-21 11:56:17.000000 find-ff-601/find_ff.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2021-08-21 11:56:17.000000 find-ff-601/find_ff.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.089968 find-ff-601/libff/
--rw-r--r--   0 lars      (1000) lars      (1000)     2709 2020-10-03 07:34:01.000000 find-ff-601/libff/__init__.py
--rw-r--r--   0 lars      (1000) lars      (1000)      914 2021-08-21 11:55:36.000000 find-ff-601/libff/__version__.py
--rw-r--r--   0 lars      (1000) lars      (1000)    14916 2021-04-09 03:41:08.000000 find-ff-601/libff/argparse.py
--rw-r--r--   0 lars      (1000) lars      (1000)    16698 2021-04-09 03:58:55.000000 find-ff-601/libff/arguments.py
--rw-r--r--   0 lars      (1000) lars      (1000)     1634 2020-06-30 06:38:14.000000 find-ff-601/libff/attribute.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.093301 find-ff-601/libff/builtin/
--rw-r--r--   0 lars      (1000) lars      (1000)      895 2020-06-30 06:38:14.000000 find-ff-601/libff/builtin/__init__.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4422 2020-06-30 06:38:14.000000 find-ff-601/libff/builtin/file.py
--rw-r--r--   0 lars      (1000) lars      (1000)     1888 2020-10-03 07:29:37.000000 find-ff-601/libff/builtin/grep.py
--rw-r--r--   0 lars      (1000) lars      (1000)     3141 2021-04-09 03:57:43.000000 find-ff-601/libff/builtin/ignore.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4977 2020-10-03 07:30:14.000000 find-ff-601/libff/builtin/media.py
--rw-r--r--   0 lars      (1000) lars      (1000)     2514 2020-10-03 07:29:21.000000 find-ff-601/libff/builtin/mime.py
--rw-r--r--   0 lars      (1000) lars      (1000)     7188 2020-06-30 06:38:14.000000 find-ff-601/libff/cache.py
--rw-r--r--   0 lars      (1000) lars      (1000)    10427 2021-08-21 11:49:31.000000 find-ff-601/libff/console.py
--rw-r--r--   0 lars      (1000) lars      (1000)     5833 2021-08-21 11:50:11.000000 find-ff-601/libff/context.py
--rw-r--r--   0 lars      (1000) lars      (1000)     5340 2021-04-07 09:21:56.000000 find-ff-601/libff/convert.py
--rw-r--r--   0 lars      (1000) lars      (1000)    11957 2020-10-03 07:30:37.000000 find-ff-601/libff/entry.py
--rw-r--r--   0 lars      (1000) lars      (1000)     2304 2020-06-30 06:38:14.000000 find-ff-601/libff/exceptions.py
--rw-r--r--   0 lars      (1000) lars      (1000)    10674 2021-04-04 12:35:57.000000 find-ff-601/libff/field.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4801 2020-06-30 06:38:14.000000 find-ff-601/libff/filter.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4453 2021-04-09 03:59:10.000000 find-ff-601/libff/find.py
--rw-r--r--   0 lars      (1000) lars      (1000)    13131 2020-10-03 07:32:53.000000 find-ff-601/libff/help.py
--rw-r--r--   0 lars      (1000) lars      (1000)     7803 2021-04-09 11:47:37.000000 find-ff-601/libff/ignore.py
--rw-r--r--   0 lars      (1000) lars      (1000)     3422 2020-06-30 06:38:14.000000 find-ff-601/libff/logger.py
--rw-r--r--   0 lars      (1000) lars      (1000)    11527 2021-04-09 03:40:20.000000 find-ff-601/libff/main.py
--rw-r--r--   0 lars      (1000) lars      (1000)    15949 2021-04-09 03:30:44.000000 find-ff-601/libff/manpage.template
--rw-r--r--   0 lars      (1000) lars      (1000)    11488 2020-10-03 07:36:44.000000 find-ff-601/libff/parser.py
--rw-r--r--   0 lars      (1000) lars      (1000)     1912 2021-04-09 04:31:01.000000 find-ff-601/libff/path.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4615 2020-06-30 06:38:14.000000 find-ff-601/libff/plugin.py
--rw-r--r--   0 lars      (1000) lars      (1000)    13160 2021-04-04 15:31:30.000000 find-ff-601/libff/processing.py
--rw-r--r--   0 lars      (1000) lars      (1000)    13676 2021-04-09 05:16:37.000000 find-ff-601/libff/registry.py
--rw-r--r--   0 lars      (1000) lars      (1000)    15054 2021-04-07 07:55:17.000000 find-ff-601/libff/type.py
--rw-r--r--   0 lars      (1000) lars      (1000)     9552 2021-04-09 03:48:19.000000 find-ff-601/libff/walk.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.093301 find-ff-601/man/
--rw-r--r--   0 lars      (1000) lars      (1000)    22237 2021-08-21 11:56:11.000000 find-ff-601/man/ff.1
--rw-r--r--   0 lars      (1000) lars      (1000)    10306 2021-08-21 11:56:11.000000 find-ff-601/man/ff.7
--rw-r--r--   0 lars      (1000) lars      (1000)     6358 2020-06-28 07:23:36.000000 find-ff-601/plugin_template.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2021-08-21 11:56:18.093301 find-ff-601/plugins/
--rw-r--r--   0 lars      (1000) lars      (1000)     5714 2020-06-30 06:38:14.000000 find-ff-601/plugins/fs.py
--rw-r--r--   0 lars      (1000) lars      (1000)     4238 2020-06-30 06:38:14.000000 find-ff-601/plugins/git.py
--rw-r--r--   0 lars      (1000) lars      (1000)     5225 2020-10-03 07:32:08.000000 find-ff-601/plugins/introspect.py
--rw-r--r--   0 lars      (1000) lars      (1000)     2183 2020-06-30 06:38:14.000000 find-ff-601/plugins/pacman.py
--rw-r--r--   0 lars      (1000) lars      (1000)     2047 2020-10-03 07:31:04.000000 find-ff-601/plugins/tar.py
--rw-r--r--   0 lars      (1000) lars      (1000)     1257 2020-08-07 05:12:52.000000 find-ff-601/plugins/test.py
--rw-r--r--   0 lars      (1000) lars      (1000)     1739 2020-06-30 06:38:14.000000 find-ff-601/plugins/xattr.py
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2021-08-21 11:56:18.093301 find-ff-601/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)     2604 2020-07-21 10:00:05.000000 find-ff-601/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.603324 find-ff-603/
+-rw-r--r--   0 lars      (1000) lars      (1000)    35149 2020-05-08 05:04:20.000000 find-ff-603/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)     3178 2023-08-05 13:16:21.603324 find-ff-603/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     2459 2021-04-07 09:17:57.000000 find-ff-603/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.593323 find-ff-603/bin/
+-rwxr-xr-x   0 lars      (1000) lars      (1000)     1506 2020-06-30 06:38:14.000000 find-ff-603/bin/ff
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.593323 find-ff-603/ff/
+-rw-r--r--   0 lars      (1000) lars      (1000)      966 2020-06-30 06:38:14.000000 find-ff-603/ff/__init__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)      951 2020-10-03 06:47:48.000000 find-ff-603/ff/__main__.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.593323 find-ff-603/find_ff.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     3178 2023-08-05 13:16:21.000000 find-ff-603/find_ff.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      946 2023-08-05 13:16:21.000000 find-ff-603/find_ff.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-08-05 13:16:21.000000 find-ff-603/find_ff.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       23 2023-08-05 13:16:21.000000 find-ff-603/find_ff.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-08-05 13:16:21.000000 find-ff-603/find_ff.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.599990 find-ff-603/libff/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2709 2020-10-03 07:34:01.000000 find-ff-603/libff/__init__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)      914 2023-08-05 13:15:35.000000 find-ff-603/libff/__version__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    14916 2021-04-09 03:41:08.000000 find-ff-603/libff/argparse.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    16698 2021-04-09 03:58:55.000000 find-ff-603/libff/arguments.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     1634 2020-06-30 06:38:14.000000 find-ff-603/libff/attribute.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.603324 find-ff-603/libff/builtin/
+-rw-r--r--   0 lars      (1000) lars      (1000)      895 2020-06-30 06:38:14.000000 find-ff-603/libff/builtin/__init__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4422 2020-06-30 06:38:14.000000 find-ff-603/libff/builtin/file.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     1938 2023-08-05 13:11:46.000000 find-ff-603/libff/builtin/grep.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     3141 2021-04-09 03:57:43.000000 find-ff-603/libff/builtin/ignore.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4961 2023-08-05 13:11:46.000000 find-ff-603/libff/builtin/media.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     2498 2023-08-05 13:11:46.000000 find-ff-603/libff/builtin/mime.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     7188 2020-06-30 06:38:14.000000 find-ff-603/libff/cache.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    10427 2021-08-21 11:49:31.000000 find-ff-603/libff/console.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     5833 2021-08-21 11:50:11.000000 find-ff-603/libff/context.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     5340 2021-04-07 09:21:56.000000 find-ff-603/libff/convert.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    11957 2020-10-03 07:30:37.000000 find-ff-603/libff/entry.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     2304 2020-06-30 06:38:14.000000 find-ff-603/libff/exceptions.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    10675 2023-08-05 13:11:46.000000 find-ff-603/libff/field.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4801 2020-06-30 06:38:14.000000 find-ff-603/libff/filter.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4453 2021-04-09 03:59:10.000000 find-ff-603/libff/find.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    13177 2023-08-05 13:11:46.000000 find-ff-603/libff/help.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     7849 2023-08-05 13:11:46.000000 find-ff-603/libff/ignore.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     3422 2020-06-30 06:38:14.000000 find-ff-603/libff/logger.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    11527 2021-04-09 03:40:20.000000 find-ff-603/libff/main.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    15949 2021-04-09 03:30:44.000000 find-ff-603/libff/manpage.template
+-rw-r--r--   0 lars      (1000) lars      (1000)    11488 2020-10-03 07:36:44.000000 find-ff-603/libff/parser.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     1966 2023-08-05 13:14:03.000000 find-ff-603/libff/path.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4615 2020-06-30 06:38:14.000000 find-ff-603/libff/plugin.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    13160 2021-04-04 15:31:30.000000 find-ff-603/libff/processing.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    13676 2021-04-09 05:16:37.000000 find-ff-603/libff/registry.py
+-rw-r--r--   0 lars      (1000) lars      (1000)    15054 2021-04-07 07:55:17.000000 find-ff-603/libff/type.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     9552 2021-04-09 03:48:19.000000 find-ff-603/libff/walk.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.603324 find-ff-603/man/
+-rw-r--r--   0 lars      (1000) lars      (1000)    22237 2023-08-05 13:16:14.000000 find-ff-603/man/ff.1
+-rw-r--r--   0 lars      (1000) lars      (1000)    10306 2023-08-05 13:16:14.000000 find-ff-603/man/ff.7
+-rw-r--r--   0 lars      (1000) lars      (1000)     6358 2020-06-28 07:23:36.000000 find-ff-603/plugin_template.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-08-05 13:16:21.603324 find-ff-603/plugins/
+-rw-r--r--   0 lars      (1000) lars      (1000)     5714 2020-06-30 06:38:14.000000 find-ff-603/plugins/fs.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     4238 2020-06-30 06:38:14.000000 find-ff-603/plugins/git.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     5271 2023-08-05 13:11:46.000000 find-ff-603/plugins/introspect.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     2234 2023-08-05 13:11:46.000000 find-ff-603/plugins/pacman.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     2047 2020-10-03 07:31:04.000000 find-ff-603/plugins/tar.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     1303 2023-08-05 13:12:44.000000 find-ff-603/plugins/test.py
+-rw-r--r--   0 lars      (1000) lars      (1000)     1739 2020-06-30 06:38:14.000000 find-ff-603/plugins/xattr.py
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-08-05 13:16:21.603324 find-ff-603/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)     2604 2020-07-21 10:00:05.000000 find-ff-603/setup.py
```

### Comparing `find-ff-601/LICENSE` & `find-ff-603/LICENSE`

 * *Files identical despite different names*

### Comparing `find-ff-601/PKG-INFO` & `find-ff-603/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: find-ff
-Version: 601
+Version: 603
 Summary: A tool for finding files in the filesystem
 Home-page: https://github.com/gustaebel/ff/
 Author: Lars Gustäbel
 Author-email: lars@gustaebel.de
 License: GPLv3+
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Filesystems
@@ -111,9 +110,7 @@
 $ python -m ff --debug info,cache ...
 ```
 
 Debug mode produces lots of messages which can be limited to certain categories
 using the `--debug category1,category2,...` option. On top of that, debug mode
 activates many internal checks using `assert()`. Therefore, it is advisable to
 use debug mode during plugin development.
-
-
```

### Comparing `find-ff-601/README.md` & `find-ff-603/README.md`

 * *Files identical despite different names*

### Comparing `find-ff-601/bin/ff` & `find-ff-603/bin/ff`

 * *Files identical despite different names*

### Comparing `find-ff-601/ff/__init__.py` & `find-ff-603/ff/__init__.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/ff/__main__.py` & `find-ff-603/ff/__main__.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/find_ff.egg-info/PKG-INFO` & `find-ff-603/find_ff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: find-ff
-Version: 601
+Version: 603
 Summary: A tool for finding files in the filesystem
 Home-page: https://github.com/gustaebel/ff/
 Author: Lars Gustäbel
 Author-email: lars@gustaebel.de
 License: GPLv3+
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Filesystems
@@ -111,9 +110,7 @@
 $ python -m ff --debug info,cache ...
 ```
 
 Debug mode produces lots of messages which can be limited to certain categories
 using the `--debug category1,category2,...` option. On top of that, debug mode
 activates many internal checks using `assert()`. Therefore, it is advisable to
 use debug mode during plugin development.
-
-
```

### Comparing `find-ff-601/find_ff.egg-info/SOURCES.txt` & `find-ff-603/find_ff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/__init__.py` & `find-ff-603/libff/__init__.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/__version__.py` & `find-ff-603/libff/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 # -----------------------------------------------------------------------
 
-__version__ = 601
+__version__ = 603
```

### Comparing `find-ff-601/libff/argparse.py` & `find-ff-603/libff/argparse.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/arguments.py` & `find-ff-603/libff/arguments.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/attribute.py` & `find-ff-603/libff/attribute.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/builtin/__init__.py` & `find-ff-603/libff/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/builtin/file.py` & `find-ff-603/libff/builtin/file.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/builtin/grep.py` & `find-ff-603/libff/builtin/grep.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ]
 
     def can_handle(self, entry):
         return entry.is_file()
 
     def process(self, entry, cached):
         try:
+            # pylint:disable=unspecified-encoding
             with open(entry.path) as fobj:
                 try:
                     lines = fobj.readlines()
                 except UnicodeDecodeError:
                     yield "text", False
                 else:
                     yield "text", True
```

### Comparing `find-ff-601/libff/builtin/ignore.py` & `find-ff-603/libff/builtin/ignore.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/builtin/media.py` & `find-ff-603/libff/builtin/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,15 @@
         ("date", String, "The date audio tag of the file."),
         ("format", String, "The format of an image ('png', 'jpeg', etc.) in case the file is an "\
                            "image."),
         ("width", Number, "The width of a visual medium (image, video) in pixel."),
         ("height", Number, "The height of a visual medium (image, video) in pixel.")
     ]
 
-    @classmethod
-    def setup(cls):
+    def setup(self):
         # pylint:disable=global-statement,import-outside-toplevel
         global pymediainfo
         try:
             import pymediainfo
         except ImportError as exc:
             raise MissingImport("pymediainfo") from exc
```

### Comparing `find-ff-601/libff/builtin/mime.py` & `find-ff-603/libff/builtin/mime.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         ("mime", String, "The full mime type of the file."),
         ("type", String, "The content type of the file, i.e. the first part of the mime type."),
         ("subtype", String, "The sub type of the file, i.e. the second part of the mime type."),
         ("encoding", String, "The encoding of the file."),
         ("name", String, "The full text description of the type of the file."),
     ]
 
-    @classmethod
-    def setup(cls):
+    def setup(self):
         # pylint:disable=global-statement,import-outside-toplevel
         global magic
         try:
             import magic
         except ImportError as exc:
             raise MissingImport("file-magic") from exc
```

### Comparing `find-ff-601/libff/cache.py` & `find-ff-603/libff/cache.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/console.py` & `find-ff-603/libff/console.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/context.py` & `find-ff-603/libff/context.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/convert.py` & `find-ff-603/libff/convert.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/entry.py` & `find-ff-603/libff/entry.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/exceptions.py` & `find-ff-603/libff/exceptions.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/field.py` & `find-ff-603/libff/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,12 +292,12 @@
 
     def store(self, argument):
         super().store(argument)
 
         if any(isinstance(field, Field) for field in self[0]):
             raise UsageError("The first part of the command must not contain placeholders!")
 
-    # pylint:disable=arguments-differ
+    # pylint:disable=arguments-renamed
     def render(self, entries):
         """Create a list of arguments from multiple Entry objects for calling a subprocess.
         """
         return ["".join(self[0])] + self.render_fields(self[1:], entries, True)
```

### Comparing `find-ff-601/libff/filter.py` & `find-ff-603/libff/filter.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/find.py` & `find-ff-603/libff/find.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/help.py` & `find-ff-603/libff/help.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
 class FullManPage(ManPage):
     """Create the ff(1) manpage.
     """
 
     def render(self):
         super().render()
 
+        # pylint:disable=unspecified-encoding
         with open(os.path.join(os.path.dirname(__file__), "manpage.template")) as lines:
             self.parse_lines(lines)
 
 
 class AttributesManPage(ManPage):
     """Create the ff(7) manpage.
     """
```

### Comparing `find-ff-601/libff/ignore.py` & `find-ff-603/libff/ignore.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,15 @@
     def __init__(self, dirname, name):
         if not dirname:
             dirname = os.sep
         assert os.path.isabs(dirname)
         self.dirname = dirname
         self.path = join(dirname, name)
 
+        # pylint:disable=unspecified-encoding
         with open(self.path) as lines:
             self.lines = list(lines)
 
         # Collect the glob patterns from the gitignore file and translate them to regular
         # expressions. We have to evaluate the patterns from the file in sequence, so in order to
         # speed up matching we compile them into groups of similar patterns which we can join into
         # one big regex. Patterns differ in whether they are inclusive or exclusive, aimed at full
```

### Comparing `find-ff-601/libff/logger.py` & `find-ff-603/libff/logger.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/main.py` & `find-ff-603/libff/main.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/manpage.template` & `find-ff-603/libff/manpage.template`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/parser.py` & `find-ff-603/libff/parser.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/path.py` & `find-ff-603/libff/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 
 def split(path:str) -> Tuple[str, str]:
     """A simpler and faster version of os.path.split().
     """
     sep:int = path.rfind(separator)
     if sep < 0:
         return "", path
+    elif sep == 0:
+        return separator, path[1:]
     else:
         return path[:sep], path[sep + 1:]
 
 def join(part1:str, part2:str) -> str:
     """A simpler and faster version of os.path.join().
     """
     if part1:
```

### Comparing `find-ff-601/libff/plugin.py` & `find-ff-603/libff/plugin.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/processing.py` & `find-ff-603/libff/processing.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/registry.py` & `find-ff-603/libff/registry.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/type.py` & `find-ff-603/libff/type.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/libff/walk.py` & `find-ff-603/libff/walk.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/man/ff.1` & `find-ff-603/man/ff.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH ff 1 "2021-08-21" "Version 601" "ff - Find files in the filesystem"
+.TH ff 1 "2023-08-05" "Version 603" "ff - Find files in the filesystem"
 .nh
 .SH NAME
 
 ff \- Find files in the filesystem
 
 
 .SH SYNOPSIS
```

### Comparing `find-ff-601/man/ff.7` & `find-ff-603/man/ff.7`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH ff 7 "2021-08-21" "Version 601" "ff Plugin Attributes Reference"
+.TH ff 7 "2023-08-05" "Version 603" "ff Plugin Attributes Reference"
 .nh
 .SH DESCRIPTION
 This is a list of all the attributes that are available. Attributes are provided by plugins. For more details on a specific plugin use '\fIff \-\-help <plugin>\fR'. Please note that if you got this help text by using '\fIman 7 ff\fR', the information you get is limited to the builtin plugins. Use '\fIff \-\-help\-attributes\fR' to get the full attribute list from all plugins that are available right now.
 
 .SH FILE PLUGIN
 
 The "file" plugin provides all essential file attributes. Among these attributes are variations of the file's path name (e.g. dirname, basename, extension) and inode information from \fBstat\fR(2) (e.g. file size, file type, modification time). The leading '\fIfile.\fR' part is optional and can be omitted.
```

### Comparing `find-ff-601/plugin_template.py` & `find-ff-603/plugin_template.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/plugins/fs.py` & `find-ff-603/plugins/fs.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/plugins/git.py` & `find-ff-603/plugins/git.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/plugins/introspect.py` & `find-ff-603/plugins/introspect.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         ("imports", ListOfStrings, "A list of module and package names that are imported "\
                                    "in a Python file.")
     ]
 
     def parse_imports(self, entry):
         """Extract the names of modules and packages that a Python script imports.
         """
+        # pylint:disable=unspecified-encoding
         with open(entry.path) as fobj:
             data = fobj.read()
 
         for node in ast.walk(ast.parse(data)):
             if isinstance(node, ast.ImportFrom):
                 if node.module is not None:
                     if node.level > 0:
```

### Comparing `find-ff-601/plugins/pacman.py` & `find-ff-603/plugins/pacman.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,21 @@
                                "installed by the package manager pacman."),
         ("pkgname", String, "Name of package the file belongs to.")
     ]
 
     def setup(self):
         self.pkglist = {}
         self.filelist = set()
-        for line in subprocess.Popen(["pacman", "-Ql"], stdout=subprocess.PIPE, text=True).stdout:
-            line = line.strip()
-            pkgname, path = line.split(None, 1)
-            path = path.rstrip(os.sep)
-            self.filelist.add(path)
-            self.pkglist.setdefault(pkgname, set()).add(path)
+        with subprocess.Popen(["pacman", "-Ql"], stdout=subprocess.PIPE, text=True) as proc:
+            for line in proc.stdout:
+                line = line.strip()
+                pkgname, path = line.split(None, 1)
+                path = path.rstrip(os.sep)
+                self.filelist.add(path)
+                self.pkglist.setdefault(pkgname, set()).add(path)
 
     def can_handle(self, entry):
         return True
 
     def process(self, entry, cached):
         if entry.path in self.filelist:
             yield "installed", True
```

### Comparing `find-ff-601/plugins/tar.py` & `find-ff-603/plugins/tar.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/plugins/test.py` & `find-ff-603/plugins/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,9 +33,10 @@
         ("foo", String, "Some test data.")
     ]
 
     def can_handle(self, entry):
         return True
 
     def process(self, entry, cached):
+        # pylint:disable=unspecified-encoding
         with open("/nonexistent"):
             pass
```

### Comparing `find-ff-601/plugins/xattr.py` & `find-ff-603/plugins/xattr.py`

 * *Files identical despite different names*

### Comparing `find-ff-601/setup.py` & `find-ff-603/setup.py`

 * *Files identical despite different names*

