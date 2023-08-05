# Comparing `tmp/hyko_sdk-0.3.0b7.tar.gz` & `tmp/hyko_sdk-0.3.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.3.0b7.tar", last modified: Fri Aug  4 21:43:08 2023, max compression
+gzip compressed data, was "hyko_sdk-0.3.0b8.tar", last modified: Fri Aug  4 23:11:11 2023, max compression
```

## Comparing `hyko_sdk-0.3.0b7.tar` & `hyko_sdk-0.3.0b8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 21:43:08.323556 hyko_sdk-0.3.0b7/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 21:43:08.323556 hyko_sdk-0.3.0b7/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       16 2023-08-04 19:47:01.000000 hyko_sdk-0.3.0b7/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 21:43:08.323556 hyko_sdk-0.3.0b7/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       63 2023-08-04 19:54:46.000000 hyko_sdk-0.3.0b7/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b7/hyko_sdk/error.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14646 2023-08-04 19:43:32.000000 hyko_sdk-0.3.0b7/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1377 2023-08-04 19:41:51.000000 hyko_sdk-0.3.0b7/hyko_sdk/metadata.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 21:36:11.000000 hyko_sdk-0.3.0b7/hyko_sdk/py.typed
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b7/hyko_sdk/utils.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 21:43:08.323556 hyko_sdk-0.3.0b7/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 21:43:08.000000 hyko_sdk-0.3.0b7/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      304 2023-08-04 21:43:08.000000 hyko_sdk-0.3.0b7/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 21:43:08.000000 hyko_sdk-0.3.0b7/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      114 2023-08-04 21:43:08.000000 hyko_sdk-0.3.0b7/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 21:43:08.000000 hyko_sdk-0.3.0b7/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b7/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      513 2023-08-04 21:43:08.326889 hyko_sdk-0.3.0b7/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       16 2023-08-04 19:47:01.000000 hyko_sdk-0.3.0b8/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       63 2023-08-04 19:54:46.000000 hyko_sdk-0.3.0b8/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b8/hyko_sdk/error.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14646 2023-08-04 19:43:32.000000 hyko_sdk-0.3.0b8/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1394 2023-08-04 23:10:51.000000 hyko_sdk-0.3.0b8/hyko_sdk/metadata.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 21:36:11.000000 hyko_sdk-0.3.0b8/hyko_sdk/py.typed
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b8/hyko_sdk/utils.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      304 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      114 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b8/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      513 2023-08-04 23:11:11.107232 hyko_sdk-0.3.0b8/setup.cfg
```

### Comparing `hyko_sdk-0.3.0b7/hyko_sdk/error.py` & `hyko_sdk-0.3.0b8/hyko_sdk/error.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b7/hyko_sdk/io.py` & `hyko_sdk-0.3.0b8/hyko_sdk/io.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b7/hyko_sdk/metadata.py` & `hyko_sdk-0.3.0b8/hyko_sdk/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class HykoExtraTypes(str, Enum):
     IMAGE = "image"
     AUDIO = "audio"
     VIDEO = "video"
     
 class Property(BaseModel):
-    type: IOPortType | HykoExtraTypes
+    type: Optional[IOPortType | HykoExtraTypes] = None
     anyOf: Optional [List['Property']] = None
     items: Optional[Union['Property', List['Property']]] = None
     prefixItems: Optional[List['Property']] = None
     minItems: Optional[int] = None
     maxItems: Optional[int] = None
     description: Optional[str] = None
     default: Optional[Any] = None
```

### Comparing `hyko_sdk-0.3.0b7/hyko_sdk/utils.py` & `hyko_sdk-0.3.0b8/hyko_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b7/setup.cfg` & `hyko_sdk-0.3.0b8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hyko_sdk
-version = 0.3.0b7
+version = 0.3.0b8
 author = Abdelmadjid Dahmani, Lotfi Lehamel
 author_email = amd2@big-mama.io, ll@big-mama.io
 url = https://hyko.ai
 
 [options]
 packages = find:
 python_requires = >=3.8
```

