# Comparing `tmp/meeseeksai-0.1.4.tar.gz` & `tmp/meeseeksai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeseeksai-0.1.4.tar", max compression
+gzip compressed data, was "meeseeksai-0.1.5.tar", max compression
```

## Comparing `meeseeksai-0.1.4.tar` & `meeseeksai-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.4/meeseeksai/__init__.py
--rw-r--r--   0        0        0     1782 2023-08-04 22:19:53.125171 meeseeksai-0.1.4/meeseeksai/meeseeksai.py
--rw-r--r--   0        0        0      356 2023-08-04 22:32:23.065010 meeseeksai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 meeseeksai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 18:37:05.638104 meeseeksai-0.1.5/meeseeksai/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-04 22:50:30.104803 meeseeksai-0.1.5/meeseeksai/meeseeksai.py
+-rw-r--r--   0        0        0      359 2023-08-04 22:50:46.574800 meeseeksai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 meeseeksai-0.1.5/PKG-INFO
```

### Comparing `meeseeksai-0.1.4/meeseeksai/meeseeksai.py` & `meeseeksai-0.1.5/meeseeksai/meeseeksai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Meeseeks AI chatbot"""
 import os
+import sys
 import openai
 from dotenv import load_dotenv
 
 
 # System message prompt for OpenAI chatbot
 SYSTEM_MESSAGE_PROMPT = "You are a friendly AI assistant called Meeseeks. Always introduce yourself to the user. Your job is to help users with their queries."
 
@@ -37,12 +38,17 @@
     if not os.environ.get("OPENAI_API_KEY"):
         os.environ["OPENAI_API_KEY"] = input("Enter your OPENAI_API_KEY: ")
     if not os.environ.get("OPENAI_API_BASE"):
         os.environ["OPENAI_API_BASE"] = input("Enter your OPENAI_API_BASE: ")
 
     openai.api_key = os.environ.get("OPENAI_API_KEY")
     openai.api_base = os.environ.get("OPENAI_API_BASE")
+
+    print(args)
+
+    if not args:
+        args = sys.argv[1:]
     
     user_prompt = ' '.join(args)
     
     messages = construct_message_with_history(user_prompt)
     return get_chat_completion(messages)
```

