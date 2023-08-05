# Comparing `tmp/open_interpreter-0.0.247.tar.gz` & `tmp/open_interpreter-0.0.248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.247.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.248.tar", max compression
```

## Comparing `open_interpreter-0.0.247.tar` & `open_interpreter-0.0.248.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.247/LICENSE
--rw-r--r--   0        0        0     6396 2023-08-02 00:13:19.900301 open_interpreter-0.0.247/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.247/interpreter/__init__.py
--rw-r--r--   0        0        0      852 2023-08-05 19:49:16.758409 open_interpreter-0.0.247/interpreter/cli.py
--rw-r--r--   0        0        0     2497 2023-08-05 18:13:24.110098 open_interpreter-0.0.247/interpreter/code_block.py
--rw-r--r--   0        0        0     6763 2023-08-05 19:57:34.880192 open_interpreter-0.0.247/interpreter/code_interpreter.py
--rw-r--r--   0        0        0     8002 2023-08-05 20:28:58.619904 open_interpreter-0.0.247/interpreter/interpreter.py
--rw-r--r--   0        0        0     7023 2023-08-05 18:23:33.196206 open_interpreter-0.0.247/interpreter/json_utils.py
--rw-r--r--   0        0        0     1111 2023-08-05 09:45:06.755389 open_interpreter-0.0.247/interpreter/message_block.py
--rw-r--r--   0        0        0     2552 2023-08-05 19:54:44.552641 open_interpreter-0.0.247/interpreter/system_message.txt
--rw-r--r--   0        0        0      585 2023-08-05 20:30:30.746151 open_interpreter-0.0.247/pyproject.toml
--rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 open_interpreter-0.0.247/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.248/LICENSE
+-rw-r--r--   0        0        0     6396 2023-08-02 00:13:19.900301 open_interpreter-0.0.248/README.md
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.248/interpreter/__init__.py
+-rw-r--r--   0        0        0      870 2023-08-05 20:49:13.634295 open_interpreter-0.0.248/interpreter/cli.py
+-rw-r--r--   0        0        0     2497 2023-08-05 18:13:24.110098 open_interpreter-0.0.248/interpreter/code_block.py
+-rw-r--r--   0        0        0     6770 2023-08-05 20:48:48.736606 open_interpreter-0.0.248/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0     8002 2023-08-05 20:28:58.619904 open_interpreter-0.0.248/interpreter/interpreter.py
+-rw-r--r--   0        0        0     7023 2023-08-05 18:23:33.196206 open_interpreter-0.0.248/interpreter/json_utils.py
+-rw-r--r--   0        0        0     1111 2023-08-05 09:45:06.755389 open_interpreter-0.0.248/interpreter/message_block.py
+-rw-r--r--   0        0        0     2552 2023-08-05 19:54:44.552641 open_interpreter-0.0.248/interpreter/system_message.txt
+-rw-r--r--   0        0        0      585 2023-08-05 20:49:33.127617 open_interpreter-0.0.248/pyproject.toml
+-rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 open_interpreter-0.0.248/PKG-INFO
```

### Comparing `open_interpreter-0.0.247/LICENSE` & `open_interpreter-0.0.248/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.247/README.md` & `open_interpreter-0.0.248/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.247/interpreter/cli.py` & `open_interpreter-0.0.248/interpreter/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,13 +21,12 @@
                       action='store_true',
                       help='execute code without user confirmation')
   args = parser.parse_args()
 
   if args.yes:
     interpreter.auto_run = True
   else:
-    print()  # Print newline
-    print(Markdown(confirm_mode_message))
-    print()  # Print newline
+    # Print message with newlines on either side (aesthetic choice)
+    print('', Markdown(confirm_mode_message), '')
 
   # Now run the chat method
   interpreter.chat()
```

### Comparing `open_interpreter-0.0.247/interpreter/code_block.py` & `open_interpreter-0.0.248/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.247/interpreter/code_interpreter.py` & `open_interpreter-0.0.248/interpreter/code_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import subprocess
 import threading
 import time
 import ast
 import astor
-import json
 
 
 # Mapping of languages to their start and print commands
 language_map = {
   "python": {
     "start_cmd": "python -i -q -u",
     "print_cmd": 'print("{}")'
@@ -18,17 +17,19 @@
   },
   "javascript": {
     "start_cmd": "node -i",
     "print_cmd": 'console.log("{}")'
   }
 }
 
-# Get forbidden_commands
+# Get forbidden_commands (disabled)
+"""
 with open("interpreter/forbidden_commands.json", "r") as f:
   forbidden_commands = json.load(f)
+"""
 
 
 class CodeInterpreter:
   """
   Code Interpreters display and run code in different languages.
   
   They can create code blocks on the terminal, then be executed to produce an output which will be displayed in real-time.
```

### Comparing `open_interpreter-0.0.247/interpreter/interpreter.py` & `open_interpreter-0.0.248/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.247/interpreter/json_utils.py` & `open_interpreter-0.0.248/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.247/interpreter/message_block.py` & `open_interpreter-0.0.248/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.247/interpreter/system_message.txt` & `open_interpreter-0.0.248/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.247/pyproject.toml` & `open_interpreter-0.0.248/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.247"
+version = "0.0.248"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.247/PKG-INFO` & `open_interpreter-0.0.248/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.247
+Version: 0.0.248
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

