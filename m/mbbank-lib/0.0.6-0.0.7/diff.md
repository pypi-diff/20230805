# Comparing `tmp/mbbank-lib-0.0.6.tar.gz` & `tmp/mbbank-lib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbbank-lib-0.0.6.tar", last modified: Sat Aug  5 09:33:16 2023, max compression
+gzip compressed data, was "mbbank-lib-0.0.7.tar", last modified: Sat Aug  5 16:09:08 2023, max compression
```

## Comparing `mbbank-lib-0.0.6.tar` & `mbbank-lib-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/mbbank/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/mbbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/mbbank/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/mbbank_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 09:33:16.000000 mbbank-lib-0.0.6/mbbank_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:33:16.729646 mbbank-lib-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 09:33:08.000000 mbbank-lib-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:09:08.492858 mbbank-lib-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 16:09:01.000000 mbbank-lib-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-05 16:09:08.492858 mbbank-lib-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:09:08.488858 mbbank-lib-0.0.7/mbbank/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-05 16:09:01.000000 mbbank-lib-0.0.7/mbbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-08-05 16:09:01.000000 mbbank-lib-0.0.7/mbbank/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:09:08.492858 mbbank-lib-0.0.7/mbbank_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-05 16:09:08.000000 mbbank-lib-0.0.7/mbbank_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 16:09:08.000000 mbbank-lib-0.0.7/mbbank_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:09:08.000000 mbbank-lib-0.0.7/mbbank_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 16:09:08.000000 mbbank-lib-0.0.7/mbbank_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 16:09:08.000000 mbbank-lib-0.0.7/mbbank_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 16:09:08.492858 mbbank-lib-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 16:09:01.000000 mbbank-lib-0.0.7/setup.py
```

### Comparing `mbbank-lib-0.0.6/LICENSE.txt` & `mbbank-lib-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.0.6/PKG-INFO` & `mbbank-lib-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -49,19 +49,19 @@
 mb.getLoanList()
 mb.userinfo()
 ```
 
 ### async
 ```py
 import asyncio
-from mbbank import mb_async as mbbank
+import mbbank
 import datetime
 
 async def main():
-    mb = mbbank.MBBank(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
+    mb = mbbank.MBBankAsync(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
     daynow = datetime.datetime.now()
     lasttime = daynow - datetime.timedelta(weeks=4*3) # maximum time 3 Month
     await mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow [, accountNo="<sub account number default is main account number>"])
     await mb.getBalance()
     await mb.getBalanceLoyalty()
     await mb.getInterestRate()
     await mb.getFavorBeneficiaryList(transactionType= "TRANSFER" or "PAYMENT", searchType="MOST" or "LATEST")
```

### Comparing `mbbank-lib-0.0.6/mbbank/main.py` & `mbbank-lib-0.0.7/mbbank/main.py`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.0.6/mbbank_lib.egg-info/PKG-INFO` & `mbbank-lib-0.0.7/mbbank_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -49,19 +49,19 @@
 mb.getLoanList()
 mb.userinfo()
 ```
 
 ### async
 ```py
 import asyncio
-from mbbank import mb_async as mbbank
+import mbbank
 import datetime
 
 async def main():
-    mb = mbbank.MBBank(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
+    mb = mbbank.MBBankAsync(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
     daynow = datetime.datetime.now()
     lasttime = daynow - datetime.timedelta(weeks=4*3) # maximum time 3 Month
     await mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow [, accountNo="<sub account number default is main account number>"])
     await mb.getBalance()
     await mb.getBalanceLoyalty()
     await mb.getInterestRate()
     await mb.getFavorBeneficiaryList(transactionType= "TRANSFER" or "PAYMENT", searchType="MOST" or "LATEST")
```

### Comparing `mbbank-lib-0.0.6/setup.py` & `mbbank-lib-0.0.7/setup.py`

 * *Files identical despite different names*

