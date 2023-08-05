# Comparing `tmp/gpt4all-code-review-0.12.tar.gz` & `tmp/gpt4all-code-review-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-code-review-0.12.tar", last modified: Sat Aug  5 15:47:43 2023, max compression
+gzip compressed data, was "gpt4all-code-review-0.13.tar", last modified: Sat Aug  5 15:56:53 2023, max compression
```

## Comparing `gpt4all-code-review-0.12.tar` & `gpt4all-code-review-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:47:43.790248 gpt4all-code-review-0.12/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      216 2023-08-05 15:47:43.790062 gpt4all-code-review-0.12/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:34:29.000000 gpt4all-code-review-0.12/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:47:43.788499 gpt4all-code-review-0.12/gpt4all_code_review/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.12/gpt4all_code_review/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6084 2023-08-05 15:35:12.000000 gpt4all-code-review-0.12/gpt4all_code_review/gpt4all_code_review.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:47:43.789839 gpt4all-code-review-0.12/gpt4all_code_review.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      216 2023-08-05 15:47:43.000000 gpt4all-code-review-0.12/gpt4all_code_review.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-05 15:47:43.000000 gpt4all-code-review-0.12/gpt4all_code_review.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 15:47:43.000000 gpt4all-code-review-0.12/gpt4all_code_review.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-05 15:47:43.000000 gpt4all-code-review-0.12/gpt4all_code_review.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 15:47:43.000000 gpt4all-code-review-0.12/gpt4all_code_review.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 15:47:43.000000 gpt4all-code-review-0.12/gpt4all_code_review.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 15:47:43.790289 gpt4all-code-review-0.12/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      661 2023-08-05 15:47:30.000000 gpt4all-code-review-0.12/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:56:53.444277 gpt4all-code-review-0.13/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2209 2023-08-05 15:56:53.444132 gpt4all-code-review-0.13/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1992 2023-08-05 15:56:45.000000 gpt4all-code-review-0.13/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:56:53.442823 gpt4all-code-review-0.13/gpt4all_code_review/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.13/gpt4all_code_review/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6122 2023-08-05 15:51:52.000000 gpt4all-code-review-0.13/gpt4all_code_review/gpt4all_code_review.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:56:53.443950 gpt4all-code-review-0.13/gpt4all_code_review.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2209 2023-08-05 15:56:53.000000 gpt4all-code-review-0.13/gpt4all_code_review.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-05 15:56:53.000000 gpt4all-code-review-0.13/gpt4all_code_review.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 15:56:53.000000 gpt4all-code-review-0.13/gpt4all_code_review.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-05 15:56:53.000000 gpt4all-code-review-0.13/gpt4all_code_review.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 15:56:53.000000 gpt4all-code-review-0.13/gpt4all_code_review.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 15:56:53.000000 gpt4all-code-review-0.13/gpt4all_code_review.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 15:56:53.444314 gpt4all-code-review-0.13/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      661 2023-08-05 15:51:52.000000 gpt4all-code-review-0.13/setup.py
```

### Comparing `gpt4all-code-review-0.12/gpt4all_code_review/gpt4all_code_review.py` & `gpt4all-code-review-0.13/gpt4all_code_review/gpt4all_code_review.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from console_progressbar import ProgressBar
 
 
 def main():
     parser = argparse.ArgumentParser(description="check.py")
     parser.add_argument(
         "--model",
-        help="model name",
+        help="Model name",
         default="orca-mini-3b.ggmlv3.q4_0.bin"
     )
     parser.add_argument(
         "--file",
-        help="file path to analyze"
+        help="File path to analyze"
     )
     parser.add_argument(
         "--all",
-        help="include all files and folders",
+        help="Include all files and folders",
         action='store_true'
     )
     parser.add_argument(
         "--output",
-        help="output type",
+        help="Output type",
         default="text"
     )
     parser.add_argument(
         "--export",
-        help="export to file"
+        help="Export to file"
     )
     parser.add_argument(
         "--export-folder",
-        help="export to folder"
+        help="Export to folder"
     )
 
     args = parser.parse_args()
     model_name = args.model
     scan_all = args.all
     output_type = args.output
     export = args.export
@@ -134,15 +134,15 @@
                     pb_chunks.print_progress_bar(current_progress_chunks)
                     print("     chunk number:", chunk_number)
                     prompt = f"The file '{file_name}' (chunk '{str(chunk_number)}') contains: {chunk}. Could you give some recommendations for improving the code? and sorting suggestions list by priority from hight to low"
 
                     with model.chat_session(system_template):
                         response = model.generate(prompt=prompt, temp=0, max_tokens=1000)
                         current_progress_chunks = chunk_number / total_chunks * 100
-                        suggestion = response.lstrip().replace("Sure!", "")
+                        suggestion = response.lstrip().replace("Sure", "").replace("Sure, ", "").replace("!", "")
                         suggestions.append(suggestion)
                 pb_chunks.print_progress_bar(100)
                 combined_suggestion = "\n".join(suggestions)
                 current_progress_files = current_file / total_files * 100
                 pb_files.print_progress_bar(current_progress_files)
                 results.append([file_path.replace(os.getcwd(), ""), combined_suggestion])
```

### Comparing `gpt4all-code-review-0.12/setup.py` & `gpt4all-code-review-0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpt4all-code-review',
-    version='0.12',
+    version='0.13',
     packages=find_packages(),
     install_requires=[
         "argparse",
         "gpt4all",
         "prettytable",
         "datetime",
         "console_progressbar",
```

