# Comparing `tmp/postfix_mta_sts_resolver-1.3.0.tar.gz` & `tmp/postfix_mta_sts_resolver-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfix_mta_sts_resolver-1.3.0.tar", last modified: Fri Mar 10 20:30:34 2023, max compression
+gzip compressed data, was "postfix_mta_sts_resolver-1.4.0.tar", last modified: Sat Aug  5 14:06:49 2023, max compression
```

## Comparing `postfix_mta_sts_resolver-1.3.0.tar` & `postfix_mta_sts_resolver-1.4.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 user      (1001) users      (100)        0 2023-03-10 20:30:34.952123 postfix_mta_sts_resolver-1.3.0/
--rw-r--r--   0 user      (1001) users      (100)     1073 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/LICENSE
--rw-r--r--   0 user      (1001) users      (100)       34 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/MANIFEST.in
--rw-r--r--   0 user      (1001) users      (100)    15948 2023-03-10 20:30:34.952123 postfix_mta_sts_resolver-1.3.0/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)    14971 2022-12-24 12:26:03.000000 postfix_mta_sts_resolver-1.3.0/README.md
-drwxr-xr-x   0 user      (1001) users      (100)        0 2023-03-10 20:30:34.948123 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/
--rw-r--r--   0 user      (1001) users      (100)        0 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/__init__.py
--rwxr-xr-x   0 user      (1001) users      (100)     1210 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/__main__.py
--rw-r--r--   0 user      (1001) users      (100)     2097 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/asdnotify.py
--rw-r--r--   0 user      (1001) users      (100)     1151 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/base_cache.py
--rw-r--r--   0 user      (1001) users      (100)      139 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/constants.py
--rw-r--r--   0 user      (1001) users      (100)     5400 2023-03-10 20:26:26.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/daemon.py
--rw-r--r--   0 user      (1001) users      (100)      551 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/defaults.py
--rw-r--r--   0 user      (1001) users      (100)     1548 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/internal_cache.py
--rw-r--r--   0 user      (1001) users      (100)     4078 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/netstring.py
--rw-r--r--   0 user      (1001) users      (100)     4742 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/proactive_fetcher.py
--rw-r--r--   0 user      (1001) users      (100)     5639 2023-02-13 14:36:00.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/redis_cache.py
--rw-r--r--   0 user      (1001) users      (100)     6940 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/resolver.py
--rw-r--r--   0 user      (1001) users      (100)    11678 2022-12-24 11:36:44.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/responder.py
--rw-r--r--   0 user      (1001) users      (100)     7458 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/sqlite_cache.py
--rw-r--r--   0 user      (1001) users      (100)     7555 2023-02-13 14:36:00.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/utils.py
-drwxr-xr-x   0 user      (1001) users      (100)        0 2023-03-10 20:30:34.948123 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/
--rw-r--r--   0 user      (1001) users      (100)    15948 2023-03-10 20:30:34.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)     1332 2023-03-10 20:30:34.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) users      (100)        1 2023-03-10 20:30:34.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) users      (100)      127 2023-03-10 20:30:34.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/entry_points.txt
--rw-r--r--   0 user      (1001) users      (100)      267 2023-03-10 20:30:34.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/requires.txt
--rw-r--r--   0 user      (1001) users      (100)       25 2023-03-10 20:30:34.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) users      (100)        1 2023-03-10 20:29:53.000000 postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/zip-safe
--rw-r--r--   0 user      (1001) users      (100)       38 2023-03-10 20:30:34.952123 postfix_mta_sts_resolver-1.3.0/setup.cfg
--rw-r--r--   0 user      (1001) users      (100)     2249 2023-03-10 20:28:08.000000 postfix_mta_sts_resolver-1.3.0/setup.py
-drwxr-xr-x   0 user      (1001) users      (100)        0 2023-03-10 20:30:34.952123 postfix_mta_sts_resolver-1.3.0/tests/
--rw-r--r--   0 user      (1001) users      (100)     3665 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_asdnotify.py
--rw-r--r--   0 user      (1001) users      (100)     5293 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/tests/test_cache.py
--rw-r--r--   0 user      (1001) users      (100)     1041 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_daemon.py
--rw-r--r--   0 user      (1001) users      (100)      751 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_main.py
--rw-r--r--   0 user      (1001) users      (100)     4371 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_netstring.py
--rw-r--r--   0 user      (1001) users      (100)     4249 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/tests/test_proactive_fetcher.py
--rw-r--r--   0 user      (1001) users      (100)     4647 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_resolver.py
--rw-r--r--   0 user      (1001) users      (100)     7215 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/tests/test_responder.py
--rw-r--r--   0 user      (1001) users      (100)     2417 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_responder_expiration.py
--rw-r--r--   0 user      (1001) users      (100)     1829 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/tests/test_responder_nosni.py
--rw-r--r--   0 user      (1001) users      (100)     1832 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/tests/test_responder_strict.py
--rw-r--r--   0 user      (1001) users      (100)     3969 2022-06-10 09:02:15.000000 postfix_mta_sts_resolver-1.3.0/tests/test_responder_volatile.py
--rw-r--r--   0 user      (1001) users      (100)     3638 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_sqliteconnpool.py
--rw-r--r--   0 user      (1001) users      (100)     5078 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/test_utils.py
--rw-r--r--   0 user      (1001) users      (100)      354 2020-06-09 13:59:27.000000 postfix_mta_sts_resolver-1.3.0/tests/testdata.py
+drwxr-xr-x   0 user      (1000) users      (100)        0 2023-08-05 14:06:49.133991 postfix_mta_sts_resolver-1.4.0/
+-rw-rw-r--   0 user      (1000) users      (100)     1073 2019-11-09 11:03:38.000000 postfix_mta_sts_resolver-1.4.0/LICENSE
+-rw-r--r--   0 user      (1000) users      (100)       34 2021-03-26 00:50:45.000000 postfix_mta_sts_resolver-1.4.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) users      (100)    16003 2023-08-05 14:06:49.133991 postfix_mta_sts_resolver-1.4.0/PKG-INFO
+-rw-r--r--   0 user      (1000) users      (100)    15001 2023-08-03 20:00:17.000000 postfix_mta_sts_resolver-1.4.0/README.md
+drwxr-xr-x   0 user      (1000) users      (100)        0 2023-08-05 14:06:49.130657 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/
+-rw-rw-r--   0 user      (1000) users      (100)        0 2019-11-09 11:03:38.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/__init__.py
+-rwxrwxr-x   0 user      (1000) users      (100)     1210 2020-04-11 20:39:01.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/__main__.py
+-rw-rw-r--   0 user      (1000) users      (100)     2097 2020-01-26 14:28:30.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/asdnotify.py
+-rw-rw-r--   0 user      (1000) users      (100)     1151 2020-03-23 00:28:31.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/base_cache.py
+-rw-rw-r--   0 user      (1000) users      (100)      139 2020-03-23 00:28:31.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/constants.py
+-rw-r--r--   0 user      (1000) users      (100)     5478 2023-08-05 13:10:39.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/daemon.py
+-rw-r--r--   0 user      (1000) users      (100)      572 2023-08-03 20:00:17.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/defaults.py
+-rw-rw-r--   0 user      (1000) users      (100)     1548 2020-03-23 00:28:31.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/internal_cache.py
+-rw-r--r--   0 user      (1000) users      (100)     4078 2021-03-14 12:38:16.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/netstring.py
+-rw-r--r--   0 user      (1000) users      (100)     4518 2023-08-05 13:10:39.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/postgres_cache.py
+-rw-rw-r--   0 user      (1000) users      (100)     4742 2020-03-23 00:28:31.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/proactive_fetcher.py
+-rw-r--r--   0 user      (1000) users      (100)     5639 2023-08-03 20:00:17.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/redis_cache.py
+-rw-r--r--   0 user      (1000) users      (100)     6940 2021-03-14 02:35:35.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/resolver.py
+-rw-r--r--   0 user      (1000) users      (100)    11678 2022-08-20 23:36:08.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/responder.py
+-rw-rw-r--   0 user      (1000) users      (100)     7458 2020-03-23 00:28:31.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/sqlite_cache.py
+-rw-r--r--   0 user      (1000) users      (100)     7733 2023-08-03 20:00:17.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/utils.py
+drwxr-xr-x   0 user      (1000) users      (100)        0 2023-08-05 14:06:49.130657 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/
+-rw-r--r--   0 user      (1000) users      (100)    16003 2023-08-05 14:06:49.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) users      (100)     1375 2023-08-05 14:06:49.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) users      (100)        1 2023-08-05 14:06:49.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) users      (100)      127 2023-08-05 14:06:49.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) users      (100)      293 2023-08-05 14:06:49.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) users      (100)       25 2023-08-05 14:06:49.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) users      (100)        1 2023-07-24 16:33:58.000000 postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/zip-safe
+-rw-r--r--   0 user      (1000) users      (100)       38 2023-08-05 14:06:49.133991 postfix_mta_sts_resolver-1.4.0/setup.cfg
+-rw-r--r--   0 user      (1000) users      (100)     2288 2023-08-05 13:10:56.000000 postfix_mta_sts_resolver-1.4.0/setup.py
+drwxr-xr-x   0 user      (1000) users      (100)        0 2023-08-05 14:06:49.133991 postfix_mta_sts_resolver-1.4.0/tests/
+-rw-rw-r--   0 user      (1000) users      (100)     3665 2020-01-14 23:10:18.000000 postfix_mta_sts_resolver-1.4.0/tests/test_asdnotify.py
+-rw-r--r--   0 user      (1000) users      (100)     6366 2023-08-05 13:10:39.000000 postfix_mta_sts_resolver-1.4.0/tests/test_cache.py
+-rw-rw-r--   0 user      (1000) users      (100)     1041 2019-11-09 11:03:39.000000 postfix_mta_sts_resolver-1.4.0/tests/test_daemon.py
+-rw-rw-r--   0 user      (1000) users      (100)      751 2019-11-09 11:03:39.000000 postfix_mta_sts_resolver-1.4.0/tests/test_main.py
+-rw-rw-r--   0 user      (1000) users      (100)     4371 2020-01-14 23:10:18.000000 postfix_mta_sts_resolver-1.4.0/tests/test_netstring.py
+-rw-r--r--   0 user      (1000) users      (100)     4249 2021-06-09 20:00:56.000000 postfix_mta_sts_resolver-1.4.0/tests/test_proactive_fetcher.py
+-rw-rw-r--   0 user      (1000) users      (100)     4647 2019-11-09 11:03:40.000000 postfix_mta_sts_resolver-1.4.0/tests/test_resolver.py
+-rw-r--r--   0 user      (1000) users      (100)     7215 2021-06-09 20:00:56.000000 postfix_mta_sts_resolver-1.4.0/tests/test_responder.py
+-rw-rw-r--   0 user      (1000) users      (100)     2417 2020-03-23 00:28:31.000000 postfix_mta_sts_resolver-1.4.0/tests/test_responder_expiration.py
+-rw-r--r--   0 user      (1000) users      (100)     1829 2021-06-09 20:00:56.000000 postfix_mta_sts_resolver-1.4.0/tests/test_responder_nosni.py
+-rw-r--r--   0 user      (1000) users      (100)     1832 2021-06-09 20:00:56.000000 postfix_mta_sts_resolver-1.4.0/tests/test_responder_strict.py
+-rw-r--r--   0 user      (1000) users      (100)     3969 2021-06-09 20:00:56.000000 postfix_mta_sts_resolver-1.4.0/tests/test_responder_volatile.py
+-rw-rw-r--   0 user      (1000) users      (100)     3638 2019-11-09 11:03:40.000000 postfix_mta_sts_resolver-1.4.0/tests/test_sqliteconnpool.py
+-rw-r--r--   0 user      (1000) users      (100)     5090 2023-08-03 20:00:17.000000 postfix_mta_sts_resolver-1.4.0/tests/test_utils.py
+-rw-rw-r--   0 user      (1000) users      (100)      354 2019-11-09 11:03:40.000000 postfix_mta_sts_resolver-1.4.0/tests/testdata.py
```

### Comparing `postfix_mta_sts_resolver-1.3.0/LICENSE` & `postfix_mta_sts_resolver-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/PKG-INFO` & `postfix_mta_sts_resolver-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix_mta_sts_resolver
-Version: 1.3.0
+Version: 1.4.0
 Summary: Daemon which provides TLS client policy for Postfix via socketmap, according to domain MTA-STS policy
 Home-page: https://github.com/Snawoot/postfix-mta-sts-resolver
 Author: Vladislav Yarmak
 Author-email: vladislav-ex-src@vm-0.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Requires-Python: >=3.5.3
 Description-Content-Type: text/markdown
 Provides-Extra: sqlite
 Provides-Extra: redis
+Provides-Extra: postgres
 Provides-Extra: dev
 Provides-Extra: uvloop
 License-File: LICENSE
 
 postfix-mta-sts-resolver
 ========================
 
@@ -59,15 +60,15 @@
 ## Installation
 
 ### Method 1. System-wide install from PyPI (recommended for humans)
 
 Run:
 
 ```bash
-sudo python3 -m pip install postfix-mta-sts-resolver[redis,sqlite]
+sudo python3 -m pip install postfix-mta-sts-resolver[redis,sqlite,postgres]
 ```
 
 If you don't need `redis` or `sqlite` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
 
 Package scripts shall be available in standard executable locations upon completion.
 
 #### pip user install
@@ -75,18 +76,18 @@
 All pip invocations can be run with `--user` option of `pip` installer. In this case superuser privileges are not required and package(s) are getting installed into user home directory. Usually, script executables will appear in `~/.local/bin`.
 
 ### Method 2. System-wide install from project source
 
 Run in project directory:
 
 ```bash
-sudo python3 -m pip install .[redis,sqlite]
+sudo python3 -m pip install .[redis,sqlite,postgres]
 ```
 
-If you don't need `redis` or `sqlite` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
+If you don't need `redis`, `sqlite` or `postgres` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
 
 Package scripts shall be available in standard executable locations upon completion.
 
 
 ### Method 3. Install into virtualenv
 
 See ["Building virtualenv"](#building-virtualenv)
```

### Comparing `postfix_mta_sts_resolver-1.3.0/README.md` & `postfix_mta_sts_resolver-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ## Installation
 
 ### Method 1. System-wide install from PyPI (recommended for humans)
 
 Run:
 
 ```bash
-sudo python3 -m pip install postfix-mta-sts-resolver[redis,sqlite]
+sudo python3 -m pip install postfix-mta-sts-resolver[redis,sqlite,postgres]
 ```
 
 If you don't need `redis` or `sqlite` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
 
 Package scripts shall be available in standard executable locations upon completion.
 
 #### pip user install
@@ -49,18 +49,18 @@
 All pip invocations can be run with `--user` option of `pip` installer. In this case superuser privileges are not required and package(s) are getting installed into user home directory. Usually, script executables will appear in `~/.local/bin`.
 
 ### Method 2. System-wide install from project source
 
 Run in project directory:
 
 ```bash
-sudo python3 -m pip install .[redis,sqlite]
+sudo python3 -m pip install .[redis,sqlite,postgres]
 ```
 
-If you don't need `redis` or `sqlite` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
+If you don't need `redis`, `sqlite` or `postgres` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
 
 Package scripts shall be available in standard executable locations upon completion.
 
 
 ### Method 3. Install into virtualenv
 
 See ["Building virtualenv"](#building-virtualenv)
```

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/__main__.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/__main__.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/asdnotify.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/asdnotify.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/base_cache.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/base_cache.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/daemon.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/daemon.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,29 +103,29 @@
         await proactive_fetcher.stop()
     await cache.teardown()
 
 
 def main():  # pragma: no cover
     args = parse_args()
     if args.pidfile is not None:
-        with open(args.pidfile, 'w') as f:
-            f.write(str(os.getpid()))
+        with open(args.pidfile, 'w', encoding='ascii') as pid_file:
+            pid_file.write(str(os.getpid()))
     if args.group is not None:
         try:
-            g = grp.getgrnam(args.group)
-            os.setegid(g.gr_gid)
-        except Exception as e:
-            print("Unable to change eGID to '{}': {}".format(args.group, e), file=sys.stderr)
+            group = grp.getgrnam(args.group)
+            os.setegid(group.gr_gid)
+        except Exception as exc:
+            print("Unable to change eGID to '{}': {}".format(args.group, exc), file=sys.stderr)
             return os.EX_OSERR
     if args.user is not None:
         try:
-            p = pwd.getpwnam(args.user)
-            os.seteuid(p.pw_uid)
-        except Exception as e:
-            print("Unable to change eUID to '{}': {}".format(args.user, e), file=sys.stderr)
+            passwd = pwd.getpwnam(args.user)
+            os.seteuid(passwd.pw_uid)
+        except Exception as exc:
+            print("Unable to change eUID to '{}': {}".format(args.user, exc), file=sys.stderr)
             return os.EX_OSERR
     with utils.AsyncLoggingHandler(args.logfile) as log_handler:
         logger = utils.setup_logger('MAIN', args.verbosity, log_handler)
         utils.setup_logger('STS', args.verbosity, log_handler)
         utils.setup_logger('PF', args.verbosity, log_handler)
         utils.setup_logger('RES', args.verbosity, log_handler)
         logger.info("MTA-STS daemon starting...")
@@ -144,7 +144,8 @@
         evloop = asyncio.get_event_loop()
         logger.info("Eventloop started.")
 
 
         evloop.run_until_complete(amain(cfg, evloop))
         evloop.close()
         logger.info("Server finished its work.")
+    return os.EX_OK
```

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/defaults.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/defaults.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 SHUTDOWN_TIMEOUT = 20
 STRICT_TESTING = False
 CONFIG_LOCATION = "/etc/mta-sts-daemon.yml"
 CACHE_BACKEND = "internal"
 INTERNAL_CACHE_SIZE = 10000
 SQLITE_THREADS = cpu_count()
 SQLITE_TIMEOUT = 5
+POSTGRES_TIMEOUT = 5
 REDIS_CONNECT_TIMEOUT = 5
 REDIS_TIMEOUT = 5
 CACHE_GRACE = 60
 PROACTIVE_FETCH_ENABLED = False
 PROACTIVE_FETCH_INTERVAL = 86400
 PROACTIVE_FETCH_CONCURRENCY_LIMIT = 100
 PROACTIVE_FETCH_GRACE_RATIO = 2.0
```

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/internal_cache.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/internal_cache.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/netstring.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/netstring.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/proactive_fetcher.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/proactive_fetcher.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/redis_cache.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/redis_cache.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/resolver.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/responder.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/responder.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/sqlite_cache.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/sqlite_cache.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver/utils.py` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -227,14 +227,18 @@
         # pylint: disable=import-outside-toplevel
         from . import redis_cache
         cache = redis_cache.RedisCache(**options)
     elif cache_type == "redis_sentinel":
         # pylint: disable=import-outside-toplevel
         from . import redis_cache
         cache = redis_cache.RedisSentinelCache(**options)
+    elif cache_type == "postgres":
+        # pylint: disable=import-outside-toplevel
+        from . import postgres_cache
+        cache = postgres_cache.PostgresCache(**options)
     else:
         raise NotImplementedError("Unsupported cache type!")
     return cache
 
 
 def check_loglevel(arg):
     try:
```

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/PKG-INFO` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix-mta-sts-resolver
-Version: 1.3.0
+Version: 1.4.0
 Summary: Daemon which provides TLS client policy for Postfix via socketmap, according to domain MTA-STS policy
 Home-page: https://github.com/Snawoot/postfix-mta-sts-resolver
 Author: Vladislav Yarmak
 Author-email: vladislav-ex-src@vm-0.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Requires-Python: >=3.5.3
 Description-Content-Type: text/markdown
 Provides-Extra: sqlite
 Provides-Extra: redis
+Provides-Extra: postgres
 Provides-Extra: dev
 Provides-Extra: uvloop
 License-File: LICENSE
 
 postfix-mta-sts-resolver
 ========================
 
@@ -59,15 +60,15 @@
 ## Installation
 
 ### Method 1. System-wide install from PyPI (recommended for humans)
 
 Run:
 
 ```bash
-sudo python3 -m pip install postfix-mta-sts-resolver[redis,sqlite]
+sudo python3 -m pip install postfix-mta-sts-resolver[redis,sqlite,postgres]
 ```
 
 If you don't need `redis` or `sqlite` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
 
 Package scripts shall be available in standard executable locations upon completion.
 
 #### pip user install
@@ -75,18 +76,18 @@
 All pip invocations can be run with `--user` option of `pip` installer. In this case superuser privileges are not required and package(s) are getting installed into user home directory. Usually, script executables will appear in `~/.local/bin`.
 
 ### Method 2. System-wide install from project source
 
 Run in project directory:
 
 ```bash
-sudo python3 -m pip install .[redis,sqlite]
+sudo python3 -m pip install .[redis,sqlite,postgres]
 ```
 
-If you don't need `redis` or `sqlite` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
+If you don't need `redis`, `sqlite` or `postgres` support, you may omit one of them in square brackets. If you don't need any of them and you plan to use internal cache without persistence, you should also omit square brackets.
 
 Package scripts shall be available in standard executable locations upon completion.
 
 
 ### Method 3. Install into virtualenv
 
 See ["Building virtualenv"](#building-virtualenv)
```

### Comparing `postfix_mta_sts_resolver-1.3.0/postfix_mta_sts_resolver.egg-info/SOURCES.txt` & `postfix_mta_sts_resolver-1.4.0/postfix_mta_sts_resolver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 postfix_mta_sts_resolver/asdnotify.py
 postfix_mta_sts_resolver/base_cache.py
 postfix_mta_sts_resolver/constants.py
 postfix_mta_sts_resolver/daemon.py
 postfix_mta_sts_resolver/defaults.py
 postfix_mta_sts_resolver/internal_cache.py
 postfix_mta_sts_resolver/netstring.py
+postfix_mta_sts_resolver/postgres_cache.py
 postfix_mta_sts_resolver/proactive_fetcher.py
 postfix_mta_sts_resolver/redis_cache.py
 postfix_mta_sts_resolver/resolver.py
 postfix_mta_sts_resolver/responder.py
 postfix_mta_sts_resolver/sqlite_cache.py
 postfix_mta_sts_resolver/utils.py
 postfix_mta_sts_resolver.egg-info/PKG-INFO
```

### Comparing `postfix_mta_sts_resolver-1.3.0/setup.py` & `postfix_mta_sts_resolver-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = path.abspath(path.dirname(__file__))  # pylint: disable=invalid-name
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()  # pylint: disable=invalid-name
 
 setup(name='postfix_mta_sts_resolver',
-      version='1.3.0',
+      version='1.4.0',
       description='Daemon which provides TLS client policy for Postfix '
                   'via socketmap, according to domain MTA-STS policy',
       url='https://github.com/Snawoot/postfix-mta-sts-resolver',
       author='Vladislav Yarmak',
       author_email='vladislav-ex-src@vm-0.com',
       license='MIT',
       packages=['postfix_mta_sts_resolver'],
@@ -23,14 +23,15 @@
           'aiodns>=1.1.1',
           'aiohttp>=3.4.4',
           'PyYAML>=3.12',
       ],
       extras_require={
           'sqlite': 'aiosqlite>=0.10.0',
           'redis': 'redis>=4.2.0rc1',
+          'postgres': 'asyncpg>=0.27',
           'dev': [
               'pytest>=3.0.0',
               'pytest-cov',
               'pytest-asyncio',
               'pytest-timeout',
               'pylint',
               'tox',
```

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_asdnotify.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_asdnotify.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_cache.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,23 +10,29 @@
     if cache_type == 'sqlite':
         tmpfile = tempfile.NamedTemporaryFile()
         cache_opts["filename"] = tmpfile.name
     cache = utils.create_cache(cache_type, cache_opts)
     await cache.setup()
     if cache_type == 'redis':
         await cache._pool.flushdb()
+    if cache_type == 'postgres':
+        async with cache._pool.acquire() as conn:
+            await conn.execute('TRUNCATE sts_policy_cache')
+            await conn.execute('TRUNCATE proactive_fetch_ts')
     return cache, tmpfile
 
 @pytest.mark.parametrize("cache_type,cache_opts,safe_set", [
     ("internal", {}, True),
     ("internal", {}, False),
     ("sqlite", {}, True),
     ("sqlite", {}, False),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, True),
-    ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, False)
+    ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, False),
+    ("postgres", {"dsn": "postgres://postgres@localhost:5432"}, True),
+    ("postgres", {"dsn": "postgres://postgres@localhost:5432"}, False),
 ])
 @pytest.mark.asyncio
 async def test_cache_lifecycle(cache_type, cache_opts, safe_set):
     cache, tmpfile = await setup_cache(cache_type, cache_opts)
 
     try:
         assert await cache.get("nonexistent") == None
@@ -43,14 +49,16 @@
         if cache_type == 'sqlite':
             tmpfile.close()
 
 @pytest.mark.parametrize("cache_type,cache_opts", [
     ("internal", {}),
     ("sqlite", {}),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}),
 ])
 @pytest.mark.asyncio
 async def test_proactive_fetch_ts_lifecycle(cache_type, cache_opts):
     cache, tmpfile = await setup_cache(cache_type, cache_opts)
 
     try:
         assert await cache.get_proactive_fetch_ts() >= 0  # works with empty db
@@ -80,14 +88,20 @@
     ("sqlite", {}, constants.DOMAIN_QUEUE_LIMIT*2, constants.DOMAIN_QUEUE_LIMIT),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, 3, 1),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, 3, 2),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, 3, 3),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, 3, 4),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, 0, 4),
     ("redis", {"url": "redis://127.0.0.1/0?socket_timeout=5&socket_connect_timeout=5"}, constants.DOMAIN_QUEUE_LIMIT*2, constants.DOMAIN_QUEUE_LIMIT),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}, 3, 1),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}, 3, 2),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}, 3, 3),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}, 3, 4),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}, 0, 4),
+    ("postgres", {"dsn": "postgres://postgres@%2Frun%2Fpostgresql/postgres"}, constants.DOMAIN_QUEUE_LIMIT*2, constants.DOMAIN_QUEUE_LIMIT),
 ])
 @pytest.mark.timeout(10)
 @pytest.mark.asyncio
 async def test_scanning_in_batches(cache_type, cache_opts, n_items, batch_size_limit):
     # Prepare
     cache, tmpfile = await setup_cache(cache_type, cache_opts)
     data = []
```

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_daemon.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_main.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_netstring.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_netstring.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_proactive_fetcher.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_proactive_fetcher.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_resolver.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_responder.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_responder.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_responder_expiration.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_responder_expiration.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_responder_nosni.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_responder_nosni.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_responder_strict.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_responder_strict.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_responder_volatile.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_responder_volatile.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_sqliteconnpool.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_sqliteconnpool.py`

 * *Files identical despite different names*

### Comparing `postfix_mta_sts_resolver-1.3.0/tests/test_utils.py` & `postfix_mta_sts_resolver-1.4.0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     assert 0 < res['port'] < 65536
     assert isinstance(res['cache_grace'], (int, float))
     assert isinstance(res['proactive_policy_fetching']['enabled'], bool)
     assert isinstance(res['proactive_policy_fetching']['interval'], int)
     assert isinstance(res['proactive_policy_fetching']['concurrency_limit'], int)
     assert isinstance(res['proactive_policy_fetching']['grace_ratio'], (int, float))
     assert isinstance(res['cache'], collections.abc.Mapping)
-    assert res['cache']['type'] in ('redis', 'sqlite', 'internal')
+    assert res['cache']['type'] in ('redis', 'sqlite', 'postgres', 'internal')
     assert isinstance(res['default_zone'], collections.abc.Mapping)
     assert isinstance(res['zones'], collections.abc.Mapping)
     for zone in list(res['zones'].values()) + [res['default_zone']]:
         assert isinstance(zone, collections.abc.Mapping)
         assert 'timeout' in zone
         assert 'strict_testing' in zone
```

