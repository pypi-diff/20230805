# Comparing `tmp/blockchyp-2.9.3.post1.tar.gz` & `tmp/blockchyp-2.9.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blockchyp-2.9.3.post1.tar", last modified: Mon Aug 30 20:58:46 2021, max compression
+gzip compressed data, was "dist/blockchyp-2.9.6.post1.tar", last modified: Fri Sep 30 14:57:35 2022, max compression
```

## Comparing `blockchyp-2.9.3.post1.tar` & `blockchyp-2.9.6.post1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-30 20:58:46.000000 blockchyp-2.9.3.post1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)    50379 2021-08-30 20:58:46.000000 blockchyp-2.9.3.post1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    49525 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-30 20:58:46.000000 blockchyp-2.9.3.post1/blockchyp/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      477 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25088 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/blockchyp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5531 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/cache.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-30 20:58:46.000000 blockchyp-2.9.3.post1/blockchyp/crypto/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/crypto/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      768 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/crypto/auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      574 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/crypto/certificate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1429 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/crypto/symmetric.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1201 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/error.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-30 20:58:46.000000 blockchyp-2.9.3.post1/blockchyp/resources/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1797 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/resources/blockchyp.crt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1137 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      216 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/blockchyp/version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-30 20:58:46.000000 blockchyp-2.9.3.post1/blockchyp.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    50379 2021-08-30 20:58:45.000000 blockchyp-2.9.3.post1/blockchyp.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2021-08-30 20:58:45.000000 blockchyp-2.9.3.post1/blockchyp.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-08-30 20:58:45.000000 blockchyp-2.9.3.post1/blockchyp.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2021-08-30 20:58:45.000000 blockchyp-2.9.3.post1/blockchyp.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2021-08-30 20:58:45.000000 blockchyp-2.9.3.post1/blockchyp.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-08-30 20:58:45.000000 blockchyp-2.9.3.post1/blockchyp.egg-info/zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1105 2021-08-30 20:58:46.000000 blockchyp-2.9.3.post1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2021-08-30 20:58:23.000000 blockchyp-2.9.3.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:57:35.000000 blockchyp-2.9.6.post1/
+-rw-r--r--   0 root         (0) root         (0)     1066 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)   108260 2022-09-30 14:57:35.000000 blockchyp-2.9.6.post1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)   107406 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:57:35.000000 blockchyp-2.9.6.post1/blockchyp/
+-rw-r--r--   0 root         (0) root         (0)      477 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42080 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/blockchyp.py
+-rw-r--r--   0 root         (0) root         (0)     5531 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:57:35.000000 blockchyp-2.9.6.post1/blockchyp/crypto/
+-rw-r--r--   0 root         (0) root         (0)      200 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      768 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/crypto/auth.py
+-rw-r--r--   0 root         (0) root         (0)      574 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/crypto/certificate.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/crypto/symmetric.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:57:35.000000 blockchyp-2.9.6.post1/blockchyp/resources/
+-rw-r--r--   0 root         (0) root         (0)     1797 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/resources/blockchyp.crt
+-rw-r--r--   0 root         (0) root         (0)     1363 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/types.py
+-rw-r--r--   0 root         (0) root         (0)      427 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/util.py
+-rw-r--r--   0 root         (0) root         (0)      216 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/blockchyp/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:57:35.000000 blockchyp-2.9.6.post1/blockchyp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)   108260 2022-09-30 14:57:34.000000 blockchyp-2.9.6.post1/blockchyp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      546 2022-09-30 14:57:34.000000 blockchyp-2.9.6.post1/blockchyp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-30 14:57:34.000000 blockchyp-2.9.6.post1/blockchyp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2022-09-30 14:57:34.000000 blockchyp-2.9.6.post1/blockchyp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-09-30 14:57:34.000000 blockchyp-2.9.6.post1/blockchyp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-30 14:57:34.000000 blockchyp-2.9.6.post1/blockchyp.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       76 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1105 2022-09-30 14:57:35.000000 blockchyp-2.9.6.post1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2022-09-30 14:57:16.000000 blockchyp-2.9.6.post1/setup.py
```

### Comparing `blockchyp-2.9.3.post1/LICENSE` & `blockchyp-2.9.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/blockchyp/cache.py` & `blockchyp-2.9.6.post1/blockchyp/cache.py`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/blockchyp/crypto/auth.py` & `blockchyp-2.9.6.post1/blockchyp/crypto/auth.py`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/blockchyp/crypto/certificate.py` & `blockchyp-2.9.6.post1/blockchyp/crypto/certificate.py`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/blockchyp/crypto/symmetric.py` & `blockchyp-2.9.6.post1/blockchyp/crypto/symmetric.py`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/blockchyp/error.py` & `blockchyp-2.9.6.post1/blockchyp/error.py`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/blockchyp/resources/blockchyp.crt` & `blockchyp-2.9.6.post1/blockchyp/resources/blockchyp.crt`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/blockchyp/types.py` & `blockchyp-2.9.6.post1/blockchyp/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class CardType:
     """Used to differentiate credit, debit, EBT, and gift cards."""
 
     CREDIT = 0
     DEBIT = 1
     EBT = 2
     GIFT = 3
+    HEALTHCARE = 4
 
 
 class SignatureFormat:
     """File formats for customer signatures."""
 
     NONE = "none"
     PNG = "png"
@@ -49,7 +50,16 @@
     """Contains customer verification methods."""
 
     SIGNATURE = "Signature"
     OFFLINE_PIN = "Offline PIN"
     ONLINE_PIN = "Online PIN"
     CDCVM = "CDCVM"
     NO_CVM = "No CVM"
+
+class HealthcareType:
+    """Contains categories of healthcare amounts."""
+
+    HEALTHCARE = "healthcare"
+    PRESCRIPTION = "prescription"
+    VISION = "vision"
+    CLINIC = "clinic"
+    DENTAL = "dental"
```

### Comparing `blockchyp-2.9.3.post1/blockchyp.egg-info/SOURCES.txt` & `blockchyp-2.9.6.post1/blockchyp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/setup.cfg` & `blockchyp-2.9.6.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `blockchyp-2.9.3.post1/setup.py` & `blockchyp-2.9.6.post1/setup.py`

 * *Files identical despite different names*

