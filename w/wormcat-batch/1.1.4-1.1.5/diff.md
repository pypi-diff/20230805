# Comparing `tmp/wormcat_batch-1.1.4.tar.gz` & `tmp/wormcat_batch-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormcat_batch-1.1.4.tar", last modified: Fri Aug  4 20:46:44 2023, max compression
+gzip compressed data, was "wormcat_batch-1.1.5.tar", last modified: Sat Aug  5 16:26:01 2023, max compression
```

## Comparing `wormcat_batch-1.1.4.tar` & `wormcat_batch-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-04 20:46:44.797946 wormcat_batch-1.1.4/
--rw-r--r--   0 dan        (501) staff       (20)      135 2023-08-02 13:35:39.000000 wormcat_batch-1.1.4/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-04 20:46:44.797690 wormcat_batch-1.1.4/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2764 2023-08-04 20:45:44.000000 wormcat_batch-1.1.4/README.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-08-04 20:46:44.798011 wormcat_batch-1.1.4/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      703 2023-08-04 20:44:41.000000 wormcat_batch-1.1.4/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-04 20:46:44.796553 wormcat_batch-1.1.4/wormcat_batch/
--rw-r--r--   0 dan        (501) staff       (20)     3888 2023-08-04 13:35:59.000000 wormcat_batch-1.1.4/wormcat_batch/create_sunburst.py
--rw-r--r--   0 dan        (501) staff       (20)     4628 2023-08-04 13:51:15.000000 wormcat_batch-1.1.4/wormcat_batch/create_wormcat_xlsx.py
--rw-r--r--   0 dan        (501) staff       (20)     2909 2023-08-04 14:01:40.000000 wormcat_batch-1.1.4/wormcat_batch/execute_r.py
--rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.4/wormcat_batch/is_wormcat_installed.R
--rwxr-xr-x   0 dan        (501) staff       (20)    10729 2023-08-04 20:29:07.000000 wormcat_batch-1.1.4/wormcat_batch/run_wormcat_batch.py
--rw-r--r--   0 dan        (501) staff       (20)   227410 2023-08-02 13:20:17.000000 wormcat_batch-1.1.4/wormcat_batch/sunburst.template
--rwxr-xr-x   0 dan        (501) staff       (20)     1807 2023-08-04 12:54:01.000000 wormcat_batch-1.1.4/wormcat_batch/worm_cat.R
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-04 20:46:44.797354 wormcat_batch-1.1.4/wormcat_batch.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-04 20:46:44.000000 wormcat_batch-1.1.4/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      516 2023-08-04 20:46:44.000000 wormcat_batch-1.1.4/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-04 20:46:44.000000 wormcat_batch-1.1.4/wormcat_batch.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2023-08-04 20:46:44.000000 wormcat_batch-1.1.4/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-04 20:46:44.000000 wormcat_batch-1.1.4/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       32 2023-08-04 20:46:44.000000 wormcat_batch-1.1.4/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       14 2023-08-04 20:46:44.000000 wormcat_batch-1.1.4/wormcat_batch.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-05 16:26:01.173877 wormcat_batch-1.1.5/
+-rw-r--r--   0 dan        (501) staff       (20)      135 2023-08-02 13:35:39.000000 wormcat_batch-1.1.5/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-05 16:26:01.173737 wormcat_batch-1.1.5/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2764 2023-08-04 20:45:44.000000 wormcat_batch-1.1.5/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-08-05 16:26:01.173917 wormcat_batch-1.1.5/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      752 2023-08-05 13:29:51.000000 wormcat_batch-1.1.5/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-05 16:26:01.172345 wormcat_batch-1.1.5/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     3888 2023-08-04 13:35:59.000000 wormcat_batch-1.1.5/wormcat_batch/create_sunburst.py
+-rw-r--r--   0 dan        (501) staff       (20)     4628 2023-08-04 13:51:15.000000 wormcat_batch-1.1.5/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2909 2023-08-04 14:01:40.000000 wormcat_batch-1.1.5/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.5/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)    12850 2023-08-05 16:09:24.000000 wormcat_batch-1.1.5/wormcat_batch/run_wormcat_batch.py
+-rw-r--r--   0 dan        (501) staff       (20)   227410 2023-08-02 13:20:17.000000 wormcat_batch-1.1.5/wormcat_batch/sunburst.template
+-rwxr-xr-x   0 dan        (501) staff       (20)     1807 2023-08-04 12:54:01.000000 wormcat_batch-1.1.5/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-05 16:26:01.173547 wormcat_batch-1.1.5/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-05 16:26:01.000000 wormcat_batch-1.1.5/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      516 2023-08-05 16:26:01.000000 wormcat_batch-1.1.5/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-05 16:26:01.000000 wormcat_batch-1.1.5/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-08-05 16:26:01.000000 wormcat_batch-1.1.5/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-05 16:26:01.000000 wormcat_batch-1.1.5/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       32 2023-08-05 16:26:01.000000 wormcat_batch-1.1.5/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-08-05 16:26:01.000000 wormcat_batch-1.1.5/wormcat_batch.egg-info/top_level.txt
```

### Comparing `wormcat_batch-1.1.4/README.md` & `wormcat_batch-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.4/setup.py` & `wormcat_batch-1.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+"""
+Setup for pypi releases of wormcat_batch
+"""
 from setuptools import setup
 
 # rm -rf dist
 # python setup.py sdist
 # pip install dist/wormcat_batch-1.0.1.tar.gz
 # twine check dist/*
 # twine upload --repository pypi dist/*
 
 setup(name='wormcat_batch',
-      version='1.1.4',
+      version='1.1.5',
       description='Batch processing for Wormcat data',
       url='https://github.com/dphiggs01/Wormcat_batch',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
       license='MIT',
 
       packages=['wormcat_batch'],
```

### Comparing `wormcat_batch-1.1.4/wormcat_batch/create_sunburst.py` & `wormcat_batch-1.1.5/wormcat_batch/create_sunburst.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.4/wormcat_batch/create_wormcat_xlsx.py` & `wormcat_batch-1.1.5/wormcat_batch/create_wormcat_xlsx.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.4/wormcat_batch/execute_r.py` & `wormcat_batch-1.1.5/wormcat_batch/execute_r.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.4/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.1.5/wormcat_batch/run_wormcat_batch.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 
 def extract_csv_files(input_excel_nm, csv_file_path):
     """
     Create CSV Files from the given Excel spreadsheet
     """
-    input_excel = pd.ExcelFile(input_excel_nm)
+    try:
+        input_excel = pd.ExcelFile(input_excel_nm)
+    except ValueError:
+        print(f"ERROR: File Name [{input_excel_nm}[] is Not a Valid Excel File.")
+        sys.exit(-1)
+    
     for sheet in input_excel.sheet_names:
         sheet_df = input_excel.parse(sheet)
         sheet_df.to_csv(
             f'{csv_file_path}{os.path.sep}{sheet}.csv', index=False)
 
 
 def process_csv_files(csv_file_path, wormcat_out_path, annotation_file):
@@ -71,17 +76,17 @@
                               'sheet', 'category', 'file', 'label'])
     process_category_files(df_process, annotation_file, out_xsl_file_nm)
 
 # Wormcat Utility functions
 
 
 def get_wormcat_lib():
-    '''
+    """
     Find the location where the R Wormcat program is installed
-    '''
+    """
     execute_r = ExecuteR()
     path = execute_r.wormcat_library_path_fun()
     if path:
         first_quote = path.find('"')
         last_quote = path.rfind('"')
         if last_quote == -1:
             print("Wormcat is not installed or cannot be found.")
@@ -123,22 +128,23 @@
             print(f"Creating backup of existing directory [{directory}]")
             # Create backup directory name with a unique timestamp suffix
             backup_dir = f"{directory}_{timestamp}.bk"
             shutil.move(directory, backup_dir)
         else:
             print("ERROR")
             print(f"Directory {directory} is not Empty and was not created by a prior run of this program.")
+            print("Change the output directory to an empty or non exsisting directory.")
             sys.exit(-1)
 
     try:
         os.makedirs(directory, exist_ok=True)
-        os.makedirs(directory, exist_ok=True)
-        created_by_flag_check = os.path.join(directory, created_by_flag)
-        with open(created_by_flag_check, 'w', encoding='utf-8') as file:
-            file.write(timestamp)
+        if with_backup:
+            created_by_flag_check = os.path.join(directory, created_by_flag)
+            with open(created_by_flag_check, 'w', encoding='utf-8') as file:
+                file.write(timestamp)
     except OSError as err:
         print(f"ERROR: Cannot create directory\n{err}")
         sys.exit(-1)
 
 
 
 def zip_directory(directory_path, zip_file_name):
@@ -148,24 +154,62 @@
     with zipfile.ZipFile(zip_file_name, 'w') as zipf:
         for root, _, files in os.walk(directory_path):
             for file in files:
                 file_path = os.path.join(root, file)
                 zipf.write(file_path, os.path.relpath(
                     file_path, directory_path))
 
-# main application functions
 
+def is_valid_directory_name(directory_name):
+    """
+    Check if the directory name string is a valid name
+    """
+    ret_val = True
+    if not isinstance(directory_name, str):
+        ret_val = False
+
+    # Check if the directory name is empty or contains only whitespace
+    if not directory_name.strip():
+        ret_val = False
+
+    # Check if the directory name contains any invalid characters
+    invalid_characters = '\'?%*|"<>'
+    if any(char in invalid_characters for char in directory_name):
+        ret_val = False
+
+    return ret_val
+
+class WormcatArgumentParser(argparse.ArgumentParser):
+    """
+    Add annotation file descriptions to help text
+    """
+    def print_help(self, file=None):
+        wormcat_path = get_wormcat_lib()
+        annotation_files = get_category_files(wormcat_path)
+        annotation_file_names = ""
+        for index, annotation_file in enumerate(sorted(annotation_files)):
+            annotation_file_names += f"\t{index+1} {annotation_file}\n"
+
+        super().print_help(file)
+        print(f"\nannotation-files:\n{annotation_file_names}")
+
+def print_error_and_quit(parser, error_msg):
+    """
+    Print command line ERROR message and quit
+    """
+    parser.print_usage()
+    print(f"ERROR: {error_msg}")
+    sys.exit(-1)
 
 def process_command_arguments():
     """
     The process_command_arguments method validates and sets the input arguments 
     to conform with downstream processing
     """
-    parser = argparse.ArgumentParser()
-    help_statement = "wormcat_cli --input-excel <path_to_excel> | --input-csv-path <path_to_csv> --output-path <path_to_out_dir> --annotation-file 'whole_genome_v2_nov-11-2021.csv' --clean-temp False"
+    parser = WormcatArgumentParser()
     parser.add_argument('-i', '--input-excel',
                         help='Input file in Excel/Wormcat format')
     parser.add_argument('-c', '--input-csv-path',
                         help='Input path to a collection of CSV files in Wormcat format')
     parser.add_argument('-o', '--output-path', help='Output path')
     parser.add_argument('-a', '--annotation-file', default='whole_genome_v2_nov-11-2021.csv',
                         help='Annotation file name or path default=whole_genome_v2_nov-11-2021.csv')
@@ -173,46 +217,62 @@
                         help='Remove files created while processing default=False')
 
     parser.add_argument('-v', '--version', action='version',
                         version=f'%(prog)s v{importlib.metadata.version("wormcat_batch")}')
     args = parser.parse_args()
 
     if not args.input_excel and not args.input_csv_path:
-        print(help_statement)
-        print("An Excel Input file or a path to CSV files is required.")
-        sys.exit(-1)
+        print_error_and_quit(parser, "An Excel Input file or a path to CSV files is required.")
 
-    if not args.output_path:
-        print(help_statement)
-        print("An Output path is required.")
-        sys.exit(-1)
+    if args.input_excel and args.input_csv_path:
+        print_error_and_quit(parser, "--input-excel [-i] and  --input-csv-path [-c] can not be used at the same time.")
+    
+    if args.input_excel and not os.path.isfile(args.input_excel):
+        print_error_and_quit(parser, f""" An Excel Input file not found.
+        [{args.input_excel}] is not a valid file name for wormcat batch.""")
+      
+    if args.input_csv_path and not os.path.isdir(args.input_csv_path):
+        print_error_and_quit(parser, f""" An CSV Directory not found.
+        [{args.input_csv_path}] is not a valid directory name for wormcat batch.""")
+
+    if not args.output_path or not is_valid_directory_name(args.output_path):
+        print_error_and_quit(parser, f""" An Output path is required with a valid name.
+        [{args.output_path}] is not valid directory path for wormcat batch.""")
 
     # if args.annotation_file is not a path to an annotation file
     # vaildate the input name and set the full path
     if not os.path.sep in args.annotation_file:
         wormcat_path = get_wormcat_lib()
         annotation_files = get_category_files(wormcat_path)
         
         if not args.annotation_file or not args.annotation_file in annotation_files:
-            print(help_statement)
-            print("Missing or incorrect annotation-file-nm.")
-            annotation_file_names = ""
-            for index, annotation_file in enumerate(sorted(annotation_files)):
-                annotation_file_names += f"\t{index+1} {annotation_file}\n"
-            print(f"Available names:\n{annotation_file_names}")
-            sys.exit(-1)
+            print_error_and_quit(parser, "Missing or incorrect annotation-file-nm. See --help for details.")
+            
         args.annotation_file = f"{wormcat_path}{os.path.sep}extdata{os.path.sep}{args.annotation_file}"
 
+    elif args.annotation_file and os.path.sep in args.annotation_file:
+        if not os.path.isfile(args.annotation_file):
+            print_error_and_quit(parser, f"""Local Annotation file not found.
+            [{args.annotation_file}] is not a valid file name for wormcat batch.""")
+
     # Support TRUE or True as input to clean temp
     # otherwise set to False
     if args.clean_temp.lower().title() == 'True':
         args.clean_temp = True
     else:
         args.clean_temp = False
 
+    print(f"\tInput Excel     = {args.input_excel}")
+    print(f"\tInput CSV Path  = {args.input_csv_path}")
+    print(f"\tOutput Path     = {args.output_path}")
+    print(f"\tAnnotation File = {args.annotation_file}")
+    print(f"\tClean Temp      = {args.clean_temp}")
+    print("\n")
+
+
     return args
 
 
 def main():
     """
     Main control execution of Wormcat Batch
     """
@@ -244,20 +304,14 @@
         input_data_nm = os.path.basename(args.input_csv_path)
 
     timestamp = datetime.now().strftime("%Y%m%d-%H%M%S")
     output_base_dir = f"{input_data_nm}_{timestamp}"
     wormcat_out_path = f"{args.output_path}{os.path.sep}{output_base_dir}"
     create_directory(wormcat_out_path)
 
-    print(f"{args.input_excel=}")
-    print(f"{args.input_csv_path=}")
-    print(f"{args.output_path=}")
-    print(f"{args.annotation_file=}")
-    print(f"{args.clean_temp=}")
-
     # Call Wormcat on each CSV file
     process_csv_files(csv_file_path, wormcat_out_path, args.annotation_file)
 
     # Create a summary spreadsheet of all CSV runs
     out_xsl_file_nm = f"{wormcat_out_path}{os.path.sep}Out_{input_data_nm}.xlsx"
     create_summary_spreadsheet(
         wormcat_out_path, args.annotation_file, out_xsl_file_nm)
```

### Comparing `wormcat_batch-1.1.4/wormcat_batch/sunburst.template` & `wormcat_batch-1.1.5/wormcat_batch/sunburst.template`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.4/wormcat_batch/worm_cat.R` & `wormcat_batch-1.1.5/wormcat_batch/worm_cat.R`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.4/wormcat_batch.egg-info/SOURCES.txt` & `wormcat_batch-1.1.5/wormcat_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

