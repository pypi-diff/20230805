# Comparing `tmp/fscraper-1.0.1.tar.gz` & `tmp/fscraper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fscraper-1.0.1.tar", last modified: Sat Jul  8 02:51:39 2023, max compression
+gzip compressed data, was "fscraper-1.0.2.tar", last modified: Sat Aug  5 03:48:46 2023, max compression
```

## Comparing `fscraper-1.0.1.tar` & `fscraper-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 02:51:39.183396 fscraper-1.0.1/
--rw-rw-rw-   0        0        0     1083 2023-04-22 01:43:56.000000 fscraper-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2968 2023-07-08 02:51:39.178472 fscraper-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2586 2023-05-29 13:08:02.000000 fscraper-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 02:51:39.053405 fscraper-1.0.1/fscraper/
--rw-rw-rw-   0        0        0      426 2023-05-15 02:47:44.000000 fscraper-1.0.1/fscraper/__init__.py
--rw-rw-rw-   0        0        0      203 2023-06-25 10:08:25.000000 fscraper-1.0.1/fscraper/kabutanscraper.py
--rw-rw-rw-   0        0        0     9918 2023-05-15 05:27:51.000000 fscraper-1.0.1/fscraper/kabuyohoscraper.py
--rw-rw-rw-   0        0        0     3211 2023-05-16 13:37:49.000000 fscraper-1.0.1/fscraper/reuterscraper.py
--rw-rw-rw-   0        0        0     5585 2023-07-01 14:35:21.000000 fscraper-1.0.1/fscraper/utils.py
--rw-rw-rw-   0        0        0     4363 2023-05-15 02:57:15.000000 fscraper-1.0.1/fscraper/xpath_table.py
--rw-rw-rw-   0        0        0     4976 2023-05-26 01:28:15.000000 fscraper-1.0.1/fscraper/yfscraper.py
-drwxrwxrwx   0        0        0        0 2023-07-08 02:51:39.163890 fscraper-1.0.1/fscraper.egg-info/
--rw-rw-rw-   0        0        0     2968 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 02:51:38.000000 fscraper-1.0.1/fscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 02:51:39.184440 fscraper-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-07-02 01:55:58.000000 fscraper-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:46.744209 fscraper-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-22 01:43:56.000000 fscraper-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3142 2023-08-05 03:48:46.742375 fscraper-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2760 2023-08-05 03:37:59.000000 fscraper-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:46.649345 fscraper-1.0.2/fscraper/
+-rw-rw-rw-   0        0        0      470 2023-08-01 13:51:23.000000 fscraper-1.0.2/fscraper/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-08-04 02:48:49.000000 fscraper-1.0.2/fscraper/kabutanscraper.py
+-rw-rw-rw-   0        0        0     9918 2023-05-15 05:27:51.000000 fscraper-1.0.2/fscraper/kabuyohoscraper.py
+-rw-rw-rw-   0        0        0     3211 2023-05-16 13:37:49.000000 fscraper-1.0.2/fscraper/reuterscraper.py
+-rw-rw-rw-   0        0        0     5585 2023-07-01 14:35:21.000000 fscraper-1.0.2/fscraper/utils.py
+-rw-rw-rw-   0        0        0     4363 2023-05-15 02:57:15.000000 fscraper-1.0.2/fscraper/xpath_table.py
+-rw-rw-rw-   0        0        0     4968 2023-08-04 02:50:05.000000 fscraper-1.0.2/fscraper/yfscraper.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:46.740160 fscraper-1.0.2/fscraper.egg-info/
+-rw-rw-rw-   0        0        0     3142 2023-08-05 03:48:46.000000 fscraper-1.0.2/fscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-08-05 03:48:46.000000 fscraper-1.0.2/fscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 03:48:46.000000 fscraper-1.0.2/fscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-08-05 03:48:46.000000 fscraper-1.0.2/fscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 03:48:46.000000 fscraper-1.0.2/fscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 03:48:46.744209 fscraper-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-08-01 13:51:56.000000 fscraper-1.0.2/setup.py
```

### Comparing `fscraper-1.0.1/LICENSE` & `fscraper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.1/PKG-INFO` & `fscraper-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fscraper
-Version: 1.0.1
-Summary: Financial Data Web Scraper
-Home-page: https://github.com/er-ri/fscraper
-Author: er-ri
-Author-email: 724chen@gmail.com
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fscraper
 Financial Data Scraper
 
 ## Introduction
 The project contains a collection of functions used to scrape financial data from the internet, mainly in Japan, and to calculate financial indicators such as *RSI*, *beta*, *MACD*, etc. Web scraping is implemented using `BeautifulSoup` and `requests` for the site that provides a RESTful API endpoint.
 
 ## Getting Started 
@@ -23,33 +10,37 @@
 
 ### Financial Data
 ```python
 import fscraper as fs
 
 # Yahoo Finance
 yfs = fs.YahooFinanceScraper('7203.T')
-df = yfs.get_stock_price(peroid='10y', interval='1d')
+df = yfs.get_stock_price(period='10y', interval='1d')
 df = yfs.get_stock_price2(start='2010-01-01', end='2020-12-12')
 
 df = yfs.get_statistics()
 
 # Reuters(Japan)
 rs = fs.ReutersScraper('7203.T')
 df = rs.get_income_statement(period='annual')
 df = rs.get_income_statement(period='interim')
 df = rs.get_balance_sheet(period='annual')
 df = rs.get_balance_sheet(period='interim')
 df = rs.get_cash_flow(period='annual')
 df = rs.get_cash_flow(period='interim')
 
 # Kabuyoho
-ks = fs.KabuyohoScraper('7203.T)
+ks = fs.KabuyohoScraper('7203.T')
 df = ks.get_report_top()
 df = ks.get_report_target()
 df = ks.get_target_price()
+
+# Kabutan
+kbs = fs.KabutanScraper('7203.T')
+df = kbs.get_stock_price_by_minutes()
 ```
 
 ### Indicator
 ```python
 # RSI
 df['rsi'] = fs.calculate_rsi(df['close'])
 df['rsi'] = fs.calculate_rsi(df['close'], periods=14)
@@ -70,14 +61,17 @@
 cor = fs.calculate_pearson_correlation(df1['close'], df2['close'])
 
 # beta with Nikkei 225
 beta = fs.calculate_beta(code='6753.T', market='^N225', period='1y')
 
 # 100 days min&max price
 df['100-high'], df['100-low'] = fs.set_x_days_high_low(df['high'], df['low'], window=100)
+
+# On Balance Volume (OBV)
+df['OBV'] = fs.calculate_obv(df['close'], df['volume'])
 ```
 
 ## Contribution
 Any suggestions for improvement or contribution to this project are appreciated.
 
 ## Disclaimer
-The project is for informational and educational purposes only. The author assumes no responsibility or liability for any errors in the content of this project. 
+The project is for informational and educational purposes only. The author assumes no responsibility or liability for any errors in the content of this project.
```

### Comparing `fscraper-1.0.1/README.md` & `fscraper-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fscraper
+Version: 1.0.2
+Summary: Financial Data Web Scraper
+Home-page: https://github.com/er-ri/fscraper
+Author: er-ri
+Author-email: 724chen@gmail.com
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # fscraper
 Financial Data Scraper
 
 ## Introduction
 The project contains a collection of functions used to scrape financial data from the internet, mainly in Japan, and to calculate financial indicators such as *RSI*, *beta*, *MACD*, etc. Web scraping is implemented using `BeautifulSoup` and `requests` for the site that provides a RESTful API endpoint.
 
 ## Getting Started 
@@ -10,33 +23,37 @@
 
 ### Financial Data
 ```python
 import fscraper as fs
 
 # Yahoo Finance
 yfs = fs.YahooFinanceScraper('7203.T')
-df = yfs.get_stock_price(peroid='10y', interval='1d')
+df = yfs.get_stock_price(period='10y', interval='1d')
 df = yfs.get_stock_price2(start='2010-01-01', end='2020-12-12')
 
 df = yfs.get_statistics()
 
 # Reuters(Japan)
 rs = fs.ReutersScraper('7203.T')
 df = rs.get_income_statement(period='annual')
 df = rs.get_income_statement(period='interim')
 df = rs.get_balance_sheet(period='annual')
 df = rs.get_balance_sheet(period='interim')
 df = rs.get_cash_flow(period='annual')
 df = rs.get_cash_flow(period='interim')
 
 # Kabuyoho
-ks = fs.KabuyohoScraper('7203.T)
+ks = fs.KabuyohoScraper('7203.T')
 df = ks.get_report_top()
 df = ks.get_report_target()
 df = ks.get_target_price()
+
+# Kabutan
+kbs = fs.KabutanScraper('7203.T')
+df = kbs.get_stock_price_by_minutes()
 ```
 
 ### Indicator
 ```python
 # RSI
 df['rsi'] = fs.calculate_rsi(df['close'])
 df['rsi'] = fs.calculate_rsi(df['close'], periods=14)
@@ -57,14 +74,17 @@
 cor = fs.calculate_pearson_correlation(df1['close'], df2['close'])
 
 # beta with Nikkei 225
 beta = fs.calculate_beta(code='6753.T', market='^N225', period='1y')
 
 # 100 days min&max price
 df['100-high'], df['100-low'] = fs.set_x_days_high_low(df['high'], df['low'], window=100)
+
+# On Balance Volume (OBV)
+df['OBV'] = fs.calculate_obv(df['close'], df['volume'])
 ```
 
 ## Contribution
 Any suggestions for improvement or contribution to this project are appreciated.
 
 ## Disclaimer
-The project is for informational and educational purposes only. The author assumes no responsibility or liability for any errors in the content of this project. 
+The project is for informational and educational purposes only. The author assumes no responsibility or liability for any errors in the content of this project.
```

### Comparing `fscraper-1.0.1/fscraper/kabuyohoscraper.py` & `fscraper-1.0.2/fscraper/kabuyohoscraper.py`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.1/fscraper/reuterscraper.py` & `fscraper-1.0.2/fscraper/reuterscraper.py`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.1/fscraper/utils.py` & `fscraper-1.0.2/fscraper/utils.py`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.1/fscraper/xpath_table.py` & `fscraper-1.0.2/fscraper/xpath_table.py`

 * *Files identical despite different names*

### Comparing `fscraper-1.0.1/fscraper/yfscraper.py` & `fscraper-1.0.2/fscraper/yfscraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,17 @@
         df.insert(len(df.columns), 'Enterprise Value/EBITDA', self.statistics_dom.xpath(yahoo_xpath['Enterprise Value/EBITDA'])[0].text)
 
         return df.transpose()
 
     def get_stock_price(self, period: str='1mo', interval: str='1d'):
         r"""
         Description:
-            Get history price 
+            Get historical price 
         Parameters:
-            range : str(`1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max`)
+            period : str(`1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max`)
             interval : str(`1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo`)
         """
         params = dict()
         params['range'] = period
         params['interval'] = interval
         params['events'] = 'div'
 
@@ -78,16 +78,16 @@
 
         df = YahooFinanceScraper.__construct_price_dataframe(self, params)
         return df
 
     def __construct_price_dataframe(self, params):
         df = pd.DataFrame()
 
-        price_url = "https://query2.finance.yahoo.com/v8/finance/chart/{}".format(self.code)
-        html = requests.get(url=price_url, params=params, headers=scraper_headers).text
+        url = "https://query2.finance.yahoo.com/v8/finance/chart/{}".format(self.code)
+        html = requests.get(url=url, params=params, headers=scraper_headers).text
         price_json = json.loads(html)
 
         df['date'] = price_json['chart']['result'][0]['timestamp']
         df['open'] = price_json['chart']['result'][0]['indicators']['quote'][0]['open']
         df['high'] = price_json['chart']['result'][0]['indicators']['quote'][0]['high']
         df['low'] = price_json['chart']['result'][0]['indicators']['quote'][0]['low']
         df['close'] = price_json['chart']['result'][0]['indicators']['quote'][0]['close']
```

### Comparing `fscraper-1.0.1/fscraper.egg-info/PKG-INFO` & `fscraper-1.0.2/fscraper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fscraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Financial Data Web Scraper
 Home-page: https://github.com/er-ri/fscraper
 Author: er-ri
 Author-email: 724chen@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
@@ -23,33 +23,37 @@
 
 ### Financial Data
 ```python
 import fscraper as fs
 
 # Yahoo Finance
 yfs = fs.YahooFinanceScraper('7203.T')
-df = yfs.get_stock_price(peroid='10y', interval='1d')
+df = yfs.get_stock_price(period='10y', interval='1d')
 df = yfs.get_stock_price2(start='2010-01-01', end='2020-12-12')
 
 df = yfs.get_statistics()
 
 # Reuters(Japan)
 rs = fs.ReutersScraper('7203.T')
 df = rs.get_income_statement(period='annual')
 df = rs.get_income_statement(period='interim')
 df = rs.get_balance_sheet(period='annual')
 df = rs.get_balance_sheet(period='interim')
 df = rs.get_cash_flow(period='annual')
 df = rs.get_cash_flow(period='interim')
 
 # Kabuyoho
-ks = fs.KabuyohoScraper('7203.T)
+ks = fs.KabuyohoScraper('7203.T')
 df = ks.get_report_top()
 df = ks.get_report_target()
 df = ks.get_target_price()
+
+# Kabutan
+kbs = fs.KabutanScraper('7203.T')
+df = kbs.get_stock_price_by_minutes()
 ```
 
 ### Indicator
 ```python
 # RSI
 df['rsi'] = fs.calculate_rsi(df['close'])
 df['rsi'] = fs.calculate_rsi(df['close'], periods=14)
@@ -70,14 +74,17 @@
 cor = fs.calculate_pearson_correlation(df1['close'], df2['close'])
 
 # beta with Nikkei 225
 beta = fs.calculate_beta(code='6753.T', market='^N225', period='1y')
 
 # 100 days min&max price
 df['100-high'], df['100-low'] = fs.set_x_days_high_low(df['high'], df['low'], window=100)
+
+# On Balance Volume (OBV)
+df['OBV'] = fs.calculate_obv(df['close'], df['volume'])
 ```
 
 ## Contribution
 Any suggestions for improvement or contribution to this project are appreciated.
 
 ## Disclaimer
 The project is for informational and educational purposes only. The author assumes no responsibility or liability for any errors in the content of this project.
```

### Comparing `fscraper-1.0.1/setup.py` & `fscraper-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
       name='fscraper',
-      version='1.0.1',
+      version='1.0.2',
       description='Financial Data Web Scraper',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='er-ri',
       author_email='724chen@gmail.com',
       url='https://github.com/er-ri/fscraper',
       packages=['fscraper'],
```

