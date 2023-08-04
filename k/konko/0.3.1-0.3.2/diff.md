# Comparing `tmp/konko-0.3.1.tar.gz` & `tmp/konko-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.3.1.tar", max compression
+gzip compressed data, was "konko-0.3.2.tar", max compression
```

## Comparing `konko-0.3.1.tar` & `konko-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0       69 2023-07-28 02:05:43.140409 konko-0.3.1/README.md
--rw-r--r--   0        0        0      781 2023-07-28 19:56:11.684067 konko-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      119 2023-07-28 02:25:11.693562 konko-0.3.1/src/konko/__init__.py
--rw-r--r--   0        0        0      271 2023-07-28 00:39:32.576415 konko-0.3.1/src/konko/app.py
--rw-r--r--   0        0        0     1887 2023-07-04 09:17:33.179238 konko-0.3.1/src/konko/evaluate.py
--rw-r--r--   0        0        0     5125 2023-07-28 19:55:24.229054 konko-0.3.1/src/konko/generate.py
--rw-r--r--   0        0        0     3109 2023-07-28 02:26:15.872754 konko-0.3.1/src/konko/models.py
--rw-r--r--   0        0        0        0 2023-07-04 09:17:33.179880 konko-0.3.1/src/konko/utils/__init__.py
--rw-r--r--   0        0        0       42 2023-07-26 11:54:54.315365 konko-0.3.1/src/konko/utils/constants.py
--rw-r--r--   0        0        0     1362 2023-07-28 02:17:37.991856 konko-0.3.1/src/konko/utils/logs.py
--rw-r--r--   0        0        0      378 2023-07-28 01:51:28.605708 konko-0.3.1/src/konko/utils/utils.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 konko-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-07-28 02:05:43.140409 konko-0.3.2/README.md
+-rw-r--r--   0        0        0      776 2023-08-04 20:51:57.300572 konko-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-08-04 21:04:02.230274 konko-0.3.2/src/konko/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-28 00:39:32.576415 konko-0.3.2/src/konko/app.py
+-rw-r--r--   0        0        0     5125 2023-07-28 19:55:24.229054 konko-0.3.2/src/konko/generate.py
+-rw-r--r--   0        0        0     3109 2023-07-28 02:26:15.872754 konko-0.3.2/src/konko/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:17:33.179880 konko-0.3.2/src/konko/utils/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-26 11:54:54.315365 konko-0.3.2/src/konko/utils/constants.py
+-rw-r--r--   0        0        0     1362 2023-07-28 02:17:37.991856 konko-0.3.2/src/konko/utils/logs.py
+-rw-r--r--   0        0        0      378 2023-07-28 01:51:28.605708 konko-0.3.2/src/konko/utils/utils.py
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 konko-0.3.2/PKG-INFO
```

### Comparing `konko-0.3.1/pyproject.toml` & `konko-0.3.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "konko"
-version = "0.3.1"
+version = "0.3.2"
 description = "\"Konko AI Python SDK: A client library to interact with Konko AI's API. With this SDK, developers can integrate, evaluate, fine-tune, and deploy Large Language Models (LLMs) using Konko AI's fully-managed, SOC 2 compliant platform. Ideal for enterprise use-cases, it allows you to focus on building great products without worrying about infrastructure.\""
 authors = ["Konko AI"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
-requests = "^2.31.0"
-fastapi = "^0.100.0"
-pydantic = "^2.0.3"
+requests = "^2.28.0"
+fastapi = "^0.95.0"
+pydantic = "^1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 uvicorn = "^0.22.0"
 locust = "^2.15.1"
 
 [build-system]
```

### Comparing `konko-0.3.1/src/konko/generate.py` & `konko-0.3.2/src/konko/generate.py`

 * *Files identical despite different names*

### Comparing `konko-0.3.1/src/konko/models.py` & `konko-0.3.2/src/konko/models.py`

 * *Files identical despite different names*

### Comparing `konko-0.3.1/src/konko/utils/logs.py` & `konko-0.3.2/src/konko/utils/logs.py`

 * *Files identical despite different names*

### Comparing `konko-0.3.1/PKG-INFO` & `konko-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: konko
-Version: 0.3.1
+Version: 0.3.2
 Summary: "Konko AI Python SDK: A client library to interact with Konko AI's API. With this SDK, developers can integrate, evaluate, fine-tune, and deploy Large Language Models (LLMs) using Konko AI's fully-managed, SOC 2 compliant platform. Ideal for enterprise use-cases, it allows you to focus on building great products without worrying about infrastructure."
 License: Proprietary
 Author: Konko AI
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.100.0,<0.101.0)
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: pydantic (>=1,<2)
+Requires-Dist: requests (>=2.28.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # For documentation please visit 
 [Link Text](https://docs.konko.ai/)
```

