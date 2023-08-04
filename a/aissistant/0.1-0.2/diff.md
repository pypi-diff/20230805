# Comparing `tmp/aissistant-0.1.tar.gz` & `tmp/aissistant-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissistant-0.1.tar", last modified: Fri Aug  4 15:59:35 2023, max compression
+gzip compressed data, was "aissistant-0.2.tar", last modified: Fri Aug  4 23:22:57 2023, max compression
```

## Comparing `aissistant-0.1.tar` & `aissistant-0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-sr-x   0 noteable  (4004) noteable  (4004)        0 2023-08-04 15:59:35.043530 aissistant-0.1/
--rw-r--r--   0 noteable  (4004) noteable  (4004)     6481 2023-08-04 15:59:35.043530 aissistant-0.1/PKG-INFO
--rw-r--r--   0 noteable  (4004) noteable  (4004)     5945 2023-08-04 15:52:32.000000 aissistant-0.1/README.md
-drwxr-sr-x   0 noteable  (4004) noteable  (4004)        0 2023-08-04 15:59:35.043530 aissistant-0.1/aissistant.egg-info/
--rw-r--r--   0 noteable  (4004) noteable  (4004)        0 2023-08-04 15:59:33.000000 aissistant-0.1/aissistant.egg-info/.noteablekeep
--rw-r--r--   0 noteable  (4004) noteable  (4004)     6481 2023-08-04 15:59:35.000000 aissistant-0.1/aissistant.egg-info/PKG-INFO
--rw-r--r--   0 noteable  (4004) noteable  (4004)      258 2023-08-04 15:59:35.000000 aissistant-0.1/aissistant.egg-info/SOURCES.txt
--rw-r--r--   0 noteable  (4004) noteable  (4004)        1 2023-08-04 15:59:35.000000 aissistant-0.1/aissistant.egg-info/dependency_links.txt
--rw-r--r--   0 noteable  (4004) noteable  (4004)       51 2023-08-04 15:59:35.000000 aissistant-0.1/aissistant.egg-info/entry_points.txt
--rw-r--r--   0 noteable  (4004) noteable  (4004)       72 2023-08-04 15:59:35.000000 aissistant-0.1/aissistant.egg-info/requires.txt
--rw-r--r--   0 noteable  (4004) noteable  (4004)        1 2023-08-04 15:59:35.000000 aissistant-0.1/aissistant.egg-info/top_level.txt
--rw-r--r--   0 noteable  (4004) noteable  (4004)       38 2023-08-04 15:59:35.043530 aissistant-0.1/setup.cfg
--rw-r--r--   0 noteable  (4004) noteable  (4004)     1826 2023-08-04 15:52:32.000000 aissistant-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 23:22:57.190468 aissistant-0.2/
+-rw-rw-rw-   0        0        0     1092 2023-08-03 13:17:02.000000 aissistant-0.2/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-08-04 13:30:15.000000 aissistant-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6597 2023-08-04 23:22:57.190468 aissistant-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-08-04 13:30:20.000000 aissistant-0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 23:22:57.182476 aissistant-0.2/aissistant.egg-info/
+-rw-rw-rw-   0        0        0     6597 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 23:22:57.000000 aissistant-0.2/aissistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 23:22:57.190468 aissistant-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     7559 2023-08-04 23:22:28.000000 aissistant-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 23:22:57.190468 aissistant-0.2/tests/
+-rw-rw-rw-   0        0        0      495 2023-08-04 13:33:39.000000 aissistant-0.2/tests/test_aissistant.py
```

### Comparing `aissistant-0.1/PKG-INFO` & `aissistant-0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,119 +1,121 @@
-Metadata-Version: 2.1
-Name: aissistant
-Version: 0.1
-Summary: Aissistant v0.1
-Home-page: https://github.com/markomanninen/aissistant
-Author: Marko Manninen
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-Provides-Extra: cpu
-
-# Aissistant v0.0.1
-
-Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) © 08/2023.
-
-Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
-
-## Start Wizard
-
-To start the chat and initiate the notebook, follow these steps one by one. Confirm each step from the user.
-
-Remember actually to run the cells, not just write them.
-
-Write headings and descriptions of each operation in markdown format to the notebook above executed cells in a human-readable way.
-
-## 1. Noteable Project and Notebook Name
-
-Use the given project or notebook URL from Noteable, or create a new project and notebook. Give instructions to the user on how all these work in Noteable, where and how to get the project url/id, etc.
-
-After creating a new document, add the main heading `1. Aissistant` and description with initialization introduction and GitHub project reference to the markdown cell at the beginning of the document.
-
-## 2. Installation
-
-Add the heading `2. Installation` and description to the notebook document.
-
-### 2.1 Install Required Libraries
-
-Add a heading and description to the markdown cells.
-
-Run the following commands in the notebook cell on behalf of the user:
-
-```
-!pip install -q faiss-cpu
-!pip install -q sentence-transformers
-```
-
-### 2.2 Download Module
-
-Add heading, description, and user decision information to the markdown cells.
-
-If the `aissistant.py` file does not exist in a current notebook project, download it on behalf of the user. Else, ask if the user wants to replace the file. In that case, append the `-O aissistant.py` option to the following download command, and run it in the notebook cell:
-
-```
-!wget https://raw.githubusercontent.com/markomanninen/aissistant/main/aissistant.py
-```
-
-Steps 2.1 and 2.2 will take time to finish, and they are mandatory to be finished before continuing to the next step!
-
-## 2.3 Upload or Create Database and Vector Index Files
-
-Add heading, description, and user decision information to the markdown cells.
-
-Ask the user to upload `conversation.db` and `faiss_index.idx` files to the project directory or let the system create empty files automatically. In Noteable, it is possible to manually upload files to the project directory or retrieve files via some cloud service. Help the user in this procedure. Typically, the user has these files downloaded from the other `aissistant` session.
-
-Note: Empty `.db` and `.idx` files are created automatically when the `aissistant` module is imported and used in the next steps and if data files are unavailable.
-
-## 2.4 Import Module Functions
-
-Add a heading and description to the markdown cells.
-
-Run the following line in the notebook cell on behalf of the user:
-
-```
-from aissistant import search, index, get_profile, set_profile
-```
-
-Then continue to the instructions.
-
-## 3. Instructions
-
-Conversation Vector Database, Personal Profile, and Other Functions
-
-Explain to the user how the following four functions can be used in two different ways:
-
-a) in the chat, by giving natural language triggers
-b) at Noteable notebook cell in a programmable way
-
-### 3.1 Conversation Functions
-
-- Search Conversations: Use `search(query, n=1, start_date=None, end_date=None, all_fields=False)` to find similar conversations from the FAISS index and SQLite database. Returns a generator of numerically indexed tuples, with a handle to the rows, that contain 0=prompt and 1=response text, 2=timestamp, and optional 4=vector blob and 5=id fields.
-- Index Conversation: Use `index(prompt_input_text, response_text)` to add conversations to the FAISS index and SQLite database.
-
-### 3.2 Profile Functions
-
-- Get Profile: Use `get_profile(field_name=None)` to retrieve profile information from the database. Reason the necessity of retrieving user profile information to enhance your responses. Usually, it contains personal contact, employment, education, interests, goals, preferences, research topics, ideological stances, and various other information.
-- Set Profile: Use `set_profile(field_name, value)` to update profile to the database. Reason the necessity of storing and updating fields and values from the user inputs.
-
-### 3.3 Additional Functions
-
-- Retrieve Cursor: Use `retrieve_cursor()` to access the database directly, for example, getting the count of the rows, etc.
-
-## 4. Further Instructions
-
-* Tell the user how to download and use SQLite database (and FAISS index) on the other chat sessions and Noteable projects.
-* Read and output the `aissistant.py` file content in the project on behalf of the user.
-  - Deduce the rest of the functionality from the file header for the user.
-* Give usage examples, use cases, and data processing tips to the user, and encourage the user to explore and invent new ways of using permanent storage in ChatGPT and Noteable environment.
-
-Don't start your responses with "certainly," "surely," "great," or similar expressions. Go straight to the point in all of your future responses. Avoid intro and conclusion sections on responses and any unnecessary repetitions.
-
-Along the way interacting with the user, ChatGPT, and Noteable notebook document, write headings and descriptions of the operations in markdown format to the notebook above each executed cell in a human-readable way.
+Metadata-Version: 2.1
+Name: aissistant
+Version: 0.2
+Summary: Aissistant v0.2
+Home-page: https://github.com/markomanninen/aissistant
+Author: Marko Manninen
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Aissistant v0.2
+
+Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
+
+Copyright © 08/2023.
+
+Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
+
+## Start Wizard
+
+To start the chat and initiate the notebook, follow these steps one by one. Confirm each step from the user.
+
+Remember actually to run the cells, not just write them.
+
+Write headings and descriptions of each operation in markdown format to the notebook above executed cells in a human-readable way.
+
+## 1. Noteable Project and Notebook Name
+
+Use the given project or notebook URL from Noteable, or create a new project and notebook. Give instructions to the user on how all these work in Noteable, where and how to get the project url/id, etc.
+
+After creating a new document, add the main heading `1. Aissistant` and description with initialization introduction and GitHub project reference to the markdown cell at the beginning of the document.
+
+## 2. Installation
+
+Add the heading `2. Installation` and description to the notebook document.
+
+### 2.1 Install Required Libraries
+
+Add a heading and description to the markdown cells.
+
+Run the following commands in the notebook cell on behalf of the user:
+
+```
+!pip install -q faiss-cpu
+!pip install -q sentence-transformers
+```
+
+### 2.2 Download Module
+
+Add heading, description, and user decision information to the markdown cells.
+
+If the `aissistant.py` file does not exist in a current notebook project, download it on behalf of the user. Else, ask if the user wants to replace the file. In that case, append the `-O aissistant.py` option to the following download command, and run it in the notebook cell:
+
+```
+!wget https://raw.githubusercontent.com/markomanninen/aissistant/main/aissistant.py
+```
+
+Steps 2.1 and 2.2 will take time to finish, and they are mandatory to be finished before continuing to the next step!
+
+## 2.3 Upload or Create Database and Vector Index Files
+
+Add heading, description, and user decision information to the markdown cells.
+
+Ask the user to upload `conversation.db` and `faiss_index.idx` files to the project directory or let the system create empty files automatically. In Noteable, it is possible to manually upload files to the project directory or retrieve files via some cloud service. Help the user in this procedure. Typically, the user has these files downloaded from the other `aissistant` session.
+
+Note: Empty `.db` and `.idx` files are created automatically when the `aissistant` module is imported and used in the next steps and if data files are unavailable.
+
+## 2.4 Import Module Functions
+
+Add a heading and description to the markdown cells.
+
+Run the following line in the notebook cell on behalf of the user:
+
+```
+from aissistant import search, index, get_profile, set_profile
+```
+
+Then continue to the instructions.
+
+## 3. Instructions
+
+Conversation Vector Database, Personal Profile, and Other Functions
+
+Explain to the user how the following four functions can be used in two different ways:
+
+a) in the chat, by giving natural language triggers
+b) at Noteable notebook cell in a programmable way
+
+### 3.1 Conversation Functions
+
+- Search Conversations: Use `search(query, n=1, start_date=None, end_date=None, all_fields=False)` to find similar conversations from the FAISS index and SQLite database. Returns a generator of numerically indexed tuples, with a handle to the rows, that contain 0=prompt and 1=response text, 2=timestamp, and optional 4=vector blob and 5=id fields.
+- Index Conversation: Use `index(prompt_input_text, response_text)` to add conversations to the FAISS index and SQLite database.
+
+### 3.2 Profile Functions
+
+- Get Profile: Use `get_profile(field_name=None)` to retrieve profile information from the database. Reason the necessity of retrieving user profile information to enhance your responses. Usually, it contains personal contact, employment, education, interests, goals, preferences, research topics, ideological stances, and various other information.
+- Set Profile: Use `set_profile(field_name, value)` to update profile to the database. Reason the necessity of storing and updating fields and values from the user inputs.
+
+### 3.3 Additional Functions
+
+- Retrieve Cursor: Use `retrieve_cursor()` to access the database directly, for example, getting the count of the rows, etc.
+
+## 4. Further Instructions
+
+* Tell the user how to download and use SQLite database (and FAISS index) on the other chat sessions and Noteable projects.
+* Read and output the `aissistant.py` file content in the project on behalf of the user.
+  - Deduce the rest of the functionality from the file header for the user.
+* Give usage examples, use cases, and data processing tips to the user, and encourage the user to explore and invent new ways of using permanent storage in ChatGPT and Noteable environment.
+
+Don't start your responses with "certainly," "surely," "great," or similar expressions. Go straight to the point in all of your future responses. Avoid intro and conclusion sections on responses and any unnecessary repetitions.
+
+Along the way interacting with the user, ChatGPT, and Noteable notebook document, write headings and descriptions of the operations in markdown format to the notebook above each executed cell in a human-readable way.
```

### Comparing `aissistant-0.1/README.md` & `aissistant-0.2/aissistant.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,31 @@
-# Aissistant v0.0.1
+Metadata-Version: 2.1
+Name: aissistant
+Version: 0.2
+Summary: Aissistant v0.2
+Home-page: https://github.com/markomanninen/aissistant
+Author: Marko Manninen
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) © 08/2023.
+
+# Aissistant v0.2
+
+Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
+
+Copyright © 08/2023.
 
 Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
 
 ## Start Wizard
 
 To start the chat and initiate the notebook, follow these steps one by one. Confirm each step from the user.
```

