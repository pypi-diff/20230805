# Comparing `tmp/litellm-0.1.237.tar.gz` & `tmp/litellm-0.1.238.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.237.tar", max compression
+gzip compressed data, was "litellm-0.1.238.tar", max compression
```

## Comparing `litellm-0.1.237.tar` & `litellm-0.1.238.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-08-05 16:46:18.802454 litellm-0.1.237/LICENSE
--rw-r--r--   0        0        0     2285 2023-08-05 16:46:18.802454 litellm-0.1.237/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/.DS_Store
--rw-r--r--   0        0        0     1964 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3548 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/integrations/helicone.py
--rw-r--r--   0        0        0    12726 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     6216 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0     2578 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4206 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     4789 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0      530 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/timeout.py
--rw-r--r--   0        0        0    15221 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/utils.py
--rw-r--r--   0        0        0      492 2023-08-05 16:46:18.810454 litellm-0.1.237/pyproject.toml
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 litellm-0.1.237/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-05 16:50:26.439035 litellm-0.1.238/LICENSE
+-rw-r--r--   0        0        0     2285 2023-08-05 16:50:26.439035 litellm-0.1.238/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/.DS_Store
+-rw-r--r--   0        0        0     1964 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3548 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0    12775 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     6216 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0     2578 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4206 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     4789 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0      530 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/timeout.py
+-rw-r--r--   0        0        0    15221 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/utils.py
+-rw-r--r--   0        0        0      492 2023-08-05 16:50:26.443035 litellm-0.1.238/pyproject.toml
+-rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 litellm-0.1.238/PKG-INFO
```

### Comparing `litellm-0.1.237/LICENSE` & `litellm-0.1.238/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/README.md` & `litellm-0.1.238/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/.DS_Store` & `litellm-0.1.238/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/__init__.py` & `litellm-0.1.238/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/integrations/helicone.py` & `litellm-0.1.238/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/main.py` & `litellm-0.1.238/litellm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     wait_random_exponential,
 )  # for exponential backoff
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
 # TODO move this to utils.py
 # TODO add translations
+# TODO see if this worked - model_name == krrish
 def get_optional_params(
     # 12 optional params
     functions = [],
     function_call = "",
     temperature = 1,
     top_p = 1,
     n = 1,
```

### Comparing `litellm-0.1.237/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.238/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.238/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.238/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.238/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.238/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.238/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.238/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_api_key_param.py` & `litellm-0.1.238/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_async_fn.py` & `litellm-0.1.238/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_bad_params.py` & `litellm-0.1.238/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_client.py` & `litellm-0.1.238/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_completion.py` & `litellm-0.1.238/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_exceptions.py` & `litellm-0.1.238/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_helicone_integration.py` & `litellm-0.1.238/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_logging.py` & `litellm-0.1.238/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_model_fallback.py` & `litellm-0.1.238/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_no_client.py` & `litellm-0.1.238/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/tests/test_timeout.py` & `litellm-0.1.238/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/timeout.py` & `litellm-0.1.238/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/litellm/utils.py` & `litellm-0.1.238/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.237/PKG-INFO` & `litellm-0.1.238/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.237
+Version: 0.1.238
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

