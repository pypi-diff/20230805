# Comparing `tmp/mbbank-lib-0.0.4.tar.gz` & `tmp/mbbank-lib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbbank-lib-0.0.4.tar", last modified: Sat Aug  5 08:07:22 2023, max compression
+gzip compressed data, was "mbbank-lib-0.0.5.tar", last modified: Sat Aug  5 09:30:14 2023, max compression
```

## Comparing `mbbank-lib-0.0.4.tar` & `mbbank-lib-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/mbbank/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/mbbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/mbbank/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/mbbank_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 08:07:22.000000 mbbank-lib-0.0.4/mbbank_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 08:07:22.276631 mbbank-lib-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 08:07:09.000000 mbbank-lib-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/mbbank/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/mbbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/mbbank/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/mbbank_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 09:30:14.000000 mbbank-lib-0.0.5/mbbank_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:30:14.618842 mbbank-lib-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 09:30:06.000000 mbbank-lib-0.0.5/setup.py
```

### Comparing `mbbank-lib-0.0.4/LICENSE.txt` & `mbbank-lib-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.0.4/PKG-INFO` & `mbbank-lib-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.4
+Version: 0.0.5
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -35,15 +35,15 @@
 ```py
 import datetime
 import mbbank
 
 mb = mbbank.MBBank(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
 daynow = datetime.datetime.now()
 lasttime = daynow - datetime.timedelta(weeks=4*3) # maximum time 3 Month
-mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow)
+mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow [, accountNo="<sub account number default is main account number>"])
 mb.getBalance()
 mb.getBalanceLoyalty()
 mb.getInterestRate()
 mb.getFavorBeneficiaryList(transactionType= "TRANSFER" or "PAYMENT", searchType="MOST" or "LATEST")
 mb.getCardList()
 mb.getSavingList()
 mb.getLoanList()
@@ -56,15 +56,15 @@
 from mbbank import mb_async as mbbank
 import datetime
 
 async def main():
     mb = mbbank.MBBank(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
     daynow = datetime.datetime.now()
     lasttime = daynow - datetime.timedelta(weeks=4*3) # maximum time 3 Month
-    await mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow)
+    await mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow [, accountNo="<sub account number default is main account number>"])
     await mb.getBalance()
     await mb.getBalanceLoyalty()
     await mb.getInterestRate()
     await mb.getFavorBeneficiaryList(transactionType= "TRANSFER" or "PAYMENT", searchType="MOST" or "LATEST")
     await mb.getCardList()
     await mb.getSavingList()
     await mb.getLoanList()
```

### Comparing `mbbank-lib-0.0.4/mbbank/main.py` & `mbbank-lib-0.0.5/mbbank/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 pass
             else:
                 err_out = data_out["result"]
                 raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
 
     def getTransactionAccountHistory(self, *, from_date: datetime.datetime, to_date: datetime.datetime):
         json_data = {
-            'accountNo': self.__userid,
+            'accountNo': self.__userid if accountNo is None else accountNo,
             'fromDate': from_date.strftime("%d/%m/%Y"),
             'toDate': to_date.strftime("%d/%m/%Y"),  # max 3 months
         }
         data_out = self._req(
             "https://online.mbbank.com.vn/retail-web-transactionservice/transaction/getTransactionAccountHistory",
             json=json_data)
         return data_out
```

### Comparing `mbbank-lib-0.0.4/mbbank_lib.egg-info/PKG-INFO` & `mbbank-lib-0.0.5/mbbank_lib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.0.4
+Version: 0.0.5
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -35,15 +35,15 @@
 ```py
 import datetime
 import mbbank
 
 mb = mbbank.MBBank(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
 daynow = datetime.datetime.now()
 lasttime = daynow - datetime.timedelta(weeks=4*3) # maximum time 3 Month
-mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow)
+mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow [, accountNo="<sub account number default is main account number>"])
 mb.getBalance()
 mb.getBalanceLoyalty()
 mb.getInterestRate()
 mb.getFavorBeneficiaryList(transactionType= "TRANSFER" or "PAYMENT", searchType="MOST" or "LATEST")
 mb.getCardList()
 mb.getSavingList()
 mb.getLoanList()
@@ -56,15 +56,15 @@
 from mbbank import mb_async as mbbank
 import datetime
 
 async def main():
     mb = mbbank.MBBank(username="<account number>", password="<account password>" [, tesseract_path="path/to/tesseract"])
     daynow = datetime.datetime.now()
     lasttime = daynow - datetime.timedelta(weeks=4*3) # maximum time 3 Month
-    await mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow)
+    await mb.getTransactionAccountHistory(from_date=lasttime, to_date=daynow [, accountNo="<sub account number default is main account number>"])
     await mb.getBalance()
     await mb.getBalanceLoyalty()
     await mb.getInterestRate()
     await mb.getFavorBeneficiaryList(transactionType= "TRANSFER" or "PAYMENT", searchType="MOST" or "LATEST")
     await mb.getCardList()
     await mb.getSavingList()
     await mb.getLoanList()
```

### Comparing `mbbank-lib-0.0.4/setup.py` & `mbbank-lib-0.0.5/setup.py`

 * *Files identical despite different names*

