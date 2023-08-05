# Comparing `tmp/pytypos-1.3.0.tar.gz` & `tmp/pytypos-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytypos-1.3.0.tar", last modified: Sat Dec  3 16:40:51 2022, max compression
+gzip compressed data, was "pytypos-1.4.0.tar", last modified: Sat Aug  5 13:49:52 2023, max compression
```

## Comparing `pytypos-1.3.0.tar` & `pytypos-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-12-03 16:40:51.629057 pytypos-1.3.0/
--rw-rw-rw-   0        0        0     1070 2022-12-03 16:16:13.000000 pytypos-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     5158 2022-12-03 16:40:51.629057 pytypos-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4101 2022-12-03 16:22:52.000000 pytypos-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2022-12-03 16:40:51.619084 pytypos-1.3.0/pytypos/
--rw-rw-rw-   0        0        0      568 2022-12-03 16:28:36.000000 pytypos-1.3.0/pytypos/__info__.py
--rw-rw-rw-   0        0        0      574 2022-12-03 16:17:04.000000 pytypos-1.3.0/pytypos/__init__.py
--rw-rw-rw-   0        0        0     8855 2022-12-03 16:19:43.000000 pytypos-1.3.0/pytypos/_pytypos.py
--rw-rw-rw-   0        0        0      156 2022-12-03 16:17:04.000000 pytypos-1.3.0/pytypos/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-12-03 16:40:51.627062 pytypos-1.3.0/pytypos.egg-info/
--rw-rw-rw-   0        0        0     5158 2022-12-03 16:40:51.000000 pytypos-1.3.0/pytypos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2022-12-03 16:40:51.000000 pytypos-1.3.0/pytypos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-03 16:40:51.000000 pytypos-1.3.0/pytypos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-12-03 16:40:51.000000 pytypos-1.3.0/pytypos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-03 16:40:51.000000 pytypos-1.3.0/pytypos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-12-03 16:40:51.000000 pytypos-1.3.0/pytypos.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2022-12-03 16:40:51.630055 pytypos-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1554 2022-12-03 16:17:04.000000 pytypos-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:49:52.367743 pytypos-1.4.0/
+-rw-rw-rw-   0        0        0     1070 2022-12-03 16:16:13.000000 pytypos-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5321 2023-08-05 13:49:52.366745 pytypos-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4263 2023-02-19 14:36:32.000000 pytypos-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 13:49:52.351786 pytypos-1.4.0/pytypos/
+-rw-rw-rw-   0        0        0      568 2023-08-05 13:47:12.000000 pytypos-1.4.0/pytypos/__info__.py
+-rw-rw-rw-   0        0        0      574 2022-12-03 16:17:04.000000 pytypos-1.4.0/pytypos/__init__.py
+-rw-rw-rw-   0        0        0     8837 2023-04-19 11:32:25.000000 pytypos-1.4.0/pytypos/_pytypos.py
+-rw-rw-rw-   0        0        0      156 2022-12-03 16:17:04.000000 pytypos-1.4.0/pytypos/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:49:52.364750 pytypos-1.4.0/pytypos.egg-info/
+-rw-rw-rw-   0        0        0     5321 2023-08-05 13:49:52.000000 pytypos-1.4.0/pytypos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-08-05 13:49:52.000000 pytypos-1.4.0/pytypos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 13:49:52.000000 pytypos-1.4.0/pytypos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-05 13:49:52.000000 pytypos-1.4.0/pytypos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 13:49:52.000000 pytypos-1.4.0/pytypos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-05 13:49:52.000000 pytypos-1.4.0/pytypos.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-08-05 13:49:52.368739 pytypos-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2022-12-03 16:17:04.000000 pytypos-1.4.0/setup.py
```

### Comparing `pytypos-1.3.0/LICENSE` & `pytypos-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytypos-1.3.0/PKG-INFO` & `pytypos-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytypos
-Version: 1.3.0
+Version: 1.4.0
 Summary: Typo and spelling checker
 Home-page: https://github.com/PApostol/pytypos
 Author: PApostol
 Author-email: foo@bar.com
 Maintainer: PApostol
 License: MIT
 Keywords: typo,spell,check
@@ -26,15 +26,16 @@
 License-File: LICENSE
 
 ## Pytypos
 
 [![PyPI version](https://badge.fury.io/py/pytypos.svg)](https://badge.fury.io/py/pytypos)
 [![Downloads](https://static.pepy.tech/personalized-badge/pytypos?period=month&units=international_system&left_color=grey&right_color=yellowgreen&left_text=total%20downloads)](https://pepy.tech/project/pytypos)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pytypos)](https://pypi.org/project/pytypos/)
-[![](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
+[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Code style: blue](https://img.shields.io/badge/code%20style-blue-blue.svg)](https://blue.readthedocs.io/)
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
 
 ### Description
 Pytypos is a typo and spelling checker used to identify spelling mistakes in comments of a various programming languages,
 such as Python, Java, C++, C#, Matlab, and others. In addition, it can check other text-oriented files such as MD, RST, TXT, or similar.
 
@@ -57,31 +58,31 @@
 
 For usage details check `help(pytypos)`.
 
 ### Usage Examples
 The below will recursively scan `my/path/project/` for comments (i.e. `# this is a comment`) in Python files:
 ```
 from pytypos import Pytypos
-prj = Pytypos(target='my/path/project/', match_identifier='#', file_extension='py', recursive=True)
+prj = Pytypos(target='my/path/project/', match_identifier='#', file_extension='py', recursive=True, suggestions=False)
 prj.find_typos()
 print(prj.typo_list)
 print(prj.typo_details)
 ```
 `Pytypos.typo_list` stores a list of all possible typos found.
 
 `Pytypos.typo_details` stores a dictionary with the following structure:
 
-If `suggestions = False` (default):
+If `suggestions == False` (default):
 ```
 {'file1': ['typo1', 'typo2'],
  'file2': ['typo1', 'typo2']
 }
 ```
 
-If `suggestions = True`:
+If `suggestions == True`:
 ```
 {'file1': [{'typo1': ['suggestion1a', 'suggestion1b'],
             'typo2': ['suggestion2a', 'suggestion2b']
            },
  'file2': [{'typo1': ['suggestion1a', 'suggestion1b'],
             'typo2': ['suggestion2a', 'suggestion2b']
            }
@@ -104,21 +105,21 @@
 
 Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
 
 `python tests/run_integration_test.py`
 
 #### Additional methods
 
-`Pytypos.fix_typos()`: Fixes typos found in-between spaces with the most likely replacement
+`pytypos.Pytypos.fix_typos()`: Fixes typos found in-between spaces with the most likely replacement
 
-`Pytypos.add_to_dictionary()`: Adds custom word list to dictionary
+`pytypos.Pytypos.add_to_dictionary()`: Adds custom word list to dictionary
 
-`Pytypos.add_to_exclusions()`: Removes custom word list from dictionary
+`pytypos.Pytypos.add_to_exclusions()`: Removes custom word list from dictionary
 
-`Pytypos.replace_word()`: Replaces words in dictionary
+`pytypos.Pytypos.replace_word()`: Replaces words in dictionary
 
 ### License
 
 Released under [MIT](/LICENSE) by [@PApostol](https://github.com/PApostol)
 
 - You can freely modify and reuse.
 - The original license must be included with copies of this software.
```

### Comparing `pytypos-1.3.0/README.md` & `pytypos-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ## Pytypos
 
 [![PyPI version](https://badge.fury.io/py/pytypos.svg)](https://badge.fury.io/py/pytypos)
 [![Downloads](https://static.pepy.tech/personalized-badge/pytypos?period=month&units=international_system&left_color=grey&right_color=yellowgreen&left_text=total%20downloads)](https://pepy.tech/project/pytypos)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pytypos)](https://pypi.org/project/pytypos/)
-[![](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
+[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Code style: blue](https://img.shields.io/badge/code%20style-blue-blue.svg)](https://blue.readthedocs.io/)
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
 
 ### Description
 Pytypos is a typo and spelling checker used to identify spelling mistakes in comments of a various programming languages,
 such as Python, Java, C++, C#, Matlab, and others. In addition, it can check other text-oriented files such as MD, RST, TXT, or similar.
 
@@ -30,31 +31,31 @@
 
 For usage details check `help(pytypos)`.
 
 ### Usage Examples
 The below will recursively scan `my/path/project/` for comments (i.e. `# this is a comment`) in Python files:
 ```
 from pytypos import Pytypos
-prj = Pytypos(target='my/path/project/', match_identifier='#', file_extension='py', recursive=True)
+prj = Pytypos(target='my/path/project/', match_identifier='#', file_extension='py', recursive=True, suggestions=False)
 prj.find_typos()
 print(prj.typo_list)
 print(prj.typo_details)
 ```
 `Pytypos.typo_list` stores a list of all possible typos found.
 
 `Pytypos.typo_details` stores a dictionary with the following structure:
 
-If `suggestions = False` (default):
+If `suggestions == False` (default):
 ```
 {'file1': ['typo1', 'typo2'],
  'file2': ['typo1', 'typo2']
 }
 ```
 
-If `suggestions = True`:
+If `suggestions == True`:
 ```
 {'file1': [{'typo1': ['suggestion1a', 'suggestion1b'],
             'typo2': ['suggestion2a', 'suggestion2b']
            },
  'file2': [{'typo1': ['suggestion1a', 'suggestion1b'],
             'typo2': ['suggestion2a', 'suggestion2b']
            }
@@ -77,21 +78,21 @@
 
 Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
 
 `python tests/run_integration_test.py`
 
 #### Additional methods
 
-`Pytypos.fix_typos()`: Fixes typos found in-between spaces with the most likely replacement
+`pytypos.Pytypos.fix_typos()`: Fixes typos found in-between spaces with the most likely replacement
 
-`Pytypos.add_to_dictionary()`: Adds custom word list to dictionary
+`pytypos.Pytypos.add_to_dictionary()`: Adds custom word list to dictionary
 
-`Pytypos.add_to_exclusions()`: Removes custom word list from dictionary
+`pytypos.Pytypos.add_to_exclusions()`: Removes custom word list from dictionary
 
-`Pytypos.replace_word()`: Replaces words in dictionary
+`pytypos.Pytypos.replace_word()`: Replaces words in dictionary
 
 ### License
 
 Released under [MIT](/LICENSE) by [@PApostol](https://github.com/PApostol)
 
 - You can freely modify and reuse.
 - The original license must be included with copies of this software.
```

### Comparing `pytypos-1.3.0/pytypos/__info__.py` & `pytypos-1.4.0/pytypos/__info__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 """
 
 __title__ = 'pytypos'
 __author__ = 'PApostol'
 __author_email__ = 'foo@bar.com'
 __maintainer__ = 'PApostol'
 __license__ = 'MIT'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 __description__ = 'Typo and spelling checker'
 __url__ = f'https://github.com/{__author__}/{__title__}'
 __bugtrack_url__ = f'{__url__}/issues'
```

### Comparing `pytypos-1.3.0/pytypos/__init__.py` & `pytypos-1.4.0/pytypos/__init__.py`

 * *Files identical despite different names*

### Comparing `pytypos-1.3.0/pytypos/_pytypos.py` & `pytypos-1.4.0/pytypos/_pytypos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Pytypos class functionality"""
 import codecs
 import glob
 import logging
 import os
 import re
 from itertools import chain
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Set
 
 import enchant
 
 from .exceptions import SuggestionsNotFound
 
 
 class Pytypos:
@@ -38,14 +38,16 @@
 
         Scan the "a/b/c.java" Java file for comments (i.e. "// this is a comment") and give suggestions with a french dictionary, but exclude words found in "exclusions.txt"
         `Pytypos(target='a/b/c.java', match_identifier='//', dictionary='fr', suggestions=True, exclude_word_file='exclusions.txt')`
 
         Note: you can only use dictionaries that you have installed. Pytypos uses dictionaries from PyEnchant: https://pyenchant.github.io/pyenchant/
     """
 
+    strip_chars: Set[str] = {'.', ',', ';', '?', '(', ')', '&', '"', "'", '{', '}', '@', '[', ']', '#'}
+
     def __init__(
         self,
         *,
         target: str,
         match_identifier: str = '#',
         file_extension: str = 'py',
         recursive: bool = False,
@@ -125,16 +127,15 @@
         logging.info('Word mappings replaced.')
 
     def _match_from_file(self, file: str) -> List[str]:
         with codecs.open(file, 'r', encoding='utf-8') as f:
             content = f.read()
 
         matches = re.findall(self.re_match, content)
-        strip_chars = {'.', ',', ';', '?', '(', ')', '&', '"', "'", '{', '}', '@', '[', ']', '#'}
-        strip_str = ''.join(list(strip_chars))
+        strip_str = ''.join(list(self.strip_chars))
         return list(
             set(word.strip(strip_str) for match in matches for word in match.split() if word.strip(strip_str).isalpha())
         )
 
     def _find_files(self) -> List[str]:
         if os.path.isfile(self.target):
             files = [self.target]
@@ -189,18 +190,18 @@
             None
         """
         if not self.suggestions:
             raise SuggestionsNotFound('No suggestions exist, please re-check for typos with `suggestions=True`.')
 
         if not self.typo_details:
             logging.info('No typos to fix.')
-        else:
-            for file, typo_list in self.typo_details.items():
-                with codecs.open(file, 'r+', encoding='utf-8') as f:
-                    content = f.read()
-                    f.seek(0)
-                    for entry in typo_list:
-                        for typo, suggestions in entry.items():
-                            content = content.replace(f' {typo} ', f' {suggestions[0]} ')
-                    f.write(content)
-                    f.truncate()
-            logging.info('Typos fixed with the most likely replacement.')
+            return
+        for file, typo_list in self.typo_details.items():
+            with codecs.open(file, 'r+', encoding='utf-8') as f:
+                content = f.read()
+                f.seek(0)
+                for entry in typo_list:
+                    for typo, suggestions in entry.items():
+                        content = content.replace(f' {typo} ', f' {suggestions[0]} ')
+                f.write(content)
+                f.truncate()
+        logging.info('Typos fixed with the most likely replacement.')
```

### Comparing `pytypos-1.3.0/pytypos.egg-info/PKG-INFO` & `pytypos-1.4.0/pytypos.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytypos
-Version: 1.3.0
+Version: 1.4.0
 Summary: Typo and spelling checker
 Home-page: https://github.com/PApostol/pytypos
 Author: PApostol
 Author-email: foo@bar.com
 Maintainer: PApostol
 License: MIT
 Keywords: typo,spell,check
@@ -26,15 +26,16 @@
 License-File: LICENSE
 
 ## Pytypos
 
 [![PyPI version](https://badge.fury.io/py/pytypos.svg)](https://badge.fury.io/py/pytypos)
 [![Downloads](https://static.pepy.tech/personalized-badge/pytypos?period=month&units=international_system&left_color=grey&right_color=yellowgreen&left_text=total%20downloads)](https://pepy.tech/project/pytypos)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pytypos)](https://pypi.org/project/pytypos/)
-[![](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
+[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Code style: blue](https://img.shields.io/badge/code%20style-blue-blue.svg)](https://blue.readthedocs.io/)
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
 
 ### Description
 Pytypos is a typo and spelling checker used to identify spelling mistakes in comments of a various programming languages,
 such as Python, Java, C++, C#, Matlab, and others. In addition, it can check other text-oriented files such as MD, RST, TXT, or similar.
 
@@ -57,31 +58,31 @@
 
 For usage details check `help(pytypos)`.
 
 ### Usage Examples
 The below will recursively scan `my/path/project/` for comments (i.e. `# this is a comment`) in Python files:
 ```
 from pytypos import Pytypos
-prj = Pytypos(target='my/path/project/', match_identifier='#', file_extension='py', recursive=True)
+prj = Pytypos(target='my/path/project/', match_identifier='#', file_extension='py', recursive=True, suggestions=False)
 prj.find_typos()
 print(prj.typo_list)
 print(prj.typo_details)
 ```
 `Pytypos.typo_list` stores a list of all possible typos found.
 
 `Pytypos.typo_details` stores a dictionary with the following structure:
 
-If `suggestions = False` (default):
+If `suggestions == False` (default):
 ```
 {'file1': ['typo1', 'typo2'],
  'file2': ['typo1', 'typo2']
 }
 ```
 
-If `suggestions = True`:
+If `suggestions == True`:
 ```
 {'file1': [{'typo1': ['suggestion1a', 'suggestion1b'],
             'typo2': ['suggestion2a', 'suggestion2b']
            },
  'file2': [{'typo1': ['suggestion1a', 'suggestion1b'],
             'typo2': ['suggestion2a', 'suggestion2b']
            }
@@ -104,21 +105,21 @@
 
 Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
 
 `python tests/run_integration_test.py`
 
 #### Additional methods
 
-`Pytypos.fix_typos()`: Fixes typos found in-between spaces with the most likely replacement
+`pytypos.Pytypos.fix_typos()`: Fixes typos found in-between spaces with the most likely replacement
 
-`Pytypos.add_to_dictionary()`: Adds custom word list to dictionary
+`pytypos.Pytypos.add_to_dictionary()`: Adds custom word list to dictionary
 
-`Pytypos.add_to_exclusions()`: Removes custom word list from dictionary
+`pytypos.Pytypos.add_to_exclusions()`: Removes custom word list from dictionary
 
-`Pytypos.replace_word()`: Replaces words in dictionary
+`pytypos.Pytypos.replace_word()`: Replaces words in dictionary
 
 ### License
 
 Released under [MIT](/LICENSE) by [@PApostol](https://github.com/PApostol)
 
 - You can freely modify and reuse.
 - The original license must be included with copies of this software.
```

### Comparing `pytypos-1.3.0/setup.py` & `pytypos-1.4.0/setup.py`

 * *Files identical despite different names*

