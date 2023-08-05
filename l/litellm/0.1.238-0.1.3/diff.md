# Comparing `tmp/litellm-0.1.238.tar.gz` & `tmp/litellm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.238.tar", max compression
+gzip compressed data, was "litellm-0.1.3.tar", max compression
```

## Comparing `litellm-0.1.238.tar` & `litellm-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-08-05 16:50:26.439035 litellm-0.1.238/LICENSE
--rw-r--r--   0        0        0     2285 2023-08-05 16:50:26.439035 litellm-0.1.238/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/.DS_Store
--rw-r--r--   0        0        0     1964 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3548 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/integrations/helicone.py
--rw-r--r--   0        0        0    12775 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     6216 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0     2578 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4206 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     4789 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0      530 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-05 16:50:26.439035 litellm-0.1.238/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/timeout.py
--rw-r--r--   0        0        0    15221 2023-08-05 16:50:26.443035 litellm-0.1.238/litellm/utils.py
--rw-r--r--   0        0        0      492 2023-08-05 16:50:26.443035 litellm-0.1.238/pyproject.toml
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 litellm-0.1.238/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-05 17:05:33.013706 litellm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2285 2023-08-05 17:05:33.013706 litellm-0.1.3/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/.DS_Store
+-rw-r--r--   0        0        0     1985 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3548 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0    11523 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     6216 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0     2578 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4206 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5840 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0      530 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/timeout.py
+-rw-r--r--   0        0        0    17739 2023-08-05 17:05:33.017706 litellm-0.1.3/litellm/utils.py
+-rw-r--r--   0        0        0      490 2023-08-05 17:05:33.017706 litellm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3098 1970-01-01 00:00:00.000000 litellm-0.1.3/PKG-INFO
```

### Comparing `litellm-0.1.238/LICENSE` & `litellm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/README.md` & `litellm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/.DS_Store` & `litellm-0.1.3/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/__init__.py` & `litellm-0.1.3/litellm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,10 +65,10 @@
 model_list = open_ai_chat_completion_models + open_ai_text_completion_models + cohere_models + anthropic_models + replicate_models
 
 ####### EMBEDDING MODELS ###################
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
 from .timeout import timeout
-from .utils import client, logging, exception_type  # Import all the symbols from main.py
+from .utils import client, logging, exception_type, get_optional_params  # Import all the symbols from main.py
 from .main import *  # Import all the symbols from main.py
 from .integrations import *
```

### Comparing `litellm-0.1.238/litellm/integrations/helicone.py` & `litellm-0.1.3/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/main.py` & `litellm-0.1.3/litellm/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,73 +2,28 @@
 from typing import Any
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 import traceback
 from functools import partial
 import dotenv
 import traceback
 import litellm
-from litellm import client, logging, exception_type, timeout
+from litellm import client, logging, exception_type, timeout, get_optional_params
 import random
 import asyncio
 from tenacity import (
     retry,
     stop_after_attempt,
     wait_random_exponential,
 )  # for exponential backoff
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
 # TODO move this to utils.py
 # TODO add translations
 # TODO see if this worked - model_name == krrish
-def get_optional_params(
-    # 12 optional params
-    functions = [],
-    function_call = "",
-    temperature = 1,
-    top_p = 1,
-    n = 1,
-    stream = False,
-    stop = None,
-    max_tokens = float('inf'),
-    presence_penalty = 0,
-    frequency_penalty = 0,
-    logit_bias = {},
-    user = "",
-    deployment_id = None
-):
-  optional_params = {}
-  if functions != []:
-      optional_params["functions"] = functions
-  if function_call != "":
-      optional_params["function_call"] = function_call
-  if temperature != 1:
-      optional_params["temperature"] = temperature
-  if top_p != 1:
-      optional_params["top_p"] = top_p
-  if n != 1:
-      optional_params["n"] = n
-  if stream:
-      optional_params["stream"] = stream
-  if stop != None:
-      optional_params["stop"] = stop
-  if max_tokens != float('inf'):
-      optional_params["max_tokens"] = max_tokens
-  if presence_penalty != 0:
-      optional_params["presence_penalty"] = presence_penalty
-  if frequency_penalty != 0:
-      optional_params["frequency_penalty"] = frequency_penalty
-  if logit_bias != {}:
-      optional_params["logit_bias"] = logit_bias
-  if user != "":
-      optional_params["user"] = user
-  if deployment_id != None:
-      optional_params["deployment_id"] = user
-  return optional_params
-
 ####### COMPLETION ENDPOINTS ################
 #############################################
 async def acompletion(*args, **kwargs):
   loop = asyncio.get_event_loop()
   
   # Use a partial function to pass your keyword arguments
   func = partial(completion, *args, **kwargs)
@@ -281,20 +236,21 @@
                       "role": "assistant"
                   }
               }
           ],
       }
       response = new_response
     else: 
+      ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       args = locals()
       raise ValueError(f"No valid completion model args passed in - {args}")
     return response
   except Exception as e:
-    # log the original exception
+    ## LOGGING
     logging(model=model, input=messages, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn, exception=e)
     ## Map to OpenAI Exception
     raise exception_type(model=model, original_exception=e)
 
 ### EMBEDDING ENDPOINTS ####################
 @client
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
```

### Comparing `litellm-0.1.238/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.3/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.3/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.3/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.3/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.3/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.3/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.3/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_api_key_param.py` & `litellm-0.1.3/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_async_fn.py` & `litellm-0.1.3/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_bad_params.py` & `litellm-0.1.3/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_client.py` & `litellm-0.1.3/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_completion.py` & `litellm-0.1.3/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_exceptions.py` & `litellm-0.1.3/litellm/tests/test_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,85 +4,108 @@
 import traceback
 sys.path.insert(0, os.path.abspath('../..'))  # Adds the parent directory to the system path
 import litellm
 from litellm import embedding, completion
 from concurrent.futures import ThreadPoolExecutor
 import pytest
 
+litellm.failure_callback = ["sentry"]
 # litellm.set_verbose = True
 #### What this tests ####
 #    This tests exception mapping -> trigger an exception from an llm provider -> assert if output is of the expected type
 
 
 # 5 providers -> OpenAI, Azure, Anthropic, Cohere, Replicate
 
 # 3 main types of exceptions -> - Rate Limit Errors, Context Window Errors, Auth errors (incorrect/rotated key, etc.)
 
 # Approach: Run each model through the test -> assert if the correct error (always the same one) is triggered
 
 # models = ["gpt-3.5-turbo", "chatgpt-test",  "claude-instant-1", "command-nightly"]
 models = ["command-nightly"]
 def logging_fn(model_call_dict):
-    print(f"model_call_dict: {model_call_dict['model']}")
+    if "model" in model_call_dict: 
+        print(f"model_call_dict: {model_call_dict['model']}")
+    else:
+        print(f"model_call_dict: {model_call_dict}")
+
+
 # Test 1: Context Window Errors
 @pytest.mark.parametrize("model", models)
 def test_context_window(model):
-    sample_text = "how does a court case get to the Supreme Court?" * 100000
+    sample_text = "how does a court case get to the Supreme Court?" * 5000
     messages = [{"content": sample_text, "role": "user"}]
     try:
         azure = model == "chatgpt-test"
         print(f"model: {model}")
         response = completion(model=model, messages=messages, azure=azure, logger_fn=logging_fn)
         print(f"response: {response}")
     except InvalidRequestError:
         print("InvalidRequestError")
         return
     except OpenAIError:
         print("OpenAIError")
         return
     except Exception as e:
         print("Uncaught Error in test_context_window")
-        # print(f"Error Type: {type(e).__name__}")
+        print(f"Error Type: {type(e).__name__}")
         print(f"Uncaught Exception - {e}")
         pytest.fail(f"Error occurred: {e}")
     return
 test_context_window("command-nightly")
-# # Test 2: InvalidAuth Errors
-# def logger_fn(model_call_object: dict):
-#     print(f"model call details: {model_call_object}")
-
-# @pytest.mark.parametrize("model", models)
-# def invalid_auth(model): # set the model key to an invalid key, depending on the model 
-#     messages = [{ "content": "Hello, how are you?","role": "user"}]
-#     try: 
-#         azure = False
-#         if model == "gpt-3.5-turbo":
-#             os.environ["OPENAI_API_KEY"] = "bad-key"
-#         elif model == "chatgpt-test":
-#             os.environ["AZURE_API_KEY"] = "bad-key"
-#             azure = True
-#         elif model == "claude-instant-1":
-#             os.environ["ANTHROPIC_API_KEY"] = "bad-key"
-#         elif model == "command-nightly":
-#             os.environ["COHERE_API_KEY"] = "bad-key"
-#         elif model == "replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1":
-#             os.environ["REPLICATE_API_KEY"] = "bad-key"
-#             os.environ["REPLICATE_API_TOKEN"] = "bad-key"
-#         print(f"model: {model}")
-#         response = completion(model=model, messages=messages, azure=azure)
-#         print(f"response: {response}")
-#     except AuthenticationError as e:
-#         return
-#     except OpenAIError: # is at least an openai error -> in case of random model errors - e.g. overloaded server
-#         return
-#     except Exception as e:
-#         print(f"Uncaught Exception - {e}")
-#         pytest.fail(f"Error occurred: {e}")
-#     return
 
+# Test 2: InvalidAuth Errors
+@pytest.mark.parametrize("model", models)
+def invalid_auth(model): # set the model key to an invalid key, depending on the model 
+    messages = [{ "content": "Hello, how are you?","role": "user"}]
+    temporary_key = None
+    try: 
+        azure = False
+        if model == "gpt-3.5-turbo":
+            temporary_key = os.environ["OPENAI_API_KEY"]
+            os.environ["OPENAI_API_KEY"] = "bad-key"
+        elif model == "chatgpt-test":
+            temporary_key = os.environ["AZURE_API_KEY"]
+            os.environ["AZURE_API_KEY"] = "bad-key"
+            azure = True
+        elif model == "claude-instant-1":
+            temporary_key = os.environ["ANTHROPIC_API_KEY"]
+            os.environ["ANTHROPIC_API_KEY"] = "bad-key"
+        elif model == "command-nightly":
+            temporary_key = os.environ["COHERE_API_KEY"]
+            os.environ["COHERE_API_KEY"] = "bad-key"
+        elif model == "replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1":
+            temporary_key = os.environ["REPLICATE_API_KEY"] 
+            os.environ["REPLICATE_API_KEY"] = "bad-key"
+        print(f"model: {model}")
+        response = completion(model=model, messages=messages, azure=azure)
+        print(f"response: {response}")
+    except AuthenticationError as e:
+        print(f"AuthenticationError Caught Exception - {e}")
+    except OpenAIError: # is at least an openai error -> in case of random model errors - e.g. overloaded server
+        print(f"OpenAIError Caught Exception - {e}")
+    except Exception as e:
+        print(type(e))
+        print(e.__class__.__name__)
+        print(f"Uncaught Exception - {e}")
+        pytest.fail(f"Error occurred: {e}")
+    if temporary_key != None: # reset the key
+        if model == "gpt-3.5-turbo":
+            os.environ["OPENAI_API_KEY"] = temporary_key
+        elif model == "chatgpt-test":
+            os.environ["AZURE_API_KEY"] = temporary_key
+            azure = True
+        elif model == "claude-instant-1":
+            os.environ["ANTHROPIC_API_KEY"] = temporary_key
+        elif model == "command-nightly":
+            os.environ["COHERE_API_KEY"] = temporary_key
+        elif model == "replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1":
+            os.environ["REPLICATE_API_KEY"] = temporary_key
+    return
+invalid_auth("command-nightly")
 # # Test 3: Rate Limit Errors 
 # def test_model(model):
 #     try: 
 #         sample_text = "how does a court case get to the Supreme Court?" * 50000
 #         messages = [{ "content": sample_text,"role": "user"}]
 #         azure = False
 #         if model == "chatgpt-test":
```

### Comparing `litellm-0.1.238/litellm/tests/test_helicone_integration.py` & `litellm-0.1.3/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_logging.py` & `litellm-0.1.3/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_model_fallback.py` & `litellm-0.1.3/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_no_client.py` & `litellm-0.1.3/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/tests/test_timeout.py` & `litellm-0.1.3/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/timeout.py` & `litellm-0.1.3/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.238/litellm/utils.py` & `litellm-0.1.3/litellm/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,73 +21,78 @@
   if litellm.set_verbose:
     print(f"LiteLLM: {print_statement}")
     if random.random() <= 0.3:
       print("Get help - https://discord.com/invite/wuPM9dRgDw")
 
 ####### LOGGING ###################
 #Logging function -> log the exact model details + what's being sent | Non-Blocking
-def logging(model, input, azure=False, additional_args={}, logger_fn=None, exception=None):
+def logging(model=None, input=None, azure=False, additional_args={}, logger_fn=None, exception=None):
   try:
     model_call_details = {}
-    model_call_details["model"] = model
-    model_call_details["azure"] = azure
-    # log exception details
+    if model:
+      model_call_details["model"] = model
+    if azure:
+      model_call_details["azure"] = azure
     if exception:
       model_call_details["original_exception"] = exception
 
     if litellm.telemetry:
       safe_crash_reporting(model=model, exception=exception, azure=azure) # log usage-crash details. Do not log any user details. If you want to turn this off, set `litellm.telemetry=False`.
 
-    model_call_details["input"] = input
+    if input:
+      model_call_details["input"] = input
     # log additional call details -> api key, etc. 
-    if azure == True or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_embedding_models:
-      model_call_details["api_type"] = openai.api_type
-      model_call_details["api_base"] = openai.api_base
-      model_call_details["api_version"] = openai.api_version
-      model_call_details["api_key"] = openai.api_key
-    elif "replicate" in model:
-      model_call_details["api_key"] = os.environ.get("REPLICATE_API_TOKEN")
-    elif model in litellm.anthropic_models:
-      model_call_details["api_key"] = os.environ.get("ANTHROPIC_API_KEY")
-    elif model in litellm.cohere_models:
-      model_call_details["api_key"] = os.environ.get("COHERE_API_KEY")
-    model_call_details["additional_args"] = additional_args
+    if model:
+      if azure == True or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_embedding_models:
+        model_call_details["api_type"] = openai.api_type
+        model_call_details["api_base"] = openai.api_base
+        model_call_details["api_version"] = openai.api_version
+        model_call_details["api_key"] = openai.api_key
+      elif "replicate" in model:
+        model_call_details["api_key"] = os.environ.get("REPLICATE_API_TOKEN")
+      elif model in litellm.anthropic_models:
+        model_call_details["api_key"] = os.environ.get("ANTHROPIC_API_KEY")
+      elif model in litellm.cohere_models:
+        model_call_details["api_key"] = os.environ.get("COHERE_API_KEY")
+      model_call_details["additional_args"] = additional_args
     ## User Logging -> if you pass in a custom logging function or want to use sentry breadcrumbs
-    print_verbose(f"Basic model call details: {model_call_details}")
+    print_verbose(f"Logging Details: logger_fn - {logger_fn} | callable(logger_fn) - {callable(logger_fn)}")
     if logger_fn and callable(logger_fn):
       try:
         logger_fn(model_call_details) # Expectation: any logger function passed in by the user should accept a dict object
-      except:
-        print_verbose(f"[Non-Blocking] Exception occurred while logging {traceback.format_exc()}")
-  except:
-    traceback.print_exc()
+      except Exception as e:
+        print(f"LiteLLM.LoggingError: [Non-Blocking] Exception occurred while logging {traceback.format_exc()}")
+  except Exception as e:
+    print(f"LiteLLM.LoggingError: [Non-Blocking] Exception occurred while logging {traceback.format_exc()}")
     pass
 
 ####### CLIENT ################### 
 # make it easy to log if completion/embedding runs succeeded or failed + see what happened | Non-Blocking
 def client(original_function):
     def function_setup(*args, **kwargs): #just run once to check if user wants to send their data anywhere - PostHog/Sentry/Slack/etc.
       try: 
-        global callback_list, add_breadcrumb
+        global callback_list, add_breadcrumb, user_logger_fn
         if (len(litellm.success_callback) > 0 or len(litellm.failure_callback) > 0) and len(callback_list) == 0: 
           callback_list = list(set(litellm.success_callback + litellm.failure_callback))
           set_callbacks(callback_list=callback_list,)
         if add_breadcrumb:
           add_breadcrumb(
                 category="litellm.llm_call",
                 message=f"Positional Args: {args}, Keyword Args: {kwargs}",
                 level="info",
             )
+        if "logger_fn" in kwargs:
+           user_logger_fn = kwargs["logger_fn"]
       except: # DO NOT BLOCK running the function because of this
         print_verbose(f"[Non-Blocking] {traceback.format_exc()}")
       pass
 
     def wrapper(*args, **kwargs):
         try:
-          function_setup(args, kwargs)
+          function_setup(*args, **kwargs)
           ## MODEL CALL
           start_time = datetime.datetime.now()
           result = original_function(*args, **kwargs)
           end_time = datetime.datetime.now()
           ## LOG SUCCESS 
           my_thread = threading.Thread(target=handle_success, args=(args, kwargs, result, start_time, end_time)) # don't interrupt execution of main thread
           my_thread.start()
@@ -96,14 +101,59 @@
           traceback_exception = traceback.format_exc()
           my_thread = threading.Thread(target=handle_failure, args=(e, traceback_exception, args, kwargs)) # don't interrupt execution of main thread
           my_thread.start()
           raise e
     return wrapper
 
 ####### HELPER FUNCTIONS ################
+def get_optional_params(
+    # 12 optional params
+    functions = [],
+    function_call = "",
+    temperature = 1,
+    top_p = 1,
+    n = 1,
+    stream = False,
+    stop = None,
+    max_tokens = float('inf'),
+    presence_penalty = 0,
+    frequency_penalty = 0,
+    logit_bias = {},
+    user = "",
+    deployment_id = None
+):
+  optional_params = {}
+  if functions != []:
+      optional_params["functions"] = functions
+  if function_call != "":
+      optional_params["function_call"] = function_call
+  if temperature != 1:
+      optional_params["temperature"] = temperature
+  if top_p != 1:
+      optional_params["top_p"] = top_p
+  if n != 1:
+      optional_params["n"] = n
+  if stream:
+      optional_params["stream"] = stream
+  if stop != None:
+      optional_params["stop"] = stop
+  if max_tokens != float('inf'):
+      optional_params["max_tokens"] = max_tokens
+  if presence_penalty != 0:
+      optional_params["presence_penalty"] = presence_penalty
+  if frequency_penalty != 0:
+      optional_params["frequency_penalty"] = frequency_penalty
+  if logit_bias != {}:
+      optional_params["logit_bias"] = logit_bias
+  if user != "":
+      optional_params["user"] = user
+  if deployment_id != None:
+      optional_params["deployment_id"] = user
+  return optional_params
+
 def set_callbacks(callback_list):
   global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel, heliconeLogger
   try:
     for callback in callback_list:
       if callback == "sentry":
         try:
             import sentry_sdk
@@ -146,24 +196,25 @@
   except:
     pass
 
 
 def handle_failure(exception, traceback_exception, args, kwargs):
     global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel
     try:
-      print_verbose(f"handle_failure args: {args}")
-      print_verbose(f"handle_failure kwargs: {kwargs}")
+      # print_verbose(f"handle_failure args: {args}")
+      # print_verbose(f"handle_failure kwargs: {kwargs}")
       
       success_handler = additional_details.pop("success_handler", None)
       failure_handler = additional_details.pop("failure_handler", None)
       
       additional_details["Event_Name"] = additional_details.pop("failed_event_name", "litellm.failed_query")
       print_verbose(f"self.failure_callback: {litellm.failure_callback}")
 
-      print_verbose(f"additional_details: {additional_details}")
+
+      # print_verbose(f"additional_details: {additional_details}")
       for callback in litellm.failure_callback:
         try:
           if callback == "slack":
             slack_msg = "" 
             if len(kwargs) > 0: 
               for key in kwargs: 
                 slack_msg += f"{key}: {kwargs[key]}\n"
@@ -202,15 +253,17 @@
       if failure_handler and callable(failure_handler):
         call_details = {
           "exception": exception,
           "additional_details": additional_details
         }
         failure_handler(call_details)
       pass
-    except:
+    except Exception as e:
+      ## LOGGING
+      logging(logger_fn=user_logger_fn, exception=e)
       pass
 
 def handle_success(args, kwargs, result, start_time, end_time):
   global heliconeLogger
   try:
     success_handler = additional_details.pop("success_handler", None)
     failure_handler = additional_details.pop("failure_handler", None)
@@ -241,60 +294,78 @@
       except:
         print_verbose(f"Success Callback Error - {traceback.format_exc()}")
         pass
 
     if success_handler and callable(success_handler):
       success_handler(args, kwargs)
     pass
-  except:
+  except Exception as e:
+    ## LOGGING
+    logging(logger_fn=user_logger_fn, exception=e)
     print_verbose(f"Success Callback Error - {traceback.format_exc()}")
     pass
 
 
 def exception_type(model, original_exception):
+    global user_logger_fn
+    exception_mapping_worked = False
     try:
       if isinstance(original_exception, OpenAIError):
           # Handle the OpenAIError
           raise original_exception
       elif model:
         error_str = str(original_exception)
         if isinstance(original_exception, BaseException):
           exception_type = type(original_exception).__name__
         else:
           exception_type = ""
         if "claude" in model: #one of the anthropics
           if "status_code" in original_exception:
             print_verbose(f"status_code: {original_exception.status_code}")
             if original_exception.status_code == 401:
+              exception_mapping_worked = True
               raise AuthenticationError(f"AnthropicException - {original_exception.message}")
             elif original_exception.status_code == 400:
+              exception_mapping_worked = True
               raise InvalidRequestError(f"AnthropicException - {original_exception.message}", f"{model}")
             elif original_exception.status_code == 429:
+              exception_mapping_worked = True
               raise RateLimitError(f"AnthropicException - {original_exception.message}")
         elif "replicate" in model:
           if "Incorrect authentication token" in error_str:
+            exception_mapping_worked = True
             raise AuthenticationError(f"ReplicateException - {error_str}")
           elif exception_type == "ModelError":
+            exception_mapping_worked = True
             raise InvalidRequestError(f"ReplicateException - {error_str}", f"{model}")
           elif "Request was throttled" in error_str:
+            exception_mapping_worked = True
             raise RateLimitError(f"ReplicateException - {error_str}")
           elif exception_type == "ReplicateError": ## ReplicateError implies an error on Replicate server side, not user side
             raise ServiceUnavailableError(f"ReplicateException - {error_str}")
         elif model == "command-nightly": #Cohere
           if "invalid api token" in error_str or "No API key provided." in error_str:
+            exception_mapping_worked = True
             raise AuthenticationError(f"CohereException - {error_str}")
           elif "too many tokens" in error_str:
+            exception_mapping_worked = True
             raise InvalidRequestError(f"CohereException - {error_str}", f"{model}")
           elif "CohereConnectionError" in exception_type: # cohere seems to fire these errors when we load test it (1k+ messages / min)
+            exception_mapping_worked = True
             raise RateLimitError(f"CohereException - {original_exception.message}")
         raise original_exception # base case - return the original exception
       else:
         raise original_exception
-    except:
-      raise original_exception
+    except Exception as e:
+      ## LOGGING
+      logging(logger_fn=user_logger_fn, additional_args={"original_exception": original_exception}, exception=e) 
+      if exception_mapping_worked:
+        raise e
+      else: # don't let an error with mapping interrupt the user from receiving an error from the llm api calls 
+         raise original_exception
 
 def safe_crash_reporting(model=None, exception=None, azure=None):
     data = {
       "model": model,
       "exception": str(exception),
       "azure": azure
     }
@@ -319,15 +390,14 @@
             file.write(uuid_value)
 
     # Prepare the data to send to localhost:3000
     payload = {
         'uuid': uuid_value,
         'data': data
     }
-    print_verbose(f"payload: {payload}")
     try:
       # Make the POST request to localhost:3000
       response = requests.post('https://litellm.berri.ai/logging', json=payload)
       response.raise_for_status()  # Raise an exception for HTTP errors
     except requests.exceptions.RequestException as e:
         # Handle any errors in the request
         pass
```

### Comparing `litellm-0.1.238/PKG-INFO` & `litellm-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.238
+Version: 0.1.3
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

