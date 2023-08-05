# Comparing `tmp/litellm-0.1.236.tar.gz` & `tmp/litellm-0.1.237.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.236.tar", last modified: Sat Aug  5 16:32:06 2023, max compression
+gzip compressed data, was "litellm-0.1.237.tar", max compression
```

## Comparing `litellm-0.1.236.tar` & `litellm-0.1.237.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-05 16:31:56.000000 litellm-0.1.236/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:32:06.285492 litellm-0.1.236/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-05 16:31:56.000000 litellm-0.1.236/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/litellm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1964 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/litellm/integrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/integrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/integrations/helicone.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12702 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15221 2023-08-05 16:31:56.000000 litellm-0.1.236/litellm/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:32:06.285492 litellm-0.1.236/litellm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-05 16:32:06.000000 litellm-0.1.236/litellm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-05 16:31:56.000000 litellm-0.1.236/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-05 16:32:06.285492 litellm-0.1.236/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-08-05 16:31:56.000000 litellm-0.1.236/setup.py
+-rw-r--r--   0        0        0     1065 2023-08-05 16:46:18.802454 litellm-0.1.237/LICENSE
+-rw-r--r--   0        0        0     2285 2023-08-05 16:46:18.802454 litellm-0.1.237/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/.DS_Store
+-rw-r--r--   0        0        0     1964 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3548 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0    12726 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     6216 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0     2578 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4206 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     4789 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0      530 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/timeout.py
+-rw-r--r--   0        0        0    15221 2023-08-05 16:46:18.806454 litellm-0.1.237/litellm/utils.py
+-rw-r--r--   0        0        0      492 2023-08-05 16:46:18.810454 litellm-0.1.237/pyproject.toml
+-rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 litellm-0.1.237/PKG-INFO
```

### Comparing `litellm-0.1.236/LICENSE` & `litellm-0.1.237/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.236/README.md` & `litellm-0.1.237/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.236/litellm/__init__.py` & `litellm-0.1.237/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.236/litellm/integrations/helicone.py` & `litellm-0.1.237/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.236/litellm/main.py` & `litellm-0.1.237/litellm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     stop_after_attempt,
     wait_random_exponential,
 )  # for exponential backoff
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
 # TODO move this to utils.py
+# TODO add translations
 def get_optional_params(
     # 12 optional params
     functions = [],
     function_call = "",
     temperature = 1,
     top_p = 1,
     n = 1,
```

### Comparing `litellm-0.1.236/litellm/timeout.py` & `litellm-0.1.237/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.236/litellm/utils.py` & `litellm-0.1.237/litellm/utils.py`

 * *Files identical despite different names*

