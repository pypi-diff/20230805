# Comparing `tmp/tja2fumen-0.6.0.tar.gz` & `tmp/tja2fumen-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.6.0.tar", last modified: Sat Jul 29 01:46:41 2023, max compression
+gzip compressed data, was "tja2fumen-0.6.1.tar", last modified: Sat Aug  5 15:20:28 2023, max compression
```

## Comparing `tja2fumen-0.6.0.tar` & `tja2fumen-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/
--rw-rw-rw-   0        0        0     1085 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0       37 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11858 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    10129 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/README.md
--rw-rw-rw-   0        0        0     1084 2023-07-29 01:46:25.000000 tja2fumen-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.049666 tja2fumen-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/src/tja2fumen/
--rw-rw-rw-   0        0        0     2094 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     2821 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    18498 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0   307495 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/hp_values.csv
--rw-rw-rw-   0        0        0    22522 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/parsers.py
--rw-rw-rw-   0        0        0    18235 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/types.py
--rw-rw-rw-   0        0        0     2468 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0    11858 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 15:20:28.530340 tja2fumen-0.6.1/
+-rw-rw-rw-   0        0        0     1085 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       37 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12287 2023-08-05 15:20:28.530340 tja2fumen-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10558 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/README.md
+-rw-rw-rw-   0        0        0     1291 2023-08-05 15:20:17.000000 tja2fumen-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 15:20:28.530340 tja2fumen-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:20:28.514779 tja2fumen-0.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 15:20:28.530340 tja2fumen-0.6.1/src/tja2fumen/
+-rw-rw-rw-   0        0        0     2323 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0    15609 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/src/tja2fumen/classes.py
+-rw-rw-rw-   0        0        0     2883 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    20050 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0   307495 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/src/tja2fumen/hp_values.csv
+-rw-rw-rw-   0        0        0    22595 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/src/tja2fumen/parsers.py
+-rw-rw-rw-   0        0        0     2553 2023-08-05 15:19:04.000000 tja2fumen-0.6.1/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:20:28.530340 tja2fumen-0.6.1/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0    12287 2023-08-05 15:20:28.000000 tja2fumen-0.6.1/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-08-05 15:20:28.000000 tja2fumen-0.6.1/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 15:20:28.000000 tja2fumen-0.6.1/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-05 15:20:28.000000 tja2fumen-0.6.1/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2023-08-05 15:20:28.000000 tja2fumen-0.6.1/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-05 15:20:28.000000 tja2fumen-0.6.1/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.6.0/LICENSE.txt` & `tja2fumen-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.6.0/PKG-INFO` & `tja2fumen-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.6.0
+Version: 0.6.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -44,16 +44,25 @@
   tja2fumen is a tool that allows you to convert TJA charts (<code>.tja</code>) to fumen charts (<code>.bin</code>).
 </p>
 
 <p align="center">
   <a href="https://github.com/vivaria/tja2fumen/actions/workflows/test_and_publish_release.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/vivaria/tja2fumen/test_and_publish_release.yml?label=Tests" alt="Test status (main branch)"></a>
   <a href="https://github.com/vivaria/tja2fumen/releases/latest"><img src="https://img.shields.io/github/v/release/vivaria/tja2fumen" alt="GitHub release (with filter)"></a>
   <a href="https://github.com/vivaria/tja2fumen/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License"></a>
+  <a href="https://github.com/pylint-dev/pylint"><img src="https://img.shields.io/badge/Linting-pylint-black" alt="Linting pylint"></a>
+  <a href="https://github.com/PyCQA/flake8"><img src="https://img.shields.io/badge/Linting-flake8-black" alt="Linting flake8"></a>
+  <a href="https://github.com/python/mypy"><img src="https://img.shields.io/badge/Typing-mypy-black" alt="Linting mypy"></a>
 </p>
 
+<p align="center">
+
+
+</p>
+
+
 
 ----
 
 ## Features
 
 - Parse `.tja` chart files.
 - Convert parsed TJA song data into fumen chart data.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tja2fumen Version: 0.6.0 Summary: Convert TJA chart
+Metadata-Version: 2.1 Name: tja2fumen Version: 0.6.1 Summary: Convert TJA chart
 files into fumen (.bin) chart files License: MIT License Copyright (c) 2023
 Vivaria Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
@@ -19,14 +19,15 @@
 tja2fumen/ Keywords: taiko,tatsujin,fumen,TJA Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE.txt  
                      [tja2fumen â TJA chart converter]
    tja2fumen is a tool that allows you to convert TJA charts (.tja) to fumen
                                 charts (.bin).
    [Test_status_(main_branch)] [GitHub_release_(with_filter)] [MIT_License]
+               [Linting_pylint] [Linting_flake8] [Linting_mypy]
 ---- ## Features - Parse `.tja` chart files. - Convert parsed TJA song data
 into fumen chart data. - Write fumen chart data to `.bin` files. - Decode
 official fumen `.bin` files. ## Usage tja2fumen is included as part of several
 existing projects. So, you may be using tja2fumen already! - **XB1/TDMX**:
 [TakoTako](https://github.com/fluto/takotako) converts both chart and audio
 files for XB1/TDMX. - **Nijiro**: [TaikoSoundEditor](https://github.com/
 NotImplementedLife/TaikoSoundEditor) converts both chart and audio files for
```

### Comparing `tja2fumen-0.6.0/README.md` & `tja2fumen-0.6.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,25 @@
   tja2fumen is a tool that allows you to convert TJA charts (<code>.tja</code>) to fumen charts (<code>.bin</code>).
 </p>
 
 <p align="center">
   <a href="https://github.com/vivaria/tja2fumen/actions/workflows/test_and_publish_release.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/vivaria/tja2fumen/test_and_publish_release.yml?label=Tests" alt="Test status (main branch)"></a>
   <a href="https://github.com/vivaria/tja2fumen/releases/latest"><img src="https://img.shields.io/github/v/release/vivaria/tja2fumen" alt="GitHub release (with filter)"></a>
   <a href="https://github.com/vivaria/tja2fumen/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License"></a>
+  <a href="https://github.com/pylint-dev/pylint"><img src="https://img.shields.io/badge/Linting-pylint-black" alt="Linting pylint"></a>
+  <a href="https://github.com/PyCQA/flake8"><img src="https://img.shields.io/badge/Linting-flake8-black" alt="Linting flake8"></a>
+  <a href="https://github.com/python/mypy"><img src="https://img.shields.io/badge/Typing-mypy-black" alt="Linting mypy"></a>
 </p>
 
+<p align="center">
+
+
+</p>
+
+
 
 ----
 
 ## Features
 
 - Parse `.tja` chart files.
 - Convert parsed TJA song data into fumen chart data.
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
  
                      [tja2fumen â TJA chart converter]
    tja2fumen is a tool that allows you to convert TJA charts (.tja) to fumen
                                 charts (.bin).
    [Test_status_(main_branch)] [GitHub_release_(with_filter)] [MIT_License]
+               [Linting_pylint] [Linting_flake8] [Linting_mypy]
 ---- ## Features - Parse `.tja` chart files. - Convert parsed TJA song data
 into fumen chart data. - Write fumen chart data to `.bin` files. - Decode
 official fumen `.bin` files. ## Usage tja2fumen is included as part of several
 existing projects. So, you may be using tja2fumen already! - **XB1/TDMX**:
 [TakoTako](https://github.com/fluto/takotako) converts both chart and audio
 files for XB1/TDMX. - **Nijiro**: [TaikoSoundEditor](https://github.com/
 NotImplementedLife/TaikoSoundEditor) converts both chart and audio files for
```

### Comparing `tja2fumen-0.6.0/pyproject.toml` & `tja2fumen-0.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.6.0"
+version = "0.6.1"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
@@ -15,22 +15,31 @@
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 tja2fumen = "tja2fumen:main"
 
 [project.optional-dependencies]
 dev = ["pytest", "build", "pyinstaller", "twine", "toml-cli",
-       "flake8", "pyproject-flake8"]
+       "flake8", "pyproject-flake8", "mypy", "pylint"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.pytest.ini_options]
 addopts = "-vv --tb=short"
 console_output_style = "count"
 
 [tool.flake8]
 exclude = "venv/"
 per-file-ignores = """
-    ./src/tja2fumen/types.py: E221
+    ./src/tja2fumen/classes.py: E221
     ./testing/test_conversion.py: E221, E272
 """
+
+[tool.pylint.'MESSAGES CONTROL']
+disable = """
+    too-many-instance-attributes,
+    too-many-branches,
+    too-many-arguments,
+    too-many-locals,
+    too-many-statements
+"""
```

### Comparing `tja2fumen-0.6.0/src/tja2fumen/__init__.py` & `tja2fumen-0.6.1/src/tja2fumen/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+"""
+Entry points for tja2fumen.
+"""
+
 import argparse
 import os
 import sys
+from typing import Sequence
 
 from tja2fumen.parsers import parse_tja
 from tja2fumen.converters import convert_tja_to_fumen
 from tja2fumen.writers import write_fumen
 from tja2fumen.constants import COURSE_IDS
+from tja2fumen.classes import TJACourse
 
 
-def main(argv=None):
+def main(argv: Sequence[str] = ()) -> None:
     """
     Main entry point for tja2fumen's command line interface.
 
     Three steps are performed:
        1. Parse TJA into multiple TJACourse objects. Then, for each course:
           2. Convert TJACourse objects into FumenCourse objects.
           3. Write each FumenCourse to its own .bin file.
@@ -31,22 +37,24 @@
     fname_tja = getattr(args, "file.tja")
     base_name = os.path.splitext(fname_tja)[0]
 
     # Parse lines in TJA file
     parsed_tja = parse_tja(fname_tja)
 
     # Convert parsed TJA courses and write each course to `.bin` files
-    for course in parsed_tja.courses.items():
-        convert_and_write(course, base_name,
-                          single_course=(len(parsed_tja.courses) == 1))
+    for course_name, course in parsed_tja.courses.items():
+        convert_and_write(course, course_name, base_name,
+                          single_course=len(parsed_tja.courses) == 1)
 
 
-def convert_and_write(parsed_course, base_name, single_course=False):
+def convert_and_write(tja_data: TJACourse,
+                      course_name: str,
+                      base_name: str,
+                      single_course: bool = False) -> None:
     """Process the parsed data for a single TJA course."""
-    course_name, tja_data = parsed_course
     fumen_data = convert_tja_to_fumen(tja_data)
     # Add course ID (e.g. '_x', '_x_1', '_x_2') to the output file's base name
     output_name = base_name
     if single_course:
         pass  # Replicate tja2bin.exe behavior by excluding course ID
     else:
         split_name = course_name.split("P")  # e.g. 'OniP2' -> ['Oni', '2']
```

### Comparing `tja2fumen-0.6.0/src/tja2fumen/constants.py` & `tja2fumen-0.6.1/src/tja2fumen/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Constant song properties of TJA and fumen files.
+"""
+
 # Names for branches in diverge songs
 BRANCH_NAMES = ("normal", "professional", "master")
 
 # Types of notes that can be found in TJA files
 TJA_NOTE_TYPES = {
     '0': 'Blank',
     '1': 'Don',
```

### Comparing `tja2fumen-0.6.0/src/tja2fumen/converters.py` & `tja2fumen-0.6.1/src/tja2fumen/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+"""
+Functions for converting TJA song data to Fumen song data.
+"""
+
 import re
+from typing import List, Dict, Tuple, Union
 
-from tja2fumen.types import TJAMeasureProcessed, FumenCourse, FumenNote
+from tja2fumen.classes import (TJACourse, TJAMeasure, TJAMeasureProcessed,
+                               FumenCourse, FumenHeader, FumenMeasure,
+                               FumenNote)
 
 
-def process_tja_commands(tja):
+def process_commands(tja_branches: Dict[str, List[TJAMeasure]], bpm: float) \
+                                -> Dict[str, List[TJAMeasureProcessed]]:
     """
-    Process each #COMMAND present in a TJASong's measures, and assign their
-    values as attributes to each measure.
+    Process all commands in each measure.
 
     This function takes care of two main tasks:
         1. Keeping track of what the current values are for BPM, scroll,
-           gogotime, barline, and time signature (#MEASURE).
+           gogotime, barline, and time signature (i.e. #MEASURE).
         2. Detecting when a command is placed in the middle of a measure,
            and splitting that measure into sub-measures.
 
     ((Note: We split measures into sub-measures because official `.bin` files
       can only have 1 value for BPM/SCROLL/GOGO per measure. So, if a TJA
       measure has multiple BPMs/SCROLLs/GOGOs, it has to be split up.))
 
     After this function is finished, all the #COMMANDS will be gone, and each
     measure will have attributes (e.g. measure.bpm, measure.scroll) instead.
     """
-    tja_branches_processed = {branch_name: []
-                              for branch_name in tja.branches.keys()}
-    for branch_name, branch_measures_tja in tja.branches.items():
-        current_bpm = tja.BPM
+    tja_branches_processed: Dict[str, List[TJAMeasureProcessed]] = {
+        branch_name: [] for branch_name in tja_branches.keys()
+    }
+    for branch_name, branch_measures_tja in tja_branches.items():
+        current_bpm = bpm
         current_scroll = 1.0
         current_gogo = False
         current_barline = True
         current_dividend = 4
         current_divisor = 4
         for measure_tja in branch_measures_tja:
             measure_tja_processed = TJAMeasureProcessed(
@@ -38,24 +46,33 @@
                 barline=current_barline,
                 time_sig=[current_dividend, current_divisor],
                 subdivisions=len(measure_tja.notes),
             )
             for data in measure_tja.combined:
                 # Handle note data
                 if data.name == 'note':
-                    measure_tja_processed.data.append(data)
+                    measure_tja_processed.notes.append(data)
 
                 # Handle commands that can only be placed between measures
                 # (i.e. no mid-measure variations)
                 elif data.name == 'delay':
-                    measure_tja_processed.delay = data.value * 1000  # ms -> s
+                    measure_tja_processed.delay = float(data.value) * 1000
                 elif data.name == 'branch_start':
-                    measure_tja_processed.branch_start = data.value
+                    branch_type, val1, val2 = data.value.split(',')
+                    if branch_type == 'r':  # r = drumRoll
+                        branch_cond = (float(val1), float(val2))
+                    elif branch_type == 'p':  # p = Percentage
+                        branch_cond = (float(val1)/100, float(val2)/100)
+                    else:
+                        raise ValueError(f"Invalid #BRANCHSTART type: "
+                                         f"'{branch_type}'.")
+                    measure_tja_processed.branch_type = branch_type
+                    measure_tja_processed.branch_cond = branch_cond
                 elif data.name == 'section':
-                    measure_tja_processed.section = data.value
+                    measure_tja_processed.section = bool(data.value)
                 elif data.name == 'levelhold':
                     measure_tja_processed.levelhold = True
                 elif data.name == 'barline':
                     current_barline = bool(int(data.value))
                     measure_tja_processed.barline = current_barline
                 elif data.name == 'measure':
                     match_measure = re.match(r"(\d+)/(\d+)", data.value)
@@ -69,25 +86,27 @@
                 # Handle commands that can be placed in the middle of a
                 # measure. (For fumen files, if there is a mid-measure change
                 # to BPM/SCROLL/GOGO, then the measure will actually be split
                 # into two small submeasures. So, we need to start a new
                 # measure in those cases.)
                 elif data.name in ['bpm', 'scroll', 'gogo']:
                     # Parse the values
+                    new_val: Union[bool, float]
                     if data.name == 'bpm':
                         new_val = current_bpm = float(data.value)
                     elif data.name == 'scroll':
-                        new_val = current_scroll = data.value
+                        new_val = current_scroll = float(data.value)
                     elif data.name == 'gogo':
                         new_val = current_gogo = bool(int(data.value))
                     # Check for mid-measure commands
                     # - Case 1: Command happens at the start of a measure;
                     #           just change the value directly
                     if data.pos == 0:
-                        measure_tja_processed.__setattr__(data.name, new_val)
+                        setattr(measure_tja_processed, data.name,
+                                new_val)  # noqa: new_val will always be set
                     # - Case 2: Command happens in the middle of a measure;
                     #           start a new sub-measure
                     else:
                         measure_tja_processed.pos_end = data.pos
                         tja_branches_processed[branch_name]\
                             .append(measure_tja_processed)
                         measure_tja_processed = TJAMeasureProcessed(
@@ -104,34 +123,27 @@
                     print(f"Unexpected event type: {data.name}")
 
             measure_tja_processed.pos_end = len(measure_tja.notes)
             tja_branches_processed[branch_name].append(measure_tja_processed)
 
     has_branches = all(len(b) for b in tja_branches_processed.values())
     if has_branches:
-        if len(set([len(b) for b in tja.branches.values()])) != 1:
-            raise ValueError(
-                "Branches do not have the same number of measures. (This "
-                "check was performed prior to splitting up the measures due "
-                "to mid-measure commands. Please check the number of ',' you"
-                "have in each branch.)"
-            )
-        if len(set([len(b) for b in tja_branches_processed.values()])) != 1:
+        if len({len(b) for b in tja_branches_processed.values()}) != 1:
             raise ValueError(
                 "Branches do not have the same number of measures. (This "
                 "check was performed after splitting up the measures due "
                 "to mid-measure commands. Please check any GOGO, BPMCHANGE, "
                 "and SCROLL commands you have in your branches, and make sure"
                 "that each branch has the same number of commands.)"
             )
 
     return tja_branches_processed
 
 
-def convert_tja_to_fumen(tja):
+def convert_tja_to_fumen(tja: TJACourse) -> FumenCourse:
     """
     Convert TJA data to Fumen data by calculating Fumen-specific values.
 
     Fumen files (`.bin`) use a very strict file structure. Certain values are
     expected at very specific byte locations in the file, such as:
       - Header metadata (first 520 bytes). The header stores information such
         as branch points for each note type, soul gauge behavior, etc.
@@ -155,46 +167,50 @@
     └─ ...
 
     ((Note: The fumen file structure is the opposite of the TJA file structure;
     branch data is stored within the measure object, rather than measure data
     being stored within the branch object.))
     """
     # Preprocess commands
-    tja_branches_processed = process_tja_commands(tja)
+    tja_branches_processed = process_commands(tja.branches, tja.bpm)
 
     # Pre-allocate the measures for the converted TJA
     n_measures = len(tja_branches_processed['normal'])
     fumen = FumenCourse(
-        measures=n_measures,
+        measures=[FumenMeasure() for _ in range(n_measures)],
+        header=FumenHeader(),
         score_init=tja.score_init,
         score_diff=tja.score_diff,
     )
 
     # Set song metadata using information from the processed measures
     fumen.header.b512_b515_number_of_measures = n_measures
     fumen.header.b432_b435_has_branches = int(all(
-        [len(b) for b in tja_branches_processed.values()]
+        len(b) for b in tja_branches_processed.values()
     ))
 
     # Iterate through the different branches in the TJA
     total_notes = {'normal': 0, 'professional': 0, 'master': 0}
     for current_branch, branch_tja in tja_branches_processed.items():
-        if not len(branch_tja):
+        # Skip empty branches (e.g. 'professional', 'master')
+        if not branch_tja:
             continue
+
+        # Track properties that will change over the course of the song
         branch_points_total = 0
         branch_points_measure = 0
-        current_drumroll = None
+        current_drumroll = FumenNote()
         current_levelhold = False
-        branch_conditions = []
+        branch_types: List[str] = []
+        branch_conditions: List[Tuple[float, float]] = []
         course_balloons = tja.balloon.copy()
 
-        # Iterate through the measures within the branch
-        for idx_m, measure_tja in enumerate(branch_tja):
-            # Fetch the corresponding fumen measure
-            measure_fumen = fumen.measures[idx_m]
+        # Iterate over pairs of TJA and Fumen measures
+        for idx_m, (measure_tja, measure_fumen) in \
+                enumerate(zip(branch_tja, fumen.measures)):
 
             # Copy over basic measure properties from the TJA
             measure_fumen.branches[current_branch].speed = measure_tja.scroll
             measure_fumen.gogo = measure_tja.gogo
             measure_fumen.bpm = measure_tja.bpm
 
             # Compute the duration of the measure
@@ -202,48 +218,50 @@
             measure_fumen.set_duration(
                 time_sig=measure_tja.time_sig,
                 measure_length=measure_length,
                 subdivisions=measure_tja.subdivisions
             )
 
             # Compute the millisecond offsets for the start/end of each measure
-            measure_fumen.set_ms_offsets(
-                song_offset=tja.offset,
-                delay=measure_tja.delay,
-                prev_measure=(fumen.measures[idx_m-1] if idx_m else None),
-                first_measure=(idx_m == 0)
-            )
+            if idx_m == 0:
+                measure_fumen.set_first_ms_offsets(song_offset=tja.offset)
+            else:
+                measure_fumen.set_ms_offsets(
+                    delay=measure_tja.delay,
+                    prev_measure=fumen.measures[idx_m-1],
+                )
 
             # Handle whether barline should be hidden:
             #     1. Measures where #BARLINEOFF has been set
             #     2. Sub-measures that don't fall on the barline
             barline_off = measure_tja.barline is False
             is_submeasure = (measure_length < measure_tja.subdivisions and
                              measure_tja.pos_start != 0)
             if barline_off or is_submeasure:
                 measure_fumen.barline = False
 
             # Check to see if the measure contains a branching condition
-            branch_condition = measure_tja.branch_start
-            if branch_condition:
+            branch_type = measure_tja.branch_type
+            branch_cond = measure_tja.branch_cond
+            if branch_type and branch_cond:
                 # Update the branch_info values for the measure
                 measure_fumen.set_branch_info(
-                    branch_condition, branch_points_total, current_branch,
-                    first_branch_condition=(not branch_conditions),
-                    has_section=bool(measure_tja.section),
+                    branch_type, branch_cond,
+                    branch_points_total, current_branch,
                     has_levelhold=current_levelhold
                 )
                 # Reset the points to prepare for the next `#BRANCHSTART p`
                 branch_points_total = 0
                 # Reset the levelhold value (so that future branch_conditions
                 # work normally)
                 current_levelhold = False
                 # Keep track of the branch conditions (to later determine how
                 # to set the header bytes for branches)
-                branch_conditions.append(branch_condition)
+                branch_types.append(branch_type)
+                branch_conditions.append(branch_cond)
 
             # NB: We update the branch condition note counter *after*
             # we check the current measure's branch condition.
             # This is because the TJA spec says:
             #    "The requirement is calculated one measure before
             #     #BRANCHSTART, changing the branch visually when it
             #     is calculated and changing the notes after #BRANCHSTART."
@@ -255,86 +273,92 @@
             # the next `#BRANCHSTART` command", so we check this value after
             # we've already processed the branch condition for this measure.
             if measure_tja.levelhold:
                 current_levelhold = True
 
             # Create notes based on TJA measure data
             branch_points_measure = 0
-            for idx_d, data in enumerate(measure_tja.data):
+            for note_tja in measure_tja.notes:
                 # Compute the ms position of the note
-                pos_ratio = ((data.pos - measure_tja.pos_start) /
+                pos_ratio = ((note_tja.pos - measure_tja.pos_start) /
                              (measure_tja.pos_end - measure_tja.pos_start))
-                note_pos = (measure_fumen.duration * pos_ratio)
+                note_pos = measure_fumen.duration * pos_ratio
 
                 # Handle '8' notes (end of a drumroll/balloon)
-                if data.value == "EndDRB":
+                if note_tja.value == "EndDRB":
+                    if not current_drumroll.note_type:
+                        raise ValueError(
+                            "'8' note encountered without matching "
+                            "drumroll/balloon/kusudama note."
+                        )
                     # If a drumroll spans a single measure, then add the
                     # difference between start/end position
                     if not current_drumroll.multimeasure:
                         current_drumroll.duration += (note_pos -
                                                       current_drumroll.pos)
                     # Otherwise, if a drumroll spans multiple measures,
                     # then we want to add the duration between the start
                     # of the measure and the drumroll's end position.
                     else:
                         current_drumroll.duration += (note_pos - 0.0)
                     current_drumroll.duration = float(int(
                         current_drumroll.duration
                     ))
-                    current_drumroll = None
+                    current_drumroll = FumenNote()
                     continue
 
                 # The TJA spec technically allows you to place
                 # double-Kusudama notes. But this is unsupported in
                 # fumens, so just skip the second Kusudama note.
-                if data.value == "Kusudama" and current_drumroll:
+                if note_tja.value == "Kusudama" and current_drumroll.note_type:
                     continue
 
-                # Handle note metadata
+                # Now that the edge cases have been taken care of ('continue'),
+                # we can initialize a note and handle general note metadata.
                 note = FumenNote()
                 note.pos = note_pos
-                note.note_type = data.value
+                note.note_type = note_tja.value
                 note.score_init = tja.score_init
                 note.score_diff = tja.score_diff
 
-                # Handle drumroll notes
-                if note.note_type in ["Balloon", "Kusudama"]:
+                # Handle drumroll-specific note metadata
+                if note.note_type in ["Drumroll", "DRUMROLL"]:
+                    current_drumroll = note
+                elif note.note_type in ["Balloon", "Kusudama"]:
                     try:
                         note.hits = course_balloons.pop(0)
-                    except IndexError:
+                    except IndexError as exc:
                         raise ValueError(f"Not enough values for 'BALLOON: "
-                                         f"{','.join(course_balloons)}'")
-                    current_drumroll = note
-                elif note.note_type in ["Drumroll", "DRUMROLL"]:
+                                         f"{course_balloons}'") from exc
                     current_drumroll = note
 
                 # Track Don/Ka notes (to later compute header values)
                 elif (note.note_type.lower().startswith('don')
                         or note.note_type.lower().startswith('ka')):
                     total_notes[current_branch] += 1
 
                 # Track branch points (to later compute `#BRANCHSTART p` vals)
                 if note.note_type in ['Don', 'Ka']:
-                    pts_to_add = fumen.header.b468_b471_branch_points_good
+                    pts_to_add = fumen.header.b468_b471_branch_pts_good
                 elif note.note_type in ['DON', 'KA']:
-                    pts_to_add = fumen.header.b484_b487_branch_points_good_big
+                    pts_to_add = fumen.header.b484_b487_branch_pts_good_big
                 elif note.note_type == 'Balloon':
-                    pts_to_add = fumen.header.b496_b499_branch_points_balloon
+                    pts_to_add = fumen.header.b496_b499_branch_pts_balloon
                 elif note.note_type == 'Kusudama':
-                    pts_to_add = fumen.header.b500_b503_branch_points_kusudama
+                    pts_to_add = fumen.header.b500_b503_branch_pts_kusudama
                 else:
                     pts_to_add = 0  # Drumrolls not relevant for `p` conditions
                 branch_points_measure += pts_to_add
 
                 # Add the note to the branch for this measure
                 measure_fumen.branches[current_branch].notes.append(note)
                 measure_fumen.branches[current_branch].length += 1
 
             # If drumroll hasn't ended by this measure, increase duration
-            if current_drumroll:
+            if current_drumroll.note_type:
                 # If drumroll spans multiple measures, add full duration
                 if current_drumroll.multimeasure:
                     current_drumroll.duration += measure_fumen.duration
                 # Otherwise, add the partial duration spanned by the drumroll
                 else:
                     current_drumroll.multimeasure = True
                     current_drumroll.duration += (measure_fumen.duration -
@@ -342,37 +366,44 @@
 
     # Compute the header bytes that dictate the soul gauge bar behavior
     fumen.header.set_hp_bytes(total_notes['normal'], tja.course, tja.level)
 
     # If song has only drumroll branching conditions (also allowing percentage
     # conditions that force a level up/level down), then set the header bytes
     # so that only drumrolls contribute to branching.
-    drumroll_only = branch_conditions != [] and all([
-        (cond[0] == 'r') or
-        (cond[0] == 'p' and cond[1] == 0.0 and cond[2] == 0.0) or
-        (cond[0] == 'p' and cond[1] > 1.00 and cond[2] > 1.00)
-        for cond in branch_conditions
-    ])
+    drumroll_only = (
+        branch_types           # noqa: branch_types will always be set
+        and branch_conditions  # noqa: branch_conditions will always be set
+        and all(
+            (branch_type == 'r') or
+            (branch_type == 'p' and cond[0] == 0.0 and cond[1] == 0.0) or
+            (branch_type == 'p' and cond[0] > 1.00 and cond[1] > 1.00)
+            for branch_type, cond in zip(branch_types, branch_conditions)
+        )
+    )
     if drumroll_only:
-        fumen.header.b468_b471_branch_points_good = 0
-        fumen.header.b484_b487_branch_points_good_big = 0
-        fumen.header.b472_b475_branch_points_ok = 0
-        fumen.header.b488_b491_branch_points_ok_big = 0
-        fumen.header.b496_b499_branch_points_balloon = 0
-        fumen.header.b500_b503_branch_points_kusudama = 0
+        fumen.header.b468_b471_branch_pts_good = 0
+        fumen.header.b484_b487_branch_pts_good_big = 0
+        fumen.header.b472_b475_branch_pts_ok = 0
+        fumen.header.b488_b491_branch_pts_ok_big = 0
+        fumen.header.b496_b499_branch_pts_balloon = 0
+        fumen.header.b500_b503_branch_pts_kusudama = 0
 
     # Alternatively, if the song has only percentage-based conditions, then set
     # the header bytes so that only notes and balloons contribute to branching.
-    percentage_only = branch_conditions != [] and all([
-        (condition[0] != 'r')
-        for condition in branch_conditions
-    ])
+    percentage_only = (
+        branch_types  # noqa: branch_types will always be set
+        and all(
+            (branch_type != 'r')
+            for branch_type in branch_types
+        )
+    )
     if percentage_only:
-        fumen.header.b480_b483_branch_points_drumroll = 0
-        fumen.header.b492_b495_branch_points_drumroll_big = 0
+        fumen.header.b480_b483_branch_pts_drumroll = 0
+        fumen.header.b492_b495_branch_pts_drumroll_big = 0
 
     # Compute the ratio between normal and professional/master branches
     if total_notes['professional']:
         fumen.header.b460_b463_normal_professional_ratio = \
             int(65536 * (total_notes['normal'] / total_notes['professional']))
     if total_notes['master']:
         fumen.header.b464_b467_normal_master_ratio = \
```

### Comparing `tja2fumen-0.6.0/src/tja2fumen/hp_values.csv` & `tja2fumen-0.6.1/src/tja2fumen/hp_values.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.6.0/src/tja2fumen/parsers.py` & `tja2fumen-0.6.1/src/tja2fumen/parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,47 @@
+"""
+Functions for parsing TJA files (.tja) and Fumen files (.bin)
+"""
+
 import os
 import re
 import struct
 from copy import deepcopy
+from typing import BinaryIO, Any, List, Dict, Tuple
 
-from tja2fumen.types import (TJASong, TJAMeasure, TJAData, FumenCourse,
-                             FumenMeasure, FumenBranch, FumenNote, FumenHeader)
+from tja2fumen.classes import (TJASong, TJACourse, TJAMeasure, TJAData,
+                               FumenCourse, FumenMeasure, FumenBranch,
+                               FumenNote, FumenHeader)
 from tja2fumen.constants import (NORMALIZE_COURSE, COURSE_NAMES, BRANCH_NAMES,
-                                 TJA_NOTE_TYPES, FUMEN_NOTE_TYPES)
+                                 TJA_COURSE_NAMES, TJA_NOTE_TYPES,
+                                 FUMEN_NOTE_TYPES)
 
 ###############################################################################
 #                          TJA-parsing functions                              #
 ###############################################################################
 
 
-def parse_tja(fname_tja):
+def parse_tja(fname_tja: str) -> TJASong:
     """Read in lines of a .tja file and load them into a TJASong object."""
     try:
-        tja_text = open(fname_tja, "r", encoding="utf-8-sig").read()
+        with open(fname_tja, "r", encoding="utf-8-sig") as tja_file:
+            tja_text = tja_file.read()
     except UnicodeDecodeError:
-        tja_text = open(fname_tja, "r", encoding="shift-jis").read()
+        with open(fname_tja, "r", encoding="shift-jis") as tja_file:
+            tja_text = tja_file.read()
 
     tja_lines = [line for line in tja_text.splitlines() if line.strip() != '']
     tja = split_tja_lines_into_courses(tja_lines)
     for course in tja.courses.values():
-        parse_tja_course_data(course)
+        course.branches = parse_tja_course_data(course.data)
 
     return tja
 
 
-def split_tja_lines_into_courses(lines):
+def split_tja_lines_into_courses(lines: List[str]) -> TJASong:
     """
     Parse TJA metadata in order to split TJA lines into separate courses.
 
     In TJA files, metadata lines are denoted by a colon (':'). These lines
     provide general info about the song (BPM, TITLE, OFFSET, etc.). They also
     define properties for each course in the song (difficulty, level, etc.).
 
@@ -55,35 +64,40 @@
     `parse_tja_course_data()` function.
     """
     # Strip leading/trailing whitespace and comments ('// Comment')
     lines = [line.split("//")[0].strip() for line in lines
              if line.split("//")[0].strip()]
 
     # Initialize song with BPM and OFFSET global metadata
-    bpm = [line.split(":")[1] for line in lines
-           if line.startswith("BPM")][0]
-    offset = [line.split(":")[1] for line in lines
-              if line.startswith("OFFSET")][0]
-    parsed_tja = TJASong(bpm, offset)
+    bpm = float([line.split(":")[1] for line in lines
+                if line.startswith("BPM")][0])
+    offset = float([line.split(":")[1] for line in lines
+                   if line.startswith("OFFSET")][0])
+    parsed_tja = TJASong(
+        bpm=bpm,
+        offset=offset,
+        courses={course: TJACourse(bpm=bpm, offset=offset, course=course)
+                 for course in TJA_COURSE_NAMES}
+    )
 
     current_course = ''
     current_course_basename = ''
     for line in lines:
         # Only metadata and #START commands are relevant for this function
-        match_metadata = re.match(r"^([A-Z]+):(.*)", line)
+        match_metadata = re.match(r"^([A-Z0-9]+):(.*)", line)
         match_start = re.match(r"^#START(?:\s+(.+))?", line)
 
         # Case 1: Metadata lines
         if match_metadata:
             name_upper = match_metadata.group(1).upper()
             value = match_metadata.group(2).strip()
 
             # Course-specific metadata fields
             if name_upper == 'COURSE':
-                if value not in NORMALIZE_COURSE.keys():
+                if value not in NORMALIZE_COURSE:
                     raise ValueError(f"Invalid COURSE value: '{value}'")
                 current_course = NORMALIZE_COURSE[value]
                 current_course_basename = current_course
             elif name_upper == 'LEVEL':
                 if value not in ['1', '2', '3', '4', '5',
                                  '6', '7', '8', '9', '10']:
                     raise ValueError(f"Invalid LEVEL value: '{value}")
@@ -113,15 +127,15 @@
             # chart. But, we want multiplayer charts to inherit the
             # metadata from the course as a whole, so we deepcopy the
             # existing course for that difficulty.
             if value in ["P1", "P2"]:
                 current_course = current_course_basename + value
                 parsed_tja.courses[current_course] = \
                     deepcopy(parsed_tja.courses[current_course_basename])
-                parsed_tja.courses[current_course].data = list()
+                parsed_tja.courses[current_course].data = []
             elif value:
                 raise ValueError(f"Invalid value '{value}' for #START.")
 
             # Since P1/P2 has been handled, we can just use a normal '#START'
             parsed_tja.courses[current_course].data.append("#START")
 
         # Case 3: For other commands and data, simply copy as-is (parse later)
@@ -141,25 +155,21 @@
     for course_name in [k for k, v in parsed_tja.courses.items()
                         if not v.data]:
         del parsed_tja.courses[course_name]
 
     return parsed_tja
 
 
-def parse_tja_course_data(course):
+def parse_tja_course_data(data: List[str]) -> Dict[str, List[TJAMeasure]]:
     """
     Parse course data (notes, commands) into a nested song structure.
 
-    The goal of this function is to take raw note and command strings
-    (e.g. '1020,', '#BPMCHANGE') and parse their values into appropriate
-    types (e.g. lists, ints, floats, etc.).
-
-    This function also processes measure separators (',') and branch commands
-    ('#BRANCHSTART`, '#N`, '#E', '#M') to split the data into branches and
-    measures, resulting in the following structure:
+    The goal of this function is to process measure separators (',') and
+    branch commands ('#BRANCHSTART`, '#N`, '#E', '#M') to split the data
+    into branches and measures, resulting in the following structure:
 
     TJACourse
     ├─ TJABranch ('normal')
     │  ├─ TJAMeasure
     │  │  ├─ TJAData (notes, commands)
     │  │  ├─ TJAData
     │  │  └─ ...
@@ -168,112 +178,109 @@
     │  └─ ...
     ├─ TJABranch ('professional')
     └─ TJABranch ('master')
 
     This provides a faithful, easy-to-inspect tree-style representation of the
     branches and measures within each course of the .tja file.
     """
-    has_branches = bool([d for d in course.data if d.startswith('#BRANCH')])
+    parsed_branches = {k: [TJAMeasure()] for k in BRANCH_NAMES}
+    has_branches = bool([d for d in data if d.startswith('#BRANCH')])
     current_branch = 'all' if has_branches else 'normal'
-    branch_condition = None
+    branch_condition = ''
 
     # Process course lines
     idx_m = 0
     idx_m_branchstart = 0
-    for idx_l, line in enumerate(course.data):
+    for idx_l, line in enumerate(data):
         # 0. Check to see whether line is a command or note data
-        command, value, notes = None, None, None
+        command, name, value, note_data = '', '', '', ''
         match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
         if match_command:
-            command, value = match_command.groups()
+            command = match_command.group(1)
+            if match_command.group(2):
+                value = match_command.group(2)
         else:
-            notes = line  # If not a command, then line must be note data
+            note_data = line  # If not a command, then line must be note data
 
         # 1. Parse measure notes
-        if notes:
+        if note_data:
             # If measure has ended, then add notes to the current measure,
             # then start a new measure by incrementing idx_m
-            if notes.endswith(','):
-                for branch in (course.branches.keys()
-                               if current_branch == 'all'
-                               else [current_branch]):
-                    course.branches[branch][idx_m].notes += notes[0:-1]
-                    course.branches[branch].append(TJAMeasure())
+            if note_data.endswith(','):
+                for branch_name in (BRANCH_NAMES if current_branch == 'all'
+                                    else [current_branch]):
+                    parsed_branches[branch_name][idx_m].notes += note_data[:-1]
+                    parsed_branches[branch_name].append(TJAMeasure())
                 idx_m += 1
             # Otherwise, keep adding notes to the current measure ('idx_m')
             else:
-                for branch in (course.branches.keys()
-                               if current_branch == 'all'
-                               else [current_branch]):
-                    course.branches[branch][idx_m].notes += notes
+                for branch_name in (BRANCH_NAMES if current_branch == 'all'
+                                    else [current_branch]):
+                    parsed_branches[branch_name][idx_m].notes += note_data
 
         # 2. Parse measure commands that produce an "event"
         elif command in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF',
                          'DELAY', 'SCROLL', 'BPMCHANGE', 'MEASURE',
                          'LEVELHOLD', 'SECTION', 'BRANCHSTART']:
             # Get position of the event
-            for branch in (course.branches.keys() if current_branch == 'all'
-                           else [current_branch]):
-                pos = len(course.branches[branch][idx_m].notes)
+            pos = 0
+            for branch_name in (BRANCH_NAMES if current_branch == 'all'
+                                else [current_branch]):
+                pos = len(parsed_branches[branch_name][idx_m].notes)
 
             # Parse event type
             if command == 'GOGOSTART':
-                current_event = TJAData('gogo', '1', pos)
+                name, value = 'gogo', '1'
             elif command == 'GOGOEND':
-                current_event = TJAData('gogo', '0', pos)
+                name, value = 'gogo', '0'
             elif command == 'BARLINEON':
-                current_event = TJAData('barline', '1', pos)
+                name, value = 'barline', '1'
             elif command == 'BARLINEOFF':
-                current_event = TJAData('barline', '0', pos)
+                name, value = 'barline', '0'
             elif command == 'DELAY':
-                current_event = TJAData('delay', float(value), pos)
+                name = 'delay'
             elif command == 'SCROLL':
-                current_event = TJAData('scroll', float(value), pos)
+                name = 'scroll'
             elif command == 'BPMCHANGE':
-                current_event = TJAData('bpm', float(value), pos)
+                name = 'bpm'
             elif command == 'MEASURE':
-                current_event = TJAData('measure', value, pos)
+                name = 'measure'
             elif command == 'LEVELHOLD':
-                current_event = TJAData('levelhold', None, pos)
+                name = 'levelhold'
             elif command == 'SECTION':
                 # If #SECTION occurs before a #BRANCHSTART, then ensure that
                 # it's present on every branch. Otherwise, #SECTION will only
                 # be present on the current branch, and so the `branch_info`
                 # values won't be correctly set for the other two branches.
-                if course.data[idx_l+1].startswith('#BRANCHSTART'):
-                    current_event = TJAData('section', None, pos)
+                if data[idx_l+1].startswith('#BRANCHSTART'):
+                    name = 'section'
                     current_branch = 'all'
                 # Otherwise, #SECTION exists in isolation. In this case, to
                 # reset the accuracy, we just repeat the previous #BRANCHSTART.
                 else:
-                    current_event = TJAData('branch_start', branch_condition,
-                                            pos)
+                    name, value = 'branch_start', branch_condition
             elif command == 'BRANCHSTART':
                 # Ensure that the #BRANCHSTART command is added to all branches
                 current_branch = 'all'
-                branch_condition = value.split(',')
-                if branch_condition[0] == 'r':  # r = drumRoll
-                    branch_condition[1] = int(branch_condition[1])  # drumrolls
-                    branch_condition[2] = int(branch_condition[2])  # drumrolls
-                elif branch_condition[0] == 'p':  # p = Percentage
-                    branch_condition[1] = float(branch_condition[1]) / 100  # %
-                    branch_condition[2] = float(branch_condition[2]) / 100  # %
-                current_event = TJAData('branch_start', branch_condition, pos)
+                name = 'branch_start'
+                branch_condition = value
                 # Preserve the index of the BRANCHSTART command to re-use
                 idx_m_branchstart = idx_m
 
             # Append event to the current measure's events
-            for branch in (course.branches.keys() if current_branch == 'all'
-                           else [current_branch]):
-                course.branches[branch][idx_m].events.append(current_event)
+            for branch_name in (BRANCH_NAMES if current_branch == 'all'
+                                else [current_branch]):
+                parsed_branches[branch_name][idx_m].events.append(
+                    TJAData(name=name, value=value, pos=pos)
+                )
 
         # 3. Parse commands that don't create an event
         #    (e.g. simply changing the current branch)
         else:
-            if command == 'START' or command == 'END':
+            if command in ('START', 'END'):
                 current_branch = 'all' if has_branches else 'normal'
             elif command == 'N':
                 current_branch = 'normal'
                 idx_m = idx_m_branchstart
             elif command == 'E':
                 current_branch = 'professional'
                 idx_m = idx_m_branchstart
@@ -284,22 +291,22 @@
                 current_branch = 'all'
 
             else:
                 print(f"Ignoring unsupported command '{command}'")
 
     # Delete the last measure in the branch if no notes or events
     # were added to it (due to preallocating empty measures)
-    for branch in course.branches.values():
+    for branch in parsed_branches.values():
         if not branch[-1].notes and not branch[-1].events:
             del branch[-1]
 
     # Merge measure data and measure events in chronological order
-    for branch_name, branch in course.branches.items():
+    for branch_name, branch in parsed_branches.items():
         for measure in branch:
-            notes = [TJAData('note', TJA_NOTE_TYPES[note], i)
+            notes = [TJAData(name='note', value=TJA_NOTE_TYPES[note], pos=i)
                      for i, note in enumerate(measure.notes) if
                      TJA_NOTE_TYPES[note] != 'Blank']
             events = measure.events
             while notes or events:
                 if events and notes:
                     if notes[0].pos >= events[0].pos:
                         measure.combined.append(events.pop(0))
@@ -308,28 +315,31 @@
                 elif events:
                     measure.combined.append(events.pop(0))
                 elif notes:
                     measure.combined.append(notes.pop(0))
 
     # Ensure all branches have the same number of measures
     if has_branches:
-        if len(set([len(b) for b in course.branches.values()])) != 1:
+        if len({len(b) for b in parsed_branches.values()}) != 1:
             raise ValueError(
                 "Branches do not have the same number of measures. (This "
                 "check was performed prior to splitting up the measures due "
                 "to mid-measure commands. Please check the number of ',' you"
                 "have in each branch.)"
             )
 
+    return parsed_branches
+
 
 ###############################################################################
 #                          Fumen-parsing functions                            #
 ###############################################################################
 
-def parse_fumen(fumen_file, exclude_empty_measures=False):
+def parse_fumen(fumen_file: str,
+                exclude_empty_measures: bool = False) -> FumenCourse:
     """
     Parse bytes of a fumen .bin file into nested measures, branches, and notes.
 
     Fumen files use a very strict file structure. Certain values are expected
     at very specific byte locations in the file. Here, we parse these specific
     byte locations into the following structure:
 
@@ -346,114 +356,111 @@
     │  │  └─ ...
     │  ├─ FumenBranch ('professional')
     │  └─ FumenBranch ('master')
     ├─ FumenMeasure
     ├─ FumenMeasure
     └─ ...
     """
-    file = open(fumen_file, "rb")
-    size = os.fstat(file.fileno()).st_size
-
-    song = FumenCourse(
-        header=FumenHeader(raw_bytes=file.read(520))
-    )
+    with open(fumen_file, "rb") as file:
+        size = os.fstat(file.fileno()).st_size
 
-    for measure_number in range(song.header.b512_b515_number_of_measures):
-        # Parse the measure data using the following `format_string`:
-        #   "ffBBHiiiiiii" (12 format characters, 40 bytes per measure)
-        #     - 'f': BPM               (one float (4 bytes))
-        #     - 'f': fumenOffset       (one float (4 bytes))
-        #     - 'B': gogo              (one unsigned char (1 byte))
-        #     - 'B': barline           (one unsigned char (1 byte))
-        #     - 'H': <padding>         (one unsigned short (2 bytes))
-        #     - 'iiiiii': branch_info  (six integers (24 bytes))
-        #     - 'i': <padding>         (one integer (4 bytes)
-        measure_struct = read_struct(file, song.header.order,
-                                     format_string="ffBBHiiiiiii")
-
-        # Create the measure dictionary using the newly-parsed measure data
-        measure = FumenMeasure(
-            bpm=measure_struct[0],
-            offset_start=measure_struct[1],
-            gogo=measure_struct[2],
-            barline=measure_struct[3],
-            padding1=measure_struct[4],
-            branch_info=list(measure_struct[5:11]),
-            padding2=measure_struct[11]
-        )
+        header = FumenHeader()
+        header.parse_header_values(file.read(520))
+        song = FumenCourse(header=header)
 
-        # Iterate through the three branch types
-        for branch_name in BRANCH_NAMES:
+        for _ in range(song.header.b512_b515_number_of_measures):
             # Parse the measure data using the following `format_string`:
-            #   "HHf" (3 format characters, 8 bytes per branch)
-            #     - 'H': total_notes ( one unsigned short (2 bytes))
-            #     - 'H': <padding>  ( one unsigned short (2 bytes))
-            #     - 'f': speed      ( one float (4 bytes)
-            branch_struct = read_struct(file, song.header.order,
-                                        format_string="HHf")
-
-            # Create the branch dictionary using the newly-parsed branch data
-            total_notes = branch_struct[0]
-            branch = FumenBranch(
-                length=total_notes,
-                padding=branch_struct[1],
-                speed=branch_struct[2],
+            #   "ffBBHiiiiiii" (12 format characters, 40 bytes per measure)
+            #     - 'f': BPM               (one float (4 bytes))
+            #     - 'f': fumenOffset       (one float (4 bytes))
+            #     - 'B': gogo              (one unsigned char (1 byte))
+            #     - 'B': barline           (one unsigned char (1 byte))
+            #     - 'H': <padding>         (one unsigned short (2 bytes))
+            #     - 'iiiiii': branch_info  (six integers (24 bytes))
+            #     - 'i': <padding>         (one integer (4 bytes)
+            measure_struct = read_struct(file, song.header.order,
+                                         format_string="ffBBHiiiiiii")
+
+            # Create the measure dictionary using the newly-parsed measure data
+            measure = FumenMeasure(
+                bpm=measure_struct[0],
+                offset_start=measure_struct[1],
+                gogo=bool(measure_struct[2]),
+                barline=bool(measure_struct[3]),
+                padding1=measure_struct[4],
+                branch_info=list(measure_struct[5:11]),
+                padding2=measure_struct[11]
             )
 
-            # Iterate through each note in the measure (per branch)
-            for note_number in range(total_notes):
-                # Parse the note data using the following `format_string`:
-                #   "ififHHf" (7 format characters, 24 bytes per note cluster)
-                #     - 'i': note type
-                #     - 'f': note position
-                #     - 'i': item
-                #     - 'f': <padding>
-                #     - 'H': score_init
-                #     - 'H': score_diff
-                #     - 'f': duration
-                # NB: 'item' doesn't seem to be used at all in this function.
-                note_struct = read_struct(file, song.header.order,
-                                          format_string="ififHHf")
-
-                # Create the note dictionary using the newly-parsed note data
-                note_type = note_struct[0]
-                note = FumenNote(
-                    note_type=FUMEN_NOTE_TYPES[note_type],
-                    pos=note_struct[1],
-                    item=note_struct[2],
-                    padding=note_struct[3],
+            # Iterate through the three branch types
+            for branch_name in BRANCH_NAMES:
+                # Parse the measure data using the following `format_string`:
+                #   "HHf" (3 format characters, 8 bytes per branch)
+                #     - 'H': total_notes ( one unsigned short (2 bytes))
+                #     - 'H': <padding>  ( one unsigned short (2 bytes))
+                #     - 'f': speed      ( one float (4 bytes)
+                branch_struct = read_struct(file, song.header.order,
+                                            format_string="HHf")
+
+                # Create the branch dictionary using newly-parsed branch data
+                total_notes = branch_struct[0]
+                branch = FumenBranch(
+                    length=total_notes,
+                    padding=branch_struct[1],
+                    speed=branch_struct[2],
                 )
 
-                if note_type == 0xa or note_type == 0xc:
-                    # Balloon hits
-                    note.hits = note_struct[4]
-                    note.hits_padding = note_struct[5]
-                else:
-                    song.score_init = note.score_init = note_struct[4]
-                    song.score_diff = note.score_diff = note_struct[5] // 4
-
-                # Drumroll/balloon duration
-                note.duration = note_struct[6]
-
-                # Account for padding at the end of drumrolls
-                if note_type == 0x6 or note_type == 0x9 or note_type == 0x62:
-                    note.drumroll_bytes = file.read(8)
-
-                # Assign the note to the branch
-                branch.notes.append(note)
-
-            # Assign the branch to the measure
-            measure.branches[branch_name] = branch
+                # Iterate through each note in the measure (per branch)
+                for _ in range(total_notes):
+                    # Parse the note data using the following `format_string`:
+                    #   "ififHHf" (7 format characters, 24b per note cluster)
+                    #     - 'i': note type
+                    #     - 'f': note position
+                    #     - 'i': item
+                    #     - 'f': <padding>
+                    #     - 'H': score_init
+                    #     - 'H': score_diff
+                    #     - 'f': duration
+                    note_struct = read_struct(file, song.header.order,
+                                              format_string="ififHHf")
+
+                    # Create the note dictionary using newly-parsed note data
+                    note_type = note_struct[0]
+                    note = FumenNote(
+                        note_type=FUMEN_NOTE_TYPES[note_type],
+                        pos=note_struct[1],
+                        item=note_struct[2],
+                        padding=note_struct[3],
+                    )
+
+                    if note_type in (0xa, 0xc):
+                        # Balloon hits
+                        note.hits = note_struct[4]
+                        note.hits_padding = note_struct[5]
+                    else:
+                        song.score_init = note.score_init = note_struct[4]
+                        song.score_diff = note.score_diff = note_struct[5] // 4
 
-        # Assign the measure to the song
-        song.measures.append(measure)
-        if file.tell() >= size:
-            break
+                    # Drumroll/balloon duration
+                    note.duration = note_struct[6]
 
-    file.close()
+                    # Account for padding at the end of drumrolls
+                    if note_type in (0x6, 0x9, 0x62):
+                        note.drumroll_bytes = file.read(8)
+
+                    # Assign the note to the branch
+                    branch.notes.append(note)
+
+                # Assign the branch to the measure
+                measure.branches[branch_name] = branch
+
+            # Assign the measure to the song
+            song.measures.append(measure)
+            if file.tell() >= size:
+                break
 
     # NB: Official fumens often include empty measures as a way of inserting
     # barlines for visual effect. But, TJA authors tend not to add these empty
     # measures, because even without them, the song plays correctly. So, in
     # tests, if we want to only compare the timing of the non-empty measures
     # between an official fumen and a converted non-official TJA, then it's
     # useful to exclude the empty measures.
@@ -462,15 +469,17 @@
                          if m.branches['normal'].length
                          or m.branches['professional'].length
                          or m.branches['master'].length]
 
     return song
 
 
-def read_struct(file, order, format_string, seek=None):
+def read_struct(file: BinaryIO,
+                order: str,
+                format_string: str) -> Tuple[Any, ...]:
     """
     Interpret bytes as packed binary data.
 
     Arguments:
         - file: The fumen's file object (presumably in 'rb' mode).
         - order: '<' or '>' (little or big endian).
         - format_string: String made up of format characters that describes
@@ -478,16 +487,14 @@
           (https://docs.python.org/3/library/struct.html#format-characters)
         - seek: The position of the read pointer to be used within the file.
 
     Return values:
         - interpreted_string: A string containing interpreted byte values,
                               based on the specified 'fmt' format characters.
     """
-    if seek:
-        file.seek(seek)
     expected_size = struct.calcsize(order + format_string)
     byte_string = file.read(expected_size)
     # One "official" fumen (AC11\deo\deo_n.bin) runs out of data early
     # This workaround fixes the issue by appending 0's to get the size to match
     if len(byte_string) != expected_size:
         byte_string += (b'\x00' * (expected_size - len(byte_string)))
     interpreted_string = struct.unpack(order + format_string, byte_string)
```

### Comparing `tja2fumen-0.6.0/src/tja2fumen/writers.py` & `tja2fumen-0.6.1/src/tja2fumen/writers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,61 @@
+"""
+Functions for writing song data to fumen files (.bin)
+"""
+
 import struct
+from typing import BinaryIO, Any, List
 
+from tja2fumen.classes import FumenCourse
 from tja2fumen.constants import BRANCH_NAMES, FUMEN_TYPE_NOTES
 
 
-def write_fumen(path_out, song):
+def write_fumen(path_out: str, song: FumenCourse) -> None:
     """
     Write the values in a FumenCourse object to a `.bin` file.
 
     This operation is the reverse of the `parse_fumen` function. Please refer
     to that function for more details about the fumen file structure.
     """
     with open(path_out, "wb") as file:
         file.write(song.header.raw_bytes)
 
-        for measure_number in range(len(song.measures)):
-            measure = song.measures[measure_number]
+        for measure in song.measures:
             measure_struct = ([measure.bpm, measure.offset_start,
                                int(measure.gogo), int(measure.barline),
                                measure.padding1] + measure.branch_info +
                               [measure.padding2])
             write_struct(file, song.header.order,
                          format_string="ffBBHiiiiiii",
                          value_list=measure_struct)
 
-            for branch_number in range(len(BRANCH_NAMES)):
-                branch = measure.branches[BRANCH_NAMES[branch_number]]
+            for branch_name in BRANCH_NAMES:
+                branch = measure.branches[branch_name]
                 branch_struct = [branch.length, branch.padding, branch.speed]
                 write_struct(file, song.header.order,
                              format_string="HHf",
                              value_list=branch_struct)
 
-                for note_number in range(branch.length):
-                    note = branch.notes[note_number]
+                for note in branch.notes:
                     note_struct = [FUMEN_TYPE_NOTES[note.note_type], note.pos,
                                    note.item, note.padding]
                     if note.hits:
                         extra_vals = [note.hits, note.hits_padding]
                     else:
                         extra_vals = [note.score_init, note.score_diff * 4]
-                    note_struct.extend(extra_vals + [note.duration])
+                    note_struct.extend(extra_vals)
+                    note_struct.append(note.duration)
                     write_struct(file, song.header.order,
                                  format_string="ififHHf",
                                  value_list=note_struct)
 
                     if note.note_type.lower() == "drumroll":
                         file.write(note.drumroll_bytes)
 
 
-def write_struct(file, order, format_string, value_list, seek=None):
+def write_struct(file: BinaryIO,
+                 order: str,
+                 format_string: str,
+                 value_list: List[Any]) -> None:
     """Pack (int, float, etc.) values into a string of bytes, then write."""
-    if seek:
-        file.seek(seek)
     packed_bytes = struct.pack(order + format_string, *value_list)
     file.write(packed_bytes)
```

### Comparing `tja2fumen-0.6.0/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.6.1/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.6.0
+Version: 0.6.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -44,16 +44,25 @@
   tja2fumen is a tool that allows you to convert TJA charts (<code>.tja</code>) to fumen charts (<code>.bin</code>).
 </p>
 
 <p align="center">
   <a href="https://github.com/vivaria/tja2fumen/actions/workflows/test_and_publish_release.yml?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/vivaria/tja2fumen/test_and_publish_release.yml?label=Tests" alt="Test status (main branch)"></a>
   <a href="https://github.com/vivaria/tja2fumen/releases/latest"><img src="https://img.shields.io/github/v/release/vivaria/tja2fumen" alt="GitHub release (with filter)"></a>
   <a href="https://github.com/vivaria/tja2fumen/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License"></a>
+  <a href="https://github.com/pylint-dev/pylint"><img src="https://img.shields.io/badge/Linting-pylint-black" alt="Linting pylint"></a>
+  <a href="https://github.com/PyCQA/flake8"><img src="https://img.shields.io/badge/Linting-flake8-black" alt="Linting flake8"></a>
+  <a href="https://github.com/python/mypy"><img src="https://img.shields.io/badge/Typing-mypy-black" alt="Linting mypy"></a>
 </p>
 
+<p align="center">
+
+
+</p>
+
+
 
 ----
 
 ## Features
 
 - Parse `.tja` chart files.
 - Convert parsed TJA song data into fumen chart data.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tja2fumen Version: 0.6.0 Summary: Convert TJA chart
+Metadata-Version: 2.1 Name: tja2fumen Version: 0.6.1 Summary: Convert TJA chart
 files into fumen (.bin) chart files License: MIT License Copyright (c) 2023
 Vivaria Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
@@ -19,14 +19,15 @@
 tja2fumen/ Keywords: taiko,tatsujin,fumen,TJA Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE.txt  
                      [tja2fumen â TJA chart converter]
    tja2fumen is a tool that allows you to convert TJA charts (.tja) to fumen
                                 charts (.bin).
    [Test_status_(main_branch)] [GitHub_release_(with_filter)] [MIT_License]
+               [Linting_pylint] [Linting_flake8] [Linting_mypy]
 ---- ## Features - Parse `.tja` chart files. - Convert parsed TJA song data
 into fumen chart data. - Write fumen chart data to `.bin` files. - Decode
 official fumen `.bin` files. ## Usage tja2fumen is included as part of several
 existing projects. So, you may be using tja2fumen already! - **XB1/TDMX**:
 [TakoTako](https://github.com/fluto/takotako) converts both chart and audio
 files for XB1/TDMX. - **Nijiro**: [TaikoSoundEditor](https://github.com/
 NotImplementedLife/TaikoSoundEditor) converts both chart and audio files for
```

