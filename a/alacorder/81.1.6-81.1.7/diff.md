# Comparing `tmp/alacorder-81.1.6.tar.gz` & `tmp/alacorder-81.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-81.1.6.tar", max compression
+gzip compressed data, was "alacorder-81.1.7.tar", max compression
```

## Comparing `alacorder-81.1.6.tar` & `alacorder-81.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.1.6/LICENSE
--rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.1.6/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 02:07:06.233018 alacorder-81.1.6/alacorder/.DS_Store
--rw-r--r--   0        0        0       72 2023-08-04 20:41:53.084285 alacorder-81.1.6/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.1.6/alacorder/__init__.py
--rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.1.6/alacorder/__main__.py
--rw-r--r--   0        0        0   275789 2023-08-05 02:11:52.587094 alacorder-81.1.6/alacorder/alac.py
--rw-r--r--   0        0        0      557 2023-08-05 02:11:55.779439 alacorder-81.1.6/pyproject.toml
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.1.7/LICENSE
+-rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.1.7/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 02:07:06.233018 alacorder-81.1.7/alacorder/.DS_Store
+-rw-r--r--   0        0        0       72 2023-08-04 20:41:53.084285 alacorder-81.1.7/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.1.7/alacorder/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.1.7/alacorder/__main__.py
+-rw-r--r--   0        0        0   275721 2023-08-05 17:03:15.053822 alacorder-81.1.7/alacorder/alac.py
+-rw-r--r--   0        0        0      557 2023-08-05 17:03:17.890631 alacorder-81.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.1.7/PKG-INFO
```

### Comparing `alacorder-81.1.6/LICENSE` & `alacorder-81.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.6/README.md` & `alacorder-81.1.7/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.6/alacorder/.DS_Store` & `alacorder-81.1.7/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.6/alacorder/alac.py` & `alacorder-81.1.7/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ┣┫┃ ┣┫┃ ┃┃┣┫┃┃┣ ┣┫
 ┛┗┗┛┛┗┗┛┗┛┛┗┻┛┗┛┛┗
 (c) 2023 Sam Robson
 
 Dependencies: Python 3.9+, Google Chrome, brotli 1.0.9+, polars 0.18.1+, pymupdf 1.21.1+, rich 13.3.3+, selenium 4.8.3+, typer 0.9.0+, xlsx2csv 0.8.1+, xlsxwriter 3.0.9+
 """
 
-__version__ = "81.1.6"
+__version__ = "81.1.7"
 
 import os
 import re
 import glob
 import time
 from datetime import datetime
 from pathlib import Path
@@ -1899,16 +1899,15 @@
                         .cast(pl.Categorical)
                         .alias("ArrestingAgencyType"),
                         pl.col("AllPagesText")
                         .str.extract(r"(.+) City Code/Name")
                         .str.strip()
                         .alias("CityCodeName"),
                         pl.col("AllPagesText")
-                        .str.extract(r"Arresting Officer: ([A-Z\s]+)")
-                        .str.replace(r"[\s\n]+[A-Z0-9]$", "")
+                        .str.extract(r"Arresting Officer: (.+)")
                         .str.strip()
                         .alias("ArrestingOfficer"),
                         pl.col("AllPagesText")
                         .str.extract(r"Grand Jury: (.+)")
                         .str.strip()
                         .alias("GrandJury"),
                         pl.col("AllPagesText")
@@ -4229,15 +4228,15 @@
     def financial_history(self, debug=False):
         """
         Make financial history table.
         """
         if debug:
             self._financial_history = None
         # if previously called with debug=True, reset
-        if isinstance(self._restitution, pl.DataFrame):
+        if isinstance(self._financial_history, pl.DataFrame):
             if "Row" in self._financial_history.columns:
                 self._financial_history = None
         if isinstance(self._financial_history, pl.DataFrame):
             return self._financial_history
         else:
             if not self.is_read:
                 self.read()
@@ -4667,18 +4666,18 @@
                         .alias("Recipient"),
                     ]
                 )
                 if not debug:
                     df = df.select(
                         [
                             "CaseNumber",
+                            "Recipient",
                             "Restitution",
                             "Description",
                             "Amount",
-                            "Recipient",
                         ]
                     )
             self._restitution = df
             return self._restitution
 
     def linked_cases(self, debug=False):
         """
@@ -6060,15 +6059,15 @@
     except:
         return ""
 
 
 def getArrestingOfficer(text):
     try:
         return (
-            re.search(r"Arresting Officer: ([A-Z\s]+)", str(text))
+            re.search(r"Arresting Officer: (.+)", str(text))
             .group(1)
             .rstrip("S")
             .rstrip("P")
             .strip()
         )
     except:
         return ""
```

### Comparing `alacorder-81.1.6/pyproject.toml` & `alacorder-81.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "81.1.6"
+version = "81.1.7"
 description = "Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `alacorder-81.1.6/PKG-INFO` & `alacorder-81.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 81.1.6
+Version: 81.1.7
 Summary: Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

