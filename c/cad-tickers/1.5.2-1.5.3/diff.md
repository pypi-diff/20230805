# Comparing `tmp/cad_tickers-1.5.2.tar.gz` & `tmp/cad_tickers-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cad_tickers-1.5.2.tar", max compression
+gzip compressed data, was "cad_tickers-1.5.3.tar", max compression
```

## Comparing `cad_tickers-1.5.2.tar` & `cad_tickers-1.5.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1065 2021-08-16 00:26:50.955684 cad_tickers-1.5.2/LICENSE
--rw-r--r--   0        0        0     1655 2021-08-16 00:26:50.955684 cad_tickers-1.5.2/ReadMe.md
--rw-r--r--   0        0        0      109 2021-08-16 00:26:50.955684 cad_tickers-1.5.2/cad_tickers/__init__.py
--rw-r--r--   0        0        0      529 2021-08-16 00:26:50.955684 cad_tickers-1.5.2/cad_tickers/exchanges/__init__.py
--rw-r--r--   0        0        0      736 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/exchanges/all_tickers.py
--rw-r--r--   0        0        0      704 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/exchanges/classes.py
--rw-r--r--   0        0        0     9174 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/exchanges/cse.py
--rw-r--r--   0        0        0      196 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/exchanges/tsx/__init__.py
--rw-r--r--   0        0        0     1283 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/exchanges/tsx/get_ticker_data.py
--rw-r--r--   0        0        0     2222 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/exchanges/tsx/get_tickers.py
--rw-r--r--   0        0        0     4450 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/exchanges/tsx/gql_data.py
--rw-r--r--   0        0        0      365 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/__init__.py
--rw-r--r--   0        0        0     1296 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/ceo/__init__.py
--rw-r--r--   0        0        0     2796 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/ceo/main.py
--rw-r--r--   0        0        0     1525 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/ceo/scrap.py
--rw-r--r--   0        0        0      372 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/ceo/spiel_class.py
--rw-r--r--   0        0        0     1086 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/ceo/utils.py
--rw-r--r--   0        0        0     1092 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/iiroc_halts.py
--rw-r--r--   0        0        0     3931 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/news/stock_news.py
--rw-r--r--   0        0        0      126 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/sedar/__init__.py
--rw-r--r--   0        0        0     1857 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/sedar/cse.py
--rw-r--r--   0        0        0     2887 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/sedar/tsx.py
--rw-r--r--   0        0        0      373 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/util/__init__.py
--rw-r--r--   0        0        0     4060 2021-08-16 00:26:50.959684 cad_tickers-1.5.2/cad_tickers/util/utils.py
--rw-r--r--   0        0        0      956 2021-08-16 00:26:50.963684 cad_tickers-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2687 2021-08-16 00:27:37.233866 cad_tickers-1.5.2/setup.py
--rw-r--r--   0        0        0     2686 2021-08-16 00:27:37.234249 cad_tickers-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/LICENSE
+-rw-r--r--   0        0        0     1443 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/ReadMe.md
+-rw-r--r--   0        0        0      109 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/all_tickers.py
+-rw-r--r--   0        0        0      809 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/classes.py
+-rw-r--r--   0        0        0     9174 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/cse.py
+-rw-r--r--   0        0        0      196 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/tsx/__init__.py
+-rw-r--r--   0        0        0     1283 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/tsx/get_ticker_data.py
+-rw-r--r--   0        0        0     2222 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/tsx/get_tickers.py
+-rw-r--r--   0        0        0     4450 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/exchanges/tsx/gql_data.py
+-rw-r--r--   0        0        0      365 2023-04-26 20:54:01.739996 cad_tickers-1.5.3/cad_tickers/news/__init__.py
+-rw-r--r--   0        0        0     1296 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/news/ceo/__init__.py
+-rw-r--r--   0        0        0     2796 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/news/ceo/main.py
+-rw-r--r--   0        0        0     1525 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/news/ceo/scrap.py
+-rw-r--r--   0        0        0      372 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/news/ceo/spiel_class.py
+-rw-r--r--   0        0        0     1086 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/news/ceo/utils.py
+-rw-r--r--   0        0        0     1092 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/news/iiroc_halts.py
+-rw-r--r--   0        0        0     3931 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/news/stock_news.py
+-rw-r--r--   0        0        0      126 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/sedar/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/sedar/cse.py
+-rw-r--r--   0        0        0     2940 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/sedar/tsx.py
+-rw-r--r--   0        0        0      171 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/test.py
+-rw-r--r--   0        0        0      373 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/util/__init__.py
+-rw-r--r--   0        0        0     4271 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/cad_tickers/util/utils.py
+-rw-r--r--   0        0        0      985 2023-04-26 20:54:01.743996 cad_tickers-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2508 2023-04-26 20:54:50.032839 cad_tickers-1.5.3/setup.py
+-rw-r--r--   0        0        0     2575 2023-04-26 20:54:50.033143 cad_tickers-1.5.3/PKG-INFO
```

### Comparing `cad_tickers-1.5.2/LICENSE` & `cad_tickers-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/ReadMe.md` & `cad_tickers-1.5.3/ReadMe.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,15 @@
 ```
 
 ```
 # Needed for readthedocs documentation
 poetry export -f requirements.txt > requirements.txt.
 ```
 
-#### Todo
+Or checkout some of my books [![Python Programming](https://m.media-amazon.com/images/I/41Mj384vgeL._SY346_.jpg)](https://www.amazon.com/dp/B0BXFLYRBD)
 
 
 #### Donate
 
 If you would like to motivate me to spend more time improving open source projects please consider donating.
 
-[![Donate with Ethereum](https://en.cryptobadges.io/badge/big/0x9d18acAB9Fe749Cbf899B2FD63Bf25e64829bbF3)](https://en.cryptobadges.io/donate/0x9d18acAB9Fe749Cbf899B2FD63Bf25e64829bbF3)
-
-[![Donate with Bitcoin](https://en.cryptobadges.io/badge/big/1BMWhjCrTE3Dn94oHnrk6XMZAS3hjq3vdD)](https://en.cryptobadges.io/donate/1BMWhjCrTE3Dn94oHnrk6XMZAS3hjq3vdD)
-
-[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Z6M6Y83D3URSU&item_name=Motivating+me+to+continue+to+produce+open+source+projects&currency_code=CAD)
+[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Z6M6Y83D3URSU&item_name=Motivating+me+to+continue+to+produce+open+source+projects&currency_code=CAD)
```

### Comparing `cad_tickers-1.5.2/cad_tickers/exchanges/__init__.py` & `cad_tickers-1.5.3/cad_tickers/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/exchanges/all_tickers.py` & `cad_tickers-1.5.3/cad_tickers/exchanges/all_tickers.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/exchanges/classes.py` & `cad_tickers-1.5.3/cad_tickers/exchanges/classes.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 
 
 class CSETicker(object):
     def __init__(
         self,
         updated_at: dict,
         metatdata: dict,
+        metadata: dict,
         quote: dict,
         depth_by_order: List[dict],
         depth_by_price: List[dict],
         ticker: dict,
+        legal: dict,
         trades: List[dict],
     ):
         self.updated_at = updated_at
         self.metatdata = metatdata
         self.quote = quote
         self.depth_by_order = depth_by_order
         self.depth_by_price = depth_by_price
         self.ticker = ticker
         self.trades = trades
+        self.metadata = metadata
+        self.legal = legal
 
 
 class CSESedarFilings(object):
     def __init__(self, categories: dict, list_items: List[dict]):
         self.categories = categories
         self.list_items = list_items
```

### Comparing `cad_tickers-1.5.2/cad_tickers/exchanges/cse.py` & `cad_tickers-1.5.3/cad_tickers/exchanges/cse.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/exchanges/tsx/get_ticker_data.py` & `cad_tickers-1.5.3/cad_tickers/exchanges/tsx/get_ticker_data.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/exchanges/tsx/get_tickers.py` & `cad_tickers-1.5.3/cad_tickers/exchanges/tsx/get_tickers.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/exchanges/tsx/gql_data.py` & `cad_tickers-1.5.3/cad_tickers/exchanges/tsx/gql_data.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/news/ceo/__init__.py` & `cad_tickers-1.5.3/cad_tickers/news/ceo/__init__.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/news/ceo/main.py` & `cad_tickers-1.5.3/cad_tickers/news/ceo/main.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/news/ceo/scrap.py` & `cad_tickers-1.5.3/cad_tickers/news/ceo/scrap.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/news/ceo/utils.py` & `cad_tickers-1.5.3/cad_tickers/news/ceo/utils.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/news/iiroc_halts.py` & `cad_tickers-1.5.3/cad_tickers/news/iiroc_halts.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/news/stock_news.py` & `cad_tickers-1.5.3/cad_tickers/news/stock_news.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/sedar/cse.py` & `cad_tickers-1.5.3/cad_tickers/sedar/cse.py`

 * *Files identical despite different names*

### Comparing `cad_tickers-1.5.2/cad_tickers/sedar/tsx.py` & `cad_tickers-1.5.3/cad_tickers/sedar/tsx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 import json
+from cad_tickers.util.utils import get_random_agent
 from datetime import datetime
 from cad_tickers.exchanges.tsx.gql_data import GQL
 from typing import Union
 
 
 def get_ticker_filings(
     symbol: str,
@@ -29,15 +30,17 @@
     r = requests.post(
         url,
         data=json.dumps(payload),
         headers={
             "authority": "app-money.tmx.com",
             "referer": f"https://money.tmx.com/en/quote/{symbol.upper()}",
             "locale": "en",
-            "Content-Type": "application/json"
+            "Content-Type": "application/json",
+            "User-Agent": get_random_agent(),
+            "Accept": "*/*"
         },
     )
     try:
         if r.status_code == 403:
             print(r.text)
             return {}
         else:
@@ -71,18 +74,17 @@
     payload["variables"]["limit"] = limit
     payload["variables"]["locale"] = locale
     url = "https://app-money.tmx.com/graphql"
     r = requests.post(
         url,
         data=json.dumps(payload),
         headers={
-            "authority": "app-money.tmx.com",
-            "referer": f"https://money.tmx.com/en/quote/{symbol.upper()}",
-            "locale": "en",
-            "Content-Type": "application/json"
+            "Content-Type": "application/json",
+            "User-Agent": get_random_agent(),
+            "Accept": "*/*"
         },
     )
     try:
         # check headings
         if r.status_code == 403:
             print(r.text)
             return {}
```

### Comparing `cad_tickers-1.5.2/cad_tickers/util/utils.py` & `cad_tickers-1.5.3/cad_tickers/util/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 import bs4
 from typing import List
+from random_user_agent.user_agent import UserAgent
 
 
 def transform_name_to_slug(raw_ticker: str) -> str:
     """
     Parameters:
       raw_ticker - cse ticker to be converted to slug
     Returns:
@@ -147,7 +148,12 @@
     Returns:
       webmoney_ticker - ticker that can be looked up in webmoney
     """
     return f"{cse_ticker}:CNX"
 
 
 # make request with query params
+
+def get_random_agent() -> str:
+    user_agent_rotator = UserAgent(limit=100)
+    user_agent = user_agent_rotator.get_random_user_agent()
+    return user_agent
```

### Comparing `cad_tickers-1.5.2/pyproject.toml` & `cad_tickers-1.5.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cad_tickers"
-version = "1.5.2"
+version = "1.5.3"
 description = "Various Stock Utilties Created by me"
 authors = ["David Li <davidli012345@gmail.com>"]
 maintainers = ["David Li <davidli012345@gmail.com>"]
 license = "MIT"
 readme = "ReadMe.md"
 repository = "https://github.com/FriendlyUser/cad_tickers"
 documentation = "https://readthedocs.org/projects/cad-tickers/"
@@ -24,14 +24,15 @@
 requests = "^2.24.0"
 coverage = "^5.2"
 beautifulsoup4 = "^4.9.1"
 lxml = "^4.5.2"
 pandas = "^1.3.0"
 xlrd = "^1.2.0"
 openpyxl = "^3.0.7"
+random-user-agent = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1"
 sphinx = "^3.2.1"
 pytest-cov = "^2.10.1"
 sphinx_rtd_theme = "^0.5.0"
```

### Comparing `cad_tickers-1.5.2/setup.py` & `cad_tickers-1.5.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 
 install_requires = \
 ['beautifulsoup4>=4.9.1,<5.0.0',
  'coverage>=5.2,<6.0',
  'lxml>=4.5.2,<5.0.0',
  'openpyxl>=3.0.7,<4.0.0',
  'pandas>=1.3.0,<2.0.0',
+ 'random-user-agent>=1.0.1,<2.0.0',
  'requests>=2.24.0,<3.0.0',
  'xlrd>=1.2.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'cad-tickers',
-    'version': '1.5.2',
+    'version': '1.5.3',
     'description': 'Various Stock Utilties Created by me',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/cad-tickers.svg)](https://badge.fury.io/py/cad-tickers) [![Downloads](https://pepy.tech/badge/cad-tickers)](https://pepy.tech/project/cad-tickers) [![Documentation Status](https://readthedocs.org/projects/cad-tickers/badge/?version=latest)](https://cad-tickers.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/gh/FriendlyUser/cad_tickers/branch/master/graph/badge.svg)](https://codecov.io/gh/FriendlyUser/cad_tickers)\n \n## Cad Tickers\nFunction to extract exchange data from the cse and tsx websites and various other data sources. This package is primarily focussed on scrapping data for the canadian stock market.\n\n\nThe entire 0.2.x version of tsx functions are now depricated.\n\nTsx has switched to graphql which I like.\n\n\n### How to run tests\n\n```\npytest\n```\n\n```\n# Needed for readthedocs documentation\npoetry export -f requirements.txt > requirements.txt.\n```\n\n#### Todo\n\n\n#### Donate\n\nIf you would like to motivate me to spend more time improving open source projects please consider donating.\n\n[![Donate with Ethereum](https://en.cryptobadges.io/badge/big/0x9d18acAB9Fe749Cbf899B2FD63Bf25e64829bbF3)](https://en.cryptobadges.io/donate/0x9d18acAB9Fe749Cbf899B2FD63Bf25e64829bbF3)\n\n[![Donate with Bitcoin](https://en.cryptobadges.io/badge/big/1BMWhjCrTE3Dn94oHnrk6XMZAS3hjq3vdD)](https://en.cryptobadges.io/donate/1BMWhjCrTE3Dn94oHnrk6XMZAS3hjq3vdD)\n\n[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Z6M6Y83D3URSU&item_name=Motivating+me+to+continue+to+produce+open+source+projects&currency_code=CAD)',
+    'long_description': '[![PyPI version](https://badge.fury.io/py/cad-tickers.svg)](https://badge.fury.io/py/cad-tickers) [![Downloads](https://pepy.tech/badge/cad-tickers)](https://pepy.tech/project/cad-tickers) [![Documentation Status](https://readthedocs.org/projects/cad-tickers/badge/?version=latest)](https://cad-tickers.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/gh/FriendlyUser/cad_tickers/branch/master/graph/badge.svg)](https://codecov.io/gh/FriendlyUser/cad_tickers)\n \n## Cad Tickers\nFunction to extract exchange data from the cse and tsx websites and various other data sources. This package is primarily focussed on scrapping data for the canadian stock market.\n\n\nThe entire 0.2.x version of tsx functions are now depricated.\n\nTsx has switched to graphql which I like.\n\n\n### How to run tests\n\n```\npytest\n```\n\n```\n# Needed for readthedocs documentation\npoetry export -f requirements.txt > requirements.txt.\n```\n\nOr checkout some of my books [![Python Programming](https://m.media-amazon.com/images/I/41Mj384vgeL._SY346_.jpg)](https://www.amazon.com/dp/B0BXFLYRBD)\n\n\n#### Donate\n\nIf you would like to motivate me to spend more time improving open source projects please consider donating.\n\n[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Z6M6Y83D3URSU&item_name=Motivating+me+to+continue+to+produce+open+source+projects&currency_code=CAD)\n',
     'author': 'David Li',
     'author_email': 'davidli012345@gmail.com',
     'maintainer': 'David Li',
     'maintainer_email': 'davidli012345@gmail.com',
     'url': 'https://github.com/FriendlyUser/cad_tickers',
     'packages': packages,
     'package_data': package_data,
```

