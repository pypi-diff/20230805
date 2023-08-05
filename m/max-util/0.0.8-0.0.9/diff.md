# Comparing `tmp/max_util-0.0.8.tar.gz` & `tmp/max_util-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "max_util-0.0.8.tar", last modified: Wed Jul 26 13:36:41 2023, max compression
+gzip compressed data, was "max_util-0.0.9.tar", last modified: Wed Jul 26 13:40:32 2023, max compression
```

## Comparing `max_util-0.0.8.tar` & `max_util-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.497042 max_util-0.0.8/
--rw-rw-rw-   0        0        0     1091 2021-10-29 14:52:05.000000 max_util-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      707 2023-07-26 13:36:41.498038 max_util-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      196 2021-11-04 16:24:29.000000 max_util-0.0.8/README.md
--rw-rw-rw-   0        0        0      122 2021-12-25 16:29:55.000000 max_util-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      646 2023-07-26 13:36:41.500033 max_util-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.432214 max_util-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.447175 max_util-0.0.8/src/alios/
--rw-rw-rw-   0        0        0       18 2023-07-26 13:35:26.000000 max_util-0.0.8/src/alios/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-07-26 13:10:13.000000 max_util-0.0.8/src/alios/api.py
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.451165 max_util-0.0.8/src/excel_util/
--rw-rw-rw-   0        0        0       30 2021-10-29 16:15:34.000000 max_util-0.0.8/src/excel_util/__init__.py
--rw-rw-rw-   0        0        0     1778 2022-07-05 13:29:05.000000 max_util-0.0.8/src/excel_util/mk_book.py
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.478091 max_util-0.0.8/src/max_util.egg-info/
--rw-rw-rw-   0        0        0      707 2023-07-26 13:36:41.000000 max_util-0.0.8/src/max_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-26 13:36:41.000000 max_util-0.0.8/src/max_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:36:41.000000 max_util-0.0.8/src/max_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-26 13:36:41.000000 max_util-0.0.8/src/max_util.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.485074 max_util-0.0.8/src/setting/
--rw-rw-rw-   0        0        0      164 2023-07-26 13:34:14.000000 max_util-0.0.8/src/setting/__init__.py
--rw-rw-rw-   0        0        0     1181 2023-07-18 14:22:15.000000 max_util-0.0.8/src/setting/json_config.py
--rw-rw-rw-   0        0        0      350 2023-07-17 14:10:08.000000 max_util-0.0.8/src/setting/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.492055 max_util-0.0.8/src/showdoc/
--rw-rw-rw-   0        0        0     3841 2023-07-26 13:35:56.000000 max_util-0.0.8/src/showdoc/__init__.py
--rw-rw-rw-   0        0        0     3781 2023-07-26 13:00:44.000000 max_util-0.0.8/src/showdoc/api.py
--rw-rw-rw-   0        0        0     2102 2023-07-20 14:10:25.000000 max_util-0.0.8/src/showdoc/entity.py
--rw-rw-rw-   0        0        0     2728 2023-07-25 13:59:48.000000 max_util-0.0.8/src/showdoc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 13:36:41.495046 max_util-0.0.8/src/turtle_util/
--rw-rw-rw-   0        0        0       30 2023-07-26 13:18:42.000000 max_util-0.0.8/src/turtle_util/__init__.py
--rw-rw-rw-   0        0        0     7989 2021-12-25 16:26:06.000000 max_util-0.0.8/src/turtle_util/christmas_2021.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.522625 max_util-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2021-10-29 14:52:05.000000 max_util-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-07-26 13:40:32.522625 max_util-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2021-11-04 16:24:29.000000 max_util-0.0.9/README.md
+-rw-rw-rw-   0        0        0      122 2021-12-25 16:29:55.000000 max_util-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      646 2023-07-26 13:40:32.524591 max_util-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.485125 max_util-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.494101 max_util-0.0.9/src/alios/
+-rw-rw-rw-   0        0        0       18 2023-07-26 13:35:26.000000 max_util-0.0.9/src/alios/__init__.py
+-rw-rw-rw-   0        0        0     1224 2023-07-26 13:39:50.000000 max_util-0.0.9/src/alios/api.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.496096 max_util-0.0.9/src/excel_util/
+-rw-rw-rw-   0        0        0       30 2021-10-29 16:15:34.000000 max_util-0.0.9/src/excel_util/__init__.py
+-rw-rw-rw-   0        0        0     1778 2022-07-05 13:29:05.000000 max_util-0.0.9/src/excel_util/mk_book.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.509630 max_util-0.0.9/src/max_util.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-07-26 13:40:32.000000 max_util-0.0.9/src/max_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-26 13:40:32.000000 max_util-0.0.9/src/max_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:40:32.000000 max_util-0.0.9/src/max_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-26 13:40:32.000000 max_util-0.0.9/src/max_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.513656 max_util-0.0.9/src/setting/
+-rw-rw-rw-   0        0        0      164 2023-07-26 13:34:14.000000 max_util-0.0.9/src/setting/__init__.py
+-rw-rw-rw-   0        0        0     1181 2023-07-18 14:22:15.000000 max_util-0.0.9/src/setting/json_config.py
+-rw-rw-rw-   0        0        0      350 2023-07-17 14:10:08.000000 max_util-0.0.9/src/setting/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.518606 max_util-0.0.9/src/showdoc/
+-rw-rw-rw-   0        0        0     3841 2023-07-26 13:35:56.000000 max_util-0.0.9/src/showdoc/__init__.py
+-rw-rw-rw-   0        0        0     3781 2023-07-26 13:00:44.000000 max_util-0.0.9/src/showdoc/api.py
+-rw-rw-rw-   0        0        0     2102 2023-07-20 14:10:25.000000 max_util-0.0.9/src/showdoc/entity.py
+-rw-rw-rw-   0        0        0     2728 2023-07-25 13:59:48.000000 max_util-0.0.9/src/showdoc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:40:32.520603 max_util-0.0.9/src/turtle_util/
+-rw-rw-rw-   0        0        0       30 2023-07-26 13:18:42.000000 max_util-0.0.9/src/turtle_util/__init__.py
+-rw-rw-rw-   0        0        0     7989 2021-12-25 16:26:06.000000 max_util-0.0.9/src/turtle_util/christmas_2021.py
```

### Comparing `max_util-0.0.8/LICENSE` & `max_util-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `max_util-0.0.8/PKG-INFO` & `max_util-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 206d 6178  : 2.1..Name: max
 00000020: 5f75 7469 6c0d 0a56 6572 7369 6f6e 3a20  _util..Version: 
-00000030: 302e 302e 380d 0a53 756d 6d61 7279 3a20  0.0.8..Summary: 
+00000030: 302e 302e 390d 0a53 756d 6d61 7279 3a20  0.0.9..Summary: 
 00000040: 696e 7365 7274 2065 7863 656c 2062 6f6f  insert excel boo
 00000050: 6b2c 2062 6173 6520 786c 7774 0d0a 486f  k, base xlwt..Ho
 00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000070: 2f67 6974 6565 2e63 6f6d 2f6d 6178 696e  /gitee.com/maxin
 00000080: 787a 2f6d 6b5f 7574 696c 5f70 7974 686f  xz/mk_util_pytho
 00000090: 6e0d 0a41 7574 686f 723a 206d 6178 0d0a  n..Author: max..
 000000a0: 4175 7468 6f72 2d65 6d61 696c 3a20 6d61  Author-email: ma
```

### Comparing `max_util-0.0.8/setup.cfg` & `max_util-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6178 5f75 7469 6c0d 0a76 6572   = max_util..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 206d 6178 0d0a 6175 7468  thor = max..auth
 00000040: 6f72 5f65 6d61 696c 203d 206d 615f 6b65  or_email = ma_ke
 00000050: 5f6d 696e 4031 3633 2e63 6f6d 0d0a 6465  _min@163.com..de
 00000060: 7363 7269 7074 696f 6e20 3d20 696e 7365  scription = inse
 00000070: 7274 2065 7863 656c 2062 6f6f 6b2c 2062  rt excel book, b
 00000080: 6173 6520 786c 7774 0d0a 6c6f 6e67 5f64  ase xlwt..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `max_util-0.0.8/src/alios/api.py` & `max_util-0.0.9/src/alios/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import oss2
 from oss2 import Auth, Bucket
+import sys
+import os
 
-from ..setting.json_config import JsonConf
+sys.path.append(os.path.abspath('..'))
+from src.setting import JsonConf
 
 conf_url = '.aliOSS/conf.json'
 
 
 class API:
     __access_key: str
     __access_secret: str
```

### Comparing `max_util-0.0.8/src/excel_util/mk_book.py` & `max_util-0.0.9/src/excel_util/mk_book.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.8/src/max_util.egg-info/PKG-INFO` & `max_util-0.0.9/src/max_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 206d 6178  : 2.1..Name: max
 00000020: 2d75 7469 6c0d 0a56 6572 7369 6f6e 3a20  -util..Version: 
-00000030: 302e 302e 380d 0a53 756d 6d61 7279 3a20  0.0.8..Summary: 
+00000030: 302e 302e 390d 0a53 756d 6d61 7279 3a20  0.0.9..Summary: 
 00000040: 696e 7365 7274 2065 7863 656c 2062 6f6f  insert excel boo
 00000050: 6b2c 2062 6173 6520 786c 7774 0d0a 486f  k, base xlwt..Ho
 00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000070: 2f67 6974 6565 2e63 6f6d 2f6d 6178 696e  /gitee.com/maxin
 00000080: 787a 2f6d 6b5f 7574 696c 5f70 7974 686f  xz/mk_util_pytho
 00000090: 6e0d 0a41 7574 686f 723a 206d 6178 0d0a  n..Author: max..
 000000a0: 4175 7468 6f72 2d65 6d61 696c 3a20 6d61  Author-email: ma
```

### Comparing `max_util-0.0.8/src/setting/json_config.py` & `max_util-0.0.9/src/setting/json_config.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.8/src/showdoc/__init__.py` & `max_util-0.0.9/src/showdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.8/src/showdoc/api.py` & `max_util-0.0.9/src/showdoc/api.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.8/src/showdoc/entity.py` & `max_util-0.0.9/src/showdoc/entity.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.8/src/showdoc/util.py` & `max_util-0.0.9/src/showdoc/util.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.8/src/turtle_util/christmas_2021.py` & `max_util-0.0.9/src/turtle_util/christmas_2021.py`

 * *Files identical despite different names*

