# Comparing `tmp/tsetmc-0.9.0.tar.gz` & `tmp/tsetmc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsetmc-0.9.0.tar", last modified: Fri Jan 29 19:35:08 2021, max compression
+gzip compressed data, was "tsetmc-0.9.1.tar", last modified: Thu Feb 18 12:44:43 2021, max compression
```

## Comparing `tsetmc-0.9.0.tar` & `tsetmc-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-01-29 19:35:08.033471 tsetmc-0.9.0/
--rw-rw-rw-   0        0        0     2019 2021-01-29 19:35:08.032474 tsetmc-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     1146 2021-01-21 14:50:58.000000 tsetmc-0.9.0/README.rst
--rw-rw-rw-   0        0        0       42 2021-01-29 19:35:08.033471 tsetmc-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      900 2021-01-29 19:35:07.000000 tsetmc-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-01-29 19:35:08.021502 tsetmc-0.9.0/test/
--rw-rw-rw-   0        0        0    17033 2021-01-29 19:24:57.000000 tsetmc-0.9.0/test/test_core.py
-drwxrwxrwx   0        0        0        0 2021-01-29 19:35:08.023499 tsetmc-0.9.0/tsetmc/
--rw-rw-rw-   0        0        0      141 2021-01-29 19:35:07.000000 tsetmc-0.9.0/tsetmc/__init__.py
--rw-rw-rw-   0        0        0    12175 2021-01-29 19:23:57.000000 tsetmc-0.9.0/tsetmc/_core.py
-drwxrwxrwx   0        0        0        0 2021-01-29 19:35:08.031477 tsetmc-0.9.0/tsetmc.egg-info/
--rw-rw-rw-   0        0        0     2019 2021-01-29 19:35:07.000000 tsetmc-0.9.0/tsetmc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2021-01-29 19:35:07.000000 tsetmc-0.9.0/tsetmc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-29 19:35:07.000000 tsetmc-0.9.0/tsetmc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2021-01-29 19:35:07.000000 tsetmc-0.9.0/tsetmc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-01-29 19:35:07.000000 tsetmc-0.9.0/tsetmc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2020-11-06 20:00:12.000000 tsetmc-0.9.0/tsetmc.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2021-02-18 12:44:43.974038 tsetmc-0.9.1/
+-rw-rw-rw-   0        0        0     2134 2021-02-18 12:44:43.974038 tsetmc-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2021-01-29 19:38:00.000000 tsetmc-0.9.1/README.rst
+-rw-rw-rw-   0        0        0       42 2021-02-18 12:44:43.975035 tsetmc-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      900 2021-02-18 12:44:42.000000 tsetmc-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2021-02-18 12:44:43.964064 tsetmc-0.9.1/test/
+-rw-rw-rw-   0        0        0    17102 2021-02-18 12:41:45.000000 tsetmc-0.9.1/test/test_core.py
+drwxrwxrwx   0        0        0        0 2021-02-18 12:44:43.966057 tsetmc-0.9.1/tsetmc/
+-rw-rw-rw-   0        0        0      141 2021-02-18 12:44:42.000000 tsetmc-0.9.1/tsetmc/__init__.py
+-rw-rw-rw-   0        0        0    12301 2021-02-18 12:42:24.000000 tsetmc-0.9.1/tsetmc/_core.py
+drwxrwxrwx   0        0        0        0 2021-02-18 12:44:43.973042 tsetmc-0.9.1/tsetmc.egg-info/
+-rw-rw-rw-   0        0        0     2134 2021-02-18 12:44:43.000000 tsetmc-0.9.1/tsetmc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2021-02-18 12:44:43.000000 tsetmc-0.9.1/tsetmc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-02-18 12:44:43.000000 tsetmc-0.9.1/tsetmc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2021-02-18 12:44:43.000000 tsetmc-0.9.1/tsetmc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2021-02-18 12:44:43.000000 tsetmc-0.9.1/tsetmc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2020-11-06 20:00:12.000000 tsetmc-0.9.1/tsetmc.egg-info/zip-safe
```

### Comparing `tsetmc-0.9.0/PKG-INFO` & `tsetmc-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: tsetmc
-Version: 0.9.0
+Version: 0.9.1
 Summary: a library to retrieve data from tsetmc.com website
 Home-page: https://github.com/5j9/tsetmc
 Author: 5j9
 Author-email: 5j9@users.noreply.github.com
 License: GNU General Public License v3 (GPLv3)
-Description: Installation
+Description: A Python library to fetch data from http://tsetmc.com.
+        
+        Installation
         ------------
+        Requires Python 3.9+.
+        
         ``pip install --user tsetmc``
         
         Overview
         --------
         There are four main functions that return `pandas`_  ``DataFrame`` s:
         
         * ``get_market_watch_init``
```

### Comparing `tsetmc-0.9.0/README.rst` & `tsetmc-0.9.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+A Python library to fetch data from http://tsetmc.com.
+
 Installation
 ------------
+Requires Python 3.9+.
+
 ``pip install --user tsetmc``
 
 Overview
 --------
 There are four main functions that return `pandas`_  ``DataFrame`` s:
 
 * ``get_market_watch_init``
```

### Comparing `tsetmc-0.9.0/setup.py` & `tsetmc-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from os.path import dirname
 
 setup(
     name='tsetmc',
-    version='0.9.0',
+    version='0.9.1',
     long_description=open(
         f'{dirname(__file__)}/README.rst', encoding='utf-8').read(),
     long_description_content_type='text/x-rst',
     description='a library to retrieve data from tsetmc.com website',
     url='https://github.com/5j9/tsetmc',
     author='5j9',
     author_email='5j9@users.noreply.github.com',
```

### Comparing `tsetmc-0.9.0/test/test_core.py` & `tsetmc-0.9.1/test/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
         text = f.read()
     return patch.object(_core, 'get_content', lambda _: text)
 
 
 @patch_get_content('fmelli.html')
 def test_get_page_info():
     d = Instrument(1).get_page_info()
-    assert d.items() >= {
+    trade_history = d.pop('trade_history')
+    related_companies = d.pop('related_companies')
+    assert d == {
         'tmax': 19820.0
         , 'tmin': 21900.0
         , 'bvol': 5479452
         , 'eps': 1639
         , 'free_float': 33
         , 'l30': 'ملی\u200c صنایع\u200c مس\u200c ایران\u200c'  # todo
         , 'sector_name': 'فلزات اساسی'
@@ -29,16 +31,16 @@
         , 'month_average_volume': 98322903
         , 'l18': 'فملی'
         , 'sector_pe': 15.4
         , 'z': 101400000000
         , 'week_max': 22000.0
         , 'week_min': 20010.0
         , 'year_max': 39810.0
-        , 'year_min': 5181.0
-        , 'related_companies': [
+        , 'year_min': 5181.0}
+    assert related_companies == [
             [46348559193224090, 'فولاد', 'فولاد مبارکه اصفهان']
             , [35425587644337450, 'فملی', 'ملی\u200c صنایع\u200c مس\u200c ایران\u200c']
             , [9211775239375291, 'ذوب', 'سهامی ذوب آهن  اصفهان']
             , [28864540805361867, 'فخوز', 'فولاد  خوزستان']
             , [66701874099226162, 'فاسمین', 'کالسیمین\u200c']
             , [60350996279289099, 'کاوه', 'فولاد کاوه جنوب کیش']
             , [59266699437480384, 'ارفع', 'شرکت آهن و فولاد ارفع']
@@ -79,16 +81,15 @@
             , [67535111875054076, 'پارس متال ', 'پارس متال']
             , [357086043812735, 'فولاد تربت', 'فولاد تربت حیدریه']
             , [41867071915439180, 'آلومینیوم جنوب', 'مجتمع آلومینیوم جنوب']
             , [40012411719639360, 'سیسکو', 'فولاد سیرجان ایرانیان']
             , [48175603054578540, 'اسفراین', 'مجتمع صنعتی اسفراین']
             , [58903026391426893, 'سیرجان', 'فولاد سیرجان']
             , [68604686987554533, 'فماکح', 'ح . ماداکتو استیل کرد']]
-    }.items()
-    assert d['trade_history'].to_dict() == {
+    assert trade_history.to_dict() == {
         'pc': {20201021: 23990.0, 20201024: 22900.0, 20201026: 21800.0, 20201027: 20790.0, 20201028: 20580.0, 20201031: 21540.0, 20201101: 20910.0, 20201102: 20860.0, 20201104: 21900.0}
         , 'pmax': {20201021: 24790.0, 20201024: 23730.0, 20201026: 22700.0, 20201027: 22050.0, 20201028: 21420.0, 20201031: 21600.0, 20201101: 22000.0, 20201102: 21490.0, 20201104: 21900.0}
         , 'pmin': {20201021: 22660.0, 20201024: 22800.0, 20201026: 21760.0, 20201027: 20710.0, 20201028: 19760.0, 20201031: 20650.0, 20201101: 20480.0, 20201102: 20010.0, 20201104: 21510.0}
         , 'py': {20201021: 23610.0, 20201024: 23990.0, 20201026: 22900.0, 20201027: 21800.0, 20201028: 20790.0, 20201031: 20580.0, 20201101: 21540.0, 20201102: 20910.0, 20201104: 20860.0}
         , 'tno': {20201021: 45582, 20201024: 9270, 20201026: 43019, 20201027: 23360, 20201028: 30277, 20201031: 20359, 20201101: 21310, 20201102: 22337, 20201104: 8953}
         , 'tval': {20201021: 3561797608680.0, 20201024: 689808784080.0, 20201026: 5372316739110.0, 20201027: 2845911615950.0, 20201028: 2064206435550.0, 20201031: 1681410500120.0, 20201101: 1700893566630.0, 20201102: 1078508781780.0, 20201104: 1759996883990.0}
         , 'tvol': {20201021: 148496612, 20201024: 30119164, 20201026: 246470643, 20201027: 136913045, 20201028: 100296057, 20201031: 78073449, 20201101: 81345212, 20201102: 51699600, 20201104: 80376009}}
```

### Comparing `tsetmc-0.9.0/tsetmc/_core.py` & `tsetmc-0.9.1/tsetmc/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,22 @@
     return get_content(url).decode().translate(FARSI_NORM)
 
 
 class Instrument:
     # warning/todo:
     # get_page_info and get_inst_info are not tested widely and fail sometimes.
 
-    def __init__(self, id: int):
+    __slots__ = 'id'
+
+    def __init__(self, id: int, l30=None):
         self.id = id
 
+    def __repr__(self):
+        return f'Instrument({self.id})'
+
     def get_page_info(self) -> dict:
         """Return the static info found on instrument's page.
 
         For the meaning of keys see:
             https://cdn.tsetmc.com/Site.aspx?ParTree=151713
         """
         text = fa_norm_text(f'http://tsetmc.com/Loader.aspx?ParTree=151311&i={self.id}')
@@ -98,19 +103,20 @@
         :keyword index: parse values related to market-index.
         """
         # apparently, http://www.tsetmc.com/tsev2/data/instinfodata.aspx?i=...
         # and http://www.tsetmc.com/tsev2/data/instinfofast.aspx?i=...
         # return the same response.
         text = get_content(
             f'http://www.tsetmc.com/tsev2/data/instinfodata.aspx'
-            f'?i={self.id}&c=').decode()
+            # note that &e=1 parameter is required to get NAV.
+            f'?i={self.id}&c=&e=1').decode()
         # the _s are unknown
         price_info, index_info, orders_info, _, _, _, group_info, _, _ = text.split(';')
         timestamp, status, pl, pc, pf, py, pmin, pmax, tno, tvol, tval, _, \
-            info_datetime_date, last_info_time, *nav_info = price_info.split(',')
+            info_datetime_date, last_info_time, nav_datetime, nav = price_info.split(',')
         result = {
             'timestamp': timestamp, 'status': status
             , 'last_info_datetime': strptime(info_datetime_date + last_info_time, '%Y%m%d%H%M%S')
             , 'pl': int(pl), 'pc': int(pc), 'pf': int(pf), 'py': int(py)
             , 'pmin': int(pmin), 'pmax': int(pmax)
             , 'tno': int(tno), 'tvol': int(tvol), 'tval': int(tval)}
         if index:
@@ -142,16 +148,15 @@
                 , 'otc_tvol': int(otc_tvol)
                 , 'otc_tval': int(otc_tval)
                 , 'otc_tno': int(otc_tno)
                 , 'derivatives_status': derivatives_status
                 , 'derivatives_tvol': int(derivatives_tvol)
                 , 'derivatives_tval': int(derivatives_tval)
                 , 'derivatives_tno': int(derivatives_tno)}
-        if nav_info:
-            nav_datetime, nav = nav_info
+        if nav:
             result['nav'] = int(nav)
             result['nav_datetime'] = jstrptime(nav_datetime, '%Y/%m/%d %H:%M:%S')
         if orders:
             result |= {
                 f'{k}{i}': int(v)
                 for i, row in enumerate(orders_info.split(','), 1)
                 for (k, v) in zip(
```

### Comparing `tsetmc-0.9.0/tsetmc.egg-info/PKG-INFO` & `tsetmc-0.9.1/tsetmc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: tsetmc
-Version: 0.9.0
+Version: 0.9.1
 Summary: a library to retrieve data from tsetmc.com website
 Home-page: https://github.com/5j9/tsetmc
 Author: 5j9
 Author-email: 5j9@users.noreply.github.com
 License: GNU General Public License v3 (GPLv3)
-Description: Installation
+Description: A Python library to fetch data from http://tsetmc.com.
+        
+        Installation
         ------------
+        Requires Python 3.9+.
+        
         ``pip install --user tsetmc``
         
         Overview
         --------
         There are four main functions that return `pandas`_  ``DataFrame`` s:
         
         * ``get_market_watch_init``
```

