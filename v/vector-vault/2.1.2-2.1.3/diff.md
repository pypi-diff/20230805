# Comparing `tmp/vector_vault-2.1.2.tar.gz` & `tmp/vector_vault-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.1.2.tar", last modified: Tue Jul 18 22:48:31 2023, max compression
+gzip compressed data, was "vector_vault-2.1.3.tar", last modified: Sat Aug  5 16:40:27 2023, max compression
```

## Comparing `vector_vault-2.1.2.tar` & `vector_vault-2.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:48:31.278995 vector_vault-2.1.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    27248 2023-07-18 22:48:31.278867 vector_vault-2.1.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    26538 2023-07-16 05:57:03.000000 vector_vault-2.1.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-07-18 22:48:31.279033 vector_vault-2.1.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1060 2023-07-18 22:48:25.000000 vector_vault-2.1.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:48:31.274719 vector_vault-2.1.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    27248 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:48:31.278514 vector_vault-2.1.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.2/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16190 2023-07-18 22:48:19.000000 vector_vault-2.1.2/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    36436 2023-07-18 22:45:52.000000 vector_vault-2.1.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 16:40:27.529618 vector_vault-2.1.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    26593 2023-08-05 16:40:27.529481 vector_vault-2.1.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    25883 2023-08-01 07:40:15.000000 vector_vault-2.1.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-05 16:40:27.529671 vector_vault-2.1.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1060 2023-08-05 16:40:18.000000 vector_vault-2.1.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 16:40:27.524485 vector_vault-2.1.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    26593 2023-08-05 16:40:27.000000 vector_vault-2.1.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-05 16:40:27.000000 vector_vault-2.1.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-05 16:40:27.000000 vector_vault-2.1.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-05 16:40:27.000000 vector_vault-2.1.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-05 16:40:27.000000 vector_vault-2.1.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 16:40:27.529104 vector_vault-2.1.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.3/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16773 2023-07-21 20:42:10.000000 vector_vault-2.1.3/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    36537 2023-08-05 16:39:44.000000 vector_vault-2.1.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.3/vectorvault/wrap.py
```

### Comparing `vector_vault-2.1.2/LICENSE` & `vector_vault-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.2/PKG-INFO` & `vector_vault-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.1.2
+Version: 2.1.3
 Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -15,21 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-By combining vector similarity search with generative ai chat, new possibilities for conversation emerge. For example, product information can be added to the Vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by ChatGPT for an accurate response. This capability allows for informed conversation that range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more. Vector Vault was built to allow you to tap into ^ **this** potential.
-
 Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters. Vector Vault ensures secure and isolated data handling and enables you to create and interact with vector databases - aka "vaults" - in under one second response times, from our serverless cloud architecture backed by Google. 
 
 We've integrated all the chat options people like to use with LangChain. By combining vector databases with OpenAI's chat in the `vectorvault` package, we've been able to hide a lot of the complexity in the background and make it really easy to build the kind of custom chat experience you want to build. 
 
-With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
+With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for a fast and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
 
 <br>
 
 ### Full Python API:
 
 `pip install vector-vault` : install
 <br>
```

### Comparing `vector_vault-2.1.2/README.md` & `vector_vault-2.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-By combining vector similarity search with generative ai chat, new possibilities for conversation emerge. For example, product information can be added to the Vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by ChatGPT for an accurate response. This capability allows for informed conversation that range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more. Vector Vault was built to allow you to tap into ^ **this** potential.
-
 Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters. Vector Vault ensures secure and isolated data handling and enables you to create and interact with vector databases - aka "vaults" - in under one second response times, from our serverless cloud architecture backed by Google. 
 
 We've integrated all the chat options people like to use with LangChain. By combining vector databases with OpenAI's chat in the `vectorvault` package, we've been able to hide a lot of the complexity in the background and make it really easy to build the kind of custom chat experience you want to build. 
 
-With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
+With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for a fast and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
 
 <br>
 
 ### Full Python API:
 
 `pip install vector-vault` : install
 <br>
```

### Comparing `vector_vault-2.1.2/setup.py` & `vector_vault-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.1.2",
+    version="2.1.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.1.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.1.3/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.1.2
+Version: 2.1.3
 Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -15,21 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-By combining vector similarity search with generative ai chat, new possibilities for conversation emerge. For example, product information can be added to the Vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by ChatGPT for an accurate response. This capability allows for informed conversation that range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more. Vector Vault was built to allow you to tap into ^ **this** potential.
-
 Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters. Vector Vault ensures secure and isolated data handling and enables you to create and interact with vector databases - aka "vaults" - in under one second response times, from our serverless cloud architecture backed by Google. 
 
 We've integrated all the chat options people like to use with LangChain. By combining vector databases with OpenAI's chat in the `vectorvault` package, we've been able to hide a lot of the complexity in the background and make it really easy to build the kind of custom chat experience you want to build. 
 
-With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
+With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for a fast and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
 
 <br>
 
 ### Full Python API:
 
 `pip install vector-vault` : install
 <br>
```

### Comparing `vector_vault-2.1.2/vectorvault/ai.py` & `vector_vault-2.1.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.2/vectorvault/cloud_api.py` & `vector_vault-2.1.3/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.2/vectorvault/cloudmanager.py` & `vector_vault-2.1.3/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.2/vectorvault/creds.py` & `vector_vault-2.1.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.2/vectorvault/download.py` & `vector_vault-2.1.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.2/vectorvault/itemize.py` & `vector_vault-2.1.3/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.2/vectorvault/tools_gpt.py` & `vector_vault-2.1.3/vectorvault/tools_gpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,34 +6,42 @@
     Every tool turns subjectivity into objectivity.
     
     Objectivity is needed for code. 
     Subjectivity is the primary human input.
     These tools bridge the gap between human interaction and code. 
     
     ToolsGPT allows you to get the following for any input:
-        1. a Rating - out of 10
-        2. a Match - to a list
-        3. a Topic - match to a list
-        4. Match or Make (M&M) - to list or make new option for the list
+        1. `get_rating` - returns a rating out of 10 for any input
+        2. `get_yes_no` - returns a 'yes' or a 'no' to any question
+        3. `get_binary` - returns a '0' or '1' to any input
+        4. `get_match` - returns a match to a list options
+        5. `match_or_make` - returns a match to a list of options, or a new option
+        6. `get_topic` - returns the topic subject matter of any input 
 
-        1. Out of 10:
+        1. `get_rating`:
             Useful to get a quality rating
+
+        2. `get_yes_no`:
+            Useful for getting a difinitive answer 
+
+        3. `get_binary`:
+            Useful for getting numeric input on a difinitive answer
         
-        2. Answer Match
+        4. `get_match`:
             Useful to get an exact match to one option in a set of options
             in: (text and list of answers)
             out: (exact match to one answer in list of answer)
 
-        3. Topic Match
+        5. `get_topic`:
             Useful to classify the topic of conversation
         
-        4. Match or Make
+        6. `match_or_make` (M&M):
             Get a match to a list of options, or make a new one if unrelated
             Useful if you aren't sure if the input will match one of your existing list options, and need flexibility of creating a new one
-
+            Also useful when starting from an empty list. - will create it from scratch
 '''
 
 class ToolsGPT():
     def __init__(self, verbose=False):
         self.verbose = verbose
         self.llm = AI().llm
 
@@ -262,40 +270,43 @@
         Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: 'No'
         \n\nRespond with a "yes" or "no" to following: "{question}"  """
 
         prompt = prompt_template.format(content=content, question=question)
 
         return self.retry_llm(custom_prompt=prompt, model=model)
     
+    # internal function 
     def yay_or_nay(self, content, question: str, model='gpt-3.5-turbo'):
         '''Not recommended for external use. Internal function'''
         prompt_template = """Do not respond with anything before the yes or no. Do not add anything after the "yes" or "no". 
         Example question 1: 'Is the Eiffel tower located in Paris?' Example answer 1: 'Yes' Example question 2: 'Do you think I am fat?' 
         Example answer 2: 'No' Example question 3: 'Should I use Matplotlib in Python to draw a graph of csv information I have' Example answer 3: 'Yes'
         Example question 4: 'As an ai language model, I can't tell you yes or no, but I it does have a tendency to work sometimes.' Example answer 4: 'Yes'
         Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: 'No'
         \n\nGiven this content: "{content}", Respond with a "yes" or "no" to following question: "{question}"  """
 
         prompt = prompt_template.format(content=content, question=question)
 
         return self.retry_llm(custom_prompt=prompt, model=model)
     
+    # internal function 
     def zero_or_one(self, content, zero_if: str, one_if: str, model='gpt-3.5-turbo'):
         '''Not recommended for external use. Internal function'''
         prompt_template = """Do not respond with anything before the 1 or 0. Do not add anything after the "1" or "0". 
         Example question 1: 'Is the Eiffel tower located in Paris?' Example answer 1: '1' Example question 2: 'Do you think I am fat?' 
         Example answer 2: '0' Example question 3: 'Should I use Matplotlib in Python to draw a graph of csv information I have' Example answer 3: '1'
         Example question 4: 'As an ai language model, I can't tell you yes or no, but I it does have a tendency to work sometimes.' Example answer 4: '1'
         Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: '0'
         \n\nGiven this content: "{content}", Respond with a "0" if {zero_if} \n... or "1" if: "{one_if}"  """
 
         prompt = prompt_template.format(content=content, zero_if=zero_if, one_if=one_if)
 
         return self.retry_llm(custom_prompt=prompt, model=model)
     
+    # internal function 
     def isolate_zero_one(self, content, model='gpt-3.5-turbo'):
         '''Not recommended for external use. Internal function'''
         prompt_template = """Do not respond with anything before the 1 or 0. Do not add anything after the "1" or "0". 
         Example question 1: 'Is the Eiffel tower located in Paris?' Example answer 1: '1' Example question 2: 'Do you think I am fat?' 
         Example answer 2: '0' Example question 3: 'Should I use Matplotlib in Python to draw a graph of csv information I have' Example answer 3: '1'
         Example question 4: 'As an ai language model, I can't tell you yes or no, but I it does have a tendency to work sometimes.' Example answer 4: '1'
         Example question 5: 'Will this happen if it's 19 percent likely to happen?' Example answer 5: '0'
```

### Comparing `vector_vault-2.1.2/vectorvault/vault.py` & `vector_vault-2.1.3/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from .ai import AI
 from .itemize import itemize, name_vecs, get_item, get_vectors, build_return, cloud_name
 from .vecreq import call_get_total_vectors, call_get_vaults, call_get_similar
 from .tools_gpt import ToolsGPT
 
 
 class Vault:
-    def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
+    def __init__(self, user: str = None, api_key: str = None, vault: str = None, openai_key: str = None, dims: int = 1536, verbose: bool = False):
+        if openai_key:
+            os.environ['OPENAI_API_KEY'] = openai_key
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
         self.dims = dims
         self.verbose = verbose
         try:
             self.cloud_manager = CloudManager(user, api_key, self.vault)
```

### Comparing `vector_vault-2.1.2/vectorvault/vecreq.py` & `vector_vault-2.1.3/vectorvault/vecreq.py`

 * *Files identical despite different names*

