# Comparing `tmp/litellm-0.1.3.tar.gz` & `tmp/litellm-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.3.tar", max compression
+gzip compressed data, was "litellm-0.1.31.tar", max compression
```

## Comparing `litellm-0.1.3.tar` & `litellm-0.1.31.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-08-05 17:05:33.013706 litellm-0.1.3/LICENSE
--rw-r--r--   0        0        0     2285 2023-08-05 17:05:33.013706 litellm-0.1.3/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/.DS_Store
--rw-r--r--   0        0        0     1985 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3548 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/integrations/helicone.py
--rw-r--r--   0        0        0    11523 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     6216 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0     2578 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4206 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5840 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0      530 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/timeout.py
--rw-r--r--   0        0        0    17739 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/utils.py
--rw-r--r--   0        0        0      490 2023-08-05 17:05:33.017706 litellm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3098 1970-01-01 00:00:00.000000 litellm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-05 17:13:09.365527 litellm-0.1.31/LICENSE
+-rw-r--r--   0        0        0     2285 2023-08-05 17:13:09.365527 litellm-0.1.31/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/.DS_Store
+-rw-r--r--   0        0        0     1985 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3548 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0    11523 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     6216 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0     2578 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4206 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5840 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0      530 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/timeout.py
+-rw-r--r--   0        0        0    17739 2023-08-05 17:13:09.365527 litellm-0.1.31/litellm/utils.py
+-rw-r--r--   0        0        0      491 2023-08-05 17:13:09.369527 litellm-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 litellm-0.1.31/PKG-INFO
```

### Comparing `litellm-0.1.3/LICENSE` & `litellm-0.1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/README.md` & `litellm-0.1.31/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/.DS_Store` & `litellm-0.1.31/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/__init__.py` & `litellm-0.1.31/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/integrations/helicone.py` & `litellm-0.1.31/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/main.py` & `litellm-0.1.31/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.31/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.31/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.31/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.31/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.31/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.31/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.31/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_api_key_param.py` & `litellm-0.1.31/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_async_fn.py` & `litellm-0.1.31/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_bad_params.py` & `litellm-0.1.31/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_client.py` & `litellm-0.1.31/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_completion.py` & `litellm-0.1.31/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_exceptions.py` & `litellm-0.1.31/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_helicone_integration.py` & `litellm-0.1.31/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_logging.py` & `litellm-0.1.31/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_model_fallback.py` & `litellm-0.1.31/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_no_client.py` & `litellm-0.1.31/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/tests/test_timeout.py` & `litellm-0.1.31/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/timeout.py` & `litellm-0.1.31/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/litellm/utils.py` & `litellm-0.1.31/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.3/PKG-INFO` & `litellm-0.1.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.3
+Version: 0.1.31
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

