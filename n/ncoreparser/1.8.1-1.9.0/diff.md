# Comparing `tmp/ncoreparser-1.8.1.tar.gz` & `tmp/ncoreparser-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncoreparser-1.8.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ncoreparser-1.8.1.tar` & `ncoreparser-1.9.0.tar`

### file list

```diff
@@ -1,13 +1,25 @@
--rw-r--r--   0        0        0     1068 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/LICENSE
--rw-r--r--   0        0        0     3125 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/Readme.md
--rw-r--r--   0        0        0      304 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/ncoreparser/__init__.py
--rw-r--r--   0        0        0     6706 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/ncoreparser/client.py
--rw-r--r--   0        0        0       23 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/ncoreparser/constant.py
--rw-r--r--   0        0        0     3897 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/ncoreparser/data.py
--rw-r--r--   0        0        0      192 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/ncoreparser/error.py
--rw-r--r--   0        0        0     5840 2022-10-04 12:49:47.462994 ncoreparser-1.8.1/ncoreparser/parser.py
--rw-r--r--   0        0        0     1107 2022-10-04 12:48:52.983129 ncoreparser-1.8.1/ncoreparser/torrent.py
--rw-r--r--   0        0        0     2224 2022-10-04 12:48:52.987129 ncoreparser-1.8.1/ncoreparser/util.py
--rw-r--r--   0        0        0      465 2022-10-04 12:54:13.930787 ncoreparser-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     3950 1970-01-01 00:00:00.000000 ncoreparser-1.8.1/setup.py
--rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 ncoreparser-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/Makefile
+-rw-r--r--   0        0        0     9542 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/dev-requirements.txt
+-rw-r--r--   0        0        0     7452 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/requirements.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/setup.cfg
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/.github/workflows/module_test.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/.github/workflows/publish_package.yml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/.github/workflows/unit_test.yml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/__init__.py
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/client.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/constant.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/data.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/error.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/parser.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/torrent.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/ncoreparser/util.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/tests/manual.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/tests/test_module/requirements.txt
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/tests/test_module/test.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/tests/test_unit/test_client.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/tests/test_unit/test_util.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/Readme.md
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ncoreparser-1.9.0/PKG-INFO
```

### Comparing `ncoreparser-1.8.1/LICENSE` & `ncoreparser-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ncoreparser-1.8.1/Readme.md` & `ncoreparser-1.9.0/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-![Test](https://img.shields.io/github/workflow/status/radaron/ncoreparser/Module%20test?label=Test&style=for-the-badge)
+![Test](https://img.shields.io/github/actions/workflow/status/radaron/ncoreparser/module_test.yml?label=Test&style=for-the-badge)
 [![pypi](https://img.shields.io/pypi/v/ncoreparser?style=for-the-badge)](https://pypi.org/project/ncoreparser/)
 [![downloads](https://img.shields.io/pypi/dm/ncoreparser?style=for-the-badge)](https://pypi.org/project/ncoreparser/)
 ![license](https://img.shields.io/github/license/radaron/ncoreparser?style=for-the-badge)
 
 # Ncoreparser
 
 ## Introduction
 
 This module provides python API-s to manage torrents from ncore.pro eg.: search, download, rssfeed, etc..
 
-
 ## Install
 
-
 ``` bash
 pip install ncoreparser
 ```
 
 ## Examples
```

### Comparing `ncoreparser-1.8.1/ncoreparser/client.py` & `ncoreparser-1.9.0/ncoreparser/client.py`

 * *Files identical despite different names*

### Comparing `ncoreparser-1.8.1/ncoreparser/data.py` & `ncoreparser-1.9.0/ncoreparser/data.py`

 * *Files identical despite different names*

### Comparing `ncoreparser-1.8.1/ncoreparser/parser.py` & `ncoreparser-1.9.0/ncoreparser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def __init__(self):
         self.type_pattern = re.compile(r'<div class="dd"><a title=".*?" href=".*?torrents.php\?csoport_listazas='
                                        r'(?P<category>.*?)">.*?</a>.*?<a title=".*?" href=".*?torrents.php\?tipus='
                                        r'(?P<type>.*?)">.*?</a></div>')
         self.date_pattern = re.compile(r'<div class="dd">(?P<date>[0-9]{4}\-[0-9]{2}\-[0-9]{2}\ '
                                        r'[0-9]{2}\:[0-9]{2}\:[0-9]{2})</div>')
         self.title_pattern = re.compile(r'<div class="torrent_reszletek_cim">(?P<title>.*?)</div>')
-        self.size_pattern = re.compile(r'<div class="dd">(?P<size>[0-9,.]+\ [K,M,G]{1}iB)\ \(.*?\)</div>')
+        self.size_pattern = re.compile(r'<div class="dd">(?P<size>[0-9,.]+\ [K,M,G,T]{1}iB)\ \(.*?\)</div>')
         self.peers_pattern = re.compile(r'div class="dt">Seederek:</div>.*?<div class="dd"><a onclick=".*?">(?P<seed>[0-9]+)'
                                         r'</a></div>.*?<div class="dt">Leecherek:</div>.*?<div class="dd"><a onclick=".*?">'
                                         r'(?P<leech>[0-9]+)</a></div>', re.DOTALL)
 
     def get_item(self, data):
         try:
             t_type = self.type_pattern.search(data)
```

### Comparing `ncoreparser-1.8.1/ncoreparser/torrent.py` & `ncoreparser-1.9.0/ncoreparser/torrent.py`

 * *Files identical despite different names*

### Comparing `ncoreparser-1.8.1/ncoreparser/util.py` & `ncoreparser-1.9.0/ncoreparser/util.py`

 * *Files identical despite different names*

### Comparing `ncoreparser-1.8.1/PKG-INFO` & `ncoreparser-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 Metadata-Version: 2.1
 Name: ncoreparser
-Version: 1.8.1
+Version: 1.9.0
 Summary: Package to download from ncore.pro
-Home-page: https://github.com/radaron/ncoreparser
-License: MIT
-Author: Aron Radics
-Author-email: aron.radics.jozsef@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: requests (>=2.23.0,<3.0.0)
+Author-email: Aron Radics <aron.radics.jozsef@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Requires-Dist: requests>=2.30
+Provides-Extra: dev
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
-![Test](https://img.shields.io/github/workflow/status/radaron/ncoreparser/Module%20test?label=Test&style=for-the-badge)
+![Test](https://img.shields.io/github/actions/workflow/status/radaron/ncoreparser/module_test.yml?label=Test&style=for-the-badge)
 [![pypi](https://img.shields.io/pypi/v/ncoreparser?style=for-the-badge)](https://pypi.org/project/ncoreparser/)
 [![downloads](https://img.shields.io/pypi/dm/ncoreparser?style=for-the-badge)](https://pypi.org/project/ncoreparser/)
 ![license](https://img.shields.io/github/license/radaron/ncoreparser?style=for-the-badge)
 
 # Ncoreparser
 
 ## Introduction
 
 This module provides python API-s to manage torrents from ncore.pro eg.: search, download, rssfeed, etc..
 
-
 ## Install
 
-
 ``` bash
 pip install ncoreparser
 ```
 
 ## Examples
 
 
@@ -126,8 +120,7 @@
 
     torrents = client.get_recommended(type=SearchParamType.SD_HUN)
     for torrent in torrents:
         print(torrent['title'], torrent['type'], torrent['size'], torrent['id'])
 
     client.logout()
 ```
-
```

