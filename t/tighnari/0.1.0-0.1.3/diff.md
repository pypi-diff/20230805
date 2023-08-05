# Comparing `tmp/tighnari-0.1.0.tar.gz` & `tmp/tighnari-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tighnari-0.1.0.tar", max compression
+gzip compressed data, was "tighnari-0.1.3.tar", max compression
```

## Comparing `tighnari-0.1.0.tar` & `tighnari-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      805 2023-08-04 11:29:14.486759 tighnari-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      220 2023-08-04 13:07:35.063172 tighnari-0.1.0/README.md
--rw-r--r--   0        0        0     1181 2023-08-04 12:01:36.083235 tighnari-0.1.0/src/tighnari/__init__.py
--rw-r--r--   0        0        0     1182 2023-08-04 12:01:27.651238 tighnari-0.1.0/src/tighnari/client/__init__.py
--rw-r--r--   0        0        0     2433 2023-08-04 12:18:06.799165 tighnari-0.1.0/src/tighnari/client/clients.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 tighnari-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      844 2023-08-05 16:11:12.215074 tighnari-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      361 2023-08-04 18:04:11.792565 tighnari-0.1.3/README.md
+-rw-r--r--   0        0        0     1181 2023-08-04 12:01:36.083235 tighnari-0.1.3/src/tighnari/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-04 12:01:27.651238 tighnari-0.1.3/src/tighnari/client/__init__.py
+-rw-r--r--   0        0        0     2450 2023-08-04 17:27:35.146308 tighnari-0.1.3/src/tighnari/client/clients.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 tighnari-0.1.3/PKG-INFO
```

### Comparing `tighnari-0.1.0/pyproject.toml` & `tighnari-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tighnari"
-version = "0.1.0"
+version = "0.1.3"
 description = "An unofficial The Cat API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/eleresai/pudgeland"
 repository = "https://github.com/eleresai/pudgeland"
@@ -16,11 +16,13 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.8",
 ]
 packages = [{ include = "tighnari", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
+requests = "^2.31.0"
+yarl = "^1.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tighnari-0.1.0/src/tighnari/__init__.py` & `tighnari-0.1.3/src/tighnari/__init__.py`

 * *Files identical despite different names*

### Comparing `tighnari-0.1.0/src/tighnari/client/__init__.py` & `tighnari-0.1.3/src/tighnari/client/__init__.py`

 * *Files identical despite different names*

### Comparing `tighnari-0.1.0/src/tighnari/client/clients.py` & `tighnari-0.1.3/src/tighnari/client/clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,24 @@
     "ImageResource",
     "Client",
 )
 
 import typing
 
 import attrs
-import httpx
 import msgspec
+import requests
+import yarl
 
 
 @attrs.define
 class Configuration:
     """"""
 
-    url: httpx.URL
+    url: yarl.URL
 
 
 @attrs.define
 class URLs:
     """"""
 
     configuration: Configuration
@@ -50,30 +51,30 @@
 class ImageResource:
     """"""
 
     urls: URLs
 
     def search(self) -> typing.Sequence[Image]:
         """"""
-        response = httpx.get(self.urls.search())
+        response = requests.get(self.urls.search())
 
         content = response.content
 
         buf = content
 
         image = msgspec.json.decode(buf, type=typing.Sequence[Image])
 
         return image
 
 
 @attrs.define
 class Client:
     """"""
 
-    __url = httpx.URL("https://api.thecatapi.com/v1")
+    __url = yarl.URL("https://api.thecatapi.com/v1")
 
     __configuration = Configuration(__url)
 
     __urls = URLs(__configuration)
 
     __image_resource = ImageResource(__urls)
```

### Comparing `tighnari-0.1.0/PKG-INFO` & `tighnari-0.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 Metadata-Version: 2.1
 Name: tighnari
-Version: 0.1.0
+Version: 0.1.3
 Summary: An unofficial The Cat API wrapper for Python
 Home-page: https://github.com/eleresai/pudgeland
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Project-URL: Repository, https://github.com/eleresai/pudgeland
 Description-Content-Type: text/markdown
 
-# tighnari
+# Tighnari
 
 > This is part of `Pudgeland 💖 Open Source` ecosystems
 
-An unofficial **[The Cat API]()** wrapper for Python
+An unofficial **[The Cat API](https://thecatapi.com)** wrapper for Python
 
 ## 📦 Packages
 
 ### 🐍 PyPI
 
-```
+```sh
 pip install tighnari
 ```
 
 ## 🔎 Examples
 
+```py
+import tighnari
+
+client = tighnari.Client()
+
+for _ in range(5):
+    print(client.images.search())
+```
+
```

