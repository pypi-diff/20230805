# Comparing `tmp/gpt4all-code-review-0.14.tar.gz` & `tmp/gpt4all-code-review-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-code-review-0.14.tar", last modified: Sat Aug  5 16:00:16 2023, max compression
+gzip compressed data, was "gpt4all-code-review-0.15.tar", last modified: Sat Aug  5 16:19:03 2023, max compression
```

## Comparing `gpt4all-code-review-0.14.tar` & `gpt4all-code-review-0.15.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:00:16.499568 gpt4all-code-review-0.14/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2675 2023-08-05 16:00:16.497584 gpt4all-code-review-0.14/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2458 2023-08-05 16:00:14.000000 gpt4all-code-review-0.14/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:00:16.496371 gpt4all-code-review-0.14/gpt4all_code_review/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.14/gpt4all_code_review/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6122 2023-08-05 15:51:52.000000 gpt4all-code-review-0.14/gpt4all_code_review/gpt4all_code_review.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:00:16.497392 gpt4all-code-review-0.14/gpt4all_code_review.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2675 2023-08-05 16:00:16.000000 gpt4all-code-review-0.14/gpt4all_code_review.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-05 16:00:16.000000 gpt4all-code-review-0.14/gpt4all_code_review.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 16:00:16.000000 gpt4all-code-review-0.14/gpt4all_code_review.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-05 16:00:16.000000 gpt4all-code-review-0.14/gpt4all_code_review.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 16:00:16.000000 gpt4all-code-review-0.14/gpt4all_code_review.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 16:00:16.000000 gpt4all-code-review-0.14/gpt4all_code_review.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 16:00:16.499651 gpt4all-code-review-0.14/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      661 2023-08-05 16:00:14.000000 gpt4all-code-review-0.14/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:19:03.302572 gpt4all-code-review-0.15/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2734 2023-08-05 16:19:03.302427 gpt4all-code-review-0.15/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2458 2023-08-05 16:00:14.000000 gpt4all-code-review-0.15/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:19:03.301264 gpt4all-code-review-0.15/gpt4all_code_review/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.15/gpt4all_code_review/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6235 2023-08-05 16:06:49.000000 gpt4all-code-review-0.15/gpt4all_code_review/gpt4all_code_review.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:19:03.302234 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2734 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 16:19:03.302609 gpt4all-code-review-0.15/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      720 2023-08-05 16:12:30.000000 gpt4all-code-review-0.15/setup.py
```

### Comparing `gpt4all-code-review-0.14/PKG-INFO` & `gpt4all-code-review-0.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.14
+Version: 0.15
 Summary: A standalone code review tool based on GPT4ALL.
+Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 # Code Review Automation Tool
 
 This program is designed to assist developers by automating the process of code review. By leveraging a pre-trained standalone machine learning model (e.g., GPT-4), it reads source code files and provides suggestions for improvements.
```

### Comparing `gpt4all-code-review-0.14/README.md` & `gpt4all-code-review-0.15/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-code-review-0.14/gpt4all_code_review/gpt4all_code_review.py` & `gpt4all-code-review-0.15/gpt4all_code_review/gpt4all_code_review.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,17 @@
 
                     with model.chat_session(system_template):
                         response = model.generate(prompt=prompt, temp=0, max_tokens=1000)
                         current_progress_chunks = chunk_number / total_chunks * 100
                         suggestion = response.lstrip().replace("Sure", "").replace("Sure, ", "").replace("!", "")
                         suggestions.append(suggestion)
                 pb_chunks.print_progress_bar(100)
-                combined_suggestion = "\n".join(suggestions)
+                combined_suggestion = ""
+                for i in range(len(suggestions)):
+                    combined_suggestion += str(i+1) + ". " + suggestions[i] + "\n"
                 current_progress_files = current_file / total_files * 100
                 pb_files.print_progress_bar(current_progress_files)
                 results.append([file_path.replace(os.getcwd(), ""), combined_suggestion])
 
         except Exception as e:
             print(e)
```

### Comparing `gpt4all-code-review-0.14/gpt4all_code_review.egg-info/PKG-INFO` & `gpt4all-code-review-0.15/gpt4all_code_review.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.14
+Version: 0.15
 Summary: A standalone code review tool based on GPT4ALL.
+Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 # Code Review Automation Tool
 
 This program is designed to assist developers by automating the process of code review. By leveraging a pre-trained standalone machine learning model (e.g., GPT-4), it reads source code files and provides suggestions for improvements.
```

### Comparing `gpt4all-code-review-0.14/setup.py` & `gpt4all-code-review-0.15/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpt4all-code-review',
-    version='0.14',
+    version='0.15',
     packages=find_packages(),
     install_requires=[
         "argparse",
         "gpt4all",
         "prettytable",
         "datetime",
         "console_progressbar",
     ],
     author='Evgenii Evstafev',
     author_email='chigwel@gmail.com',
     description='A standalone code review tool based on GPT4ALL.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
+    url='https://github.com/chigwell/gpt4all-code-review',
     entry_points={
         'console_scripts': [
             'gpt4all_code_review = gpt4all_code_review.gpt4all_code_review:main',
         ],
     },
 )
```

