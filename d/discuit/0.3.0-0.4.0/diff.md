# Comparing `tmp/discuit-0.3.0.tar.gz` & `tmp/discuit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discuit-0.3.0.tar", last modified: Tue Aug  1 11:21:38 2023, max compression
+gzip compressed data, was "discuit-0.4.0.tar", last modified: Sat Aug  5 10:47:35 2023, max compression
```

## Comparing `discuit-0.3.0.tar` & `discuit-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.742740 discuit-0.3.0/
--rw-r--r--   0 doerte     (501) staff       (20)      454 2023-08-01 07:36:22.000000 discuit-0.3.0/CITATION.cff
--rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.3.0/LICENSE
--rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.3.0/MANIFEST.in
--rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.3.0/NOTICE
--rw-r--r--   0 doerte     (501) staff       (20)     7706 2023-08-01 11:21:38.742824 discuit-0.3.0/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)     6624 2023-07-31 18:59:36.000000 discuit-0.3.0/README.md
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.741088 discuit-0.3.0/discuit/
--rw-r--r--   0 doerte     (501) staff       (20)      206 2023-07-31 18:15:19.000000 discuit-0.3.0/discuit/__init__.py
--rw-r--r--   0 doerte     (501) staff       (20)     1909 2023-08-01 07:39:44.000000 discuit-0.3.0/discuit/calculations.py
--rw-r--r--   0 doerte     (501) staff       (20)     4681 2023-08-01 07:28:02.000000 discuit-0.3.0/discuit/clustering.py
--rw-r--r--   0 doerte     (501) staff       (20)     6125 2023-08-01 07:39:44.000000 discuit-0.3.0/discuit/command_line.py
--rw-r--r--   0 doerte     (501) staff       (20)     2494 2023-08-01 07:45:08.000000 discuit-0.3.0/discuit/run.py
--rw-r--r--   0 doerte     (501) staff       (20)     2991 2023-08-01 07:34:05.000000 discuit-0.3.0/discuit/write.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.742213 discuit-0.3.0/discuit.egg-info/
--rw-r--r--   0 doerte     (501) staff       (20)     7706 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)      465 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/SOURCES.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/dependency_links.txt
--rw-r--r--   0 doerte     (501) staff       (20)       54 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/entry_points.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.3.0/discuit.egg-info/not-zip-safe
--rw-r--r--   0 doerte     (501) staff       (20)      276 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/requires.txt
--rw-r--r--   0 doerte     (501) staff       (20)       14 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/top_level.txt
--rw-r--r--   0 doerte     (501) staff       (20)      376 2023-02-25 18:49:41.000000 discuit-0.3.0/pyproject.toml
--rw-r--r--   0 doerte     (501) staff       (20)     1977 2023-08-01 11:21:38.743246 discuit-0.3.0/setup.cfg
--rw-r--r--   0 doerte     (501) staff       (20)      206 2023-08-01 11:21:30.000000 discuit-0.3.0/setup.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.742457 discuit-0.3.0/tests/
--rw-r--r--   0 doerte     (501) staff       (20)        0 2023-02-15 15:09:44.000000 discuit-0.3.0/tests/__init__.py
--rw-r--r--   0 doerte     (501) staff       (20)      343 2023-08-01 07:45:59.000000 discuit-0.3.0/tests/test_my_module.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-05 10:47:35.588274 discuit-0.4.0/
+-rw-r--r--   0 doerte     (501) staff       (20)      454 2023-08-05 10:38:12.000000 discuit-0.4.0/CITATION.cff
+-rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.4.0/LICENSE
+-rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.4.0/MANIFEST.in
+-rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.4.0/NOTICE
+-rw-r--r--   0 doerte     (501) staff       (20)     7706 2023-08-05 10:47:35.588354 discuit-0.4.0/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)     6624 2023-07-31 18:59:36.000000 discuit-0.4.0/README.md
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-05 10:47:35.586989 discuit-0.4.0/discuit/
+-rw-r--r--   0 doerte     (501) staff       (20)      241 2023-08-05 10:32:12.000000 discuit-0.4.0/discuit/__init__.py
+-rw-r--r--   0 doerte     (501) staff       (20)     1909 2023-08-01 07:39:44.000000 discuit-0.4.0/discuit/calculations.py
+-rw-r--r--   0 doerte     (501) staff       (20)     4681 2023-08-01 07:28:02.000000 discuit-0.4.0/discuit/clustering.py
+-rw-r--r--   0 doerte     (501) staff       (20)     6223 2023-08-04 19:01:17.000000 discuit-0.4.0/discuit/command_line.py
+-rw-r--r--   0 doerte     (501) staff       (20)      733 2023-08-05 10:45:29.000000 discuit-0.4.0/discuit/data.py
+-rw-r--r--   0 doerte     (501) staff       (20)     2563 2023-08-05 10:46:06.000000 discuit-0.4.0/discuit/run.py
+-rw-r--r--   0 doerte     (501) staff       (20)     3282 2023-08-05 10:12:43.000000 discuit-0.4.0/discuit/save_stats.py
+-rw-r--r--   0 doerte     (501) staff       (20)     1449 2023-08-04 19:25:22.000000 discuit-0.4.0/discuit/write.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-05 10:47:35.587969 discuit-0.4.0/discuit.egg-info/
+-rw-r--r--   0 doerte     (501) staff       (20)     7706 2023-08-05 10:47:35.000000 discuit-0.4.0/discuit.egg-info/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)      503 2023-08-05 10:47:35.000000 discuit-0.4.0/discuit.egg-info/SOURCES.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-08-05 10:47:35.000000 discuit-0.4.0/discuit.egg-info/dependency_links.txt
+-rw-r--r--   0 doerte     (501) staff       (20)       54 2023-08-05 10:47:35.000000 discuit-0.4.0/discuit.egg-info/entry_points.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.4.0/discuit.egg-info/not-zip-safe
+-rw-r--r--   0 doerte     (501) staff       (20)      276 2023-08-05 10:47:35.000000 discuit-0.4.0/discuit.egg-info/requires.txt
+-rw-r--r--   0 doerte     (501) staff       (20)       14 2023-08-05 10:47:35.000000 discuit-0.4.0/discuit.egg-info/top_level.txt
+-rw-r--r--   0 doerte     (501) staff       (20)      414 2023-08-02 18:41:56.000000 discuit-0.4.0/pyproject.toml
+-rw-r--r--   0 doerte     (501) staff       (20)     1977 2023-08-05 10:47:35.588758 discuit-0.4.0/setup.cfg
+-rw-r--r--   0 doerte     (501) staff       (20)      206 2023-08-01 11:21:30.000000 discuit-0.4.0/setup.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-05 10:47:35.588175 discuit-0.4.0/tests/
+-rw-r--r--   0 doerte     (501) staff       (20)        0 2023-02-15 15:09:44.000000 discuit-0.4.0/tests/__init__.py
+-rw-r--r--   0 doerte     (501) staff       (20)      343 2023-08-01 07:45:59.000000 discuit-0.4.0/tests/test_my_module.py
```

### Comparing `discuit-0.3.0/LICENSE` & `discuit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discuit-0.3.0/PKG-INFO` & `discuit-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discuit-0.3.0/README.md` & `discuit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `discuit-0.3.0/discuit/calculations.py` & `discuit-0.4.0/discuit/calculations.py`

 * *Files identical despite different names*

### Comparing `discuit-0.3.0/discuit/clustering.py` & `discuit-0.4.0/discuit/clustering.py`

 * *Files identical despite different names*

### Comparing `discuit-0.3.0/discuit/command_line.py` & `discuit-0.4.0/discuit/command_line.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 # TODO: consider stopping if silhouette score is too low. Exit with error message.
 # TODO: guess variable type
 
 import argparse
 import pathlib
 import sys
 import pandas as pd
+from .data import Output
 from .run import run_all
+from .write import write_to_file
 
 
-# set defaults
-iterations = 1
-no_sets = 2
-filename = "placeholder"
-input_d = pd.DataFrame()
+final_output = Output(runs=[])
 
-
-# The following info must come from user. In GUI this should be selected in the GUI after opening a file!
+# The following info must come from user.
 categorical_features = []
 continuous_features = []
 absolute_features = []
 label = []
 disregard = []
 
 # check whether path and number of sets arguments were provided
@@ -60,16 +57,19 @@
         print("Parse error")
         sys.exit(1)  # abort
     except Exception:
         print("Something else went wrong. \n "
               "Make sure your input looks as follows: \n"
               "'model.py [path to csv file] [number of sets].'")
         sys.exit(1)  # abort
-    # number of runs provided as an argument. If nothing is provided it's 1. Also needs to come from GUI!
-    iterations = args.runs
+    # number of runs provided as an argument. If nothing is provided it's 1.
+    if args.runs is None:
+        iterations = 1
+    else:
+        iterations = args.runs
 
     # Check all the columns and ask about status. Label and absolute can only be chosen once.
     if args.columns is None or len(args.columns) != len(input_d.columns):  # noqa: MC0001
         print("You didn't provide valid data type indications when running the program. Please specify them now")
         for column in input_d.columns:
             feature = None
             while feature is None:
@@ -116,30 +116,34 @@
             print("More than one 'label' was specified. Please use -h to get help in providing suitable arguments")
             sys.exit(1)  # abort
         if len(absolute_features) > 1:
             print(
                 "More than one 'absolute' variable was specified. Please use -h to get help in "
                 "providing suitable arguments")
             sys.exit(1)  # abort
-    # actually run the program
 
+    # actually run the program
     for it_num in range(iterations):
         # progress bar
         perc = 20 // iterations
         progress = '=' * it_num * perc
         percdone = round(it_num / iterations * 100, None)
         sys.stdout.write('\r')
         sys.stdout.write(f"[{progress:20}] {percdone}%")
         sys.stdout.flush()
 
         # initiate loop-tracking
         i = 0
         # start first loop
-        run_all(i, it_num, no_sets, input_d, continuous_features, categorical_features, label, disregard,
-                absolute_features, filename)
+        output_run = run_all(i, it_num, no_sets, input_d, continuous_features, categorical_features, label, disregard,
+                             absolute_features, filename)
+        final_output.runs.append(output_run)
+
+    # write results to file
+    write_to_file(final_output)
 
     # final progress bar
     sys.stdout.write('\r')
     sys.stdout.write(f"[{'=' * 20:20}] 100%\n")
     sys.stdout.flush()
```

### Comparing `discuit-0.3.0/discuit/run.py` & `discuit-0.4.0/discuit/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import sys
 from .calculations import do_statistics
 from .clustering import clustering
 from .clustering import divide_in_sets
 from .clustering import prepare_data
 from .clustering import split
-from .write import write_out
+from .save_stats import to_dataclass
 
 
 def run_all(i, it_num, no_sets, input_d, continuous_features, categorical_features, label, disregard,
             absolute_features, filename):
     output_sets = []
     for _ in range(0, no_sets):
         output_sets.append([])
@@ -55,18 +55,20 @@
     for var_type in stats:
         for var in var_type:
             if var[5] < 0.2:
                 all_ns = False
 
     # write to files
     if all_ns:
-        write_out(stats, i, False, it_num, filename, input_d, no_sets, absolute_features, categorical_features,
-                  continuous_features)
-    elif i < 19:
+        output = to_dataclass(stats, i, False, it_num, filename, input_d, no_sets, absolute_features,
+                              categorical_features, continuous_features)
+        return output
+    if i < 19:
         i = i + 1
         run_all(i, it_num, no_sets, input_d, continuous_features, categorical_features, label, disregard,
                 absolute_features, filename)
-    else:
-        print("\nCouldn't split into sets as expected. The output might be less than optimal, please run again for "
-              "better results")
-        write_out(stats, i, True, it_num, filename, input_d, no_sets, absolute_features, categorical_features,
-                  continuous_features)
+
+    print("\nCouldn't split into sets as expected. The output might be less than optimal, please run again for "
+          "better results")
+    output = to_dataclass(stats, i, True, it_num, filename, input_d, no_sets, absolute_features,
+                          categorical_features, continuous_features)
+    return output
```

### Comparing `discuit-0.3.0/discuit.egg-info/PKG-INFO` & `discuit-0.4.0/discuit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discuit-0.3.0/setup.cfg` & `discuit-0.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 keywords = clustering
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = discuit
 project_urls = 
 	Bug Tracker = https://github.com/doerte/discuit-project/issues
 url = https://github.com/doerte/discuit-project
-version = 0.3.0
+version = 0.4.0
 
 [options]
 zip_safe = False
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires =
```

