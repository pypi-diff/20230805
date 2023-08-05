# Comparing `tmp/one-api-tool-0.5.2.tar.gz` & `tmp/one-api-tool-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.5.2.tar", last modified: Mon Jul 24 03:53:58 2023, max compression
+gzip compressed data, was "one-api-tool-0.5.4.tar", last modified: Sat Aug  5 02:57:44 2023, max compression
```

## Comparing `one-api-tool-0.5.2.tar` & `one-api-tool-0.5.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.574556 one-api-tool-0.5.2/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.2/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     8209 2023-07-24 03:53:58.574046 one-api-tool-0.5.2/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     7653 2023-07-24 03:51:04.000000 one-api-tool-0.5.2/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.571337 one-api-tool-0.5.2/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     8209 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       91 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.572987 one-api-tool-0.5.2/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.2/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.573512 one-api-tool-0.5.2/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.2/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.2/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    23648 2023-07-24 03:42:18.000000 one-api-tool-0.5.2/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1106 2023-07-24 03:49:05.000000 one-api-tool-0.5.2/oneapi/one_api_test.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.2/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-24 03:53:58.574629 one-api-tool-0.5.2/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1094 2023-07-24 03:51:47.000000 one-api-tool-0.5.2/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.452815 one-api-tool-0.5.4/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.4/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 02:57:44.452621 one-api-tool-0.5.4/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7668 2023-07-24 03:57:21.000000 one-api-tool-0.5.4/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.450446 one-api-tool-0.5.4/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.451458 one-api-tool-0.5.4/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.4/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.452058 one-api-tool-0.5.4/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.4/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.4/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    23633 2023-08-05 02:39:58.000000 one-api-tool-0.5.4/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1204 2023-08-05 02:53:46.000000 one-api-tool-0.5.4/oneapi/one_api_test.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.4/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-08-05 02:57:44.452865 one-api-tool-0.5.4/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1099 2023-08-05 02:57:07.000000 one-api-tool-0.5.4/setup.py
```

### Comparing `one-api-tool-0.5.2/LICENSE` & `one-api-tool-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.2/PKG-INFO` & `one-api-tool-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.2
+Version: 0.5.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -90,14 +90,15 @@
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
 ### Batch request with asyncio
 ```python
 from oneapi.one_api import batch_chat
+import asyncio
 
 claude_config = 'anthropic_config.json'
 openai_config = 'openapi_config.json'
 azure_config = 'openapi_azure_config.json'
 # The coccurent number of requests would be 3, which is the same as the length of the configs list.
 configs = [claude_config, openai_config, azure_config]
 prompts = ['How\'s the weather today?', 'How\'s the weather today?', 'How\'s the weather today?']
```

### Comparing `one-api-tool-0.5.2/README.md` & `one-api-tool-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
 ### Batch request with asyncio
 ```python
 from oneapi.one_api import batch_chat
+import asyncio
 
 claude_config = 'anthropic_config.json'
 openai_config = 'openapi_config.json'
 azure_config = 'openapi_azure_config.json'
 # The coccurent number of requests would be 3, which is the same as the length of the configs list.
 configs = [claude_config, openai_config, azure_config]
 prompts = ['How\'s the weather today?', 'How\'s the weather today?', 'How\'s the weather today?']
```

### Comparing `one-api-tool-0.5.2/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.5.4/one_api_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.2
+Version: 0.5.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -90,14 +90,15 @@
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
 ### Batch request with asyncio
 ```python
 from oneapi.one_api import batch_chat
+import asyncio
 
 claude_config = 'anthropic_config.json'
 openai_config = 'openapi_config.json'
 azure_config = 'openapi_azure_config.json'
 # The coccurent number of requests would be 3, which is the same as the length of the configs list.
 configs = [claude_config, openai_config, azure_config]
 prompts = ['How\'s the weather today?', 'How\'s the weather today?', 'How\'s the weather today?']
```

### Comparing `one-api-tool-0.5.2/oneapi/commands/one_api_requst.py` & `one-api-tool-0.5.4/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.2/oneapi/one_api.py` & `one-api-tool-0.5.4/oneapi/one_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,35 +242,38 @@
     """
     https://console.anthropic.com/claude
     https://github.com/anthropics/anthropic-sdk-python/blob/main/examples/basic_stream.py
     https://console.anthropic.com/docs/api/reference
     """
     def __init__(self,method : AbstrctMethod) -> None:
         self.method = method
-        self.client = anthropic.Client(method.api_key)
+        self.client = anthropic.Client(api_key=method.api_key)
+        self.aclient = anthropic.AsyncClient(api_key=method.api_key)
     
     async def asimple_chat(self, args: ClaudeDecodingArguments):
         if args.stream:
-            resp = await self.client.acompletion_stream(**args.dict())
-            async for data in resp:
-                if data["stop_reason"] == "stop_sequence" or data["stop_reason"] == "max_tokens":
-                    return data["completion"]
+            stream = await self.aclient.completions.create(**args.dict())
+            text = ""
+            async for data in stream:
+                text += data.completion
+            return text
         else:
-            resp = await self.client.acompletion(**args.dict())
-            return resp["completion"]
-        
+            resp = await self.aclient.completions.create(**args.dict())
+            return resp.completion
+                
     def simple_chat(self, args: ClaudeDecodingArguments):
         if args.stream:
-            resp = self.client.completion_stream(**args.dict())
+            resp = self.client.completions.create(**args.dict())
+            text = ""
             for  data in resp:
-                if data["stop_reason"] == "stop_sequence" or data["stop_reason"] == "max_tokens":
-                    return data["completion"]
+                text += data.completion
+            return text
         else:
-            resp = self.client.completion(**args.dict())
-            return resp["completion"]
+            resp = self.client.completions.create(**args.dict())
+            return resp.completion
 
             
             
 
 class OneAPITool():
     def __init__(self, tool: AbstractAPITool) -> None:
         self.tool = tool
```

### Comparing `one-api-tool-0.5.2/oneapi/one_api_test.py` & `one-api-tool-0.5.4/oneapi/one_api_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import os
 from typing import Callable, Optional, Sequence, List
 import tiktoken
 import asyncio
 import logging
 from openai.openai_object import OpenAIObject
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
-from oneapi.one_api import batch_chat
+from oneapi.one_api import batch_chat, OneAPITool
 
 
 if __name__ == "__main__":
     claude_config = '../../ant/config/anthropic_config_personal.json'
     openai_config = '../../ant/config/openapi_official_chenghao.json'
     azure_config = '../../ant/config/openapi_azure_config_xiaoduo_dev.json'
-    config_file = openai_config
+    config_file = claude_config
     # tool = OneAPITool.from_config_file(config_file)
+    
     # prompt = '今天天气不错？'
-    # res = asyncio.run(tool.asimple_chat(prompt, stream=False))
+    # res = asyncio.run(tool.asimple_chat(prompt, stream=True))
     # print(res)
-    res = asyncio.run(batch_chat([claude_config, openai_config, azure_config], ['今天天气不错？', '今天天气不错？', '今天天气不错？'], stream=False))
+    res = asyncio.run(batch_chat([claude_config, openai_config, azure_config], ['心率异常可以局部麻醉吗', '今天天气不错？', '你好？', '上午是几点', '热天吃什么', '胖子爱出汗', '窦性心率是什么'], stream=False))
     print(res)
```

### Comparing `one-api-tool-0.5.2/oneapi/utils.py` & `one-api-tool-0.5.4/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.2/setup.py` & `one-api-tool-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.5.2",
+    version="0.5.4",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
-        "anthropic",
+        "anthropic>=0.3",
         "requests",
         "httpx",
         "aiohttp",
         "tiktoken",
         "tqdm",
         "tokenizers",
         "docstring_parser"
```

