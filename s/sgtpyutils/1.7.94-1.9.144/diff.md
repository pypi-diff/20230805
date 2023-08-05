# Comparing `tmp/sgtpyutils-1.7.94.tar.gz` & `tmp/sgtpyutils-1.9.144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgtpyutils-1.7.94.tar", last modified: Thu Jun  9 07:44:17 2022, max compression
+gzip compressed data, was "sgtpyutils-1.9.144.tar", last modified: Sun Jun 12 01:46:22 2022, max compression
```

## Comparing `sgtpyutils-1.7.94.tar` & `sgtpyutils-1.9.144.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.411090 sgtpyutils-1.7.94/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-09 07:44:17.411090 sgtpyutils-1.7.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 07:44:17.411090 sgtpyutils-1.7.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/demo_3des.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/demo_aes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/demo_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/demo_des.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/demo_rsa.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/crypto/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/extensions/clazz.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/extensions/clazz_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/logger/
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/network/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/network/SimpleCaculateService/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/network/SimpleCaculateService/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/BaseTcpHandler/
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/BaseTcpHandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/EventArgs/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/EventArgs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/MessageHandler/
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/MessageHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/network/TcpClient.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/xls_txt/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/xls_txt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils/xls_txt/dict/
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/xls_txt/dict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.411090 sgtpyutils-1.7.94/sgtpyutils/xls_txt/list/
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/xls_txt/list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.411090 sgtpyutils-1.7.94/sgtpyutils/xlsx/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/xlsx/openpyxl_extend.py
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-06-09 07:43:57.000000 sgtpyutils-1.7.94/sgtpyutils/xlsx/xlsx_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 07:44:17.407090 sgtpyutils-1.7.94/sgtpyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-09 07:44:16.000000 sgtpyutils-1.7.94/sgtpyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-06-09 07:44:17.000000 sgtpyutils-1.7.94/sgtpyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 07:44:16.000000 sgtpyutils-1.7.94/sgtpyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 07:44:16.000000 sgtpyutils-1.7.94/sgtpyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-09 07:44:17.000000 sgtpyutils-1.7.94/sgtpyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-09 07:44:17.000000 sgtpyutils-1.7.94/sgtpyutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.162322 sgtpyutils-1.9.144/sgtpyutils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.162322 sgtpyutils-1.9.144/sgtpyutils/crypto/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/demo_3des.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/demo_aes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/demo_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/demo_des.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/demo_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/crypto/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.162322 sgtpyutils-1.9.144/sgtpyutils/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/extensions/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/extensions/clazz_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/logger/
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/network/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/network/SimpleCaculateService/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/network/SimpleCaculateService/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/BaseTcpHandler/
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/BaseTcpHandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/EventArgs/
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/EventArgs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/MessageHandler/
+-rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/MessageHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/network/TcpClient.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/xls_txt/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/xls_txt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/xls_txt/dict/
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/xls_txt/dict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/xls_txt/list/
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/xls_txt/list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.166322 sgtpyutils-1.9.144/sgtpyutils/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/xlsx/openpyxl_extend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-06-12 01:46:08.000000 sgtpyutils-1.9.144/sgtpyutils/xlsx/xlsx_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 01:46:22.162322 sgtpyutils-1.9.144/sgtpyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-06-12 01:46:21.000000 sgtpyutils-1.9.144/sgtpyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-06-12 01:46:22.000000 sgtpyutils-1.9.144/sgtpyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-12 01:46:21.000000 sgtpyutils-1.9.144/sgtpyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-12 01:46:21.000000 sgtpyutils-1.9.144/sgtpyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-12 01:46:22.000000 sgtpyutils-1.9.144/sgtpyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-12 01:46:22.000000 sgtpyutils-1.9.144/sgtpyutils.egg-info/top_level.txt
```

### Comparing `sgtpyutils-1.7.94/PKG-INFO` & `sgtpyutils-1.9.144/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgtpyutils
-Version: 1.7.94
+Version: 1.9.144
 Summary: sgtpyutils is a public library for use.
 Home-page: https://github.com/serfend/sgtpyutils
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: lib,utils
 Platform: any
```

### Comparing `sgtpyutils-1.7.94/setup.py` & `sgtpyutils-1.9.144/setup.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/crypto/demo.py` & `sgtpyutils-1.9.144/sgtpyutils/crypto/demo.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/crypto/demo_3des.py` & `sgtpyutils-1.9.144/sgtpyutils/crypto/demo_3des.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/crypto/demo_aes.py` & `sgtpyutils-1.9.144/sgtpyutils/crypto/demo_aes.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/crypto/demo_blowfish.py` & `sgtpyutils-1.9.144/sgtpyutils/crypto/demo_blowfish.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/crypto/demo_des.py` & `sgtpyutils-1.9.144/sgtpyutils/crypto/demo_des.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/crypto/demo_rsa.py` & `sgtpyutils-1.9.144/sgtpyutils/crypto/demo_rsa.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/extensions/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/extensions/clazz.py` & `sgtpyutils-1.9.144/sgtpyutils/extensions/clazz.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/extensions/clazz_ext.py` & `sgtpyutils-1.9.144/sgtpyutils/extensions/clazz_ext.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/logger/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/network/SimpleCaculateService/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/network/SimpleCaculateService/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/BaseTcpHandler/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/BaseTcpHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/EventArgs/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/EventArgs/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/MessageHandler/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/MessageHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/network/SimpleTcpService/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/network/SimpleTcpService/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/network/TcpClient.py` & `sgtpyutils-1.9.144/sgtpyutils/network/TcpClient.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/xls_txt/dict/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/xls_txt/dict/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from typing import Callable, Dict
 
 
 def dict2sheet(data: Dict, formatter: Callable = None, header: dict = {'key': 'value', '-'*20: '-'*30}, margin: int = 30):
     '''
       convert key-value to sheet
-      if formatter is set , no need to set margin
+      formatter: Callable[line:str,lines_dict:Dict] -> str : specify how to format a line
+            default set is lambda x,dic:f'{left_just(x)}\t{hex(dic[x]) if isinstance(dic[x],int) else dic[x]}'
+            if formatter is set , no need to set margin
+      
     '''
     result = dict(header)
     result.update(data)
 
     def left_just(x: str):
+        x = str(x)
         return x.ljust(margin, ' ')
     if not formatter:
         def formatter(
             x, dic): return f'{left_just(x)}\t{hex(dic[x]) if isinstance(dic[x],int) else dic[x]}'
     output = [formatter(x, result) for x in result]
     return output
```

### Comparing `sgtpyutils-1.7.94/sgtpyutils/xls_txt/list/__init__.py` & `sgtpyutils-1.9.144/sgtpyutils/xls_txt/list/__init__.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/xlsx/openpyxl_extend.py` & `sgtpyutils-1.9.144/sgtpyutils/xlsx/openpyxl_extend.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils/xlsx/xlsx_handler.py` & `sgtpyutils-1.9.144/sgtpyutils/xlsx/xlsx_handler.py`

 * *Files identical despite different names*

### Comparing `sgtpyutils-1.7.94/sgtpyutils.egg-info/PKG-INFO` & `sgtpyutils-1.9.144/sgtpyutils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgtpyutils
-Version: 1.7.94
+Version: 1.9.144
 Summary: sgtpyutils is a public library for use.
 Home-page: https://github.com/serfend/sgtpyutils
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: lib,utils
 Platform: any
```

### Comparing `sgtpyutils-1.7.94/sgtpyutils.egg-info/SOURCES.txt` & `sgtpyutils-1.9.144/sgtpyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

