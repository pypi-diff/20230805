# Comparing `tmp/ICICONSOLE-0.6.0.tar.gz` & `tmp/ICICONSOLE-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.6.0.tar", last modified: Thu Jul 20 21:13:30 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.7.0.tar", last modified: Sat Aug  5 01:54:20 2023, max compression
```

## Comparing `ICICONSOLE-0.6.0.tar` & `ICICONSOLE-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 21:13:30.404761 ICICONSOLE-0.6.0/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 21:13:30.403516 ICICONSOLE-0.6.0/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1076 2023-07-03 21:32:23.000000 ICICONSOLE-0.6.0/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1279 2023-07-20 20:33:44.000000 ICICONSOLE-0.6.0/ICICONSOLE/Utilities.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.6.0/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    13012 2023-07-20 21:11:33.000000 ICICONSOLE-0.6.0/ICICONSOLE/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLE-0.6.0/ICICONSOLE/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-20 21:13:30.404376 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    44456 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-07-20 21:13:30.000000 ICICONSOLE-0.6.0/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.6.0/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.6.0/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)    44456 2023-07-20 21:13:30.404621 ICICONSOLE-0.6.0/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     3328 2023-07-20 17:56:36.000000 ICICONSOLE-0.6.0/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)      939 2023-07-20 21:03:58.000000 ICICONSOLE-0.6.0/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-20 21:13:30.404796 ICICONSOLE-0.6.0/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-08-05 01:54:20.360427 ICICONSOLE-0.7.0/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-08-05 01:54:20.359132 ICICONSOLE-0.7.0/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      752 2023-08-05 00:44:49.000000 ICICONSOLE-0.7.0/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1279 2023-07-20 20:33:44.000000 ICICONSOLE-0.7.0/ICICONSOLE/Utilities.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-0.7.0/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    14856 2023-08-05 01:52:14.000000 ICICONSOLE-0.7.0/ICICONSOLE/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      323 2023-08-05 00:42:38.000000 ICICONSOLE-0.7.0/ICICONSOLE/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-08-05 01:54:20.360061 ICICONSOLE-0.7.0/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    44568 2023-08-05 01:54:20.000000 ICICONSOLE-0.7.0/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      381 2023-08-05 01:54:20.000000 ICICONSOLE-0.7.0/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-08-05 01:54:20.000000 ICICONSOLE-0.7.0/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-08-05 01:54:20.000000 ICICONSOLE-0.7.0/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-08-05 01:54:20.000000 ICICONSOLE-0.7.0/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-08-05 01:54:20.000000 ICICONSOLE-0.7.0/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-07-17 20:04:48.000000 ICICONSOLE-0.7.0/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       35 2023-07-17 20:04:54.000000 ICICONSOLE-0.7.0/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    44568 2023-08-05 01:54:20.360289 ICICONSOLE-0.7.0/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     3440 2023-08-05 01:53:13.000000 ICICONSOLE-0.7.0/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      939 2023-08-05 01:53:41.000000 ICICONSOLE-0.7.0/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-08-05 01:54:20.360463 ICICONSOLE-0.7.0/setup.cfg
```

### Comparing `ICICONSOLE-0.6.0/ICICONSOLE/Utilities.py` & `ICICONSOLE-0.7.0/ICICONSOLE/Utilities.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.6.0/ICICONSOLE/__main__.py` & `ICICONSOLE-0.7.0/ICICONSOLE/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,24 +45,23 @@
 global pod_id
 # Global variable to store username, set upon initial input from login to TAPIS
 global user
 
 global t
 
 
-
 # Welcome message, formatted with the heavyFormat function
 heavyFormat("Welcome to ICICONSOLE. Login to get started. ")
 
 
 def console(graph, kg):
     global tapis_base_url, valid_key
     lightFormat("Type \"new\" to access a different pod, or type \"exit\" to leave ICICONSOLE. Type \"help\" for help!\nNote that the scrolling menu, which appears on some queries, has a separate help menu.")
 
-    while(True):
+    while True:
         query = str(input("[" + user + "@" + kg + "]$ "))
 
         execute_cypher = True
 
         match query:
             case "exit":
                 os._exit(0)
@@ -78,55 +77,82 @@
                 try:
                     helpCypher()
                     execute_cypher = False
                 except:
                     pass
             case "all":
                 query = bcc.getAll()
-            case "allNames":
-                query = bcc.getAllNames()
-            case "oneByName":
-                query = bcc.getOneByName()
             case "allProperty":
-                query = bcc.allProperty()
+                property = str(input("Enter property: "))
+                query = bcc.allProperty(property)
             case "allProperties":
                 query = bcc.allProperties()
             case "allPropertiesForNode":
                 query = bcc.allPropertiesForNode()
             case "GPT":
                 if not valid_key:
-                    try:
+                    key = os.environ.get("OPENAI_API_KEY")
+                    if key is not None:
                         openai.api_key = os.environ.get("OPENAI_API_KEY")
-                    except:
-                        openai.api_key = getpass("Please enter your OpenAI API key: ")
+                    else:
+                        success = False
+                        while not success:
+                            access_option = str(input("Key not found. Read key via: file, input, env_var "))
+                            if access_option == "file":
+                                file_path = os.environ.get('KEY_FILE')
+                                if file_path is None:
+                                    file_path = str(input("Enter the path to the file with your key: "))
+                                try:
+                                    with open(file_path, 'r') as f:
+                                        file_contents = f.read().strip()
+                                        openai.api_key = file_contents
+                                        os.environ['KEY_FILE'] = file_path
+                                        success = True
+                                except FileNotFoundError:
+                                    print(f"The file '{file_path}' was not found.")
+                                except Exception as e:
+                                    print(f"An error occurred: {e}")
+                            elif access_option == "input":
+                                openai.api_key = getpass("Please enter your OpenAI API key: ")
+                                success = True
+                            elif access_option == "env_var":
+                                env_var = str(input("Enter environment variable name: "))
+                                key = os.environ.get(env_var)
+                                if key is not None:
+                                    openai.api_key = key
+                                else:
+                                    print("Invalid environment variable")
+                            else:
+                                print("Please select a valid option.")
+
                 message = input("[GPT@" + kg + "] ")
                 try:
                     if message:
                         messages.append(
                             {"role": "user", "content": message},
                         )
                         try:
                             chat = openai.ChatCompletion.create(
                                 model="gpt-3.5-turbo", messages=messages
                             )
+                            reply = chat.choices[0].message.content
+                            print(str(reply))
                             valid_key = True
                             os.environ['OPENAI_API_KEY'] = openai.api_key
+
+                            validate = input("Run this? (y/n) ")
+                            if validate == "y":
+                                query = str(reply)
+                            else:
+                                execute_cypher = False
                         except:
                             "Error: OpenAI API key is invalid."
                             valid_key = False
-
-                    reply = chat.choices[0].message.content
-                    print(str(reply))
                 except Exception as e:
                     print(e)
-                validate = input("Run this? (y/n) ")
-                if validate == "y":
-                    query = str(reply)
-                else:
-                    execute_cypher = False
             case _:
                 pass
 
         if execute_cypher:
             try:
                 # queries = query.splitlines()
                 # for query in queries:
@@ -249,15 +275,14 @@
             er = e
             if flag.exit():
                 break
             print("There was a connection error.")
             break
 
 
-
 def tapis_login():
     global t
     global user
     global tapis_base_url
     while True:
         try:
             change_base_url = str(input(f"Change base url from {tapis_base_url}? (y/n) "))
```

### Comparing `ICICONSOLE-0.6.0/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.7.0/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.6.0
+Version: 0.7.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -771,11 +771,11 @@
 
 Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
 ```
 
-If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). Then, you can simply type in a query in natural language and get the Cypher code for it.
+If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). You can tell the program to look for your key in a file or environment variable, or simply type it in as input. Then, you can simply type in a query in natural language and get the Cypher code for it.
 
 The welcome message for the Knowledge Graph console contains helpful tips, like "new", "exit", "clear", and "help".
```

### Comparing `ICICONSOLE-0.6.0/LICENSE` & `ICICONSOLE-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.6.0/PKG-INFO` & `ICICONSOLE-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.6.0
+Version: 0.7.0
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -771,11 +771,11 @@
 
 Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
 ```
 
-If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). Then, you can simply type in a query in natural language and get the Cypher code for it.
+If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). You can tell the program to look for your key in a file or environment variable, or simply type it in as input. Then, you can simply type in a query in natural language and get the Cypher code for it.
 
 The welcome message for the Knowledge Graph console contains helpful tips, like "new", "exit", "clear", and "help".
```

### Comparing `ICICONSOLE-0.6.0/README.md` & `ICICONSOLE-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,11 +81,11 @@
 
 Once you access either a Tapis Pod or your local database, you will be in a custom made console for interfacing with your Knowledge Graph, using the Cypher language. If you know Cypher, you can start typing in commands like 
 
 ```
 MATCH(n) RETURN n LIMIT 10
 ```
 
-If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). Then, you can simply type in a query in natural language and get the Cypher code for it.
+If you are not familiar with Cypher, don't worry! This is meant for users who have never used Cypher before. Type in "help" to view some of the built in commands to start exploring the knowledge graph. These commands are very limited however; you can query more creatively and extensively using the power of GPT. Type in the "GPT" command for this. Note that you will need an OpenAI key, which you can get [here](https://beta.openai.com/). You can tell the program to look for your key in a file or environment variable, or simply type it in as input. Then, you can simply type in a query in natural language and get the Cypher code for it.
 
 The welcome message for the Knowledge Graph console contains helpful tips, like "new", "exit", "clear", and "help".
```

### Comparing `ICICONSOLE-0.6.0/pyproject.toml` & `ICICONSOLE-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.6.0"
+version = "0.7.0"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

