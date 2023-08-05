# Comparing `tmp/plateaukit-0.1.1.tar.gz` & `tmp/plateaukit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plateaukit-0.1.1.tar", max compression
+gzip compressed data, was "plateaukit-0.2.0.tar", max compression
```

## Comparing `plateaukit-0.1.1.tar` & `plateaukit-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0        0 2023-01-25 10:05:54.179931 plateaukit-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2403 2023-02-20 20:28:28.888524 plateaukit-0.1.1/README.md
--rw-r--r--   0        0        0      102 2023-02-15 05:45:06.171105 plateaukit-0.1.1/plateaukit/__init__.py
--rw-r--r--   0        0        0    10796 2023-02-20 20:22:07.797627 plateaukit-0.1.1/plateaukit/cli.py
--rw-r--r--   0        0        0     1511 2023-02-20 20:05:53.017946 plateaukit-0.1.1/plateaukit/config.py
--rw-r--r--   0        0        0      342 2023-02-01 09:19:50.251365 plateaukit-0.1.1/plateaukit/constants.py
--rw-r--r--   0        0        0      176 2023-01-04 09:01:29.252896 plateaukit-0.1.1/plateaukit/db.py
--rw-r--r--   0        0        0       28 2023-01-25 11:52:41.173316 plateaukit-0.1.1/plateaukit/download/__init__.py
--rw-r--r--   0        0        0     3124 2023-02-20 19:22:31.645954 plateaukit-0.1.1/plateaukit/download/downloader.py
--rw-r--r--   0        0        0    16465 2023-02-20 19:56:06.737527 plateaukit-0.1.1/plateaukit/download/list.py
--rw-r--r--   0        0        0       50 2023-02-01 07:57:22.009188 plateaukit-0.1.1/plateaukit/extractors/__init__.py
--rw-r--r--   0        0        0     3534 2023-02-01 07:57:22.999088 plateaukit-0.1.1/plateaukit/extractors/commands.py
--rw-r--r--   0        0        0     4110 2023-01-25 18:07:04.449073 plateaukit-0.1.1/plateaukit/extractors/utils.py
--rw-r--r--   0        0        0      115 2023-02-15 05:32:55.576474 plateaukit-0.1.1/plateaukit/generators/__init__.py
--rw-r--r--   0        0        0     6372 2023-02-20 20:30:10.810839 plateaukit-0.1.1/plateaukit/generators/_geojson.py
--rw-r--r--   0        0        0     1467 2023-01-25 16:23:24.478400 plateaukit-0.1.1/plateaukit/generators/cityjson.py
--rw-r--r--   0        0        0     2016 2023-02-10 03:52:17.351972 plateaukit-0.1.1/plateaukit/generators/quantized_mesh.py
--rw-r--r--   0        0        0     8979 2023-02-09 15:01:43.087655 plateaukit-0.1.1/plateaukit/generators/simplecityjson.py
--rw-r--r--   0        0        0      669 2023-01-25 09:30:56.713474 plateaukit-0.1.1/plateaukit/generators/utils.py
--rw-r--r--   0        0        0      817 2023-01-04 09:11:09.158451 plateaukit-0.1.1/plateaukit/models.py
--rw-r--r--   0        0        0      537 2023-02-09 15:01:25.939660 plateaukit-0.1.1/plateaukit/utils.py
--rw-r--r--   0        0        0      931 2023-02-20 20:36:07.525772 plateaukit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 plateaukit-0.1.1/setup.py
--rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 plateaukit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-05 20:23:37.128244 plateaukit-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2695 2023-08-05 20:24:43.812016 plateaukit-0.2.0/README.md
+-rw-r--r--   0        0        0      102 2023-08-05 20:23:37.131452 plateaukit-0.2.0/plateaukit/__init__.py
+-rw-r--r--   0        0        0    10796 2023-08-05 20:23:37.131793 plateaukit-0.2.0/plateaukit/cli.py
+-rw-r--r--   0        0        0     1397 2023-08-05 20:23:37.132212 plateaukit-0.2.0/plateaukit/config.py
+-rw-r--r--   0        0        0      342 2023-08-05 20:23:37.132437 plateaukit-0.2.0/plateaukit/constants.py
+-rw-r--r--   0        0        0      176 2023-08-05 20:23:37.132711 plateaukit-0.2.0/plateaukit/db.py
+-rw-r--r--   0        0        0       28 2023-08-05 20:23:37.133049 plateaukit-0.2.0/plateaukit/download/__init__.py
+-rw-r--r--   0        0        0     3124 2023-08-05 20:23:37.133363 plateaukit-0.2.0/plateaukit/download/downloader.py
+-rw-r--r--   0        0        0    16465 2023-08-05 20:23:37.133837 plateaukit-0.2.0/plateaukit/download/list.py
+-rw-r--r--   0        0        0       50 2023-08-05 20:23:37.134175 plateaukit-0.2.0/plateaukit/extractors/__init__.py
+-rw-r--r--   0        0        0     3534 2023-08-05 20:23:37.134599 plateaukit-0.2.0/plateaukit/extractors/commands.py
+-rw-r--r--   0        0        0     4110 2023-08-05 20:23:37.135004 plateaukit-0.2.0/plateaukit/extractors/utils.py
+-rw-r--r--   0        0        0      115 2023-08-05 20:23:37.135385 plateaukit-0.2.0/plateaukit/generators/__init__.py
+-rw-r--r--   0        0        0     6372 2023-08-05 20:23:37.135650 plateaukit-0.2.0/plateaukit/generators/_geojson.py
+-rw-r--r--   0        0        0     1467 2023-08-05 20:23:37.135933 plateaukit-0.2.0/plateaukit/generators/cityjson.py
+-rw-r--r--   0        0        0     2016 2023-08-05 20:23:37.136162 plateaukit-0.2.0/plateaukit/generators/quantized_mesh.py
+-rw-r--r--   0        0        0     8979 2023-08-05 20:23:37.136401 plateaukit-0.2.0/plateaukit/generators/simplecityjson.py
+-rw-r--r--   0        0        0      669 2023-08-05 20:23:37.136619 plateaukit-0.2.0/plateaukit/generators/utils.py
+-rw-r--r--   0        0        0      817 2023-08-05 20:23:37.136818 plateaukit-0.2.0/plateaukit/models.py
+-rw-r--r--   0        0        0      537 2023-08-05 20:23:37.137166 plateaukit-0.2.0/plateaukit/utils.py
+-rw-r--r--   0        0        0     1140 2023-08-05 20:26:25.993749 plateaukit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 plateaukit-0.2.0/PKG-INFO
```

### Comparing `plateaukit-0.1.1/README.md` & `plateaukit-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # PlateauKit
 
+[![PyPI](https://img.shields.io/pypi/v/plateaukit.svg)](https://pypi.org/project/plateaukit/)
+<!-- [![PyPI downloads](https://img.shields.io/pypi/dm/plateaukit.svg)](https://pypistats.org/packages/plateaukit) -->
+
 > Python library and converter for 3D city models by MLIT Project PLATEAU
 
 国土交通省PLATEAU 3D都市モデルのPythonライブラリおよび変換ツール (WIP)
 
+**ドキュメント Documentation:** <https://ozekik.github.io/plateaukit/>
+
 ## 特徴 Features
 
 - [x] PLATEAUデータセットのインストール・管理
 - [x] 並列処理でのデータ変換
 - [x] citygml-tools / citygml4j (Java) に依存せずCityJSONを生成 (一部)
 - [ ] JupyterLab / Jupyer Notebookでの3D都市モデル表示 (LOD1/2)
```

### Comparing `plateaukit-0.1.1/plateaukit/cli.py` & `plateaukit-0.2.0/plateaukit/cli.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/download/downloader.py` & `plateaukit-0.2.0/plateaukit/download/downloader.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/download/list.py` & `plateaukit-0.2.0/plateaukit/download/list.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/extractors/commands.py` & `plateaukit-0.2.0/plateaukit/extractors/commands.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/extractors/utils.py` & `plateaukit-0.2.0/plateaukit/extractors/utils.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/generators/_geojson.py` & `plateaukit-0.2.0/plateaukit/generators/_geojson.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/generators/cityjson.py` & `plateaukit-0.2.0/plateaukit/generators/cityjson.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/generators/quantized_mesh.py` & `plateaukit-0.2.0/plateaukit/generators/quantized_mesh.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/generators/simplecityjson.py` & `plateaukit-0.2.0/plateaukit/generators/simplecityjson.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/generators/utils.py` & `plateaukit-0.2.0/plateaukit/generators/utils.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/models.py` & `plateaukit-0.2.0/plateaukit/models.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/plateaukit/utils.py` & `plateaukit-0.2.0/plateaukit/utils.py`

 * *Files identical despite different names*

### Comparing `plateaukit-0.1.1/pyproject.toml` & `plateaukit-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plateaukit"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Kentaro Ozeki <32771324+ozekik@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "plateaukit" }]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
@@ -18,25 +18,33 @@
 xmltodict = "^0.13.0"
 tortoise-orm = "^0.19.2"
 joblib = "^1.2.0"
 aiomultiprocess = "^0.9.0"
 geopandas = "^0.12.2"
 prettytable = "^3.6.0"
 requests = "^2.28.2"
-xdg = "^5.1.1"
 pydantic = "^1.10.4"
 bidict = "^0.22.1"
 pyogrio = "^0.5.1"
 quantized-mesh-encoder = "^0.4.3"
 numpy = "<1.24"
+platformdirs = "^3.10.0"
 
 [tool.poetry.scripts]
 plateaukit = "plateaukit.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
 pyglet = "^1.5.27"
 scipy = "^1.10.0"
 matplotlib = "^3.6.3"
 
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.5.2"
+mkdocs-material = "^9.1.21"
+mkdocstrings-python = "^1.2.1"
+mkdocs-exclude = "^1.0.2"
+markdown-exec = {extras = ["ansi"], version = "^1.6.0"}
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `plateaukit-0.1.1/PKG-INFO` & `plateaukit-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plateaukit
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Kentaro Ozeki
 Author-email: 32771324+ozekik@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,32 +16,37 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: geojson (>=2.5.0,<3.0.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: numpy (<1.24)
+Requires-Dist: platformdirs (>=3.10.0,<4.0.0)
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pyogrio (>=0.5.1,<0.6.0)
 Requires-Dist: pyproj (>=3.4.1,<4.0.0)
 Requires-Dist: quantized-mesh-encoder (>=0.4.3,<0.5.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tortoise-orm (>=0.19.2,<0.20.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: xdg (>=5.1.1,<6.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # PlateauKit
 
+[![PyPI](https://img.shields.io/pypi/v/plateaukit.svg)](https://pypi.org/project/plateaukit/)
+<!-- [![PyPI downloads](https://img.shields.io/pypi/dm/plateaukit.svg)](https://pypistats.org/packages/plateaukit) -->
+
 > Python library and converter for 3D city models by MLIT Project PLATEAU
 
 国土交通省PLATEAU 3D都市モデルのPythonライブラリおよび変換ツール (WIP)
 
+**ドキュメント Documentation:** <https://ozekik.github.io/plateaukit/>
+
 ## 特徴 Features
 
 - [x] PLATEAUデータセットのインストール・管理
 - [x] 並列処理でのデータ変換
 - [x] citygml-tools / citygml4j (Java) に依存せずCityJSONを生成 (一部)
 - [ ] JupyterLab / Jupyer Notebookでの3D都市モデル表示 (LOD1/2)
```

