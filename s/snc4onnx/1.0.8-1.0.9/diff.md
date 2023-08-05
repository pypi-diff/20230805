# Comparing `tmp/snc4onnx-1.0.8.tar.gz` & `tmp/snc4onnx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snc4onnx-1.0.8.tar", last modified: Tue Sep  6 02:02:32 2022, max compression
+gzip compressed data, was "snc4onnx-1.0.9.tar", last modified: Wed Sep  7 11:20:48 2022, max compression
```

## Comparing `snc4onnx-1.0.8.tar` & `snc4onnx-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 02:02:32.302802 snc4onnx-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-06 02:02:25.000000 snc4onnx-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10335 2022-09-06 02:02:32.302802 snc4onnx-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9956 2022-09-06 02:02:25.000000 snc4onnx-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 02:02:32.302802 snc4onnx-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-09-06 02:02:25.000000 snc4onnx-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 02:02:32.298802 snc4onnx-1.0.8/snc4onnx/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-06 02:02:25.000000 snc4onnx-1.0.8/snc4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-06 02:02:25.000000 snc4onnx-1.0.8/snc4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21344 2022-09-06 02:02:25.000000 snc4onnx-1.0.8/snc4onnx/onnx_network_combine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 02:02:32.298802 snc4onnx-1.0.8/snc4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10335 2022-09-06 02:02:32.000000 snc4onnx-1.0.8/snc4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-06 02:02:32.000000 snc4onnx-1.0.8/snc4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 02:02:32.000000 snc4onnx-1.0.8/snc4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-06 02:02:32.000000 snc4onnx-1.0.8/snc4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-06 02:02:32.000000 snc4onnx-1.0.8/snc4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 11:20:48.821158 snc4onnx-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-07 11:20:34.000000 snc4onnx-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10460 2022-09-07 11:20:48.821158 snc4onnx-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10081 2022-09-07 11:20:34.000000 snc4onnx-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-07 11:20:48.821158 snc4onnx-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-09-07 11:20:35.000000 snc4onnx-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 11:20:48.821158 snc4onnx-1.0.9/snc4onnx/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-07 11:20:35.000000 snc4onnx-1.0.9/snc4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-07 11:20:35.000000 snc4onnx-1.0.9/snc4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21434 2022-09-07 11:20:35.000000 snc4onnx-1.0.9/snc4onnx/onnx_network_combine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 11:20:48.821158 snc4onnx-1.0.9/snc4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10460 2022-09-07 11:20:48.000000 snc4onnx-1.0.9/snc4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-07 11:20:48.000000 snc4onnx-1.0.9/snc4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 11:20:48.000000 snc4onnx-1.0.9/snc4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-07 11:20:48.000000 snc4onnx-1.0.9/snc4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-07 11:20:48.000000 snc4onnx-1.0.9/snc4onnx.egg-info/top_level.txt
```

### Comparing `snc4onnx-1.0.8/LICENSE` & `snc4onnx-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snc4onnx-1.0.8/PKG-INFO` & `snc4onnx-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: snc4onnx
-Version: 1.0.8
-Summary: Simple tool to combine onnx models. Simple Network Combine Tool for ONNX.
-Home-page: https://github.com/PINTO0309/sne4onnx
-Author: Katsuya Hyodo
-Author-email: rmsdh122@yahoo.co.jp
-License: MIT License
-Platform: linux
-Platform: unix
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # snc4onnx
 Simple tool to combine(merge) onnx models. **S**imple **N**etwork **C**ombine Tool for **ONNX**.
 
 https://github.com/PINTO0309/simple-onnx-processing-tools
 
 [![Downloads](https://static.pepy.tech/personalized-badge/snc4onnx?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/snc4onnx) ![GitHub](https://img.shields.io/github/license/PINTO0309/snc4onnx?color=2BAF2B) [![PyPI](https://img.shields.io/pypi/v/snc4onnx?color=2BAF2B)](https://pypi.org/project/snc4onnx/) [![CodeQL](https://github.com/PINTO0309/snc4onnx/workflows/CodeQL/badge.svg)](https://github.com/PINTO0309/snc4onnx/actions?query=workflow%3ACodeQL)
 
@@ -37,62 +23,64 @@
 && python3 -m pip install -U onnx_graphsurgeon --index-url https://pypi.ngc.nvidia.com \
 && pip install -U snc4onnx
 ```
 ### 1-2. Docker
 https://github.com/PINTO0309/simple-onnx-processing-tools#docker
 
 ## 2. CLI Usage
-```bash
+```
 $ snc4onnx -h
 
 usage:
   snc4onnx [-h]
-    --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
-    --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
-    [--op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]]
-    [--output_onnx_file_path OUTPUT_ONNX_FILE_PATH]
-    [--output_of_onnx_file_in_the_process_of_fusion]
-    [--non_verbose]
+    -if INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
+    -sd SRCOP_DESTOP [SRCOP_DESTOP ...]
+    [-opam OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]]
+    [-of OUTPUT_ONNX_FILE_PATH]
+    [-f]
+    [-n]
 
 optional arguments:
   -h, --help
-    show this help message and exit
+    show this help message and exit.
 
-  --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
-    Input onnx file paths. At least two onnx files must be specified.
+  -if INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...], --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
+      Input onnx file paths. At least two onnx files must be specified.
 
-  --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
-    The names of the output OP to join from and the input OP to join to are
-    out1 in1 out2 in2 out3 in3 .... format.
-    In other words, to combine model1 and model2,
-    --srcop_destop model1_out1 model2_in1 model1_out2 model2_in2
-    Also, --srcop_destop can be specified multiple times.
-    The first --srcop_destop specifies the correspondence between model1 and model2,
-    and the second --srcop_destop specifies the correspondence
-    between model1 and model2 combined and model3.
-    It is necessary to take into account that the prefix specified
-    in op_prefixes_after_merging is given at the beginning of each OP name.
-    e.g. To combine model1 with model2 and model3.
-    --srcop_destop model1_src_op1 model2_dest_op1 model1_src_op2 model2_dest_op2 ...
-    --srcop_destop comb_model12_src_op1 model3_dest_op1 comb_model12_src_op2 model3_dest_op2 ...
-
-  --op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]
-    Since a single ONNX file cannot contain multiple OPs with the same name,
-    a prefix is added to all OPs in each input ONNX model to avoid duplication.
-    Specify the same number of paths as input_onnx_file_paths.
-    e.g. --op_prefixes_after_merging model1_prefix model2_prefix model3_prefix ...
+  -sd SRCOP_DESTOP [SRCOP_DESTOP ...], --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
+      The names of the output OP to join from and the input OP to join to are
+      out1 in1 out2 in2 out3 in3 ....
+      format.
+      In other words, to combine model1 and model2,
+      --srcop_destop model1_out1 model2_in1 model1_out2 model2_in2
+      Also, --srcop_destop can be specified multiple times.
+      The first --srcop_destop specifies the correspondence between model1 and model2,
+      and the second --srcop_destop specifies the correspondence between
+      model1 and model2 combined and model3.
+      It is necessary to take into account that the prefix specified
+      in op_prefixes_after_merging is
+      given at the beginning of each OP name.
+      e.g. To combine model1 with model2 and model3.
+      --srcop_destop model1_src_op1 model2_dest_op1 model1_src_op2 model2_dest_op2 ...
+      --srcop_destop combined_model1.2_src_op1 model3_dest_op1 combined_model1.2_src_op2 model3_dest_op2 ...
+
+  -opam OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...], --op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]
+      Since a single ONNX file cannot contain multiple OPs with the same name,
+      a prefix is added to all OPs in each input ONNX model to avoid duplication.
+      Specify the same number of paths as input_onnx_file_paths.
+      e.g. --op_prefixes_after_merging model1_prefix model2_prefix model3_prefix ...
 
-  --output_onnx_file_path OUTPUT_ONNX_FILE_PATH
-    Output onnx file path.
+  -of OUTPUT_ONNX_FILE_PATH, --output_onnx_file_path OUTPUT_ONNX_FILE_PATH
+      Output onnx file path.
 
-  --output_of_onnx_file_in_the_process_of_fusion
-    Output of onnx files in the process of fusion.
+  -f, --output_of_onnx_file_in_the_process_of_fusion
+      Output of onnx files in the process of fusion.
 
-  --non_verbose
-    Do not show all information logs. Only error logs are displayed.
+  -n, --non_verbose
+      Do not show all information logs. Only error logs are displayed.
 ```
 
 ## 3. In-script Usage
 ```python
 $ python
 >>> from snc4onnx import combine
 >>> help(combine)
```

### Comparing `snc4onnx-1.0.8/README.md` & `snc4onnx-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: snc4onnx
+Version: 1.0.9
+Summary: Simple tool to combine onnx models. Simple Network Combine Tool for ONNX.
+Home-page: https://github.com/PINTO0309/sne4onnx
+Author: Katsuya Hyodo
+Author-email: rmsdh122@yahoo.co.jp
+License: MIT License
+Platform: linux
+Platform: unix
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # snc4onnx
 Simple tool to combine(merge) onnx models. **S**imple **N**etwork **C**ombine Tool for **ONNX**.
 
 https://github.com/PINTO0309/simple-onnx-processing-tools
 
 [![Downloads](https://static.pepy.tech/personalized-badge/snc4onnx?period=total&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/snc4onnx) ![GitHub](https://img.shields.io/github/license/PINTO0309/snc4onnx?color=2BAF2B) [![PyPI](https://img.shields.io/pypi/v/snc4onnx?color=2BAF2B)](https://pypi.org/project/snc4onnx/) [![CodeQL](https://github.com/PINTO0309/snc4onnx/workflows/CodeQL/badge.svg)](https://github.com/PINTO0309/snc4onnx/actions?query=workflow%3ACodeQL)
 
@@ -23,62 +37,64 @@
 && python3 -m pip install -U onnx_graphsurgeon --index-url https://pypi.ngc.nvidia.com \
 && pip install -U snc4onnx
 ```
 ### 1-2. Docker
 https://github.com/PINTO0309/simple-onnx-processing-tools#docker
 
 ## 2. CLI Usage
-```bash
+```
 $ snc4onnx -h
 
 usage:
   snc4onnx [-h]
-    --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
-    --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
-    [--op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]]
-    [--output_onnx_file_path OUTPUT_ONNX_FILE_PATH]
-    [--output_of_onnx_file_in_the_process_of_fusion]
-    [--non_verbose]
+    -if INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
+    -sd SRCOP_DESTOP [SRCOP_DESTOP ...]
+    [-opam OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]]
+    [-of OUTPUT_ONNX_FILE_PATH]
+    [-f]
+    [-n]
 
 optional arguments:
   -h, --help
-    show this help message and exit
+    show this help message and exit.
 
-  --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
-    Input onnx file paths. At least two onnx files must be specified.
+  -if INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...], --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
+      Input onnx file paths. At least two onnx files must be specified.
 
-  --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
-    The names of the output OP to join from and the input OP to join to are
-    out1 in1 out2 in2 out3 in3 .... format.
-    In other words, to combine model1 and model2,
-    --srcop_destop model1_out1 model2_in1 model1_out2 model2_in2
-    Also, --srcop_destop can be specified multiple times.
-    The first --srcop_destop specifies the correspondence between model1 and model2,
-    and the second --srcop_destop specifies the correspondence
-    between model1 and model2 combined and model3.
-    It is necessary to take into account that the prefix specified
-    in op_prefixes_after_merging is given at the beginning of each OP name.
-    e.g. To combine model1 with model2 and model3.
-    --srcop_destop model1_src_op1 model2_dest_op1 model1_src_op2 model2_dest_op2 ...
-    --srcop_destop comb_model12_src_op1 model3_dest_op1 comb_model12_src_op2 model3_dest_op2 ...
-
-  --op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]
-    Since a single ONNX file cannot contain multiple OPs with the same name,
-    a prefix is added to all OPs in each input ONNX model to avoid duplication.
-    Specify the same number of paths as input_onnx_file_paths.
-    e.g. --op_prefixes_after_merging model1_prefix model2_prefix model3_prefix ...
+  -sd SRCOP_DESTOP [SRCOP_DESTOP ...], --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
+      The names of the output OP to join from and the input OP to join to are
+      out1 in1 out2 in2 out3 in3 ....
+      format.
+      In other words, to combine model1 and model2,
+      --srcop_destop model1_out1 model2_in1 model1_out2 model2_in2
+      Also, --srcop_destop can be specified multiple times.
+      The first --srcop_destop specifies the correspondence between model1 and model2,
+      and the second --srcop_destop specifies the correspondence between
+      model1 and model2 combined and model3.
+      It is necessary to take into account that the prefix specified
+      in op_prefixes_after_merging is
+      given at the beginning of each OP name.
+      e.g. To combine model1 with model2 and model3.
+      --srcop_destop model1_src_op1 model2_dest_op1 model1_src_op2 model2_dest_op2 ...
+      --srcop_destop combined_model1.2_src_op1 model3_dest_op1 combined_model1.2_src_op2 model3_dest_op2 ...
+
+  -opam OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...], --op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]
+      Since a single ONNX file cannot contain multiple OPs with the same name,
+      a prefix is added to all OPs in each input ONNX model to avoid duplication.
+      Specify the same number of paths as input_onnx_file_paths.
+      e.g. --op_prefixes_after_merging model1_prefix model2_prefix model3_prefix ...
 
-  --output_onnx_file_path OUTPUT_ONNX_FILE_PATH
-    Output onnx file path.
+  -of OUTPUT_ONNX_FILE_PATH, --output_onnx_file_path OUTPUT_ONNX_FILE_PATH
+      Output onnx file path.
 
-  --output_of_onnx_file_in_the_process_of_fusion
-    Output of onnx files in the process of fusion.
+  -f, --output_of_onnx_file_in_the_process_of_fusion
+      Output of onnx files in the process of fusion.
 
-  --non_verbose
-    Do not show all information logs. Only error logs are displayed.
+  -n, --non_verbose
+      Do not show all information logs. Only error logs are displayed.
 ```
 
 ## 3. In-script Usage
 ```python
 $ python
 >>> from snc4onnx import combine
 >>> help(combine)
```

### Comparing `snc4onnx-1.0.8/setup.py` & `snc4onnx-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `snc4onnx-1.0.8/snc4onnx/onnx_network_combine.py` & `snc4onnx-1.0.9/snc4onnx/onnx_network_combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,21 +429,23 @@
     # 6. Return
     return combined_model
 
 
 def main():
     parser = ArgumentParser()
     parser.add_argument(
+        '-if',
         '--input_onnx_file_paths',
         type=str,
         required=True,
         nargs='+',
         help='Input onnx file paths. At least two onnx files must be specified.'
     )
     parser.add_argument(
+        '-sd',
         '--srcop_destop',
         type=str,
         required=True,
         nargs='+',
         action='append',
         help=\
             'The names of the output OP to join from and the input OP to join to are '+
@@ -456,35 +458,39 @@
             'It is necessary to take into account that the prefix specified '+
             'in op_prefixes_after_merging is given at the beginning of each OP name. \n'+
             'e.g. To combine model1 with model2 and model3. \n'+
             '--srcop_destop model1_src_op1 model2_dest_op1 model1_src_op2 model2_dest_op2 ... \n'+
             '--srcop_destop combined_model1.2_src_op1 model3_dest_op1 combined_model1.2_src_op2 model3_dest_op2 ...'
     )
     parser.add_argument(
+        '-opam',
         '--op_prefixes_after_merging',
         type=str,
         nargs='+',
         help=\
             'Since a single ONNX file cannot contain multiple OPs with the same name, '+
             'a prefix is added to all OPs in each input ONNX model to avoid duplication. \n'+
             'Specify the same number of paths as input_onnx_file_paths. \n'+
             'e.g. --op_prefixes_after_merging model1_prefix model2_prefix model3_prefix ...'
     )
     parser.add_argument(
+        '-of',
         '--output_onnx_file_path',
         type=str,
         default='merged_model.onnx',
         help='Output onnx file path.'
     )
     parser.add_argument(
+        '-f',
         '--output_of_onnx_file_in_the_process_of_fusion',
         action='store_true',
         help='Output of onnx files in the process of fusion.'
     )
     parser.add_argument(
+        '-n',
         '--non_verbose',
         action='store_true',
         help='Do not show all information logs. Only error logs are displayed.'
     )
     args = parser.parse_args()
 
     # Model combine
```

### Comparing `snc4onnx-1.0.8/snc4onnx.egg-info/PKG-INFO` & `snc4onnx-1.0.9/snc4onnx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snc4onnx
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple tool to combine onnx models. Simple Network Combine Tool for ONNX.
 Home-page: https://github.com/PINTO0309/sne4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -37,62 +37,64 @@
 && python3 -m pip install -U onnx_graphsurgeon --index-url https://pypi.ngc.nvidia.com \
 && pip install -U snc4onnx
 ```
 ### 1-2. Docker
 https://github.com/PINTO0309/simple-onnx-processing-tools#docker
 
 ## 2. CLI Usage
-```bash
+```
 $ snc4onnx -h
 
 usage:
   snc4onnx [-h]
-    --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
-    --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
-    [--op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]]
-    [--output_onnx_file_path OUTPUT_ONNX_FILE_PATH]
-    [--output_of_onnx_file_in_the_process_of_fusion]
-    [--non_verbose]
+    -if INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
+    -sd SRCOP_DESTOP [SRCOP_DESTOP ...]
+    [-opam OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]]
+    [-of OUTPUT_ONNX_FILE_PATH]
+    [-f]
+    [-n]
 
 optional arguments:
   -h, --help
-    show this help message and exit
+    show this help message and exit.
 
-  --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
-    Input onnx file paths. At least two onnx files must be specified.
+  -if INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...], --input_onnx_file_paths INPUT_ONNX_FILE_PATHS [INPUT_ONNX_FILE_PATHS ...]
+      Input onnx file paths. At least two onnx files must be specified.
 
-  --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
-    The names of the output OP to join from and the input OP to join to are
-    out1 in1 out2 in2 out3 in3 .... format.
-    In other words, to combine model1 and model2,
-    --srcop_destop model1_out1 model2_in1 model1_out2 model2_in2
-    Also, --srcop_destop can be specified multiple times.
-    The first --srcop_destop specifies the correspondence between model1 and model2,
-    and the second --srcop_destop specifies the correspondence
-    between model1 and model2 combined and model3.
-    It is necessary to take into account that the prefix specified
-    in op_prefixes_after_merging is given at the beginning of each OP name.
-    e.g. To combine model1 with model2 and model3.
-    --srcop_destop model1_src_op1 model2_dest_op1 model1_src_op2 model2_dest_op2 ...
-    --srcop_destop comb_model12_src_op1 model3_dest_op1 comb_model12_src_op2 model3_dest_op2 ...
-
-  --op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]
-    Since a single ONNX file cannot contain multiple OPs with the same name,
-    a prefix is added to all OPs in each input ONNX model to avoid duplication.
-    Specify the same number of paths as input_onnx_file_paths.
-    e.g. --op_prefixes_after_merging model1_prefix model2_prefix model3_prefix ...
+  -sd SRCOP_DESTOP [SRCOP_DESTOP ...], --srcop_destop SRCOP_DESTOP [SRCOP_DESTOP ...]
+      The names of the output OP to join from and the input OP to join to are
+      out1 in1 out2 in2 out3 in3 ....
+      format.
+      In other words, to combine model1 and model2,
+      --srcop_destop model1_out1 model2_in1 model1_out2 model2_in2
+      Also, --srcop_destop can be specified multiple times.
+      The first --srcop_destop specifies the correspondence between model1 and model2,
+      and the second --srcop_destop specifies the correspondence between
+      model1 and model2 combined and model3.
+      It is necessary to take into account that the prefix specified
+      in op_prefixes_after_merging is
+      given at the beginning of each OP name.
+      e.g. To combine model1 with model2 and model3.
+      --srcop_destop model1_src_op1 model2_dest_op1 model1_src_op2 model2_dest_op2 ...
+      --srcop_destop combined_model1.2_src_op1 model3_dest_op1 combined_model1.2_src_op2 model3_dest_op2 ...
+
+  -opam OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...], --op_prefixes_after_merging OP_PREFIXES_AFTER_MERGING [OP_PREFIXES_AFTER_MERGING ...]
+      Since a single ONNX file cannot contain multiple OPs with the same name,
+      a prefix is added to all OPs in each input ONNX model to avoid duplication.
+      Specify the same number of paths as input_onnx_file_paths.
+      e.g. --op_prefixes_after_merging model1_prefix model2_prefix model3_prefix ...
 
-  --output_onnx_file_path OUTPUT_ONNX_FILE_PATH
-    Output onnx file path.
+  -of OUTPUT_ONNX_FILE_PATH, --output_onnx_file_path OUTPUT_ONNX_FILE_PATH
+      Output onnx file path.
 
-  --output_of_onnx_file_in_the_process_of_fusion
-    Output of onnx files in the process of fusion.
+  -f, --output_of_onnx_file_in_the_process_of_fusion
+      Output of onnx files in the process of fusion.
 
-  --non_verbose
-    Do not show all information logs. Only error logs are displayed.
+  -n, --non_verbose
+      Do not show all information logs. Only error logs are displayed.
 ```
 
 ## 3. In-script Usage
 ```python
 $ python
 >>> from snc4onnx import combine
 >>> help(combine)
```

