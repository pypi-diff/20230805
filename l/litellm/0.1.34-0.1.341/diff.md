# Comparing `tmp/litellm-0.1.34.tar.gz` & `tmp/litellm-0.1.341.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.34.tar", last modified: Sat Aug  5 17:25:35 2023, max compression
+gzip compressed data, was "litellm-0.1.341.tar", max compression
```

## Comparing `litellm-0.1.34.tar` & `litellm-0.1.341.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.064738 litellm-0.1.34/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.34/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      150 2023-08-05 17:25:35.064620 litellm-0.1.34/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2285 2023-08-03 14:15:52.000000 litellm-0.1.34/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.062936 litellm-0.1.34/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1985 2023-08-05 16:52:05.000000 litellm-0.1.34/litellm/__init__.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.064396 litellm-0.1.34/litellm/integrations/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       15 2023-08-03 15:30:17.000000 litellm-0.1.34/litellm/integrations/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3548 2023-08-03 15:22:44.000000 litellm-0.1.34/litellm/integrations/helicone.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11523 2023-08-05 16:53:43.000000 litellm-0.1.34/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2893 2023-08-03 16:40:54.000000 litellm-0.1.34/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    17739 2023-08-05 16:52:05.000000 litellm-0.1.34/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-05 17:25:35.063950 litellm-0.1.34/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      150 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      333 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       80 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-05 17:25:35.000000 litellm-0.1.34/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      491 2023-08-05 17:18:11.000000 litellm-0.1.34/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-05 17:25:35.064786 litellm-0.1.34/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      544 2023-08-05 17:25:21.000000 litellm-0.1.34/setup.py
+-rw-r--r--   0        0        0     1065 2023-08-05 19:21:37.549398 litellm-0.1.341/LICENSE
+-rw-r--r--   0        0        0     2285 2023-08-05 19:21:37.549398 litellm-0.1.341/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/.DS_Store
+-rw-r--r--   0        0        0     1985 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3548 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0    13738 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0     2578 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4506 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5840 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0      530 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/timeout.py
+-rw-r--r--   0        0        0    17992 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/utils.py
+-rw-r--r--   0        0        0      512 2023-08-05 19:21:37.553398 litellm-0.1.341/pyproject.toml
+-rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 litellm-0.1.341/PKG-INFO
```

### Comparing `litellm-0.1.34/LICENSE` & `litellm-0.1.341/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.34/README.md` & `litellm-0.1.341/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.34/litellm/__init__.py` & `litellm-0.1.341/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.34/litellm/integrations/helicone.py` & `litellm-0.1.341/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.34/litellm/main.py` & `litellm-0.1.341/litellm/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import os, openai, cohere, replicate, sys
 from typing import Any
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
-import traceback
 from functools import partial
-import dotenv
-import traceback
+import dotenv, traceback, random, asyncio, time
+from copy import deepcopy
 import litellm
 from litellm import client, logging, exception_type, timeout, get_optional_params
-import random
-import asyncio
+import tiktoken
+encoding = tiktoken.get_encoding("cl100k_base")
 from tenacity import (
     retry,
     stop_after_attempt,
     wait_random_exponential,
 )  # for exponential backoff
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
+new_response = {
+        "choices": [
+          {
+            "finish_reason": "stop",
+            "index": 0,
+            "message": {
+                "role": "assistant"
+            }
+          }
+        ]
+      }
 # TODO move this to utils.py
 # TODO add translations
 # TODO see if this worked - model_name == krrish
 ####### COMPLETION ENDPOINTS ################
 #############################################
 async def acompletion(*args, **kwargs):
   loop = asyncio.get_event_loop()
@@ -40,14 +50,16 @@
     functions=[], function_call="", # optional params
     temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
     presence_penalty=0, frequency_penalty=0, logit_bias={}, user="", deployment_id=None,
     # Optional liteLLM function params
     *, return_async=False, api_key=None, force_timeout=60, azure=False, logger_fn=None, verbose=False
   ):
   try:
+    global new_response
+    model_response = deepcopy(new_response) # deep copy the default response format so we can mutate it and it's thread-safe. 
     # check if user passed in any of the OpenAI optional params
     optional_params = get_optional_params(
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user, deployment_id=deployment_id
     )
     if azure == True:
@@ -124,14 +136,23 @@
           headers = litellm.headers,
         )
       else:
         response = openai.Completion.create(
             model=model,
             prompt = prompt
         )
+      completion_response = response["choices"]["text"]
+      ## LOGGING
+      logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
+      ## RESPONSE OBJECT
+      model_response["choices"][0]["message"]["content"] = completion_response
+      model_response["created"] = response["created"]
+      model_response["model"] = model
+      model_response["usage"] = response["usage"]
+      response = model_response
     elif "replicate" in model:
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
       if not os.environ.get("REPLICATE_API_TOKEN") and os.environ.get("REPLICATE_API_KEY"):
         replicate_api_token = os.environ.get("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
       elif api_key:
@@ -149,27 +170,29 @@
       ## COMPLETION CALL
       output = replicate.run(
         model,
         input=input)
       response = ""
       for item in output: 
         response += item
-      new_response = {
-        "choices": [
-          {
-            "finish_reason": "stop",
-            "index": 0,
-            "message": {
-                "content": response,
-                "role": "assistant"
-            }
-          }
-        ]
-      }
-      response = new_response
+      completion_response = response
+      ## LOGGING
+      logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
+      prompt_tokens = len(encoding.encode(prompt))
+      completion_tokens = len(encoding.encode(completion_response))
+      ## RESPONSE OBJECT
+      model_response["choices"][0]["message"]["content"] = completion_response
+      model_response["created"] = time.time()
+      model_response["model"] = model
+      model_response["usage"] = {
+          "prompt_tokens": prompt_tokens,
+          "completion_tokens": completion_tokens,
+          "total_tokens": prompt_tokens + completion_tokens
+        }
+      response = model_response
     elif model in litellm.anthropic_models:
       #anthropic defaults to os.environ.get("ANTHROPIC_API_KEY")
       if api_key:
          os.environ["ANTHROPIC_API_KEY"] = api_key
       elif litellm.anthropic_key:
          os.environ["ANTHROPIC_API_TOKEN"] = litellm.anthropic_key
       prompt = f"{HUMAN_PROMPT}" 
@@ -179,41 +202,42 @@
             prompt += f"{HUMAN_PROMPT}{message['content']}"
           else:
             prompt += f"{AI_PROMPT}{message['content']}"
         else:
           prompt += f"{HUMAN_PROMPT}{message['content']}"
       prompt += f"{AI_PROMPT}"
       anthropic = Anthropic()
-      # check if user passed in max_tokens != float('inf')
       if max_tokens != float('inf'):
         max_tokens_to_sample = max_tokens
       else:
         max_tokens_to_sample = litellm.max_tokens # default in Anthropic docs https://docs.anthropic.com/claude/reference/client-libraries
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
       ## COMPLETION CALL
       completion = anthropic.completions.create(
             model=model,
             prompt=prompt,
             max_tokens_to_sample=max_tokens_to_sample
         )
-      new_response = {
-        "choices": [
-          {
-            "finish_reason": "stop",
-            "index": 0,
-            "message": {
-                "content": completion.completion,
-                "role": "assistant"
-            }
-          }
-        ]
-      }
-      print_verbose(f"new response: {new_response}")
-      response = new_response
+      completion_response = completion.completion
+      ## LOGGING
+      logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
+      prompt_tokens = anthropic.count_tokens(prompt)
+      completion_tokens = anthropic.count_tokens(completion_response)
+      ## RESPONSE OBJECT
+      print(f"model_response: {model_response}")
+      model_response["choices"][0]["message"]["content"] = completion_response
+      model_response["created"] = time.time()
+      model_response["model"] = model
+      model_response["usage"] = {
+          "prompt_tokens": prompt_tokens,
+          "completion_tokens": completion_tokens,
+          "total_tokens": prompt_tokens + completion_tokens
+        }
+      response = model_response
     elif model in litellm.cohere_models:
       if api_key:
         cohere_key = api_key
       elif litellm.cohere_key:
         cohere_key = litellm.cohere_key
       else:
         cohere_key = os.environ.get("COHERE_API_KEY")
@@ -222,27 +246,29 @@
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = co.generate(  
         model=model,
         prompt = prompt
       )
-      new_response = {
-          "choices": [
-              {
-                  "finish_reason": "stop",
-                  "index": 0,
-                  "message": {
-                      "content": response[0].text,
-                      "role": "assistant"
-                  }
-              }
-          ],
-      }
-      response = new_response
+      completion_response = response[0].text
+      ## LOGGING
+      logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
+      prompt_tokens = len(encoding.encode(prompt))
+      completion_tokens = len(encoding.encode(completion_response))
+      ## RESPONSE OBJECT
+      model_response["choices"][0]["message"]["content"] = completion_response
+      model_response["created"] = time.time()
+      model_response["model"] = model
+      model_response["usage"] = {
+          "prompt_tokens": prompt_tokens,
+          "completion_tokens": completion_tokens,
+          "total_tokens": prompt_tokens + completion_tokens
+        }
+      response = model_response
     else: 
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       args = locals()
       raise ValueError(f"No valid completion model args passed in - {args}")
     return response
   except Exception as e:
```

### Comparing `litellm-0.1.34/litellm/timeout.py` & `litellm-0.1.341/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.34/litellm/utils.py` & `litellm-0.1.341/litellm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,35 +29,37 @@
   try:
     model_call_details = {}
     if model:
       model_call_details["model"] = model
     if azure:
       model_call_details["azure"] = azure
     if exception:
-      model_call_details["original_exception"] = exception
+      model_call_details["exception"] = exception
 
     if litellm.telemetry:
       safe_crash_reporting(model=model, exception=exception, azure=azure) # log usage-crash details. Do not log any user details. If you want to turn this off, set `litellm.telemetry=False`.
 
     if input:
       model_call_details["input"] = input
+    
+    if len(additional_args):
+       model_call_details["additional_args"] = additional_args
     # log additional call details -> api key, etc. 
     if model:
       if azure == True or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_embedding_models:
         model_call_details["api_type"] = openai.api_type
         model_call_details["api_base"] = openai.api_base
         model_call_details["api_version"] = openai.api_version
         model_call_details["api_key"] = openai.api_key
       elif "replicate" in model:
         model_call_details["api_key"] = os.environ.get("REPLICATE_API_TOKEN")
       elif model in litellm.anthropic_models:
         model_call_details["api_key"] = os.environ.get("ANTHROPIC_API_KEY")
       elif model in litellm.cohere_models:
         model_call_details["api_key"] = os.environ.get("COHERE_API_KEY")
-      model_call_details["additional_args"] = additional_args
     ## User Logging -> if you pass in a custom logging function or want to use sentry breadcrumbs
     print_verbose(f"Logging Details: logger_fn - {logger_fn} | callable(logger_fn) - {callable(logger_fn)}")
     if logger_fn and callable(logger_fn):
       try:
         logger_fn(model_call_details) # Expectation: any logger function passed in by the user should accept a dict object
       except Exception as e:
         print(f"LiteLLM.LoggingError: [Non-Blocking] Exception occurred while logging {traceback.format_exc()}")
@@ -314,14 +316,15 @@
           raise original_exception
       elif model:
         error_str = str(original_exception)
         if isinstance(original_exception, BaseException):
           exception_type = type(original_exception).__name__
         else:
           exception_type = ""
+        logging(model=model, additional_args={"error_str": error_str, "exception_type": exception_type, "original_exception": original_exception}, logger_fn=user_logger_fn)
         if "claude" in model: #one of the anthropics
           if "status_code" in original_exception:
             print_verbose(f"status_code: {original_exception.status_code}")
             if original_exception.status_code == 401:
               exception_mapping_worked = True
               raise AuthenticationError(f"AnthropicException - {original_exception.message}")
             elif original_exception.status_code == 400:
@@ -353,15 +356,15 @@
             exception_mapping_worked = True
             raise RateLimitError(f"CohereException - {original_exception.message}")
         raise original_exception # base case - return the original exception
       else:
         raise original_exception
     except Exception as e:
       ## LOGGING
-      logging(logger_fn=user_logger_fn, additional_args={"original_exception": original_exception}, exception=e) 
+      logging(logger_fn=user_logger_fn, additional_args={"exception_mapping_worked": exception_mapping_worked, "original_exception": original_exception}, exception=e) 
       if exception_mapping_worked:
         raise e
       else: # don't let an error with mapping interrupt the user from receiving an error from the llm api calls 
          raise original_exception
 
 def safe_crash_reporting(model=None, exception=None, azure=None):
     data = {
```

