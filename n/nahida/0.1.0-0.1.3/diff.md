# Comparing `tmp/nahida-0.1.0.tar.gz` & `tmp/nahida-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nahida-0.1.0.tar", max compression
+gzip compressed data, was "nahida-0.1.3.tar", max compression
```

## Comparing `nahida-0.1.0.tar` & `nahida-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      804 2023-08-04 11:29:01.060538 nahida-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      219 2023-08-04 13:07:30.843140 nahida-0.1.0/README.md
--rw-r--r--   0        0        0     1181 2023-08-04 12:04:03.147147 nahida-0.1.0/src/nahida/__init__.py
--rw-r--r--   0        0        0     1182 2023-08-04 12:03:56.879299 nahida-0.1.0/src/nahida/client/__init__.py
--rw-r--r--   0        0        0     3460 2023-08-04 12:17:02.069798 nahida-0.1.0/src/nahida/client/clients.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 nahida-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      843 2023-08-05 16:01:31.114153 nahida-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      403 2023-08-04 17:47:52.478242 nahida-0.1.3/README.md
+-rw-r--r--   0        0        0     1181 2023-08-04 12:04:03.147147 nahida-0.1.3/src/nahida/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-04 12:03:56.879299 nahida-0.1.3/src/nahida/client/__init__.py
+-rw-r--r--   0        0        0     3480 2023-08-04 17:31:32.058279 nahida-0.1.3/src/nahida/client/clients.py
+-rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 nahida-0.1.3/PKG-INFO
```

### Comparing `nahida-0.1.0/pyproject.toml` & `nahida-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nahida"
-version = "0.1.0"
+version = "0.1.3"
 description = "An unofficial Waifu.pics API wrapper for Python"
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
 packages = [{ include = "nahida", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
+requests = "^2.31.0"
+yarl = "^1.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nahida-0.1.0/src/nahida/__init__.py` & `nahida-0.1.3/src/nahida/__init__.py`

 * *Files identical despite different names*

### Comparing `nahida-0.1.0/src/nahida/client/__init__.py` & `nahida-0.1.3/src/nahida/client/__init__.py`

 * *Files identical despite different names*

### Comparing `nahida-0.1.0/src/nahida/client/clients.py` & `nahida-0.1.3/src/nahida/client/clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     "SFWResource",
     "Client",
 )
 
 import typing
 
 import attrs
-import httpx
+import requests
+import yarl
 
 NSFWCategory = typing.Literal["waifu", "neko", "trap", "blowjob"]
 SFWCategory = typing.Literal[
     "waifu",
     "neko",
     "shinobu",
     "megumin",
@@ -54,15 +55,15 @@
 ]
 
 
 @attrs.define
 class Configuration:
     """"""
 
-    url: httpx.URL
+    url: yarl.URL
 
 
 @attrs.define
 class URLs:
     """"""
 
     configuration: Configuration
@@ -89,15 +90,15 @@
 
     urls: URLs
 
     def search(self, category: NSFWCategory) -> Image:
         """"""
         url = self.urls.nsfw(category)
 
-        response = httpx.get(url)
+        response = requests.get(url)
 
         image = Image(**response.json())
 
         return image
 
 
 @attrs.define
@@ -106,26 +107,26 @@
 
     urls: URLs
 
     def search(self, category: SFWCategory) -> Image:
         """"""
         url = self.urls.sfw(category)
 
-        response = httpx.get(url)
+        response = requests.get(url)
 
         image = Image(**response.json())
 
         return image
 
 
 @attrs.define
 class Client:
     """"""
 
-    __url = httpx.URL("https://api.waifu.pics")
+    __url = yarl.URL("https://api.waifu.pics")
 
     __configuration = Configuration(__url)
 
     __urls = URLs(__configuration)
 
     __nsfw_resource = NSFWResource(__urls)
     __sfw_resource = SFWResource(__urls)
```

### Comparing `nahida-0.1.0/PKG-INFO` & `nahida-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 Metadata-Version: 2.1
 Name: nahida
-Version: 0.1.0
+Version: 0.1.3
 Summary: An unofficial Waifu.pics API wrapper for Python
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
 
-# nahida
+# Nahida
 
 > This is part of `Pudgeland 💖 Open Source` ecosystems
 
-An unofficial **[Waifu.pics]()** API wrapper for Python
+An unofficial **[Waifu.pics](https://waifu.pics)** API wrapper for Python
 
 ## 📦 Packages
 
 ### 🐍 PyPI
 
-```
+```sh
 pip install nahida
 ```
 
 ## 🔎 Examples
 
+```py
+import nahida
+
+client = nahida.Client()
+
+print(client.nsfw.search("neko"))
+
+print(client.sfw.search("awoo"))
+print(client.sfw.search("bite"))
+```
+
```

