# Comparing `tmp/llmx-0.0.5a0.tar.gz` & `tmp/llmx-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmx-0.0.5a0.tar", last modified: Fri Aug  4 17:30:02 2023, max compression
+gzip compressed data, was "llmx-0.0.6a0.tar", last modified: Sat Aug  5 01:08:49 2023, max compression
```

## Comparing `llmx-0.0.5a0.tar` & `llmx-0.0.6a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3170 2023-08-03 03:11:18.000000 llmx-0.0.5a0/.gitignore
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1083 2023-08-04 04:13:34.000000 llmx-0.0.5a0/LICENSE
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       27 2023-08-02 21:17:22.000000 llmx-0.0.5a0/MANIFEST.in
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-04 17:30:02.662583 llmx-0.0.5a0/PKG-INFO
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4948 2023-08-04 16:57:35.000000 llmx-0.0.5a0/README.md
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.658583 llmx-0.0.5a0/llmx/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      185 2023-08-02 22:29:16.000000 llmx-0.0.5a0/llmx/__init__.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1322 2023-08-04 03:49:25.000000 llmx-0.0.5a0/llmx/datamodel.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.658583 llmx-0.0.5a0/llmx/generators/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      128 2023-08-02 22:29:06.000000 llmx-0.0.5a0/llmx/generators/__init__.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/llmx/generators/text/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-02 20:54:42.000000 llmx-0.0.5a0/llmx/generators/text/__init__.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1063 2023-08-02 23:44:59.000000 llmx-0.0.5a0/llmx/generators/text/base_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2865 2023-08-02 23:47:07.000000 llmx-0.0.5a0/llmx/generators/text/cohere_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     8497 2023-08-02 23:46:52.000000 llmx-0.0.5a0/llmx/generators/text/hf_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2728 2023-08-02 23:46:09.000000 llmx-0.0.5a0/llmx/generators/text/openai_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3599 2023-08-04 04:05:33.000000 llmx-0.0.5a0/llmx/generators/text/palm_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1505 2023-08-02 23:47:30.000000 llmx-0.0.5a0/llmx/generators/text/textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4050 2023-08-04 04:03:40.000000 llmx-0.0.5a0/llmx/utils.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       37 2023-08-04 17:22:00.000000 llmx-0.0.5a0/llmx/version.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.658583 llmx-0.0.5a0/llmx.egg-info/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/PKG-INFO
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      670 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/SOURCES.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/dependency_links.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/entry_points.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      119 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/requires.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        5 2023-08-04 17:30:02.000000 llmx-0.0.5a0/llmx.egg-info/top_level.txt
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/notebooks/
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/notebooks/research/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      775 2023-08-01 22:45:11.000000 llmx-0.0.5a0/notebooks/research/travelbenchmark.ipynb
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3669 2023-08-04 14:18:45.000000 llmx-0.0.5a0/notebooks/tutorial.ipynb
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1384 2023-08-04 14:14:13.000000 llmx-0.0.5a0/pyproject.toml
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-04 17:30:02.662583 llmx-0.0.5a0/setup.cfg
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-01 22:45:11.000000 llmx-0.0.5a0/setup.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-04 17:30:02.662583 llmx-0.0.5a0/tests/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1916 2023-08-04 14:18:02.000000 llmx-0.0.5a0/tests/test_generators.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3170 2023-08-03 03:11:18.000000 llmx-0.0.6a0/.gitignore
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1083 2023-08-04 04:13:34.000000 llmx-0.0.6a0/LICENSE
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       27 2023-08-02 21:17:22.000000 llmx-0.0.6a0/MANIFEST.in
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-05 01:08:49.743155 llmx-0.0.6a0/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4948 2023-08-04 16:57:35.000000 llmx-0.0.6a0/README.md
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      185 2023-08-02 22:29:16.000000 llmx-0.0.6a0/llmx/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1322 2023-08-04 03:49:25.000000 llmx-0.0.6a0/llmx/datamodel.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx/generators/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      128 2023-08-02 22:29:06.000000 llmx-0.0.6a0/llmx/generators/__init__.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx/generators/text/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-02 20:54:42.000000 llmx-0.0.6a0/llmx/generators/text/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1063 2023-08-02 23:44:59.000000 llmx-0.0.6a0/llmx/generators/text/base_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2865 2023-08-02 23:47:07.000000 llmx-0.0.6a0/llmx/generators/text/cohere_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     8497 2023-08-02 23:46:52.000000 llmx-0.0.6a0/llmx/generators/text/hf_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2728 2023-08-02 23:46:09.000000 llmx-0.0.6a0/llmx/generators/text/openai_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4110 2023-08-04 21:13:28.000000 llmx-0.0.6a0/llmx/generators/text/palm_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1561 2023-08-04 18:29:17.000000 llmx-0.0.6a0/llmx/generators/text/textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4369 2023-08-04 20:18:07.000000 llmx-0.0.6a0/llmx/utils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       37 2023-08-05 01:08:42.000000 llmx-0.0.6a0/llmx/version.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx.egg-info/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      670 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/SOURCES.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/dependency_links.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/entry_points.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      119 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/requires.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        5 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/top_level.txt
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/notebooks/
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/notebooks/research/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      775 2023-08-01 22:45:11.000000 llmx-0.0.6a0/notebooks/research/travelbenchmark.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3669 2023-08-04 14:18:45.000000 llmx-0.0.6a0/notebooks/tutorial.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1384 2023-08-04 14:14:13.000000 llmx-0.0.6a0/pyproject.toml
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-05 01:08:49.743155 llmx-0.0.6a0/setup.cfg
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-01 22:45:11.000000 llmx-0.0.6a0/setup.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/tests/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1936 2023-08-05 01:07:46.000000 llmx-0.0.6a0/tests/test_generators.py
```

### Comparing `llmx-0.0.5a0/.gitignore` & `llmx-0.0.6a0/.gitignore`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/LICENSE` & `llmx-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/PKG-INFO` & `llmx-0.0.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmx
-Version: 0.0.5a0
+Version: 0.0.6a0
 Summary: LLMX: A library for LLM Text Generation
 Author-email: Victor Dibia <victor.dibia@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) <year> Adam Veldhousen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `llmx-0.0.5a0/README.md` & `llmx-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/llmx/datamodel.py` & `llmx-0.0.6a0/llmx/datamodel.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/llmx/generators/text/base_textgen.py` & `llmx-0.0.6a0/llmx/generators/text/base_textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/llmx/generators/text/cohere_textgen.py` & `llmx-0.0.6a0/llmx/generators/text/cohere_textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/llmx/generators/text/hf_textgen.py` & `llmx-0.0.6a0/llmx/generators/text/hf_textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/llmx/generators/text/openai_textgen.py` & `llmx-0.0.6a0/llmx/generators/text/openai_textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/llmx/generators/text/palm_textgen.py` & `llmx-0.0.6a0/llmx/generators/text/palm_textgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,64 +23,75 @@
     def format_messages(self, messages):
         palm_messages = []
         system_messages = ""
         for message in messages:
             if message["role"] == "system":
                 system_messages += message["content"] + "\n"
             else:
-                palm_message = {
-                    "author": message["role"],
-                    "content": message["content"],
-                }
-                palm_messages.append(palm_message)
+                if not palm_messages or palm_messages[-1]['author'] != message['role']:
+                    palm_message = {
+                        "author": message["role"],
+                        "content": message["content"],
+                    }
+                    palm_messages.append(palm_message)
+                else:
+                    palm_messages[-1]['content'] += '\n' + message['content']
+
+        if palm_messages and len(palm_messages) % 2 == 0:
+            merged_content = palm_messages[-2]['content'] + '\n' + palm_messages[-1]['content']
+            palm_messages[-2]['content'] = merged_content
+            palm_messages.pop()
+
         return system_messages, palm_messages
 
     def generate(
             self, messages: Union[list[dict],
                                   str],
             config: TextGenerationConfig = TextGenerationConfig(),
             **kwargs) -> TextGenerationResponse:
 
         use_cache = config.use_cache
         model = config.model or "codechat-bison"
         system_messages, messages = self.format_messages(messages)
         self.model_name = model
 
+        print("*********", messages)
+
         api_url = f"https://us-central1-aiplatform.googleapis.com/v1/projects/{self.project_id}/locations/{self.project_location}/publishers/google/models/{model}:predict"
 
 #  'candidateCount': max(1, min(8, config.n)),  # 1 <= n <= 8,
 # 'topP': config.top_p,
 #                 'topK': config.top_k,
 
         palm_config = {
             'temperature': config.temperature,
-            'maxOutputTokens': config.max_tokens}
+            'maxOutputTokens': config.max_tokens or 2040}
         palm_payload = {
             'instances': [
                 {'messages': messages,
                  'context': system_messages,
                  'examples': [],
                  }
             ],
             'parameters': palm_config
         }
-        # print("*********", palm_payload)
-
-        palm_response = gcp_request(
-            url=api_url,
-            body=palm_payload,
-            method="POST",
-            credentials=self.credentials)
+        # print("*********", use_cache, palm_payload)
 
         cache_key_params = palm_payload
         if use_cache:
             response = cache_request(cache=self.cache, params=cache_key_params)
             if response:
                 return TextGenerationResponse(**response)
 
+        palm_response = gcp_request(
+            url=api_url,
+            body=palm_payload,
+            method="POST",
+            credentials=self.credentials)
+
         response_text = [
             Message(
                 role="assistant" if x["author"] == "1" else x["author"],
                 content=x["content"],
             )
             for x in palm_response["predictions"][0]["candidates"]
         ]
```

### Comparing `llmx-0.0.5a0/llmx/generators/text/textgen.py` & `llmx-0.0.6a0/llmx/generators/text/textgen.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .openai_textgen import OpenAITextGenerator
 from .palm_textgen import PalmTextGenerator
 from .cohere_textgen import CohereTextGenerator
 
 
 def text_generator(provider: str = "openai", **kwargs):
-    if provider == "openai" or provider == "default":
+    if provider.lower() == "openai" or provider.lower() == "default":
         return OpenAITextGenerator(**kwargs)
-    elif provider == "palm" or provider == "google":
+    elif provider.lower() == "palm" or provider.lower() == "google":
         return PalmTextGenerator(provider=provider, **kwargs)
-    elif provider == "cohere":
+    elif provider.lower() == "cohere":
         return CohereTextGenerator(provider=provider, **kwargs)
-    elif provider == "hf" or provider == "huggingface":
+    elif provider.lower() == "hf" or provider.lower() == "huggingface":
         try:
             import transformers
             from transformers import (
                 AutoTokenizer,
                 AutoModelForCausalLM,
                 GenerationConfig,
             )
```

### Comparing `llmx-0.0.5a0/llmx/utils.py` & `llmx-0.0.6a0/llmx/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,9 +108,18 @@
     headers = headers or {}
     headers["Authorization"] = f"Bearer {credentials.token}"
     headers["Content-Type"] = "application/json"
 
     response = requests.request(
         method=method, url=url, json=body, headers=headers, **kwargs
     )
-    response.raise_for_status()
+
+    if response.status_code not in range(200, 300):
+        try:
+            error_message = response.json().get("error", {}).get("message", "")
+        except json.JSONDecodeError:
+            error_message = response.content
+        raise Exception(
+            f"Request failed with status code {response.status_code}: {error_message}"
+        )
+
     return response.json()
```

### Comparing `llmx-0.0.5a0/llmx.egg-info/PKG-INFO` & `llmx-0.0.6a0/llmx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmx
-Version: 0.0.5a0
+Version: 0.0.6a0
 Summary: LLMX: A library for LLM Text Generation
 Author-email: Victor Dibia <victor.dibia@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) <year> Adam Veldhousen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `llmx-0.0.5a0/llmx.egg-info/SOURCES.txt` & `llmx-0.0.6a0/llmx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/notebooks/research/travelbenchmark.ipynb` & `llmx-0.0.6a0/notebooks/research/travelbenchmark.ipynb`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/notebooks/tutorial.ipynb` & `llmx-0.0.6a0/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/pyproject.toml` & `llmx-0.0.6a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmx-0.0.5a0/tests/test_generators.py` & `llmx-0.0.6a0/tests/test_generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     answer = cohere_response.text[0].content
     print(cohere_response.text[0].content)
 
     assert ("paris" in answer.lower())
     assert len(cohere_response.text) == 2
 
 
-@pytest.mark.skipif("RUNALL" not in os.environ, reason="takes too long")
+@pytest.mark.skipif(os.environ.get("LLMX_RUNALL", None) == "False", reason="takes too long")
 def test_hf_local():
     hf_local_gen = generator(
         provider="hf",
         model="TheBloke/Llama-2-7b-chat-fp16",
         device_map="auto")
     hf_local_response = hf_local_gen.generate(messages, config=config)
     answer = hf_local_response.text[0].content
```

