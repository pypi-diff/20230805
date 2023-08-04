# Comparing `tmp/libnacl-1.8.0.tar.gz` & `tmp/libnacl-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libnacl-1.8.0.tar", last modified: Tue Jul  6 20:07:55 2021, max compression
+gzip compressed data, was "libnacl-1.9.0.tar", max compression
```

## Comparing `libnacl-1.8.0.tar` & `libnacl-1.9.0.tar`

### file list

```diff
@@ -1,99 +1,16 @@
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.951435 libnacl-1.8.0/
--rw-r--r--   0 akmod     (1000) akmod     (1000)       40 2020-11-23 09:58:54.000000 libnacl-1.8.0/AUTHORS
--rw-r--r--   0 akmod     (1000) akmod     (1000)    11313 2020-11-23 09:58:54.000000 libnacl-1.8.0/LICENSE
--rw-r--r--   0 akmod     (1000) akmod     (1000)      128 2020-11-23 09:58:54.000000 libnacl-1.8.0/MANIFEST.in
--rw-r--r--   0 akmod     (1000) akmod     (1000)      846 2021-07-06 20:07:55.951435 libnacl-1.8.0/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1729 2020-11-23 09:58:54.000000 libnacl-1.8.0/README.rst
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.948102 libnacl-1.8.0/doc/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     6782 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/Makefile
--rw-r--r--   0 akmod     (1000) akmod     (1000)    10276 2021-07-06 19:52:45.000000 libnacl-1.8.0/doc/conf.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      450 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/index.rst
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.948102 libnacl-1.8.0/doc/topics/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2822 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/dual.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3059 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/public.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      806 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/raw_generichash.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      621 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/raw_hash.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2519 2021-07-06 19:52:48.000000 libnacl-1.8.0/doc/topics/raw_public.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1144 2021-07-06 19:52:48.000000 libnacl-1.8.0/doc/topics/raw_sealed.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1860 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/raw_secret.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1826 2021-07-06 19:52:48.000000 libnacl-1.8.0/doc/topics/raw_sign.rst
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.948102 libnacl-1.8.0/doc/topics/releases/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      421 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.0.0.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      615 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.1.0.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      838 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.2.0.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      176 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.3.0.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      124 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.3.1.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      151 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.3.2.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      191 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.3.3.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      259 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.3.4.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      331 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.4.0.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      192 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.4.1.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      188 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.4.2.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      507 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.4.3.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      824 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.4.4.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      327 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.4.5.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      534 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.5.0.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      576 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.5.1.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      424 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.5.2.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1043 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.6.0.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      225 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.6.1.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      544 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.7.1.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)      328 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/1.7.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)       96 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/releases/index.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1080 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/sealed.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1308 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/secret.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1530 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/sign.rst
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1562 2020-11-23 09:58:54.000000 libnacl-1.8.0/doc/topics/utils.rst
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.951435 libnacl-1.8.0/libnacl/
--rw-r--r--   0 akmod     (1000) akmod     (1000)    42768 2021-07-06 19:52:48.000000 libnacl-1.8.0/libnacl/__init__.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2557 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/aead.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1888 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/base.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      950 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/blake.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      862 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/dual.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      933 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/encode.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3309 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/public.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      916 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/sealed.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1540 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/secret.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1559 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/secret_easy.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1517 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/sign.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3027 2021-07-06 19:52:45.000000 libnacl-1.8.0/libnacl/utils.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)       42 2021-07-06 20:07:55.000000 libnacl-1.8.0/libnacl/version.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.951435 libnacl-1.8.0/libnacl.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      846 2021-07-06 20:07:55.000000 libnacl-1.8.0/libnacl.egg-info/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2147 2021-07-06 20:07:55.000000 libnacl-1.8.0/libnacl.egg-info/SOURCES.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)        1 2021-07-06 20:07:55.000000 libnacl-1.8.0/libnacl.egg-info/dependency_links.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)        8 2021-07-06 20:07:55.000000 libnacl-1.8.0/libnacl.egg-info/top_level.txt
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.948102 libnacl-1.8.0/pkg/
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.951435 libnacl-1.8.0/pkg/rpm/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4312 2020-11-23 09:58:55.000000 libnacl-1.8.0/pkg/rpm/python-libnacl.spec
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.951435 libnacl-1.8.0/pkg/suse/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      441 2020-11-23 09:58:55.000000 libnacl-1.8.0/pkg/suse/python-libnacl.changes
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2161 2020-11-23 09:58:55.000000 libnacl-1.8.0/pkg/suse/python-libnacl.spec
--rw-r--r--   0 akmod     (1000) akmod     (1000)       67 2021-07-06 20:07:55.951435 libnacl-1.8.0/setup.cfg
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1078 2020-11-23 09:58:54.000000 libnacl-1.8.0/setup.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.951435 libnacl-1.8.0/tests/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      549 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/runtests.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-07-06 20:07:55.951435 libnacl-1.8.0/tests/unit/
--rw-r--r--   0 akmod     (1000) akmod     (1000)       24 2020-11-23 09:58:54.000000 libnacl-1.8.0/tests/unit/__init__.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1523 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_aead.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4689 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_auth_verify.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1476 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_blake.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2005 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_dual.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1434 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_public.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      560 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_auth_sym.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      575 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_auth_sym_easy.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1468 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_generichash.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      904 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_hash.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3678 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_public.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3629 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_random.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      924 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_secret.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      959 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_secret_easy.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1379 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_raw_sign.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3102 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_save.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1046 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_seal.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      653 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_secret.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      680 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_secret_easy.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4532 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_sign.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1974 2021-07-06 19:52:45.000000 libnacl-1.8.0/tests/unit/test_stream.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2520 2020-11-23 09:58:54.000000 libnacl-1.8.0/tests/unit/test_verify.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      734 2020-11-23 09:58:54.000000 libnacl-1.8.0/tests/unit/test_version.py
+-rw-r--r--   0        0        0    11313 2023-08-04 21:07:41.149581 libnacl-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1729 2023-08-04 21:07:41.149581 libnacl-1.9.0/README.rst
+-rw-r--r--   0        0        0    42904 2023-08-04 21:12:50.102368 libnacl-1.9.0/libnacl/__init__.py
+-rw-r--r--   0        0        0     2584 2023-08-04 22:02:31.514975 libnacl-1.9.0/libnacl/aead.py
+-rw-r--r--   0        0        0     2021 2023-08-04 21:56:41.178688 libnacl-1.9.0/libnacl/base.py
+-rw-r--r--   0        0        0      950 2023-08-04 21:07:41.149581 libnacl-1.9.0/libnacl/blake.py
+-rw-r--r--   0        0        0      889 2023-08-04 21:57:18.509004 libnacl-1.9.0/libnacl/dual.py
+-rw-r--r--   0        0        0      933 2023-08-04 21:07:41.149581 libnacl-1.9.0/libnacl/encode.py
+-rw-r--r--   0        0        0     3363 2023-08-04 21:57:09.148925 libnacl-1.9.0/libnacl/public.py
+-rw-r--r--   0        0        0      916 2023-08-04 21:07:41.149581 libnacl-1.9.0/libnacl/sealed.py
+-rw-r--r--   0        0        0     1540 2023-08-04 21:07:41.152914 libnacl-1.9.0/libnacl/secret.py
+-rw-r--r--   0        0        0     1586 2023-08-04 22:01:56.531348 libnacl-1.9.0/libnacl/secret_easy.py
+-rw-r--r--   0        0        0     1571 2023-08-04 22:01:13.470985 libnacl-1.9.0/libnacl/sign.py
+-rw-r--r--   0        0        0     3027 2023-08-04 21:07:41.152914 libnacl-1.9.0/libnacl/utils.py
+-rw-r--r--   0        0        0     1339 2023-08-04 22:46:46.624501 libnacl-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 libnacl-1.9.0/PKG-INFO
```

### Comparing `libnacl-1.8.0/LICENSE` & `libnacl-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libnacl-1.8.0/README.rst` & `libnacl-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `libnacl-1.8.0/libnacl/__init__.py` & `libnacl-1.9.0/libnacl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # -*- coding: utf-8 -*-
 '''
 Wrap libsodium routines
 '''
 # pylint: disable=C0103
 # Import python libs
-import ctypes
+import ctypes, ctypes.util
 import sys
 import os
 
 __SONAMES = (23, 18, 17, 13, 10, 5, 4)
 
 
 def _get_nacl():
     '''
     Locate the nacl c libs to use
     '''
     # Import libsodium
+    l_path = ctypes.util.find_library('sodium')
+    if l_path is not None:
+        return ctypes.cdll.LoadLibrary(l_path)
+
     if sys.platform.startswith('win'):
         try:
             return ctypes.cdll.LoadLibrary('libsodium')
         except OSError:
             pass
         for soname_ver in __SONAMES:
             try:
```

### Comparing `libnacl-1.8.0/libnacl/aead.py` & `libnacl-1.9.0/libnacl/aead.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     def __init__(self, key=None):
         if key is None:
             key = libnacl.utils.aead_key()
         if len(key) != libnacl.crypto_aead_chacha20poly1305_ietf_KEYBYTES:  # same size for both
             raise ValueError('Invalid key')
         self.sk = key
         self.usingAES = False
+        super().__init__()
 
     def useAESGCM(self):
         self.usingAES = True
         return self
 
     def encrypt(self, msg, aad, nonce=None, pack_nonce_aad=True):
         '''
```

### Comparing `libnacl-1.8.0/libnacl/base.py` & `libnacl-1.9.0/libnacl/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 import os
 import stat
 
 class BaseKey(object):
     '''
     Include methods for key management convenience
     '''
+    def __init__(self):
+        self.sk_hex = self.hex_sk()
+        self.pk_hex = self.hex_pk()
+        self.vk_hex = self.hex_vk()
+
     def hex_sk(self):
         if hasattr(self, 'sk'):
             return libnacl.encode.hex_encode(self.sk)
         else:
             return ''
 
     def hex_pk(self):
```

### Comparing `libnacl-1.8.0/libnacl/blake.py` & `libnacl-1.9.0/libnacl/blake.py`

 * *Files identical despite different names*

### Comparing `libnacl-1.8.0/libnacl/dual.py` & `libnacl-1.9.0/libnacl/dual.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     def __init__(self, crypt=None, sign=None):
         self.crypt = libnacl.public.SecretKey(crypt)
         self.signer = libnacl.sign.Signer(sign)
         self.sk = self.crypt.sk
         self.seed = self.signer.seed
         self.pk = self.crypt.pk
         self.vk = self.signer.vk
+        super().__init__()
 
     def sign(self, msg):
         '''
         Sign the given message
         '''
         return self.signer.sign(msg)
```

### Comparing `libnacl-1.8.0/libnacl/encode.py` & `libnacl-1.9.0/libnacl/encode.py`

 * *Files identical despite different names*

### Comparing `libnacl-1.8.0/libnacl/public.py` & `libnacl-1.9.0/libnacl/public.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     This class is used to manage public keys
     '''
     def __init__(self, pk):
         if len(pk) == libnacl.crypto_box_PUBLICKEYBYTES:
             self.pk = pk
         else:
             raise ValueError('Passed in invalid public key')
+        super().__init__()
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self.pk == other.pk
         else:
             return False
 
@@ -44,14 +45,15 @@
         if sk is None:
             self.pk, self.sk = libnacl.crypto_box_keypair()
         elif len(sk) == libnacl.crypto_box_SECRETKEYBYTES:
             self.sk = sk
             self.pk = libnacl.crypto_scalarmult_base(sk)
         else:
             raise ValueError('Passed in invalid secret key')
+        super().__init__()
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self.sk == other.sk and self.pk == other.pk
         else:
             return False
```

### Comparing `libnacl-1.8.0/libnacl/sealed.py` & `libnacl-1.9.0/libnacl/sealed.py`

 * *Files identical despite different names*

### Comparing `libnacl-1.8.0/libnacl/secret.py` & `libnacl-1.9.0/libnacl/secret.py`

 * *Files identical despite different names*

### Comparing `libnacl-1.8.0/libnacl/secret_easy.py` & `libnacl-1.9.0/libnacl/secret_easy.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     '''
     def __init__(self, key=None):
         if key is None:
             key = libnacl.utils.salsa_key()
         if len(key) != libnacl.crypto_secretbox_KEYBYTES:
             raise ValueError('Invalid key')
         self.sk = key
+        super().__init__()
 
     def encrypt(self, msg, nonce=None, pack_nonce=True):
         '''
         Encrypt the given message. If a nonce is not given it will be
         generated via the rand_nonce function
         '''
         if nonce is None:
```

### Comparing `libnacl-1.8.0/libnacl/sign.py` & `libnacl-1.9.0/libnacl/sign.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             if len(seed) != libnacl.crypto_sign_SEEDBYTES:
                 raise ValueError('Invalid seed bytes')
             self.vk, self.sk = libnacl.crypto_sign_seed_keypair(seed)
         else:
             seed = libnacl.randombytes(libnacl.crypto_sign_SEEDBYTES)
             self.vk, self.sk = libnacl.crypto_sign_seed_keypair(seed)
         self.seed = seed
+        super().__init__()
 
     def sign(self, msg):
         '''
         Sign the given message with this key
         '''
         return libnacl.crypto_sign(msg, self.sk)
 
@@ -43,13 +44,14 @@
     Verify signed messages
     '''
     def __init__(self, vk_hex):
         '''
         Create a verification key from a hex encoded vkey
         '''
         self.vk = libnacl.encode.hex_decode(vk_hex)
+        super().__init__()
 
     def verify(self, msg):
         '''
         Verify the message with tis key
         '''
         return libnacl.crypto_sign_open(msg, self.vk)
```

### Comparing `libnacl-1.8.0/libnacl/utils.py` & `libnacl-1.9.0/libnacl/utils.py`

 * *Files identical despite different names*

