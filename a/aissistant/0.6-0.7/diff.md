# Comparing `tmp/aissistant-0.6.tar.gz` & `tmp/aissistant-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissistant-0.6.tar", last modified: Sat Aug  5 00:26:10 2023, max compression
+gzip compressed data, was "aissistant-0.7.tar", last modified: Sat Aug  5 00:56:06 2023, max compression
```

## Comparing `aissistant-0.6.tar` & `aissistant-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 00:26:10.101442 aissistant-0.6/
--rw-rw-rw-   0        0        0     1092 2023-08-03 13:17:02.000000 aissistant-0.6/LICENSE
--rw-rw-rw-   0        0        0       57 2023-08-04 13:30:15.000000 aissistant-0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6639 2023-08-05 00:26:10.093438 aissistant-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-08-04 13:30:20.000000 aissistant-0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-05 00:26:10.077437 aissistant-0.6/aissistant/
--rw-rw-rw-   0        0        0      190 2023-08-05 00:17:15.000000 aissistant-0.6/aissistant/__init__.py
--rw-rw-rw-   0        0        0    23781 2023-08-05 00:24:44.000000 aissistant-0.6/aissistant/aissistant.py
-drwxrwxrwx   0        0        0        0 2023-08-05 00:26:10.093438 aissistant-0.6/aissistant.egg-info/
--rw-rw-rw-   0        0        0     6639 2023-08-05 00:26:09.000000 aissistant-0.6/aissistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-08-05 00:26:10.000000 aissistant-0.6/aissistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 00:26:09.000000 aissistant-0.6/aissistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-08-05 00:26:09.000000 aissistant-0.6/aissistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-08-05 00:26:09.000000 aissistant-0.6/aissistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-05 00:26:09.000000 aissistant-0.6/aissistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 00:26:10.101442 aissistant-0.6/setup.cfg
--rw-rw-rw-   0        0        0     7642 2023-08-05 00:24:52.000000 aissistant-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 00:26:10.093438 aissistant-0.6/tests/
--rw-rw-rw-   0        0        0      495 2023-08-04 13:33:39.000000 aissistant-0.6/tests/test_aissistant.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:56:06.140334 aissistant-0.7/
+-rw-rw-rw-   0        0        0     1092 2023-08-03 13:17:02.000000 aissistant-0.7/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-08-04 13:30:15.000000 aissistant-0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6639 2023-08-05 00:56:06.140334 aissistant-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-08-04 13:30:20.000000 aissistant-0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-05 00:56:06.125334 aissistant-0.7/aissistant/
+-rw-rw-rw-   0        0        0      190 2023-08-05 00:17:15.000000 aissistant-0.7/aissistant/__init__.py
+-rw-rw-rw-   0        0        0    23706 2023-08-05 00:52:53.000000 aissistant-0.7/aissistant/aissistant.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:56:06.135331 aissistant-0.7/aissistant.egg-info/
+-rw-rw-rw-   0        0        0     6639 2023-08-05 00:56:06.000000 aissistant-0.7/aissistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-08-05 00:56:06.000000 aissistant-0.7/aissistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 00:56:06.000000 aissistant-0.7/aissistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-08-05 00:56:06.000000 aissistant-0.7/aissistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-08-05 00:56:06.000000 aissistant-0.7/aissistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-05 00:56:06.000000 aissistant-0.7/aissistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 00:56:06.140334 aissistant-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     7642 2023-08-05 00:53:40.000000 aissistant-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:56:06.138331 aissistant-0.7/tests/
+-rw-rw-rw-   0        0        0      495 2023-08-04 13:33:39.000000 aissistant-0.7/tests/test_aissistant.py
```

### Comparing `aissistant-0.6/LICENSE` & `aissistant-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aissistant-0.6/PKG-INFO` & `aissistant-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aissistant
-Version: 0.6
-Summary: Aissistant v0.6
+Version: 0.7
+Summary: Aissistant v0.7
 Home-page: https://github.com/markomanninen/aissistant
 Author: Marko Manninen
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 Provides-Extra: cpu
 License-File: LICENSE
 
 
-# Aissistant v0.6
+# Aissistant v0.7
 
 Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
 
 Copyright © 08/2023.
 
 Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
```

### Comparing `aissistant-0.6/README.rst` & `aissistant-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aissistant-0.6/aissistant/aissistant.py` & `aissistant-0.7/aissistant/aissistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         output_text (str): The output text (response) of the conversation.
 
     Returns:
         bool: True if the operation is successful, False if any error occurs.
     """
     try:
         # Convert the conversation to a vector
-        conversation_vector = model.encode([input_text + ' ' + output_text], show_progress_bar=False)[0]
+        conversation_vector = model.encode([input_text + ' ' + output_text])[0]
 
         # Get the current timestamp
         timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
         # Ensure that the connection is established
         ensure_connection()
 
@@ -379,15 +379,15 @@
             print(result)
     """
     return search_conversation_with_date_filter_and_n_results(query, n=n, start_date=start_date, end_date=end_date, all_fields=all_fields)
 
 def search_conversation_with_date_filter_and_n_results(query: str, n: int = 1, start_date: str = None, end_date: str = None, all_fields: bool = False) -> Generator[Union[Tuple[str, str, str], Tuple[str, str, str, bytes, int]], None, None]:
     try:
         # Convert the query to a vector
-        query_vector = model.encode([query], show_progress_bar=False)
+        query_vector = model.encode([query])
 
         # Perform a search in the FAISS index for the top n matches
         D, I = faiss_index.search(np.array(query_vector).astype('float32'), k=n)
 
         sql_select = 'input, output, timestamp'
         if all_fields:
             sql_select = 'input, output, timestamp, vector, id'
@@ -440,15 +440,15 @@
 
     try:
         # Ensure that the connection is established
         ensure_connection()
 
         # Add the sample conversations to the database and FAISS index
         for input_text, output_text, timestamp in sample_conversations:
-            conversation_vector = model.encode([input_text + ' ' + output_text], show_progress_bar=False)[0]
+            conversation_vector = model.encode([input_text + ' ' + output_text])[0]
             query = f'INSERT INTO {CONVERSATIONS_TABLE} (input, output, vector, timestamp) VALUES (?, ?, ?, ?)'
             c.execute(query, (input_text, output_text, conversation_vector.tobytes(), timestamp))
             faiss_index.add(np.array([conversation_vector]))
             conn.commit()
 
         # Save the FAISS index to a file
         faiss.write_index(faiss_index, FAISS_INDEX_FILE)
```

### Comparing `aissistant-0.6/aissistant.egg-info/PKG-INFO` & `aissistant-0.7/aissistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aissistant
-Version: 0.6
-Summary: Aissistant v0.6
+Version: 0.7
+Summary: Aissistant v0.7
 Home-page: https://github.com/markomanninen/aissistant
 Author: Marko Manninen
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 Provides-Extra: cpu
 License-File: LICENSE
 
 
-# Aissistant v0.6
+# Aissistant v0.7
 
 Initialization prompt for persistent conversation vector database and personal profile in ChatGPT using Noteable plugin and `aissistant` module written by Marko T. Manninen ([https://github.com/markomanninen/aissistant/](https://github.com/markomanninen/aissistant/)) ©
 
 Copyright © 08/2023.
 
 Get creative and productive with this initialization script in ChatGPT that utilizes the Noteable plugin. Natively, you can create, edit, and run code and generate data within notebooks as well as in ChatGPT interchangeably, back and forth. By using this initialization prompt, you can use the combined environment to store data and explore past conversations, as well as manage profile information for a more intelligent chat and coding experience.
```

### Comparing `aissistant-0.6/setup.py` & `aissistant-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
-version = 0.6
+version = 0.7
 
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         print("\n\nWelcome to aissistant!")
         print("For usage tips and help, you can call `help(aissistant)` or access `aissistant.__doc__`, and `dir(aissistant)` to see the functions and `help(any_function)` after importing the module.")
         print("\nEnjoy!\n")
```

