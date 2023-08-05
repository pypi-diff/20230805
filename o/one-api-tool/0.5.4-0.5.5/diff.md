# Comparing `tmp/one-api-tool-0.5.4.tar.gz` & `tmp/one-api-tool-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.5.4.tar", last modified: Sat Aug  5 02:57:44 2023, max compression
+gzip compressed data, was "one-api-tool-0.5.5.tar", last modified: Sat Aug  5 03:13:59 2023, max compression
```

## Comparing `one-api-tool-0.5.4.tar` & `one-api-tool-0.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.452815 one-api-tool-0.5.4/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.4/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 02:57:44.452621 one-api-tool-0.5.4/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     7668 2023-07-24 03:57:21.000000 one-api-tool-0.5.4/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.450446 one-api-tool-0.5.4/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-08-05 02:57:44.000000 one-api-tool-0.5.4/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.451458 one-api-tool-0.5.4/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.4/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 02:57:44.452058 one-api-tool-0.5.4/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.4/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.4/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    23633 2023-08-05 02:39:58.000000 one-api-tool-0.5.4/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1204 2023-08-05 02:53:46.000000 one-api-tool-0.5.4/oneapi/one_api_test.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.4/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-08-05 02:57:44.452865 one-api-tool-0.5.4/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1099 2023-08-05 02:57:07.000000 one-api-tool-0.5.4/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:13:59.152206 one-api-tool-0.5.5/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.5/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 03:13:59.152001 one-api-tool-0.5.5/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7668 2023-07-24 03:57:21.000000 one-api-tool-0.5.5/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:13:59.150148 one-api-tool-0.5.5/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 03:13:59.000000 one-api-tool-0.5.5/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-08-05 03:13:59.000000 one-api-tool-0.5.5/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-08-05 03:13:59.000000 one-api-tool-0.5.5/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-08-05 03:13:59.000000 one-api-tool-0.5.5/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-08-05 03:13:59.000000 one-api-tool-0.5.5/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-08-05 03:13:59.000000 one-api-tool-0.5.5/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:13:59.151038 one-api-tool-0.5.5/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.5/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:13:59.151500 one-api-tool-0.5.5/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.5/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.5/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    23838 2023-08-05 03:12:48.000000 one-api-tool-0.5.5/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1280 2023-08-05 03:12:15.000000 one-api-tool-0.5.5/oneapi/one_api_test.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.5/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-08-05 03:13:59.152252 one-api-tool-0.5.5/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1099 2023-08-05 03:13:12.000000 one-api-tool-0.5.5/setup.py
```

### Comparing `one-api-tool-0.5.4/LICENSE` & `one-api-tool-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.4/PKG-INFO` & `one-api-tool-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.4
+Version: 0.5.5
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.5.4/README.md` & `one-api-tool-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.4/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.5.5/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.4
+Version: 0.5.5
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.5.4/oneapi/commands/one_api_requst.py` & `one-api-tool-0.5.5/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.4/oneapi/one_api.py` & `one-api-tool-0.5.5/oneapi/one_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,17 @@
             for  data in resp:
                 text += data.completion
             return text
         else:
             resp = self.client.completions.create(**args.dict())
             return resp.completion
 
-            
+    def count_tokens(self, texts: List[str]) -> int:
+        return sum([self.client.count_tokens(text) for text in texts])
+        
             
 
 class OneAPITool():
     def __init__(self, tool: AbstractAPITool) -> None:
         self.tool = tool
 
     @classmethod
@@ -433,18 +435,19 @@
     def get_embedding(self, text: str, engine="text-embedding-ada-002") -> List[float]:
         if isinstance(self.tool, OpenAITool):
             return self.tool.get_embedding(text, engine)
         else:
             raise AssertionError(f"Not supported api type for embeddings: {type(self.tool)}")
     
     def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
+        assert isinstance(texts, list), f"Input texts must be a list of strings. Got {type(texts)} instead."
         if isinstance(self.tool, OpenAITool):
             return self.tool.count_tokens(texts, encoding_name)
         elif isinstance(self.tool, ClaudeAITool):
-            return sum([anthropic.count_tokens(text) for text in texts])
+            return self.tool.count_tokens(texts)
         else:
             raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
 
 
 async def bound_fetch(sem, pbar, tool: OneAPITool, prompt: str, model: str, **kwargs):
     async with sem:
         try:
```

### Comparing `one-api-tool-0.5.4/oneapi/one_api_test.py` & `one-api-tool-0.5.5/oneapi/one_api_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 
 if __name__ == "__main__":
     claude_config = '../../ant/config/anthropic_config_personal.json'
     openai_config = '../../ant/config/openapi_official_chenghao.json'
     azure_config = '../../ant/config/openapi_azure_config_xiaoduo_dev.json'
     config_file = claude_config
-    # tool = OneAPITool.from_config_file(config_file)
-    
-    # prompt = '今天天气不错？'
+    tool = OneAPITool.from_config_file(config_file)
+
+    prompt = '今天天气不错？'
+    prompt = 'how is the weather today?'
+    print(tool.count_tokens([prompt]))
     # res = asyncio.run(tool.asimple_chat(prompt, stream=True))
     # print(res)
-    res = asyncio.run(batch_chat([claude_config, openai_config, azure_config], ['心率异常可以局部麻醉吗', '今天天气不错？', '你好？', '上午是几点', '热天吃什么', '胖子爱出汗', '窦性心率是什么'], stream=False))
-    print(res)
+    # res = asyncio.run(batch_chat([claude_config, openai_config, azure_config], ['心率异常可以局部麻醉吗', '今天天气不错？', '你好？', '上午是几点', '热天吃什么', '胖子爱出汗', '窦性心率是什么'], stream=False))
+    # print(res)
```

### Comparing `one-api-tool-0.5.4/oneapi/utils.py` & `one-api-tool-0.5.5/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.4/setup.py` & `one-api-tool-0.5.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.5.4",
+    version="0.5.5",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic>=0.3",
         "requests",
```

