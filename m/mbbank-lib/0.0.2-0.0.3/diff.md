# Comparing `tmp/mbbank-lib-0.0.2.tar.gz` & `tmp/mbbank-lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbbank-lib-0.0.2.tar", last modified: Tue Apr  4 16:27:36 2023, max compression
+gzip compressed data, was "mbbank-lib-0.0.3.tar", last modified: Sat Aug  5 07:30:37 2023, max compression
```

## Comparing `mbbank-lib-0.0.2.tar` & `mbbank-lib-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 thedt     (1000) thedt     (1000)        0 2023-04-04 16:27:36.098419 mbbank-lib-0.0.2/
--rw-r--r--   0 thedt     (1000) thedt     (1000)    11357 2023-04-04 15:44:10.000000 mbbank-lib-0.0.2/LICENSE.txt
--rw-r--r--   0 thedt     (1000) thedt     (1000)     1575 2023-04-04 16:27:36.098419 mbbank-lib-0.0.2/PKG-INFO
-drwxr-xr-x   0 thedt     (1000) thedt     (1000)        0 2023-04-04 16:27:36.088419 mbbank-lib-0.0.2/mbbank/
--rw-r--r--   0 thedt     (1000) thedt     (1000)       24 2023-04-04 12:35:49.000000 mbbank-lib-0.0.2/mbbank/__init__.py
--rw-r--r--   0 thedt     (1000) thedt     (1000)     6521 2023-04-04 16:02:22.000000 mbbank-lib-0.0.2/mbbank/main.py
-drwxr-xr-x   0 thedt     (1000) thedt     (1000)        0 2023-04-04 16:27:36.098419 mbbank-lib-0.0.2/mbbank_lib.egg-info/
--rw-r--r--   0 thedt     (1000) thedt     (1000)     1575 2023-04-04 16:27:36.000000 mbbank-lib-0.0.2/mbbank_lib.egg-info/PKG-INFO
--rw-r--r--   0 thedt     (1000) thedt     (1000)      223 2023-04-04 16:27:36.000000 mbbank-lib-0.0.2/mbbank_lib.egg-info/SOURCES.txt
--rw-r--r--   0 thedt     (1000) thedt     (1000)        1 2023-04-04 16:27:36.000000 mbbank-lib-0.0.2/mbbank_lib.egg-info/dependency_links.txt
--rw-r--r--   0 thedt     (1000) thedt     (1000)       57 2023-04-04 16:27:36.000000 mbbank-lib-0.0.2/mbbank_lib.egg-info/requires.txt
--rw-r--r--   0 thedt     (1000) thedt     (1000)        7 2023-04-04 16:27:36.000000 mbbank-lib-0.0.2/mbbank_lib.egg-info/top_level.txt
--rw-r--r--   0 thedt     (1000) thedt     (1000)       38 2023-04-04 16:27:36.098419 mbbank-lib-0.0.2/setup.cfg
--rw-r--r--   0 thedt     (1000) thedt     (1000)      546 2023-04-04 16:27:01.000000 mbbank-lib-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/mbbank/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/mbbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/mbbank/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/mbbank_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 07:30:37.000000 mbbank-lib-0.0.3/mbbank_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 07:30:37.747768 mbbank-lib-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 07:30:31.000000 mbbank-lib-0.0.3/setup.py
```

### Comparing `mbbank-lib-0.0.2/LICENSE.txt` & `mbbank-lib-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.0.2/mbbank/main.py` & `mbbank-lib-0.0.3/mbbank/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,159 +3,175 @@
 import re
 import datetime
 import base64
 import hashlib
 import typing
 import io
 import platform
-import aiohttp
+import requests
 
 headers_default = {
     'Cache-Control': 'no-cache',
     'Accept': 'application/json, text/plain, */*',
     'Authorization': 'Basic RU1CUkVUQUlMV0VCOlNEMjM0ZGZnMzQlI0BGR0AzNHNmc2RmNDU4NDNm',
     'User-Agent': f'Mozilla/5.0 (X11; {platform.system()} {platform.processor()})',
     "Origin": "https://online.mbbank.com.vn",
     "Referer": "https://online.mbbank.com.vn/"
 }
 
 
 def get_now_time():
     now = datetime.datetime.now()
     microsecond = int(now.strftime("%f")[:2])
-    return now.strftime(f"%Y%m%d%H%M{microsecond }")
+    return now.strftime(f"%Y%m%d%H%M{microsecond}")
 
 
 class MBBank:
-    
     deviceIdCommon = f'yeumtmdx-mbib-0000-0000-{get_now_time()}'
-    
+
     def __init__(self, *, username, password, tesseract_path=None):
-        self.userid = username
-        self.password = password
+        self.__userid = username
+        self.__password = password
         if tesseract_path is not None:
             pytesseract.pytesseract.tesseract_cmd = tesseract_path
         self.sessionId = None
         self._userinfo = None
         self._temp = {}
-        
-    
-    async def _req(self, url, *, json={}, headers={}):
+
+    def _req(self, url, *, json=None, headers=None):
+        if headers is None:
+            headers = {}
+        if json is None:
+            json = {}
         while True:
-            rid = f"{self.userid}-{get_now_time()}"
+            if self.sessionId is None:
+                self.authenticate()
+            rid = f"{self.__userid}-{get_now_time()}"
             json_data = {
                 'sessionId': self.sessionId if self.sessionId is not None else "",
                 'refNo': rid,
                 'deviceIdCommon': self.deviceIdCommon,
             }
             json_data.update(json)
             headers.update(headers_default)
             headers["X-Request-Id"] = rid
-            async with aiohttp.ClientSession() as s:
-                async with s.post(url, headers=headers, json=json_data) as r:
-                    data_out = await r.json()
+            with requests.Session() as s:
+                with s.post(url, headers=headers, json=json_data) as r:
+                    data_out = r.json()
             if data_out["result"] is None:
-                  await self.getBalance()
+                self.getBalance()
             elif data_out["result"]["ok"]:
                 data_out.pop("result", None)
-                data_out.pop("refNo", None)
                 break
             elif data_out["result"]["responseCode"] == "GW200":
-                await self.authenticate()
+                self.authenticate()
             else:
                 err_out = data_out["result"]
                 raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
         return data_out
-    
-    async def authenticate(self):
+
+    def authenticate(self):
         while True:
             self._userinfo = None
             self.sessionId = None
             self._temp = {}
-            data_out = await self._req("https://online.mbbank.com.vn/retail-web-internetbankingms/getCaptchaImage")
-            imgbyte = io.BytesIO(base64.b64decode(data_out["imageString"]))
-            img = Image.open(imgbyte)
+            rid = f"{self.__userid}-{get_now_time()}"
+            json_data = {
+                'sessionId': "",
+                'refNo': rid,
+                'deviceIdCommon': self.deviceIdCommon,
+            }
+            headers = headers_default.copy()
+            headers["X-Request-Id"] = rid
+            with requests.Session() as s:
+                with s.post("https://online.mbbank.com.vn/retail-web-internetbankingms/getCaptchaImage",
+                            headers=headers, json=json_data) as r:
+                    data_out = r.json()
+            img_byte = io.BytesIO(base64.b64decode(data_out["imageString"]))
+            img = Image.open(img_byte)
             img = img.convert('RGBA')
             pix = img.load()
             for y in range(img.size[1]):
                 for x in range(img.size[0]):
                     if pix[x, y][0] < 102 or pix[x, y][1] < 102 or pix[x, y][2] < 102:
                         pix[x, y] = (0, 0, 0, 255)
                     else:
                         pix[x, y] = (255, 255, 255, 255)
             text = pytesseract.image_to_string(img)
             text = re.sub(r"\s+", "", text, flags=re.MULTILINE)
             payload = {
-                "userId": self.userid,
-                "password": hashlib.md5(self.password.encode()).hexdigest(),
+                "userId": self.__userid,
+                "password": hashlib.md5(self.__password.encode()).hexdigest(),
                 "captcha": text,
                 'sessionId': "",
-                'refNo': f'{self.userid}-{get_now_time()}',
+                'refNo': f'{self.__userid}-{get_now_time()}',
                 'deviceIdCommon': self.deviceIdCommon,
             }
-
-            async with aiohttp.ClientSession() as s:
-                async with s.post("https://online.mbbank.com.vn/retail_web/internetbanking/doLogin", headers=headers_default, json=payload) as r:
-                    data_out = await r.json()
-                    
+            with requests.Session() as s:
+                with s.post("https://online.mbbank.com.vn/retail_web/internetbanking/doLogin",
+                            headers=headers_default, json=payload) as r:
+                    data_out = r.json()
             if data_out["result"]["ok"]:
                 self.sessionId = data_out["sessionId"]
                 self._userinfo = data_out
                 return
             elif data_out["result"]["responseCode"] == "GW283":
                 pass
             else:
                 err_out = data_out["result"]
                 raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
 
-    async def getTransactionAccountHistory(self, *, from_date: datetime.datetime, to_date: datetime.datetime):
+    def getTransactionAccountHistory(self, *, from_date: datetime.datetime, to_date: datetime.datetime):
         json_data = {
-            'accountNo': self.userid,
+            'accountNo': self.__userid,
             'fromDate': from_date.strftime("%d/%m/%Y"),
-            'toDate': to_date.strftime("%d/%m/%Y"), # max 3 months
+            'toDate': to_date.strftime("%d/%m/%Y"),  # max 3 months
         }
-
-        data_out = await self._req("https://online.mbbank.com.vn/retail-web-transactionservice/transaction/getTransactionAccountHistory", json=json_data)
+        data_out = self._req(
+            "https://online.mbbank.com.vn/retail-web-transactionservice/transaction/getTransactionAccountHistory",
+            json=json_data)
         return data_out
 
-    async def getBalance(self):
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail-web-accountms/getBalance")
+    def getBalance(self):
+        data_out = self._req("https://online.mbbank.com.vn/api/retail-web-accountms/getBalance")
         return data_out
-    
-    async def getBalanceLoyalty(self):
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/loyalty/getBalanceLoyalty")
+
+    def getBalanceLoyalty(self):
+        data_out = self._req("https://online.mbbank.com.vn/api/retail_web/loyalty/getBalanceLoyalty")
         return data_out
-    
-    async def getInterestRate(self, currency:str ="VND"):
+
+    def getInterestRate(self, currency: str = "VND"):
         json_data = {
             "productCode": "TIENGUI.KHN.EMB",
             "currency": currency,
         }
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/saving/getInterestRate", json=json_data)
+        data_out = self._req("https://online.mbbank.com.vn/api/retail_web/saving/getInterestRate", json=json_data)
         return data_out
-    
-    async def getFavorBeneficiaryList(self, *, transactionType: typing.Literal["TRANSFER", "PAYMENT"], searchType: typing.Literal["MOST", "LATEST"]):
+
+    def getFavorBeneficiaryList(self, *, transactionType: typing.Literal["TRANSFER", "PAYMENT"],
+                                searchType: typing.Literal["MOST", "LATEST"]):
         json_data = {
             "transactionType": transactionType,
             "searchType": searchType
         }
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/internetbanking/getFavorBeneficiaryList", json=json_data)
+        data_out = self._req(
+            "https://online.mbbank.com.vn/api/retail_web/internetbanking/getFavorBeneficiaryList", json=json_data)
+        return data_out
+
+    def getCardList(self):
+        data_out = self._req("https://online.mbbank.com.vn/api/retail_web/card/getList")
         return data_out
-    
-    async def getCardList(self):
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/card/getList")
-        return data_out
-    
-    async def getSavingList(self):
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/saving/getList")
-        return data_out
-    
-    async def getLoanList(self):
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/loan/getList")
+
+    def getSavingList(self):
+        data_out = self._req("https://online.mbbank.com.vn/api/retail_web/saving/getList")
         return data_out
-    
-    async def userinfo(self):
+
+    def getLoanList(self):
+        data_out = self._req("https://online.mbbank.com.vn/api/retail_web/loan/getList")
+        return data_out
+
+    def userinfo(self):
         if self._userinfo is None:
-            await self.authenticate()
+            self.authenticate()
         else:
-            await self.getBalance()
-        return self._userinfo
+            self.getBalance()
+        return self._userinfo
```

