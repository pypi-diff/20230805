# Comparing `tmp/litellm-0.1.230.tar.gz` & `tmp/litellm-0.1.232.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.230.tar", last modified: Thu Aug  3 22:06:55 2023, max compression
+gzip compressed data, was "litellm-0.1.232.tar", last modified: Fri Aug  4 21:56:14 2023, max compression
```

## Comparing `litellm-0.1.230.tar` & `litellm-0.1.232.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.077892 litellm-0.1.230/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-03 22:06:43.000000 litellm-0.1.230/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 22:06:55.073892 litellm-0.1.230/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-03 22:06:43.000000 litellm-0.1.230/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.073892 litellm-0.1.230/litellm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.073892 litellm-0.1.230/litellm/integrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/integrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3548 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/integrations/helicone.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15221 2023-08-03 22:06:43.000000 litellm-0.1.230/litellm/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 22:06:55.073892 litellm-0.1.230/litellm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-03 22:06:55.000000 litellm-0.1.230/litellm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-03 22:06:43.000000 litellm-0.1.230/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 22:06:55.077892 litellm-0.1.230/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-08-03 22:06:43.000000 litellm-0.1.230/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.761462 litellm-0.1.232/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-07-27 00:10:35.000000 litellm-0.1.232/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-04 21:56:14.761350 litellm-0.1.232/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2285 2023-08-03 17:46:06.000000 litellm-0.1.232/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.759959 litellm-0.1.232/litellm/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1872 2023-08-04 21:54:38.000000 litellm-0.1.232/litellm/__init__.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.761144 litellm-0.1.232/litellm/integrations/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       15 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/integrations/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3548 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/integrations/helicone.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    12673 2023-08-04 21:54:38.000000 litellm-0.1.232/litellm/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2893 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/timeout.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    15221 2023-08-03 17:46:06.000000 litellm-0.1.232/litellm/utils.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-04 21:56:14.760813 litellm-0.1.232/litellm.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      333 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       80 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        8 2023-08-04 21:56:14.000000 litellm-0.1.232/litellm.egg-info/top_level.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      473 2023-08-03 04:02:44.000000 litellm-0.1.232/pyproject.toml
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-08-04 21:56:14.761501 litellm-0.1.232/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      546 2023-08-04 21:54:59.000000 litellm-0.1.232/setup.py
```

### Comparing `litellm-0.1.230/LICENSE` & `litellm-0.1.232/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.230/README.md` & `litellm-0.1.232/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.230/litellm/integrations/helicone.py` & `litellm-0.1.232/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.230/litellm/main.py` & `litellm-0.1.232/litellm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   # Use a partial function to pass your keyword arguments
   func = partial(completion, *args, **kwargs)
 
   # Call the synchronous function using run_in_executor
   return await loop.run_in_executor(None, func)
 
 @client
-@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(2), reraise=True, retry_error_callback=lambda retry_state: setattr(retry_state.outcome, 'retry_variable', litellm.retry)) # retry call, turn this off by setting `litellm.retry = False`
+# @retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(2), reraise=True, retry_error_callback=lambda retry_state: setattr(retry_state.outcome, 'retry_variable', litellm.retry)) # retry call, turn this off by setting `litellm.retry = False`
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def completion(
     model, messages, # required params
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     functions=[], function_call="", # optional params
     temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
     presence_penalty=0, frequency_penalty=0, logit_bias={}, user="", deployment_id=None,
@@ -251,16 +251,16 @@
         ]
       }
       print_verbose(f"new response: {new_response}")
       response = new_response
     elif model in litellm.cohere_models:
       if api_key:
         cohere_key = api_key
-      elif litellm.api_key:
-        cohere_key = litellm.api_key
+      elif litellm.cohere_key:
+        cohere_key = litellm.cohere_key
       else:
         cohere_key = os.environ.get("COHERE_API_KEY")
       co = cohere.Client(cohere_key)
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
@@ -326,14 +326,15 @@
     
     return response
   except Exception as e:
     # log the original exception
     logging(model=model, input=input, azure=azure, logger_fn=logger_fn, exception=e)
     ## Map to OpenAI Exception
     raise exception_type(model=model, original_exception=e)
+    raise e
 ####### HELPER FUNCTIONS ################
 ## Set verbose to true -> ```litellm.set_verbose = True```    
 def print_verbose(print_statement):
   if litellm.set_verbose:
     print(f"LiteLLM: {print_statement}")
     if random.random() <= 0.3:
       print("Get help - https://discord.com/invite/wuPM9dRgDw")
```

### Comparing `litellm-0.1.230/litellm/timeout.py` & `litellm-0.1.232/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.230/litellm/utils.py` & `litellm-0.1.232/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.230/setup.py` & `litellm-0.1.232/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='litellm',
-    version='0.1.230',
+    version='0.1.232',
     description='Library to easily interface with LLM API providers',
     author='BerriAI',
     packages=[
         'litellm'
     ],
     package_data={
         "litellm": ["integrations/*"],  # Specify the directory path relative to your package
```

