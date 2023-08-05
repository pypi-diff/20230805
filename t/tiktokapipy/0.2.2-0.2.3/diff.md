# Comparing `tmp/tiktokapipy-0.2.2.tar.gz` & `tmp/tiktokapipy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktokapipy-0.2.2.tar", last modified: Tue Jul 25 17:25:21 2023, max compression
+gzip compressed data, was "tiktokapipy-0.2.3.tar", last modified: Sat Aug  5 19:57:34 2023, max compression
```

## Comparing `tiktokapipy-0.2.2.tar` & `tiktokapipy-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.371191 tiktokapipy-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.371191 tiktokapipy-0.2.2/src/tiktokapipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/async_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.375191 tiktokapipy-0.2.2/src/tiktokapipy/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/models/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.375191 tiktokapipy-0.2.2/src/tiktokapipy/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/deferred_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/src/tiktokapipy/util/signing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.375191 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 17:25:21.000000 tiktokapipy-0.2.2/src/tiktokapipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:25:21.379190 tiktokapipy-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_slideshow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-25 17:25:06.000000 tiktokapipy-0.2.2/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:34.453376 tiktokapipy-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-05 19:57:34.453376 tiktokapipy-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 19:57:34.453376 tiktokapipy-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:34.445376 tiktokapipy-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:34.449376 tiktokapipy-0.2.3/src/tiktokapipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/async_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:34.449376 tiktokapipy-0.2.3/src/tiktokapipy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/models/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/models/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/models/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:34.449376 tiktokapipy-0.2.3/src/tiktokapipy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/util/deferred_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/util/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/src/tiktokapipy/util/signing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:34.449376 tiktokapipy-0.2.3/src/tiktokapipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-05 19:57:34.000000 tiktokapipy-0.2.3/src/tiktokapipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-05 19:57:34.000000 tiktokapipy-0.2.3/src/tiktokapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:57:34.000000 tiktokapipy-0.2.3/src/tiktokapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-05 19:57:34.000000 tiktokapipy-0.2.3/src/tiktokapipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-05 19:57:34.000000 tiktokapipy-0.2.3/src/tiktokapipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:57:34.449376 tiktokapipy-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/tests/test_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/tests/test_slideshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-05 19:57:24.000000 tiktokapipy-0.2.3/tests/test_video.py
```

### Comparing `tiktokapipy-0.2.2/LICENSE` & `tiktokapipy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/PKG-INFO` & `tiktokapipy-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.2 Summary: Asyncio TikTok
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.3 Summary: Asyncio TikTok
 data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `tiktokapipy-0.2.2/README.md` & `tiktokapipy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/pyproject.toml` & `tiktokapipy-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tiktokapipy"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name="Russell Newton", email="russell.newton01@gmail.com" },
 ]
 description = "Asyncio TikTok data scraping tool"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/__init__.py` & `tiktokapipy-0.2.3/src/tiktokapipy/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/api.py` & `tiktokapipy-0.2.3/src/tiktokapipy/api.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/async_api.py` & `tiktokapipy-0.2.3/src/tiktokapipy/async_api.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/models/__init__.py` & `tiktokapipy-0.2.3/src/tiktokapipy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/models/challenge.py` & `tiktokapipy-0.2.3/src/tiktokapipy/models/challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/models/comment.py` & `tiktokapipy-0.2.3/src/tiktokapipy/models/comment.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/models/raw_data.py` & `tiktokapipy-0.2.3/src/tiktokapipy/models/raw_data.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/models/user.py` & `tiktokapipy-0.2.3/src/tiktokapipy/models/user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/models/video.py` & `tiktokapipy-0.2.3/src/tiktokapipy/models/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 class VideoStats(CamelCaseModel):
     digg_count: int
     share_count: int
     comment_count: int
     play_count: int
+    collect_count: int
 
 
 class SubtitleData(TitleCaseModel):
     language_id: int
     language_code_name: str
     url: str
     url_expire: int
@@ -115,15 +116,15 @@
 class ImagePost(CamelCaseModel):
     images: List[ImageData]
     """All images in the slideshow"""
     cover: ImageData
     """Still image on the video before playing"""
     share_cover: ImageData
     """Still image embedded with a sharing link"""
-    title: str
+    title: Optional[str] = None
 
 
 class LightVideo(CamelCaseModel):
     """Bare minimum information for scraping"""
 
     id: int = Field(validation_alias=AliasChoices("cid", "uid", "id"))
     """The unique video ID"""
```

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/util/deferred_collectors.py` & `tiktokapipy-0.2.3/src/tiktokapipy/util/deferred_collectors.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/util/queries.py` & `tiktokapipy-0.2.3/src/tiktokapipy/util/queries.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy/util/signing.py` & `tiktokapipy-0.2.3/src/tiktokapipy/util/signing.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy.egg-info/PKG-INFO` & `tiktokapipy-0.2.3/src/tiktokapipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.2 Summary: Asyncio TikTok
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.3 Summary: Asyncio TikTok
 data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `tiktokapipy-0.2.2/src/tiktokapipy.egg-info/SOURCES.txt` & `tiktokapipy-0.2.3/src/tiktokapipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/tests/test_challenge.py` & `tiktokapipy-0.2.3/tests/test_challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/tests/test_slideshow.py` & `tiktokapipy-0.2.3/tests/test_slideshow.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/tests/test_user.py` & `tiktokapipy-0.2.3/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.2/tests/test_video.py` & `tiktokapipy-0.2.3/tests/test_video.py`

 * *Files identical despite different names*

