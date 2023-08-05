# Comparing `tmp/findmyorder-1.7.3.tar.gz` & `tmp/findmyorder-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.7.3.tar", max compression
+gzip compressed data, was "findmyorder-1.7.5.tar", max compression
```

## Comparing `findmyorder-1.7.3.tar` & `findmyorder-1.7.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-08-03 20:06:00.966118 findmyorder-1.7.3/LICENSE
--rw-r--r--   0        0        0     3022 2023-08-03 20:06:00.966118 findmyorder-1.7.3/README.md
--rw-r--r--   0        0        0      113 2023-08-03 20:06:04.494188 findmyorder-1.7.3/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-08-03 20:06:00.970118 findmyorder-1.7.3/findmyorder/config.py
--rw-r--r--   0        0        0     3221 2023-08-03 20:06:00.970118 findmyorder-1.7.3/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5931 2023-08-03 20:06:00.970118 findmyorder-1.7.3/findmyorder/main.py
--rw-r--r--   0        0        0     2878 2023-08-03 20:06:04.486188 findmyorder-1.7.3/pyproject.toml
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 findmyorder-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-05 16:15:37.301501 findmyorder-1.7.5/LICENSE
+-rw-r--r--   0        0        0     2834 2023-08-05 16:15:37.301501 findmyorder-1.7.5/README.md
+-rw-r--r--   0        0        0      113 2023-08-05 16:15:47.497521 findmyorder-1.7.5/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-08-05 16:15:37.305501 findmyorder-1.7.5/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-08-05 16:15:37.305501 findmyorder-1.7.5/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5931 2023-08-05 16:15:37.305501 findmyorder-1.7.5/findmyorder/main.py
+-rw-r--r--   0        0        0     2878 2023-08-05 16:15:47.489521 findmyorder-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 findmyorder-1.7.5/PKG-INFO
```

### Comparing `findmyorder-1.7.3/LICENSE` & `findmyorder-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.3/README.md` & `findmyorder-1.7.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 <table style="border: 1px solid transparent">
   <tr>
     <td>
-<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a><br>
-<a href="https://github.com/mraniki/findmyorder/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a>
-<a href="https://discord.gg/gMNERs5M9"><img src="https://img.shields.io/discord/1049307055867035648?style=for-the-badge&logo=discord&logoColor=white&label=%20%20&color=blue"></a>
+<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
+<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
+<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/v/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/dm/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
```

#### html2text {}

```diff
@@ -1,32 +1,39 @@
-[https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
-the-badge&logo=wikipedia&logoColor=white]
+[https://img.shields.io/badge/Wiki-
+%23000000.svg?style=for-the-
+badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
 %23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [https://img.shields.io/
-docker/pulls/mraniki/tt?style=for-the-badge]                        [Logo]
-[https://img.shields.io/badge/tips-000000?style=for-the-
-badge&logo=buymeacoffee&logoColor=white] [https://
-img.shields.io/badge/talky-blue?style=for-the-
-badge&logo=telegram&logoColor=white] [https://
-img.shields.io/discord/1049307055867035648?style=for-the-
-badge&logo=discord&logoColor=white&label=%20%20&color=blue]
-[https://img.shields.io/pypi/v/findmyorder?style=for-the-
+badge&logo=github&logoColor=white]
+[https://img.shields.io/badge/tips-                          [Logo]
+000000?style=for-the-
+badge&logo=buymeacoffee&logoColor=white]
+[https://img.shields.io/docker/pulls/
+mraniki/tt?style=for-the-badge] [https:/
+/img.shields.io/badge/talky-
+blue?style=for-the-
+badge&logo=telegram&logoColor=white]
+[https://img.shields.io/pypi/v/
+findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/pypi/dm/findmyorder?style=for-the-
+[https://img.shields.io/pypi/dm/
+findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/github/actions/workflow/status/     Find My order,
-mraniki/findmyorder/%F0%9F%91%B7Flow.yml?style=for-the-     a parsing package
-badge&logo=GitHub&logoColor=white]                          to find trading
-[https://readthedocs.org/projects/findmyorder/badge/        order
+[https://img.shields.io/github/actions/
+workflow/status/mraniki/findmyorder/     Find My order,
+%F0%9F%91%B7Flow.yml?style=for-the-      a parsing package to find trading
+badge&logo=GitHub&logoColor=white]       order
+[https://readthedocs.org/projects/
+findmyorder/badge/
 ?version=latest&style=for-the-badge]
-[https://codebeat.co/badges/9b113098-d22d-498d-9c61-
-eb1e96c1311a]
-[https://codecov.io/gh/mraniki/findmyorder/branch/main/
-graph/badge.svg?token=4838MSZNCC]
+[https://codebeat.co/badges/9b113098-
+d22d-498d-9c61-eb1e96c1311a]
+[https://codecov.io/gh/mraniki/
+findmyorder/branch/main/graph/
+badge.svg?token=4838MSZNCC]
 ** How to use it **
 
       from findmyorder import FindMyOrder
          fmo = FindMyOrder()
          msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
          order = await fmo.get_order(msg_order)
          #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000',
```

### Comparing `findmyorder-1.7.3/findmyorder/config.py` & `findmyorder-1.7.5/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.3/findmyorder/default_settings.toml` & `findmyorder-1.7.5/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.3/findmyorder/main.py` & `findmyorder-1.7.5/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.3/pyproject.toml` & `findmyorder-1.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.7.3"
+version = "1.7.5"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

### Comparing `findmyorder-1.7.3/PKG-INFO` & `findmyorder-1.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.7.3
+Version: 1.7.5
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,20 +19,19 @@
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
-<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a><br>
-<a href="https://github.com/mraniki/findmyorder/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a>
-<a href="https://discord.gg/gMNERs5M9"><img src="https://img.shields.io/discord/1049307055867035648?style=for-the-badge&logo=discord&logoColor=white&label=%20%20&color=blue"></a>
+<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
+<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
+<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/v/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/dm/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
```

#### html2text {}

```diff
@@ -1,45 +1,52 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.7.3 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.7.5 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist: loguru
 (>=0.7.0,<0.8.0) Requires-Dist: pyparsing (>=3.0.9,<4.0.0) Project-URL:
 Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues Project-URL:
 Support, https://github.com/mraniki/findmyorder/discussions Description-
 Content-Type: text/markdown
-[https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
-the-badge&logo=wikipedia&logoColor=white]
+[https://img.shields.io/badge/Wiki-
+%23000000.svg?style=for-the-
+badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
 %23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [https://img.shields.io/
-docker/pulls/mraniki/tt?style=for-the-badge]                        [Logo]
-[https://img.shields.io/badge/tips-000000?style=for-the-
-badge&logo=buymeacoffee&logoColor=white] [https://
-img.shields.io/badge/talky-blue?style=for-the-
-badge&logo=telegram&logoColor=white] [https://
-img.shields.io/discord/1049307055867035648?style=for-the-
-badge&logo=discord&logoColor=white&label=%20%20&color=blue]
-[https://img.shields.io/pypi/v/findmyorder?style=for-the-
+badge&logo=github&logoColor=white]
+[https://img.shields.io/badge/tips-                          [Logo]
+000000?style=for-the-
+badge&logo=buymeacoffee&logoColor=white]
+[https://img.shields.io/docker/pulls/
+mraniki/tt?style=for-the-badge] [https:/
+/img.shields.io/badge/talky-
+blue?style=for-the-
+badge&logo=telegram&logoColor=white]
+[https://img.shields.io/pypi/v/
+findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/pypi/dm/findmyorder?style=for-the-
+[https://img.shields.io/pypi/dm/
+findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/github/actions/workflow/status/     Find My order,
-mraniki/findmyorder/%F0%9F%91%B7Flow.yml?style=for-the-     a parsing package
-badge&logo=GitHub&logoColor=white]                          to find trading
-[https://readthedocs.org/projects/findmyorder/badge/        order
+[https://img.shields.io/github/actions/
+workflow/status/mraniki/findmyorder/     Find My order,
+%F0%9F%91%B7Flow.yml?style=for-the-      a parsing package to find trading
+badge&logo=GitHub&logoColor=white]       order
+[https://readthedocs.org/projects/
+findmyorder/badge/
 ?version=latest&style=for-the-badge]
-[https://codebeat.co/badges/9b113098-d22d-498d-9c61-
-eb1e96c1311a]
-[https://codecov.io/gh/mraniki/findmyorder/branch/main/
-graph/badge.svg?token=4838MSZNCC]
+[https://codebeat.co/badges/9b113098-
+d22d-498d-9c61-eb1e96c1311a]
+[https://codecov.io/gh/mraniki/
+findmyorder/branch/main/graph/
+badge.svg?token=4838MSZNCC]
 ** How to use it **
 
       from findmyorder import FindMyOrder
          fmo = FindMyOrder()
          msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
          order = await fmo.get_order(msg_order)
          #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000',
```

