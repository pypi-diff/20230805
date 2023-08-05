# Comparing `tmp/mbbank-lib-0.0.5.tar.gz` & `tmp/mbbank-lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbbank-lib-0.0.5.tar", last modified: Sat Aug  5 09:30:14 2023, max compression
+gzip compressed data, was "mbbank-lib-0.0.6.tar", last modified: Sat Aug  5 09:33:16 2023, max compression
```

## Comparing `mbbank-lib-0.0.5.tar` & `mbbank-lib-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/mbbank/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/mbbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/mbbank/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/mbbank_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/mbbank/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/mbbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/mbbank/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/mbbank_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/setup.py
```

### Comparing `mbbank-lib-0.0.5/LICENSE.txt` & `mbbank-lib-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.0.5/PKG-INFO` & `mbbank-lib-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mbbank-lib-0.0.5/mbbank/main.py` & `mbbank-lib-0.0.6/mbbank/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                 return
             elif data_out["result"]["responseCode"] == "GW283":
                 pass
             else:
                 err_out = data_out["result"]
                 raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
 
-    def getTransactionAccountHistory(self, *, from_date: datetime.datetime, to_date: datetime.datetime):
+    def getTransactionAccountHistory(self, *, accountNo:str=None, from_date: datetime.datetime, to_date: datetime.datetime):
         json_data = {
             'accountNo': self.__userid if accountNo is None else accountNo,
             'fromDate': from_date.strftime("%d/%m/%Y"),
             'toDate': to_date.strftime("%d/%m/%Y"),  # max 3 months
         }
         data_out = self._req(
             "https://online.mbbank.com.vn/retail-web-transactionservice/transaction/getTransactionAccountHistory",
```

### Comparing `mbbank-lib-0.0.5/mbbank_lib.egg-info/PKG-INFO` & `mbbank-lib-0.0.6/mbbank_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mbbank-lib-0.0.5/setup.py` & `mbbank-lib-0.0.6/setup.py`

 * *Files identical despite different names*

