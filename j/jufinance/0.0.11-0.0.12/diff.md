# Comparing `tmp/jufinance-0.0.11.tar.gz` & `tmp/jufinance-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jufinance-0.0.11.tar", last modified: Tue Jul 25 21:29:05 2023, max compression
+gzip compressed data, was "jufinance-0.0.12.tar", last modified: Sat Aug  5 18:40:56 2023, max compression
```

## Comparing `jufinance-0.0.11.tar` & `jufinance-0.0.12.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.048964 jufinance-0.0.11/
--rw-r--r--   0 prannay    (501) staff       (20)      634 2023-07-25 21:29:05.048816 jufinance-0.0.11/PKG-INFO
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.047333 jufinance-0.0.11/jufinance/
--rw-r--r--   0 prannay    (501) staff       (20)       47 2023-07-25 20:40:36.000000 jufinance-0.0.11/jufinance/__init__.py
--rw-r--r--   0 prannay    (501) staff       (20)       40 2023-04-16 20:00:34.000000 jufinance-0.0.11/jufinance/historical.py
--rw-r--r--   0 prannay    (501) staff       (20)     4817 2023-07-25 21:27:22.000000 jufinance-0.0.11/jufinance/quote.py
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.048621 jufinance-0.0.11/jufinance/scrapers/
--rw-r--r--   0 prannay    (501) staff       (20)       77 2023-07-25 20:47:32.000000 jufinance-0.0.11/jufinance/scrapers/__init__.py
--rw-r--r--   0 prannay    (501) staff       (20)     3133 2023-07-25 21:06:44.000000 jufinance-0.0.11/jufinance/scrapers/investing.py
--rw-r--r--   0 prannay    (501) staff       (20)     5840 2023-07-25 21:11:01.000000 jufinance-0.0.11/jufinance/scrapers/moneycontrol.py
--rw-r--r--   0 prannay    (501) staff       (20)     7986 2023-07-25 21:10:49.000000 jufinance-0.0.11/jufinance/scrapers/screener.py
-drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-07-25 21:29:05.048046 jufinance-0.0.11/jufinance.egg-info/
--rw-r--r--   0 prannay    (501) staff       (20)      634 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/PKG-INFO
--rw-r--r--   0 prannay    (501) staff       (20)      366 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/SOURCES.txt
--rw-r--r--   0 prannay    (501) staff       (20)        1 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/dependency_links.txt
--rw-r--r--   0 prannay    (501) staff       (20)      253 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/requires.txt
--rw-r--r--   0 prannay    (501) staff       (20)       10 2023-07-25 21:29:05.000000 jufinance-0.0.11/jufinance.egg-info/top_level.txt
--rw-r--r--   0 prannay    (501) staff       (20)       38 2023-07-25 21:29:05.049005 jufinance-0.0.11/setup.cfg
--rw-r--r--   0 prannay    (501) staff       (20)     1563 2023-07-25 21:28:32.000000 jufinance-0.0.11/setup.py
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-08-05 18:40:56.270897 jufinance-0.0.12/
+-rw-r--r--   0 prannay    (501) staff       (20)      440 2023-08-05 18:40:56.270770 jufinance-0.0.12/PKG-INFO
+-rw-r--r--   0 prannay    (501) staff       (20)       69 2023-08-05 18:36:07.000000 jufinance-0.0.12/README.md
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-08-05 18:40:56.269170 jufinance-0.0.12/jufinance/
+-rw-r--r--   0 prannay    (501) staff       (20)       21 2023-07-27 18:25:04.000000 jufinance-0.0.12/jufinance/__init__.py
+-rw-r--r--   0 prannay    (501) staff       (20)     4858 2023-08-05 18:31:26.000000 jufinance-0.0.12/jufinance/quote.py
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-08-05 18:40:56.270269 jufinance-0.0.12/jufinance/scrapers/
+-rw-r--r--   0 prannay    (501) staff       (20)       77 2023-08-05 18:29:09.000000 jufinance-0.0.12/jufinance/scrapers/__init__.py
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-08-05 18:40:56.270526 jufinance-0.0.12/jufinance/scrapers/data/
+-rw-r--r--   0 prannay    (501) staff       (20)       21 2023-08-05 18:28:17.000000 jufinance-0.0.12/jufinance/scrapers/data/__init__.py
+-rw-r--r--   0 prannay    (501) staff       (20)   114583 2023-08-05 18:25:56.000000 jufinance-0.0.12/jufinance/scrapers/data/links.py
+-rw-r--r--   0 prannay    (501) staff       (20)     3338 2023-08-05 18:34:44.000000 jufinance-0.0.12/jufinance/scrapers/investing.py
+-rw-r--r--   0 prannay    (501) staff       (20)     5960 2023-08-05 18:33:59.000000 jufinance-0.0.12/jufinance/scrapers/moneycontrol.py
+-rw-r--r--   0 prannay    (501) staff       (20)     7986 2023-07-25 21:10:49.000000 jufinance-0.0.12/jufinance/scrapers/screener.py
+drwxr-xr-x   0 prannay    (501) staff       (20)        0 2023-08-05 18:40:56.269785 jufinance-0.0.12/jufinance.egg-info/
+-rw-r--r--   0 prannay    (501) staff       (20)      440 2023-08-05 18:40:56.000000 jufinance-0.0.12/jufinance.egg-info/PKG-INFO
+-rw-r--r--   0 prannay    (501) staff       (20)      421 2023-08-05 18:40:56.000000 jufinance-0.0.12/jufinance.egg-info/SOURCES.txt
+-rw-r--r--   0 prannay    (501) staff       (20)        1 2023-08-05 18:40:56.000000 jufinance-0.0.12/jufinance.egg-info/dependency_links.txt
+-rw-r--r--   0 prannay    (501) staff       (20)      253 2023-08-05 18:40:56.000000 jufinance-0.0.12/jufinance.egg-info/requires.txt
+-rw-r--r--   0 prannay    (501) staff       (20)       10 2023-08-05 18:40:56.000000 jufinance-0.0.12/jufinance.egg-info/top_level.txt
+-rw-r--r--   0 prannay    (501) staff       (20)       38 2023-08-05 18:40:56.270930 jufinance-0.0.12/setup.cfg
+-rw-r--r--   0 prannay    (501) staff       (20)     1381 2023-08-05 18:35:43.000000 jufinance-0.0.12/setup.py
```

### Comparing `jufinance-0.0.11/jufinance/quote.py` & `jufinance-0.0.12/jufinance/quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Get the quote details
 # - current price, company info, etc.
 
 from jufinance.scrapers import Investing, MoneyControl, Screener
+import datetime as dt
 
 
 class Quote:
     def __init__(self, ticker):
         # print("Invoked Quote module...")
         self.screener = Screener(ticker=ticker)
         self.screener.get_soup()
         self.mc = MoneyControl(ticker=ticker)
         self.mc.get_soup()
         self.investing = Investing(
-            ticker=ticker, start_time=1070343000, end_time=1681671410
+            ticker=ticker, start_time=1070343000, end_time=dt.datetime.now().timestamp()
         )
 
     def get_all_stock_data(self):
         """
         Retrieves all stock data for a given stock.
 
         :param self: The instance of the class.
```

### Comparing `jufinance-0.0.11/jufinance/scrapers/investing.py` & `jufinance-0.0.12/jufinance/scrapers/investing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import datetime as dt
+import json
 
 from bs4 import BeautifulSoup
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
+from jufinance.scrapers.data.links import links_dict
 
 
 class Investing:
     def __init__(self, ticker, start_time, end_time):
         # self.start_time = int(dt.datetime(start_time).timestamp())
         # self.end_time = int(dt.datetime(end_time).timestamp())
         self.ticker = ticker
-        self.URL = f"https://in.investing.com/equities/larsen-toubro-infotech-ltd-historical-data?end_date={end_time}&st_date=-{start_time}"
+        with open("jufinance/scrapers/links.json", "r") as file:
+            link_dict = json.load(file)
+        base_URL = link_dict[self.ticker]["investing_link"]
+        self.URL = (
+            base_URL + f"-historical-data?end_date={end_time}&st_date=-{start_time}"
+        )
 
     def page_html(self):
         options = webdriver.ChromeOptions()
         options.add_argument("--headless")
         options.add_argument("--disable-gpu")
         options.add_argument("--no-sandbox")
         options.add_argument("--disable-dev-shm-usage")
```

### Comparing `jufinance-0.0.11/jufinance/scrapers/moneycontrol.py` & `jufinance-0.0.12/jufinance/scrapers/moneycontrol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import requests
 from bs4 import BeautifulSoup
+import json
+from jufinance.scrapers.data.links import links_dict
 
 
 class MoneyControl:
     def __init__(self, ticker):
         # print("Invoked Money Control Module")
         self.ticker = ticker
 
     def get_soup(self):
-        self.mc_URL = "https://www.moneycontrol.com/india/stockpricequote/paintsvarnishes/bergerpaintsindia/BPI02"
+        with open("jufinance/scrapers/links.json", "r") as file:
+            link_dict = json.load(file)
+        self.mc_URL = link_dict[self.ticker]["moneycontrol_link"]
         api_response = requests.get(self.mc_URL).text
         self.soup = BeautifulSoup(api_response, "html.parser")
 
     def current_price(self):
         """
         Returns the current price of a stock.
 
-        This function uses web scraping to find the current price of a stock. It searches for a specific HTML element 
+        This function uses web scraping to find the current price of a stock. It searches for a specific HTML element
         using the BeautifulSoup library and extracts the text value of that element. The stock price is then returned.
 
         Parameters:
             self (object): The instance of the class.
 
         Returns:
             str: The current price of the stock as a string.
```

### Comparing `jufinance-0.0.11/jufinance/scrapers/screener.py` & `jufinance-0.0.12/jufinance/scrapers/screener.py`

 * *Files identical despite different names*

### Comparing `jufinance-0.0.11/setup.py` & `jufinance-0.0.12/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.11"
+VERSION = "0.0.12"
 DESCRIPTION = "Python Package to access Indian Stock market data."
 LONG_DESCRIPTION = "Python Package to access Indian Stock market data. This is for educational purposes only."
 
 # Setting up
 setup(
     name="jufinance",
     version=VERSION,
@@ -40,17 +40,13 @@
         "trio",
         "trio-websocket",
         "tzdata",
         "urllib3",
         "wsproto",
     ],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
-    keywords=["python", "first package"],
+    keywords=["python", "finance", "stock market"],
     classifiers=[
-        "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
-        # "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
     ],
 )
```

