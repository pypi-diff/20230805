# Comparing `tmp/litellm-0.1.331.tar.gz` & `tmp/litellm-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.331.tar", max compression
+gzip compressed data, was "litellm-0.1.34.tar", last modified: Sat Aug  5 17:25:35 2023, max compression
```

## Comparing `litellm-0.1.331.tar` & `litellm-0.1.34.tar`

### file list

```diff
@@ -1,33 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-08-05 17:34:52.671441 litellm-0.1.331/LICENSE
--rw-r--r--   0        0        0     2285 2023-08-05 17:34:52.671441 litellm-0.1.331/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 17:34:52.671441 litellm-0.1.331/litellm/.DS_Store
--rw-r--r--   0        0        0     1985 2023-08-05 17:34:52.671441 litellm-0.1.331/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3548 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/integrations/helicone.py
--rw-r--r--   0        0        0    11523 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     6216 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0     2578 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4206 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5840 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0      530 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/timeout.py
--rw-r--r--   0        0        0    17739 2023-08-05 17:34:52.675441 litellm-0.1.331/litellm/utils.py
--rw-r--r--   0        0        0      492 2023-08-05 17:34:52.675441 litellm-0.1.331/pyproject.toml
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 litellm-0.1.331/PKG-INFO
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.064738 litellm-0.1.34/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.34/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      150 2023-08-05 17:25:35.064620 litellm-0.1.34/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.34/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.062936 litellm-0.1.34/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1985 2023-08-05 16:52:05.000000 litellm-0.1.34/litellm/__init__.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.064396 litellm-0.1.34/litellm/integrations/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       15 2023-08-03 15:30:17.000000 litellm-0.1.34/litellm/integrations/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3548 2023-08-03 15:22:44.000000 litellm-0.1.34/litellm/integrations/helicone.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11523 2023-08-05 16:53:43.000000 litellm-0.1.34/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2893 2023-08-03 16:40:54.000000 litellm-0.1.34/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    17739 2023-08-05 16:52:05.000000 litellm-0.1.34/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.063950 litellm-0.1.34/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      150 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      333 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       80 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      491 2023-08-05 17:18:11.000000 litellm-0.1.34/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-05 17:25:35.064786 litellm-0.1.34/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      544 2023-08-05 17:25:21.000000 litellm-0.1.34/setup.py
```

### Comparing `litellm-0.1.331/LICENSE` & `litellm-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.331/README.md` & `litellm-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.331/litellm/__init__.py` & `litellm-0.1.34/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.331/litellm/integrations/helicone.py` & `litellm-0.1.34/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.331/litellm/main.py` & `litellm-0.1.34/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.331/litellm/timeout.py` & `litellm-0.1.34/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.331/litellm/utils.py` & `litellm-0.1.34/litellm/utils.py`

 * *Files identical despite different names*

