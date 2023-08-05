# Comparing `tmp/alhaitham-0.1.0.tar.gz` & `tmp/alhaitham-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alhaitham-0.1.0.tar", max compression
+gzip compressed data, was "alhaitham-0.1.3.tar", max compression
```

## Comparing `alhaitham-0.1.0.tar` & `alhaitham-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      826 2023-08-04 11:42:48.792056 alhaitham-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      222 2023-08-04 13:07:25.608557 alhaitham-0.1.0/README.md
--rw-r--r--   0        0        0     1181 2023-08-04 12:55:25.322215 alhaitham-0.1.0/src/alhaitham/__init__.py
--rw-r--r--   0        0        0     1182 2023-08-04 11:58:50.689698 alhaitham-0.1.0/src/alhaitham/client/__init__.py
--rw-r--r--   0        0        0     2433 2023-08-04 12:15:02.331814 alhaitham-0.1.0/src/alhaitham/client/clients.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 alhaitham-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      865 2023-08-05 16:06:31.603005 alhaitham-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      365 2023-08-04 17:48:45.689643 alhaitham-0.1.3/README.md
+-rw-r--r--   0        0        0     1181 2023-08-04 12:55:25.322215 alhaitham-0.1.3/src/alhaitham/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-04 11:58:50.689698 alhaitham-0.1.3/src/alhaitham/client/__init__.py
+-rw-r--r--   0        0        0     2450 2023-08-04 17:26:56.558692 alhaitham-0.1.3/src/alhaitham/client/clients.py
+-rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 alhaitham-0.1.3/PKG-INFO
```

### Comparing `alhaitham-0.1.0/pyproject.toml` & `alhaitham-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alhaitham"
-version = "0.1.0"
+version = "0.1.3"
 description = "An unofficial The Dog API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/eleresai/pudgeland"
 repository = "https://github.com/eleresai/pudgeland"
@@ -17,11 +17,13 @@
     "Programming Language :: Python :: 3.8",
 ]
 packages = [{ include = "alhaitham", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 attrs = "^23.1.0"
+requests = "^2.31.0"
+yarl = "^1.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alhaitham-0.1.0/src/alhaitham/__init__.py` & `alhaitham-0.1.3/src/alhaitham/__init__.py`

 * *Files identical despite different names*

### Comparing `alhaitham-0.1.0/src/alhaitham/client/__init__.py` & `alhaitham-0.1.3/src/alhaitham/client/__init__.py`

 * *Files identical despite different names*

### Comparing `alhaitham-0.1.0/src/alhaitham/client/clients.py` & `alhaitham-0.1.3/src/alhaitham/client/clients.py`

 * *Files 7% similar despite different names*

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
 
-    __url = httpx.URL("https://api.thedogapi.com/v1")
+    __url = yarl.URL("https://api.thedogapi.com/v1")
 
     __configuration = Configuration(__url)
 
     __urls = URLs(__configuration)
 
     __image_resource = ImageResource(__urls)
```

### Comparing `alhaitham-0.1.0/PKG-INFO` & `alhaitham-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alhaitham
-Version: 0.1.0
+Version: 0.1.3
 Summary: An unofficial The Dog API wrapper for Python
 Home-page: https://github.com/eleresai/pudgeland
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
@@ -12,26 +12,37 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Project-URL: Repository, https://github.com/eleresai/pudgeland
 Description-Content-Type: text/markdown
 
-# alhaitham
+# Alhaitham
 
 > This is part of `Pudgeland 💖 Open Source` ecosystems
 
-An unofficial **[The Dog API]()** wrapper for Python
+An unofficial **[The Dog API](https://thedogapi.com)** wrapper for Python
 
 ## 📦 Packages
 
 ### 🐍 PyPI
 
-```
+```sh
 pip install alhaitham
 ```
 
 ## 🔎 Examples
 
+```py
+import alhaitham
+
+client = alhaitham.Client()
+
+for _ in range(5):
+    print(client.images.search())
+```
+
```

