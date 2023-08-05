# Comparing `tmp/vercel_llm_api-0.3.0-py3-none-any.whl.zip` & `tmp/vercel_llm_api-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 18576 bytes, number of entries: 6
--rw-r--r--  2.0 unx     6042 b- defN 23-Jul-25 02:22 vercel_ai.py
--rw-r--r--  2.0 unx    35148 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7729 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      491 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/RECORD
-6 files, 49512 bytes uncompressed, 17686 bytes compressed:  64.3%
+Zip file size: 18659 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     6193 b- defN 23-Aug-05 06:13 vercel_ai.py
+-rw-r--r--  2.0 unx    35148 b- defN 23-Aug-05 06:13 vercel_llm_api-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7729 b- defN 23-Aug-05 06:13 vercel_llm_api-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 06:13 vercel_llm_api-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-05 06:13 vercel_llm_api-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      491 b- defN 23-Aug-05 06:13 vercel_llm_api-0.3.1.dist-info/RECORD
+6 files, 49663 bytes uncompressed, 17769 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vercel_ai.py
 Comment: 
 
-Filename: vercel_llm_api-0.3.0.dist-info/LICENSE
+Filename: vercel_llm_api-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: vercel_llm_api-0.3.0.dist-info/METADATA
+Filename: vercel_llm_api-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: vercel_llm_api-0.3.0.dist-info/WHEEL
+Filename: vercel_llm_api-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: vercel_llm_api-0.3.0.dist-info/top_level.txt
+Filename: vercel_llm_api-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vercel_llm_api-0.3.0.dist-info/RECORD
+Filename: vercel_llm_api-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vercel_ai.py

```diff
@@ -4,14 +4,15 @@
 import json
 import base64
 import quickjs
 import queue
 import threading
 import uuid
 import random
+import struct
 from curl_cffi import requests
 
 logging.basicConfig()
 logger = logging.getLogger()
 
 class Client:
   base_url = "https://sdk.vercel.ai"
@@ -69,15 +70,15 @@
       thread.start()
       threads.append(thread)
     
     for thread in threads:
       thread.join()
     
     for script in scripts:
-      models_regex = r'let .="\\n\\nHuman:\",r=(.+?),.='
+      models_regex = r'let .="\\n\\nHuman:\",.=(.+?),.='
       matches = re.findall(models_regex, script)
 
       if matches:
         models_str = matches[0]
         stop_sequences_regex = r'(?<=stopSequences:{value:\[)\D(?<!\])'
         models_str = re.sub(stop_sequences_regex, re.escape('"\\n\\nHuman:"'), models_str)
 
@@ -86,29 +87,32 @@
         return json.loads(json_str)
 
     return []
 
   def get_token(self):
     logger.info("Fetching token from "+self.token_url)
     b64 = self.session.get(self.token_url).text
-    data = json.loads(base64.b64decode(b64))
+    data = json.loads(base64.b64decode(b64, validate=True))
 
     script = """
-      var globalThis = {{data: "sentinel"}};
+      String.prototype.fontcolor = function() {{
+        return `<font>${{this}}</font>`
+      }}
+      var globalThis = {{marker: "mark"}};
       ({script})({key})
     """.format(script=data["c"], key=data["a"])
-    
     context = quickjs.Context()
     token_data = json.loads(context.eval(script).json())
+    token_data[2] = "mark"
     token = {
       "r": token_data,
       "t": data["t"]
     }
-    token_string = json.dumps(token, separators=(',', ':')).encode()
-    return base64.b64encode(token_string).decode()
+    token_str = json.dumps(token, separators=(',', ':')).encode("utf-16le")
+    return base64.b64encode(token_str).decode()
 
   def get_default_params(self, model_id):
     model = self.models[model_id]
     defaults = {}
     for key, param in model["parameters"].items():
       defaults[key] = param["value"]
     return defaults
```

## Comparing `vercel_llm_api-0.3.0.dist-info/LICENSE` & `vercel_llm_api-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vercel_llm_api-0.3.0.dist-info/METADATA` & `vercel_llm_api-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vercel-llm-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: A reverse engineered API for the Vercel AI playground.
 Home-page: https://github.com/ading2210/vercel-llm-api
 Author: ading2210
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

