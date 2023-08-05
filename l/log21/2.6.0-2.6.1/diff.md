# Comparing `tmp/log21-2.6.0.tar.gz` & `tmp/log21-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.6.0.tar", last modified: Fri Aug  4 08:40:19 2023, max compression
+gzip compressed data, was "log21-2.6.1.tar", last modified: Sat Aug  5 12:35:25 2023, max compression
```

## Comparing `log21-2.6.0.tar` & `log21-2.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-04 08:40:09.000000 log21-2.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-08-04 08:40:19.659241 log21-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-08-04 08:40:09.000000 log21-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 08:40:09.000000 log21-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:40:19.659241 log21-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.655241 log21-2.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/src/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Argumentify.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/src/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-08-04 08:40:09.000000 log21-2.6.0/src/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:40:19.659241 log21-2.6.0/src/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 08:40:19.000000 log21-2.6.0/src/log21.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:35:25.930298 log21-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-05 12:35:16.000000 log21-2.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-08-05 12:35:25.930298 log21-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-08-05 12:35:16.000000 log21-2.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-05 12:35:16.000000 log21-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:35:25.930298 log21-2.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:35:25.918298 log21-2.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:35:25.926298 log21-2.6.1/src/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/Argumentify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:35:25.930298 log21-2.6.1/src/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26981 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24142 2023-08-05 12:35:16.000000 log21-2.6.1/src/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:35:25.926298 log21-2.6.1/src/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-08-05 12:35:25.000000 log21-2.6.1/src/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-05 12:35:25.000000 log21-2.6.1/src/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:35:25.000000 log21-2.6.1/src/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-05 12:35:25.000000 log21-2.6.1/src/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 12:35:25.000000 log21-2.6.1/src/log21.egg-info/top_level.txt
```

### Comparing `log21-2.6.0/LICENSE.txt` & `log21-2.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.6.0/PKG-INFO` & `log21-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/log21)
@@ -79,17 +80,20 @@
 ```bash
 pip install git+https://github.com/MPCodeWriter21/log21
 ```
 
 Changes
 -------
 
-### 2.6.0
+### 2.6.1
 
-Added the `Argumentify` module. Check the examples.
+Added `encoding` to `log21.CrashReporter.FileReporter`.
+Added configs for `pylint`, `yapf` and `isort` to `pyproject.toml`.
+Added optional `dev` dependencies to `pyproject.toml`.
+Improved overall code quality.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
 
@@ -115,15 +119,15 @@
 logger.error(log21.get_colors('LightRed') + "I'm still here ;1")
 ```
 
 ![Basic Logging](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-1.png)
 
 ----------------
 
-### Argument Parsing (See Also: [Argumentify](https://github.com/MPCodeWriter21/log21#argumentify))
+### Argument Parsing (See Also: [Argumentify](https://github.com/MPCodeWriter21/log21#argumentify-check-out-the-manual-way))
 
 ```python
 import log21
 from log21 import ColorizingArgumentParser, get_logger, get_colors as gc
 
 parser = ColorizingArgumentParser(description="This is a simple example of a ColorizingArgumentParser.",
                                   colors={'help': 'LightCyan'})
@@ -273,15 +277,15 @@
 ```
 
 ![ProgressBar - Example 1](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.1.gif)
 ![ProgressBar - Example 2](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.2.gif)
 
 ------------------
 
-### Argumentify (Check out [the manual way](https://github.com/MPCodeWriter21/log21#argument-parsing))
+### Argumentify (Check out [the manual way](https://github.com/MPCodeWriter21/log21#argumentify-check-out-the-manual-way))
 
 ```python
 # Common Section
 import log21
 
 
 class ReversedText:
```

### Comparing `log21-2.6.0/README.md` & `log21-2.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,20 @@
 ```bash
 pip install git+https://github.com/MPCodeWriter21/log21
 ```
 
 Changes
 -------
 
-### 2.6.0
+### 2.6.1
 
-Added the `Argumentify` module. Check the examples.
+Added `encoding` to `log21.CrashReporter.FileReporter`.
+Added configs for `pylint`, `yapf` and `isort` to `pyproject.toml`.
+Added optional `dev` dependencies to `pyproject.toml`.
+Improved overall code quality.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
 
@@ -93,15 +96,15 @@
 logger.error(log21.get_colors('LightRed') + "I'm still here ;1")
 ```
 
 ![Basic Logging](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-1.png)
 
 ----------------
 
-### Argument Parsing (See Also: [Argumentify](https://github.com/MPCodeWriter21/log21#argumentify))
+### Argument Parsing (See Also: [Argumentify](https://github.com/MPCodeWriter21/log21#argumentify-check-out-the-manual-way))
 
 ```python
 import log21
 from log21 import ColorizingArgumentParser, get_logger, get_colors as gc
 
 parser = ColorizingArgumentParser(description="This is a simple example of a ColorizingArgumentParser.",
                                   colors={'help': 'LightCyan'})
@@ -251,15 +254,15 @@
 ```
 
 ![ProgressBar - Example 1](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.1.gif)
 ![ProgressBar - Example 2](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.2.gif)
 
 ------------------
 
-### Argumentify (Check out [the manual way](https://github.com/MPCodeWriter21/log21#argument-parsing))
+### Argumentify (Check out [the manual way](https://github.com/MPCodeWriter21/log21#argumentify-check-out-the-manual-way))
 
 ```python
 # Common Section
 import log21
 
 
 class ReversedText:
```

### Comparing `log21-2.6.0/pyproject.toml` & `log21-2.6.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -22,16 +22,44 @@
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X"
 ]
 dependencies = [
   "webcolors",
   "docstring-parser"
 ]
-version = "2.6.0"
+version = "2.6.1"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project.urls]
 Homepage = "https://github.com/MPCodeWriter21/log21"
 Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
 Source = "https://github.com/MPCodeWriter21/log21"
+
+[project.optional-dependencies]
+dev = ["yapf", "isort", "docformatter", "pylint"]
+
+[tool.pylint.messages_control]
+max-line-length = 88
+
+disable = [
+  "protected-access",
+  "too-few-public-methods",
+  "too-many-arguments",
+  "too-many-locals",
+  "fixme",
+]
+
+[tool.pylint.design]
+max-returns = 8
+
+[tool.yapf]
+column_limit = 88
+split_before_dot = true
+split_before_first_argument = true
+dedent_closing_brackets = true
+
+[tool.isort]
+line_length = 88
+combine_as_imports = true
+order_by_type = true
```

### Comparing `log21-2.6.0/src/log21/Argparse.py` & `log21-2.6.1/src/log21/Argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # log21.Argparse.py
 # CodeWriter21
 
 import re as _re
 import sys as _sys
-import log21 as _log21
 import argparse as _argparse
-
+from typing import Mapping as _Mapping, Optional as _Optional
 from gettext import gettext as _gettext
 from textwrap import TextWrapper as _TextWrapper
-from typing import Mapping as _Mapping, Optional as _Optional
 
+import log21 as _log21
 from log21.Colors import get_colors as _gc
 from log21.Formatters import DecolorizingFormatter as _Formatter
 
-__all__ = ['ColorizingArgumentParser', 'ColorizingHelpFormatter', 'ColorizingTextWrapper']
+__all__ = [
+    'ColorizingArgumentParser', 'ColorizingHelpFormatter', 'ColorizingTextWrapper'
+]
 
 
 class ColorizingHelpFormatter(_argparse.HelpFormatter):
-    def __init__(self, prog, indent_increment=2, max_help_position=24, width=None,
-                 colors: _Optional[_Mapping[str, str]] = None):
+
+    def __init__(
+        self,
+        prog,
+        indent_increment=2,
+        max_help_position=24,
+        width=None,
+        colors: _Optional[_Mapping[str, str]] = None
+    ):
         super().__init__(prog, indent_increment, max_help_position, width)
-        
+
         self.colors = {
             'usage': 'Cyan',
             'brackets': 'LightRed',
             'switches': 'LightCyan',
             'values': 'Green',
             'colons': 'LightRed',
             'commas': 'LightRed',
@@ -35,14 +43,15 @@
 
         if colors:
             for key, value in colors.items():
                 if key in self.colors:
                     self.colors[key] = value
 
     class _Section(object):
+
         def __init__(self, formatter, parent, heading=None):
             self.formatter = formatter
             self.parent = parent
             self.heading = heading
             self.items = []
 
         def format_help(self):
@@ -63,49 +72,57 @@
                 current_indent = self.formatter._current_indent
                 heading = '%*s%s' % (current_indent, '', self.heading) + _gc(self.formatter.colors['colons']) + \
                           ':\033[0m\n'
             else:
                 heading = ''
 
             # join the section-initial newline, the heading and the help
-            return join(['\n', heading, _gc(self.formatter.colors['help']), item_help, '\n'])
+            return join(
+                ['\n', heading,
+                 _gc(self.formatter.colors['help']), item_help, '\n']
+            )
 
     def _add_item(self, func, args):
         self._current_section.items.append((func, args))
 
     def _fill_text(self, text, width, indent):
         text = self._whitespace_matcher.sub(' ', text).strip()
-        return ColorizingTextWrapper(width=width, initial_indent=indent, subsequent_indent=indent).fill(text)
+        return ColorizingTextWrapper(
+            width=width, initial_indent=indent, subsequent_indent=indent
+        ).fill(text)
 
     def _split_lines(self, text, width):
         text = self._whitespace_matcher.sub(' ', text).strip()
         return ColorizingTextWrapper(width=width).wrap(text)
 
     def start_section(self, heading):
         self._indent()
-        section = self._Section(self, self._current_section,
-                                _gc(self.colors['section headers']) + str(heading) + '\033[0m')
+        section = self._Section(
+            self, self._current_section,
+            _gc(self.colors['section headers']) + str(heading) + '\033[0m'
+        )
         self._add_item(section.format_help, [])
         self._current_section = section
 
     def _format_action(self, action):
         # determine the required width and the entry label
-        help_position = min(self._action_max_length + 2,
-                            self._max_help_position)
+        help_position = min(self._action_max_length + 2, self._max_help_position)
         help_width = max(self._width - help_position, 11)
         action_width = help_position - self._current_indent - 2
         action_header = _gc('rst') + self._format_action_invocation(action)
 
         indent_first = 0
         # no help; start on same line and add a final newline
         if not action.help:
             action_header = self._current_indent * ' ' + action_header + '\n'
         # short action name; start on the same line and pad two spaces
         elif len(action_header) <= action_width:
-            action_header = '%*s%-*s  ' % (self._current_indent, '', action_width, action_header)
+            action_header = '%*s%-*s  ' % (
+                self._current_indent, '', action_width, action_header
+            )
         # long action name; start on the next line
         else:
             action_header = self._current_indent * ' ' + action_header + '\n'
             indent_first = help_position
 
         # collect the pieces of the action help
         parts = [action_header]
@@ -177,15 +194,16 @@
                     lines = []
                     line = []
                     if prefix is not None:
                         line_len = len(prefix) - 1
                     else:
                         line_len = len(indent) - 1
                     for part in parts:
-                        if line_len + 1 + len(_Formatter.decolorize(part)) > text_width and line:
+                        if line_len + 1 + len(_Formatter.decolorize(part)
+                                              ) > text_width and line:
                             lines.append(indent + ' '.join(line))
                             line = []
                             line_len = len(indent) - 1
                         line.append(part)
                         line_len += len(_Formatter.decolorize(part)) + 1
                     if line:
                         lines.append(indent + ' '.join(line))
@@ -293,21 +311,23 @@
                     part = _gc(self.colors['switches']) + action.format_usage()
 
                 # if the Optional takes a value, format is:
                 #    -s ARGS or --long ARGS
                 else:
                     default = self._get_default_metavar_for_optional(action)
                     args_string = self._format_args(action, default)
-                    part = _gc(self.colors['switches']) + '%s %s%s' % (option_string, _gc(self.colors['values']),
-                                                                       args_string)
+                    part = _gc(self.colors['switches']) + '%s %s%s' % (
+                        option_string, _gc(self.colors['values']), args_string
+                    )
 
                 # make it look optional if it's not required or in a group
                 if not action.required and action not in group_actions:
                     part = _gc(self.colors['brackets']) + '[' + part + _gc(
-                        self.colors['brackets']) + ']\033[0m'
+                        self.colors['brackets']
+                    ) + ']\033[0m'
 
                 # add the action string to the list
                 parts.append(part)
 
         # insert things at the necessary indices
         for i in sorted(inserts, reverse=True):
             parts[i:i] = [inserts[i]]
@@ -344,16 +364,18 @@
 
             # if the Optional takes a value, format is:
             #    -s ARGS, --long ARGS
             else:
                 default = self._get_default_metavar_for_optional(action)
                 args_string = self._format_args(action, default)
                 for option_string in action.option_strings:
-                    parts.append(_gc(self.colors['switches']) + '%s %s%s' % (option_string, _gc(self.colors['values']),
-                                                                             args_string))
+                    parts.append(
+                        _gc(self.colors['switches']) + '%s %s%s' %
+                        (option_string, _gc(self.colors['values']), args_string)
+                    )
 
             return _gc(self.colors['commas']) + ', '.join(parts)
 
     def _metavar_formatter(self, action, default_metavar):
         if action.metavar is not None:
             result = action.metavar
         elif action.choices is not None:
@@ -364,15 +386,15 @@
         else:
             result = default_metavar
 
         def format(tuple_size):
             if isinstance(result, tuple):
                 return result
             else:
-                return (result,) * tuple_size
+                return (result, ) * tuple_size
 
         return format
 
 
 class ColorizingTextWrapper(_TextWrapper):
     # modified upstream code, not going to refactor for complexity.
     def _wrap_chunks(self, chunks):  # noqa: C901
@@ -417,15 +439,16 @@
                 indent = self.initial_indent
 
             # Maximum width for this line.
             width = self.width - len(indent)
 
             # First chunk on the line is whitespace -- drop it, unless this
             # is the very beginning of the text (i.e. no lines started yet).
-            if self.drop_whitespace and _Formatter.decolorize(chunks[-1]).strip() == '' and lines:
+            if self.drop_whitespace and _Formatter.decolorize(chunks[-1]
+                                                              ).strip() == '' and lines:
                 del chunks[-1]
 
             while chunks:
                 # modified upstream code, not going to refactor for ambiguous variable name.
                 length = len(_Formatter.decolorize(chunks[-1]))  # noqa: E741
 
                 # Can at least squeeze this chunk onto the current line.
@@ -440,32 +463,31 @@
             # The current line is full, and the next chunk is too big to
             # fit on *any* line (not just this one).
             if chunks and len(_Formatter.decolorize(chunks[-1])) > width:
                 self._handle_long_word(chunks, current_line, current_len, width)
                 current_len = sum(map(len, current_line))
 
             # If the last chunk on this line is all whitespace, drop it.
-            if self.drop_whitespace and current_line and _Formatter.decolorize(current_line[-1]).strip() == '':
+            if self.drop_whitespace and current_line and _Formatter.decolorize(
+                    current_line[-1]).strip() == '':
                 current_len -= len(_Formatter.decolorize(current_line[-1]))
                 del current_line[-1]
 
             if current_line:
-                if (self.max_lines is None or
-                        len(lines) + 1 < self.max_lines or
-                        (not chunks or
-                         self.drop_whitespace and
-                         len(chunks) == 1 and
-                         not chunks[0].strip()) and current_len <= width):
+                if (self.max_lines is None or len(lines) + 1 < self.max_lines
+                        or (not chunks or self.drop_whitespace and len(chunks) == 1
+                            and not chunks[0].strip()) and current_len <= width):
                     # Convert current line back to a string and store it in
                     # list of all lines (return value).
                     lines.append(indent + ''.join(current_line))
                 else:
                     while current_line:
-                        if _Formatter.decolorize(current_line[-1]).strip() and current_len + len(
-                                self.placeholder) <= width:
+                        if _Formatter.decolorize(
+                                current_line[-1]
+                        ).strip() and current_len + len(self.placeholder) <= width:
                             current_line.append(self.placeholder)
                             lines.append(indent + ''.join(current_line))
                             break
                         current_len -= len(_Formatter.decolorize(current_line[-1]))
                         del current_line[-1]
                     else:
                         if lines:
@@ -477,15 +499,21 @@
                         lines.append(indent + self.placeholder.lstrip())
                     break
 
         return lines
 
 
 class ColorizingArgumentParser(_argparse.ArgumentParser):
-    def __init__(self, formatter_class=ColorizingHelpFormatter, colors: _Optional[_Mapping[str, str]] = None, **kwargs):
+
+    def __init__(
+        self,
+        formatter_class=ColorizingHelpFormatter,
+        colors: _Optional[_Mapping[str, str]] = None,
+        **kwargs
+    ):
         self.logger = _log21.Logger('ArgumentParser')
         self.colors = colors
         super().__init__(formatter_class=formatter_class, **kwargs)
 
     def _print_message(self, message, file=None):
         if message:
             self.logger.handlers.clear()
@@ -497,14 +525,19 @@
         if message:
             self._print_message(_gc('lr') + message + _gc('rst'), _sys.stderr)
         _sys.exit(status)
 
     def error(self, message):
         self.print_usage(_sys.stderr)
         args = {'prog': self.prog, 'message': message}
-        self.exit(2, _gettext(f'%(prog)s: {_gc("r")}error{_gc("lr")}:{_gc("rst")} %(message)s\n') % args)
+        self.exit(
+            2,
+            _gettext(
+                f'%(prog)s: {_gc("r")}error{_gc("lr")}:{_gc("rst")} %(message)s\n'
+            ) % args
+        )
 
     def _get_formatter(self):
         if hasattr(self.formatter_class, 'colors'):
             return self.formatter_class(prog=self.prog, colors=self.colors)
         else:
             return self.formatter_class(prog=self.prog)
```

### Comparing `log21-2.6.0/src/log21/Argumentify.py` & `log21-2.6.1/src/log21/Argumentify.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
         self.docstring = _parse(self.function.__doc__ or '')
         for parameter in self.docstring.params:
             if parameter.arg_name in self.arguments:
                 self.arguments[parameter.arg_name].help = parameter.description
 
 
-def generate_flag(
+def generate_flag(  # pylint: disable=too-many-branches
     argument: Argument,
     no_dash: bool = False,
     reserved_flags: _Optional[_Set[str]] = None
 ) -> _List[str]:
     """Generates one or more flags for an argument based on its attributes.
 
     :param argument: The argument to generate flags for.
@@ -206,17 +206,20 @@
         flag1 = flag1_base + normalize_name(
             ' '.join(normalize_name_to_snake_case(argument.name, '-').split('-')
                      ).capitalize(),
             sep_char='-'
         )
     if flag1 in reserved_flags:
         flag1 = flag1_base + normalize_name(argument.name, sep_char='-').upper()
-    if flag1 in reserved_flags and no_dash:
-        raise FlagGenerationError(f"Failed to generate a flag for argument: {argument}")
-    if flag1 not in reserved_flags:
+    if flag1 in reserved_flags:
+        if no_dash:
+            raise FlagGenerationError(
+                f"Failed to generate a flag for argument: {argument}"
+            )
+    else:
         flags.append(flag1)
 
     if not no_dash:
         flag2 = '-' + argument.name[:1].lower()
         if flag2 in reserved_flags:
             flag2 = flag2.upper()
         if flag2 in reserved_flags:
```

### Comparing `log21-2.6.0/src/log21/Colors.py` & `log21-2.6.1/src/log21/Colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,25 +274,25 @@
     if closest_name in Colors.change_map:
         closest_name = Colors.change_map[closest_name]
     return closest_name
 
 
 def get_color(color: _Union[str, _Sequence], raise_exceptions: bool = False) -> str:
     """Gets a color name and returns it in ansi format
-    
+
     >>>
     >>> get_color('LightRed')
     '\x1b[91m'
     >>>
     >>> import log21
     >>> log21.get_logger().info(log21.get_color('Blue') + 'Hello World!')
     [21:21:21] [INFO] Hello World!
     >>> # Note that you must run it yourself to see the colorful result ;D
     >>>
-    
+
     :param color: color name(Example: Blue)
     :param raise_exceptions: bool = False:
         False: It will return '' instead of raising exceptions when an error occurs.
         True: It may raise TypeError or KeyError
     :raises TypeError: `color` must be str
     :raises KeyError: `color` not found!
     :return: str: an ansi color
```

### Comparing `log21-2.6.0/src/log21/CrashReporter/Formatters.py` & `log21-2.6.1/src/log21/CrashReporter/Formatters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 # log21.CrashReporter.Formatters.py
 # CodeWriter21
 
 import traceback
-
+from typing import (Any as _Any, Union as _Union, Mapping as _Mapping,
+                    Callable as _Callable, Optional as _Optional)
 from datetime import datetime as _datetime
-from typing import Mapping as _Mapping, Union as _Union, Callable as _Callable, Any as _Any
 
-__all__ = ['Formatter', 'CONSOLE_REPORTER_FORMAT', 'FILE_REPORTER_FORMAT', 'EMAIL_REPORTER_FORMAT']
+__all__ = [
+    'Formatter', 'CONSOLE_REPORTER_FORMAT', 'FILE_REPORTER_FORMAT',
+    'EMAIL_REPORTER_FORMAT'
+]
 
 RESERVED_KEYS = (
-    '__name__',
-    'type',
-    'message',
-    'traceback',
-    'name',
-    'file',
-    'lineno',
-    'function',
+    '__name__', 'type', 'message', 'traceback', 'name', 'file', 'lineno', 'function',
     'asctime'
 )
 
 
 class Formatter:
-    def __init__(self, format_: str, style: str = '%', datefmt: str = '%Y-%m-%d %H:%M:%S',
-                 extra_values: _Mapping[str, _Union[str, _Callable, _Any]] = None):
+    """The base class for all CrashReporter formatters."""
+
+    def __init__(
+        self,
+        format_: str,
+        style: str = '%',
+        datefmt: str = '%Y-%m-%d %H:%M:%S',
+        extra_values: _Optional[_Mapping[str, _Union[str, _Callable, _Any]]] = None
+    ):
+        """Initialize the formatter.
+
+        :param format_: The format string.
+        :param style: The style of the format string. Valid styles: %, {
+        :param datefmt: The date format string.
+        :param extra_values: A mapping of extra values to be added to the log record.
+        """
         self._format = format_
 
         if style in ['%', '{']:
             self.__style = style
         else:
             raise ValueError('Invalid style: "' + str(style) + '" Valid styles: %, {')
 
         self.datefmt = datefmt
-        self.extra_values = dict()
+        self.extra_values = {}
         if extra_values:
             for key in extra_values:
                 if key in RESERVED_KEYS:
-                    raise ValueError(f'`{key}` is a reserved-key and cannot be used in `extra_values`.')
+                    raise ValueError(
+                        f'`{key}` is a reserved-key and cannot be used in '
+                        '`extra_values`.'
+                    )
                 self.extra_values[key] = extra_values[key]
 
-    def format(self, exception: BaseException):
+    def format(self, exception: BaseException) -> str:
+        """Format the exception.
+
+        :param exception: The exception to format.
+        :raises ValueError: If the style is not either '%' or '{'.
+        :return: The formatted exception.
+        """
         exception_dict = {
             '__name__': __name__,
             'type': type(exception),
             'message': exception.args[0],
             'traceback': traceback.format_tb(exception.__traceback__.tb_next),
             'name': exception.__class__.__name__,
             'file': exception.__traceback__.tb_next.tb_frame.f_code.co_filename,
@@ -55,43 +74,48 @@
             if callable(value):
                 exception_dict[key] = value()
             else:
                 exception_dict[key] = value
 
         if self.__style == '%':
             return self._format % exception_dict
-        elif self.__style == '{':
+        if self.__style == '{':
             return self._format.format(**exception_dict)
-        else:
-            raise ValueError('Invalid style: "' + str(self.__style) + '" Valid styles: %, {')
-
+        raise ValueError(
+            'Invalid style: "' + str(self.__style) + '" Valid styles: %, {'
+        )
+
+
+CONSOLE_REPORTER_FORMAT = {
+    'format_':
+    '\033[91m%(name)s: %(message)s\033[0m\n'  # Name and message of the exception.
+    '\tFile\033[91m:\033[0m "%(file)s"\n'  # The file that exception was raised in.
+    '\tLine\033[91m:\033[0m %(lineno)d',  # The line that exception was raised on.
+    'style':
+    '%'
+}
+
+FILE_REPORTER_FORMAT = {
+    'format_':
+    '[%(asctime)s] %(name)s: %(message)s'  # Name and message of the exception.
+    '; File: "%(file)s"'  # The file that exception was raised in.
+    '; Line: %(lineno)d\n',  # The line that exception was raised on.
+    'style':
+    '%'
+}
 
-CONSOLE_REPORTER_FORMAT = dict(
-    format_=f'\033[91m%(name)s: %(message)s\033[0m\n'  # Name and message of the exception.
-            f'\tFile\033[91m:\033[0m "%(file)s"\n'  # The file that exception was raised in.
-            f'\tLine\033[91m:\033[0m %(lineno)d',  # The line that exception was raised on.
-    style='%'
-)
-
-FILE_REPORTER_FORMAT = dict(
-    format_=f'[%(asctime)s] %(name)s: %(message)s'  # Name and message of the exception.
-            f'; File: "%(file)s"'  # The file that exception was raised in.
-            f'; Line: %(lineno)d\n',  # The line that exception was raised on.
-    style='%'
-)
-
-EMAIL_REPORTER_FORMAT = dict(
-    format_="""
+EMAIL_REPORTER_FORMAT = {
+    'format_': """
     <html>
         <body>
             <h1>Crash Report: %(__name__)s</h1>
             <h2>%(name)s: %(message)s</h2>
             <p>
                 <span style="bold">File:</span> "%(file)s"<br>
                 <span style="bold">Line:</span> %(lineno)d<br>
                 <span style="center">%(asctime)s</span><br>
             </p>
         <body>
     </html>
     """,
-    style='%'
-)
+    'style': '%'
+}
```

### Comparing `log21-2.6.0/src/log21/CrashReporter/Reporters.py` & `log21-2.6.1/src/log21/CrashReporter/Reporters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 # log21.CrashReporter.Reporters.py
 # CodeWriter21
 
+from __future__ import annotations
+
 import ssl as _ssl
 import smtplib as _smtplib  # This module is used to send emails.
-
 from os import PathLike as _PathLike
-from typing import Callable as _Callable, Any as _Any, Union as _Union, IO as _IO, Set as _Set, Iterable as _Iterable, \
-    Type as _Type
+from typing import (IO as _IO, Any as _Any, Set as _Set, Type as _Type, Union as _Union,
+                    Callable as _Callable, Iterable as _Iterable, Optional as _Optional)
 from functools import wraps as _wraps
 from email.mime.text import MIMEText as _MIMEText
 from email.mime.multipart import MIMEMultipart as _MIMEMultipart
 
 import log21 as _log21
 
-from .Formatters import CONSOLE_REPORTER_FORMAT as _CONSOLE_REPORTER_FORMAT, \
-    FILE_REPORTER_FORMAT as _FILE_REPORTER_FORMAT, EMAIL_REPORTER_FORMAT as _EMAIL_REPORTER_FORMAT
+from .Formatters import (FILE_REPORTER_FORMAT as _FILE_REPORTER_FORMAT,
+                         EMAIL_REPORTER_FORMAT as _EMAIL_REPORTER_FORMAT,
+                         CONSOLE_REPORTER_FORMAT as _CONSOLE_REPORTER_FORMAT)
 
 __all__ = ['Reporter', 'ConsoleReporter', 'FileReporter', 'EmailReporter']
 
 
+# pylint: disable=redefined-builtin
 def print(*msg, args: tuple = (), end='\033[0m\n', **kwargs):
-    logger = _log21.get_logger('log21.print', level='DEBUG', show_time=False, show_level=False)
+    """Prints a message to the console using the log21.Logger."""
+    logger = _log21.get_logger(
+        'log21.print', level='DEBUG', show_time=False, show_level=False
+    )
     logger.print(*msg, args=args, end=end, **kwargs)
 
 
 class Reporter:
-    """
-    Reporter is a decorator that wraps a function and calls a function when an exception is raised.
+    """Reporter is a decorator that wraps a function and calls a function when
+    an exception is raised.
 
     Usage Example:
         >>>
         >>> # Define a function that gets an exception and somehow reports it to you
         >>> def report_function(exception):
         ...     print(exception)
         ...
         >>>
         >>> # Create a Reporter object and pass the reporter function you defined to it
         >>> reporter_object = Reporter(report_function, False)
         >>>
         >>> # Define the function you want to wrap
         >>> # This function might raise an exception
-        >>> # You can wrap your main function, so that you get notified whenever your app crashes
+        >>> # You can wrap your main function, so that you get notified whenever your
+        >>> # app crashes
         >>> @reporter_object.reporter
         ... def divide(a, b):
         ...     return a / b
         ...
         >>>
         >>> divide(21, 3)
         7.0
@@ -57,76 +64,89 @@
         >>> wrapped_sqrt(121)
         11.0
         >>> wrapped_sqrt(-1)
         math domain error
         >>>
     """
 
-    _reporter_function: _Callable[[BaseException], _Any]  # A function that will be called when an exception is raised.
+    _reporter_function: _Callable[[
+        BaseException
+    ], _Any]  # A function that will be called when an exception is raised.
     _exceptions_to_catch: _Set = None
     _exceptions_to_ignore: _Set = None
     raise_after_report: bool
 
-    def __init__(self, report_function: _Callable[[BaseException], _Any], raise_after_report: bool = False,
-                 formatter: '_log21.CrashReporter.Formatter' = None,
-                 exceptions_to_catch: _Iterable[BaseException] = None,
-                 exceptions_to_ignore: _Iterable[BaseException] = None):
+    def __init__(
+        self,
+        report_function: _Optional[_Callable[[BaseException], _Any]],
+        raise_after_report: bool = False,
+        formatter: _Optional[_log21.CrashReporter.Formatter] = None,
+        exceptions_to_catch: _Optional[_Iterable[BaseException]] = None,
+        exceptions_to_ignore: _Optional[_Iterable[BaseException]] = None
+    ):
         """
         :param report_function: Function to call when an exception is raised.
-        :param raise_after_report: If True, the exception will be raised after the report_function is called.
+        :param raise_after_report: If True, the exception will be raised after the
+            report_function is called.
         """
         self._reporter_function = report_function
         self.raise_after_report = raise_after_report
         self.formatter = formatter
-        self._exceptions_to_catch = set(exceptions_to_catch) if exceptions_to_catch else None
-        self._exceptions_to_ignore = set(exceptions_to_ignore) if exceptions_to_ignore else None
+        self._exceptions_to_catch = set(
+            exceptions_to_catch
+        ) if exceptions_to_catch else None
+        self._exceptions_to_ignore = set(
+            exceptions_to_ignore
+        ) if exceptions_to_ignore else None
 
     def reporter(self, func):
-        """
-        It will wrap the function and call the report_function when an exception is raised.
+        """It will wrap the function and call the report_function when an
+        exception is raised.
 
         :param func: Function to wrap.
         :return: Wrapped function.
         """
 
-        exceptions_to_catch = tuple(self._exceptions_to_catch) if self._exceptions_to_catch else BaseException
-        exceptions_to_ignore = tuple(self._exceptions_to_ignore) if self._exceptions_to_ignore else tuple()
+        exceptions_to_catch = tuple(
+            self._exceptions_to_catch
+        ) if self._exceptions_to_catch else BaseException
+        exceptions_to_ignore = tuple(self._exceptions_to_ignore
+                                     ) if self._exceptions_to_ignore else tuple()
 
         @_wraps(func)
         def wrap(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except BaseException as e:
-                if isinstance(e, exceptions_to_catch) and not isinstance(e, exceptions_to_ignore):
+                if isinstance(e, exceptions_to_catch) and not isinstance(
+                        e, exceptions_to_ignore):
                     self._reporter_function(e)
                     if self.raise_after_report:
                         raise e
                 else:
                     raise e
 
         return wrap
 
     def catch(self, exception: _Type[BaseException]):
-        """
-        Add an exception to the list of exceptions to catch.
+        """Add an exception to the list of exceptions to catch.
 
         :param exception: Exception to catch.
         """
         if not issubclass(exception, BaseException):
             raise TypeError('`exception` must be a subclass of BaseException.')
         if self._exceptions_to_catch is None:
             self._exceptions_to_catch = set()
         if exception not in self._exceptions_to_catch:
             self._exceptions_to_catch.add(exception)
         else:
             raise ValueError('exception is already in the list of exceptions to catch')
 
     def ignore(self, exception: _Type[BaseException]):
-        """
-        Add an exception to the list of exceptions to ignore.
+        """Add an exception to the list of exceptions to ignore.
 
         :param exception: Exception to ignore.
         """
         if not issubclass(exception, BaseException):
             raise TypeError('`exception` must be a subclass of BaseException.')
         if self._exceptions_to_ignore is None:
             self._exceptions_to_ignore = set()
@@ -136,16 +156,16 @@
             raise ValueError('exception is already in the list of exceptions to ignore')
 
     def __call__(self, func):
         return self.reporter(func)
 
 
 class ConsoleReporter(Reporter):
-    """
-    ConsoleReporter is a Reporter that prints the exception to the console.
+    """ConsoleReporter is a Reporter that prints the exception to the console.
+
     Usage Example:
         >>>
         >>> # Define a ConsoleReporter object
         >>> console_reporter = ConsoleReporter()
         >>>
         >>> # Define a function that raises an exception
         >>> @console_reporter.reporter
@@ -182,89 +202,108 @@
         >>> divide(21, 3)
         7.0
         >>> divide(10, 0)
         [2121-12-21 21:21:21] divide: Line 3: ZeroDivisionError: division by zero
         >>>
     """
 
-    def __init__(self, raise_after_report: bool = False, formatter: '_log21.CrashReporter.Formatter' = None,
-                 print_function: _Callable = print, exceptions_to_catch: _Iterable[BaseException] = None,
-                 exceptions_to_ignore: _Iterable[BaseException] = None):
+    def __init__(
+        self,
+        raise_after_report: bool = False,
+        formatter: _Optional[_log21.CrashReporter.Formatter] = None,
+        print_function: _Optional[_Callable] = print,
+        exceptions_to_catch: _Optional[_Iterable[BaseException]] = None,
+        exceptions_to_ignore: _Optional[_Iterable[BaseException]] = None
+    ):
         """
-        :param raise_after_report: If True, the exception will be raised after the report_function is called.
+        :param raise_after_report: If True, the exception will be raised after the
+            report_function is called.
         :param print_function: Function to use to print the message.
         """
-        super().__init__(self._report, raise_after_report, formatter, exceptions_to_catch, exceptions_to_ignore)
+        super().__init__(
+            self._report, raise_after_report, formatter, exceptions_to_catch,
+            exceptions_to_ignore
+        )
 
         if formatter:
             if isinstance(formatter, _log21.CrashReporter.Formatter):
                 self.formatter = formatter
             else:
                 raise ValueError('formatter must be a log21.CrashReporter.Formatter')
         else:
-            self.formatter = _log21.CrashReporter.Formatters.Formatter(**_CONSOLE_REPORTER_FORMAT)
+            self.formatter = _log21.CrashReporter.Formatters.Formatter(
+                **_CONSOLE_REPORTER_FORMAT
+            )
 
         self.print = print_function
 
     def _report(self, exception: BaseException):
-        """
-        Prints the exception to the console.
+        """Prints the exception to the console.
 
         :param exception: Exception to print.
         :return:
         """
 
         self.print(self.formatter.format(exception))
 
 
 class FileReporter(Reporter):
-    """
-    FileReporter is a Reporter that writes the exception to a file.
-    """
+    """FileReporter is a Reporter that writes the exception to a file."""
 
-    def __init__(self, file: _Union[str, _PathLike, _IO], raise_after_report: bool = True,
-                 formatter: '_log21.CrashReporter.Formatter' = None,
-                 exceptions_to_catch: _Iterable[BaseException] = None,
-                 exceptions_to_ignore: _Iterable[BaseException] = None):
-        super().__init__(self._report, raise_after_report, formatter, exceptions_to_catch, exceptions_to_ignore)
+    def __init__(
+        self,
+        *,
+        file: _Union[str, _PathLike, _IO],
+        encoding: str = 'utf-8',
+        raise_after_report: bool = True,
+        formatter: _Optional[_log21.CrashReporter.Formatter] = None,
+        exceptions_to_catch: _Optional[_Iterable[BaseException]] = None,
+        exceptions_to_ignore: _Optional[_Iterable[BaseException]] = None
+    ):
+        super().__init__(
+            self._report, raise_after_report, formatter, exceptions_to_catch,
+            exceptions_to_ignore
+        )
+        # pylint: disable=consider-using-with
         if isinstance(file, str):
-            self.file = open(file, 'a')
+            self.file = open(file, 'a', encoding=encoding)
         elif isinstance(file, _PathLike):
-            self.file = open(file, 'a')
+            self.file = open(file, 'a', encoding=encoding)
         elif isinstance(file, _IO):
             if file.writable():
                 self.file = file
             else:
                 raise ValueError('file must be writable')
         else:
             raise ValueError('file must be a string, PathLike, or IO object')
 
         if formatter:
             if isinstance(formatter, _log21.CrashReporter.Formatter):
                 self.formatter = formatter
             else:
                 raise ValueError('formatter must be a log21.CrashReporter.Formatter')
         else:
-            self.formatter = _log21.CrashReporter.Formatters.Formatter(**_FILE_REPORTER_FORMAT)
+            self.formatter = _log21.CrashReporter.Formatters.Formatter(
+                **_FILE_REPORTER_FORMAT
+            )
 
     def _report(self, exception: BaseException):
-        """
-        Writes the exception to the file.
+        """Writes the exception to the file.
 
         :param exception: Exception to write.
         :return:
         """
 
         self.file.write(self.formatter.format(exception))
         self.file.flush()
 
 
-class EmailReporter(Reporter):
-    """
-    EmailReporter is a Reporter that sends an email with the exception.
+class EmailReporter(Reporter):  # pylint: disable=too-many-instance-attributes
+    """EmailReporter is a Reporter that sends an email with the exception.
+
     Usage Example:
         >>>
         >>> # Define a EmailReporter object
         >>> email_reporter = EmailReporter(
         ...     mail_host='smtp.yandex.ru',
         ...     port=465,
         ...     from_address='MyEmail@yandex.ru',
@@ -291,19 +330,32 @@
             return func(*args, **kwargs)
           File "<stdin>", line 3, in divide
         ZeroDivisionError: division by zero
         >>> # At this point a Crash Report is sent to my email: CodeWriter21@gmail.com
         >>>
     """
 
-    def __init__(self, mail_host: str, port: int, from_address: str, to_address: str, password: str, username: str = '',
-                 tls: bool = True, raise_after_report: bool = True, formatter: '_log21.CrashReporter.Formatter' = None,
-                 exceptions_to_catch: _Iterable[BaseException] = None,
-                 exceptions_to_ignore: _Iterable[BaseException] = None):
-        super().__init__(self._report, raise_after_report, formatter, exceptions_to_catch, exceptions_to_ignore)
+    def __init__(
+        self,
+        mail_host: str,
+        port: int,
+        from_address: str,
+        to_address: str,
+        password: str,
+        username: str = '',
+        tls: bool = True,
+        raise_after_report: bool = True,
+        formatter: _Optional[_log21.CrashReporter.Formatter] = None,
+        exceptions_to_catch: _Optional[_Iterable[BaseException]] = None,
+        exceptions_to_ignore: _Optional[_Iterable[BaseException]] = None
+    ):
+        super().__init__(
+            self._report, raise_after_report, formatter, exceptions_to_catch,
+            exceptions_to_ignore
+        )
         self.mail_host = mail_host
         self.port = port
         self.from_address = from_address
         self.to_address = to_address
         self.password = password
         if username:
             self.username = username
@@ -319,39 +371,41 @@
                     server.ehlo()
                     server.login(self.username, self.password)
             else:
                 with _smtplib.SMTP(self.mail_host, port) as server:
                     server.ehlo()
                     server.login(self.username, self.password)
                     server.ehlo()
-        except Exception as e:
-            raise e
+        except Exception as ex:  # pylint: disable=broad-except
+            raise ex
 
         if formatter:
             if isinstance(formatter, _log21.CrashReporter.Formatter):
                 self.formatter = formatter
             else:
                 raise ValueError('formatter must be a log21.CrashReporter.Formatter')
         else:
-            self.formatter = _log21.CrashReporter.Formatters.Formatter(**_EMAIL_REPORTER_FORMAT)
+            self.formatter = _log21.CrashReporter.Formatters.Formatter(
+                **_EMAIL_REPORTER_FORMAT
+            )
 
     def _report(self, exception: BaseException):
-        """
-        Sends an email with the exception.
+        """Sends an email with the exception.
 
         :param exception: Exception to send.
         :return:
         """
         message = _MIMEMultipart()
         message['From'] = self.from_address  # Sender
         message['To'] = self.to_address  # Receiver
         message['Subject'] = f'Crash Report: {exception.__class__.__name__}'  # Subject
         message.attach(_MIMEText(self.formatter.format(exception), 'html'))
         if self.tls:
             context = _ssl.create_default_context()
-            with _smtplib.SMTP_SSL(self.mail_host, port=self.port, context=context) as server:
+            with _smtplib.SMTP_SSL(self.mail_host, port=self.port,
+                                   context=context) as server:
                 server.login(self.username, self.password)
                 server.sendmail(self.from_address, self.to_address, message.as_string())
         else:
             with _smtplib.SMTP(self.username, port=self.port) as server:
                 server.login(self.from_address, self.password)
                 server.sendmail(self.from_address, self.to_address, message.as_string())
```

### Comparing `log21-2.6.0/src/log21/Formatters.py` & `log21-2.6.1/src/log21/Formatters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # log21.Formatters.py
 # CodeWriter21
 
 import time as _time
+from typing import (Dict as _Dict, Tuple as _Tuple, Mapping as _Mapping,
+                    Optional as _Optional)
 from logging import Formatter as __Formatter
-from typing import Mapping as _Mapping, Tuple as _Tuple, Dict as _Dict, Optional as _Optional
+
 from log21.Colors import get_colors as _gc, ansi_escape
-from log21.Levels import INPUT, CRITICAL, ERROR, WARNING, INFO, DEBUG, PRINT
+from log21.Levels import INFO, DEBUG, ERROR, INPUT, PRINT, WARNING, CRITICAL
 
 __all__ = ['ColorizingFormatter', 'DecolorizingFormatter']
 
 
 class _Formatter(__Formatter):
-    def __init__(self, fmt: _Optional[str] = None, datefmt: _Optional[str] = None, style: str = '%',
-                 level_names: _Optional[_Mapping[int, str]] = None):
+
+    def __init__(
+        self,
+        fmt: _Optional[str] = None,
+        datefmt: _Optional[str] = None,
+        style: str = '%',
+        level_names: _Optional[_Mapping[int, str]] = None
+    ):
         """
         `level_names` usage:
         >>> import log21
         >>> logger = log21.Logger('MyLogger', log21.DEBUG)
         >>> stream_handler = log21.ColorizingStreamHandler()
         >>> formatter = log21.ColorizingFormatter(fmt='[%(levelname)s] %(message)s',
-        ...             level_names={log21.DEBUG: ' ', log21.INFO: '+', log21.WARNING: '-', log21.ERROR: '!',
+        ...             level_names={log21.DEBUG: ' ', log21.INFO: '+',
+        ...                          log21.WARNING: '-', log21.ERROR: '!',
         ...                          log21.CRITICAL: 'X'})
         >>> stream_handler.setFormatter(formatter)
         >>> logger.addHandler(stream_handler)
         >>>
         >>> logger.debug('Just wanna see if this works...')
         [ ] Just wanna see if this works...
         >>> logger.info("FYI: I'm glad somebody read this 8)")
@@ -33,14 +42,19 @@
         >>> logger.error('AN ERROR OCCURRED! (told ya ;))')
         [!] AN ERROR OCCURRED! (told ya ;))
         >>> logger.critical('Crashed....')
         [X] Crashed....
         >>>
         >>> # Hope you've enjoyed
         >>>
+
+        :param fmt: The format string to use.
+        :param datefmt: The date format string to use.
+        :param style: The style to use.
+        :param level_names: A dictionary mapping logging levels to their names.
         """
         super().__init__(fmt=fmt, datefmt=datefmt, style=style)
 
         self._level_names: _Dict[int, str] = {
             DEBUG: 'DEBUG',
             INFO: 'INFO',
             WARNING: 'WARNING',
@@ -52,76 +66,113 @@
 
         if level_names:
             for level, name in level_names.items():
                 self.level_names[level] = name
 
     @property
     def level_names(self):
+        """Get the level names mapping."""
         return self._level_names
 
     @level_names.setter
     def level_names(self, level_names: _Mapping[int, str]):
         if level_names:
             if not isinstance(level_names, _Mapping):
-                raise TypeError('`level_names` must be a Mapping, a dictionary like object!')
+                raise TypeError(
+                    '`level_names` must be a Mapping, a dictionary like object!'
+                )
             self._level_names = level_names
         else:
-            self._level_names = dict()
+            self._level_names = {}
 
     def format(self, record) -> str:
         record.message = record.getMessage()
         if self.usesTime():
             record.asctime = self.formatTime(record, self.datefmt)
 
         record.levelname = self.level_names.get(record.levelno, 'NOTSET')
 
-        s = self.formatMessage(record)
+        s = self.formatMessage(record)  # pylint: disable=invalid-name
         if record.exc_info:
             if not record.exc_text:
                 record.exc_text = self.formatException(record.exc_info)
         if record.exc_text:
             if s[-1:] != "\n":
                 s = s + "\n"
             s = s + record.exc_text
         if record.stack_info:
             if s[-1:] != "\n":
                 s = s + "\n"
             s = s + self.formatStack(record.stack_info)
         return s
 
 
-class ColorizingFormatter(_Formatter):
-    time_color: _Tuple[str, ...] = ('lightblue',)
-    name_color = pathname_color = filename_color = module_color = func_name_color = thread_name_color = \
-        message_color = tuple()
-
-    def __init__(self, fmt: _Optional[str] = None, datefmt: _Optional[str] = None, style: str = '%',
-                 level_names: _Optional[_Mapping[int, str]] = None,
-                 level_colors: _Optional[_Mapping[int, _Tuple[str]]] = None,
-                 time_color: _Optional[_Tuple[str, ...]] = None, name_color: _Optional[_Tuple[str, ...]] = None,
-                 pathname_color: _Optional[_Tuple[str, ...]] = None, filename_color: _Optional[_Tuple[str, ...]] = None,
-                 module_color: _Optional[_Tuple[str, ...]] = None, func_name_color: _Optional[_Tuple[str, ...]] = None,
-                 thread_name_color: _Optional[_Tuple[str, ...]] = None,
-                 message_color: _Optional[_Tuple[str, ...]] = None):
+class ColorizingFormatter(_Formatter):  # pylint: disable=too-many-instance-attributes
+    """A formatter that helps adding colors to the log records."""
+    time_color: _Tuple[str, ...] = ('lightblue', )
+    name_color = pathname_color = filename_color = module_color = func_name_color = \
+        thread_name_color = message_color = tuple()
+
+    def __init__(
+        self,
+        fmt: _Optional[str] = None,
+        datefmt: _Optional[str] = None,
+        style: str = '%',
+        level_names: _Optional[_Mapping[int, str]] = None,
+        level_colors: _Optional[_Mapping[int, _Tuple[str]]] = None,
+        time_color: _Optional[_Tuple[str, ...]] = None,
+        name_color: _Optional[_Tuple[str, ...]] = None,
+        pathname_color: _Optional[_Tuple[str, ...]] = None,
+        filename_color: _Optional[_Tuple[str, ...]] = None,
+        module_color: _Optional[_Tuple[str, ...]] = None,
+        func_name_color: _Optional[_Tuple[str, ...]] = None,
+        thread_name_color: _Optional[_Tuple[str, ...]] = None,
+        message_color: _Optional[_Tuple[str, ...]] = None
+    ):  # pylint: disable=too-many-branches
+        """Initialize the formatter.
+
+        :param fmt: The format string to use for the message.
+        :param datefmt: The format string to use for the date/time
+            portion of the message.
+        :param style: The format style to use.
+        :param level_names: A mapping of level numbers to level names.
+        :param level_colors: A mapping of level numbers to level colors.
+        :param time_color: The color to use for the time portion of the
+            message.
+        :param name_color: The color to use for the logger name portion
+            of the message.
+        :param pathname_color: The color to use for the pathname portion
+            of the message.
+        :param filename_color: The color to use for the filename portion
+            of the message.
+        :param module_color: The color to use for the module portion of
+            the message.
+        :param func_name_color: The color to use for the function name
+            portion of the message.
+        :param thread_name_color: The color to use for the thread name
+            portion of the message.
+        :param message_color: The color to use for the message portion
+            of the message.
+        """
         super().__init__(fmt=fmt, datefmt=datefmt, style=style, level_names=level_names)
         self.level_colors: _Dict[int, _Tuple[str, ...]] = {
-            DEBUG: ('lightblue',),
-            INFO: ('green',),
-            WARNING: ('lightyellow',),
-            ERROR: ('light red',),
+            DEBUG: ('lightblue', ),
+            INFO: ('green', ),
+            WARNING: ('lightyellow', ),
+            ERROR: ('light red', ),
             CRITICAL: ('background red', 'white'),
-            PRINT: ('Cyan',),
-            INPUT: ('Magenta',)
+            PRINT: ('Cyan', ),
+            INPUT: ('Magenta', )
         }
         # Checks and sets colors
         if level_colors:
             if not isinstance(level_colors, _Mapping):
                 raise TypeError('`level_colors` must be a dictionary like object!')
             for level, color in level_colors.items():
-                self.level_colors[level] = (_gc(*color),)
+                self.level_colors[level] = (_gc(*color), )
         if time_color:
             if not isinstance(time_color, tuple):
                 raise TypeError('`time_color` must be a tuple!')
             self.time_color = time_color
         if name_color:
             if not isinstance(name_color, tuple):
                 raise TypeError('`name_color` must be a tuple!')
@@ -148,29 +199,24 @@
             self.thread_name_color = thread_name_color
         if message_color:
             if not isinstance(message_color, tuple):
                 raise TypeError('`message_color` must be a tuple!')
             self.message_color = message_color
 
     def format(self, record) -> str:
-        """
-        Colorizes the record and returns the formatted message.
-
-        :param record:
-        :return: str
-        """
+        """Colorizes the record and returns the formatted message."""
         record.message = record.getMessage()
         if self.usesTime():
             record.asctime = self.formatTime(record, self.datefmt)
 
         record.levelname = self.level_names.get(record.levelno, 'NOTSET')
 
         record = self.colorize(record)
 
-        s = self.formatMessage(record)
+        s = self.formatMessage(record)  # pylint: disable=invalid-name
         if record.exc_info:
             # Cache the traceback text to avoid converting it multiple times
             # (it's constant anyway)
             if not record.exc_text:
                 record.exc_text = self.formatException(record.exc_info)
         if record.exc_text:
             if s[-1:] != "\n":
@@ -179,27 +225,27 @@
         if record.stack_info:
             if s[-1:] != "\n":
                 s = s + "\n"
             s = s + self.formatStack(record.stack_info)
         return s
 
     def colorize(self, record):
-        """
-        Colorizes the record attributes.
+        """Colorizes the record attributes.
 
         :param record:
         :return: colorized record
         """
         reset = '\033[0m'
 
         if hasattr(record, 'asctime'):
             record.asctime = _gc(*self.time_color) + record.asctime + reset
         if hasattr(record, 'levelno'):
-            record.levelname = _gc(*self.level_colors.get(int(record.levelno), ('lw',))) + \
-                               getattr(record, 'levelname', 'NOTSET') + reset
+            record.levelname = _gc(
+                *self.level_colors.get(int(record.levelno), ('lw', ))
+            ) + getattr(record, 'levelname', 'NOTSET') + reset
         if hasattr(record, 'name'):
             record.name = _gc(*self.name_color) + str(record.name) + reset
         if hasattr(record, 'pathname'):
             record.pathname = _gc(*self.pathname_color) + record.pathname + reset
         if hasattr(record, 'filename'):
             record.filename = _gc(*self.filename_color) + record.filename + reset
         if hasattr(record, 'module'):
@@ -211,38 +257,37 @@
         if hasattr(record, 'message'):
             record.message = _gc(*self.message_color) + record.message
 
         return record
 
 
 class DecolorizingFormatter(_Formatter):
+    """Formatter that removes color codes from the log records."""
+
     def formatTime(self, record, datefmt=None):
-        """
-        Returns the creation time of the specified LogRecord as formatted text.
-        """
+        """Returns the creation time of the specified LogRecord as formatted
+        text."""
         ct = self.converter(int(record.created))
         if datefmt:
             s = _time.strftime(datefmt, ct)
         else:
             t = _time.strftime(self.default_time_format, ct)
             s = self.default_msec_format % (t, record.msecs)
         return s
 
     def format(self, record) -> str:
-        """
-        Decolorizes the record and returns the formatted message.
+        """Decolorizes the record and returns the formatted message.
 
         :param record:
         :return: str
         """
         return self.decolorize(super().format(record))
 
     @staticmethod
     def decolorize(text: str):
-        """
-        Removes all ansi colors in the text.
+        """Removes all ansi colors in the text.
 
         :param text: str: Input text
         :return: str: decolorized text
         """
 
         return ansi_escape.sub('', text)
```

### Comparing `log21-2.6.0/src/log21/LoggingWindow.py` & `log21-2.6.1/src/log21/LoggingWindow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # log21.LoggingWindow.py
-# CodeWriter21
+# CodeWriter2
+
+from __future__ import annotations
+
 import re as _re
 import threading as _threading
 import subprocess as _subprocess
-
-from time import sleep as _sleep
 from enum import Enum as _Enum
+from time import sleep as _sleep
 from uuid import uuid4 as _uuid4
-from typing import Union as _Union
 from string import printable as _printable
+from typing import Union as _Union
 from logging import FileHandler as _FileHandler
 from argparse import Namespace as _Namespace
 
+from log21.Colors import hex_escape as _hex_escape, ansi_escape as _ansi_escape
 from log21.Levels import NOTSET as _NOTSET
 from log21.Logger import Logger as _Logger
 from log21.StreamHandler import StreamHandler as _StreamHandler
-from log21.Colors import ansi_escape as _ansi_escape, hex_escape as _hex_escape
 
 __all__ = ['LoggingWindow', 'LoggingWindowHandler']
 
 try:
     import tkinter as _tkinter
 except ImportError:
     _tkinter = None
 
-ansi_to_hex_color_map = {  # https://chrisyeh96.github.io/2020/03/28/terminal-colors.html
+ansi_to_hex_color_map = {
+    # https://chrisyeh96.github.io/2020/03/28/terminal-colors.html
     '30': ('#000000', 'foreground'),  # Black foreground
     '31': ('#cc0000', 'foreground'),  # Red foreground
     '32': ('#4e9a06', 'foreground'),  # Green foreground
     '33': ('#c4a000', 'foreground'),  # Yellow foreground
     '34': ('#729fcf', 'foreground'),  # Blue foreground
     '35': ('#75507b', 'foreground'),  # Magenta foreground
     '36': ('#06989a', 'foreground'),  # Cyan foreground
@@ -59,58 +62,77 @@
     '107': ('#ffffff', 'background'),  # Bright white background
 }
 
 _lock = _threading.RLock()
 
 
 class GettingInputStatus(_Enum):
+    """An enum for the status of getting input."""
     NOT_GETTING_INPUT = 0
     GETTING_INPUT = 1
     CANCELLED = 2
 
 
 class CancelledInputError(InterruptedError, Exception):
-    pass
+    """An exception raised when the input is cancelled."""
 
 
 class LoggingWindowHandler(_StreamHandler):
-    def __init__(self, logging_window: 'LoggingWindow', handle_carriage_return: bool = True,
-                 handle_new_line: bool = True):
+    """A handler for logging to a LoggingWindow."""
+
+    def __init__(
+        self,
+        logging_window: LoggingWindow,
+        handle_carriage_return: bool = True,
+        handle_new_line: bool = True
+    ):
+        """Initialize the LoggingWindowHandler.
+
+        :param logging_window: The LoggingWindow to log to.
+        :param handle_carriage_return: Whether to handle carriage
+            returns.
+        :param handle_new_line: Whether to handle new lines.
+        """
         self.HandleCR = handle_carriage_return
         self.HandleNL = handle_new_line
         self.__carriage_return: bool = False
-        self.LoggingWindow = logging_window
+        self.LoggingWindow = logging_window  # pylint: disable=invalid-name
         super().__init__(stream=None)
 
     def emit(self, record):
         try:
             if self.HandleCR:
                 self.check_cr(record)
             if self.HandleNL:
                 self.check_nl(record)
             msg = self.format(record)
             self.write(msg)
             self.write(self.terminator)
-        except Exception:
+        except Exception:  # pylint: disable=broad-except
             self.handleError(record)
 
-    def write(self, message):
-        if self.LoggingWindow is not None:
+    def write(self, message):  # pylint: disable=too-many-branches
+        """Write a message to the LoggingWindow.
+
+        :param message: The message to write.
+        """
+        if self.LoggingWindow is not None:  # pylint: disable=too-many-nested-blocks
             # Sets the element's state to normal so that it can be modified.
             self.LoggingWindow.logs.config(state=_tkinter.NORMAL)
 
             # Handles carriage return
             parts = _re.split(r'(\r)', message)
 
             while parts:
                 part = parts.pop(0)
 
                 if self.__carriage_return:
                     # Checks if the part is printable
-                    if any((char in _printable[:-6]) for char in _hex_escape.sub('', _ansi_escape.sub('', part))):
+                    if any((char in _printable[:-6])
+                           for char in _hex_escape.sub('', _ansi_escape.sub('', part))):
                         # Removes the last line
                         self.LoggingWindow.logs.delete('end - 1 lines', _tkinter.END)
                         if self.LoggingWindow.logs.count('0.0', 'end')[0] != 1:
                             self.LoggingWindow.logs.insert('end', '\n')
                         self.__carriage_return = False
 
                 tags = []
@@ -130,60 +152,86 @@
 
                             if hex_parts:
                                 hex_color = hex_parts.pop(0)
 
                                 tag = str(_uuid4())
                                 # Foreground color
                                 if hex_parts.pop(0) == 'f':
-                                    tags.append({'name': tag, 'start': self.LoggingWindow.logs.index('end-1c'),
-                                                 'config': {'foreground': hex_color}})
+                                    tags.append(
+                                        {
+                                            'name': tag,
+                                            'start':
+                                            self.LoggingWindow.logs.index('end-1c'),
+                                            'config': {
+                                                'foreground': hex_color
+                                            }
+                                        }
+                                    )
                                 # Background color
                                 else:
-                                    tags.append({'name': tag, 'start': self.LoggingWindow.logs.index('end-1c'),
-                                                 'config': {'background': hex_color}})
+                                    tags.append(
+                                        {
+                                            'name': tag,
+                                            'start':
+                                            self.LoggingWindow.logs.index('end-1c'),
+                                            'config': {
+                                                'background': hex_color
+                                            }
+                                        }
+                                    )
 
                     if ansi_parts:
                         ansi_params = ansi_parts.pop(0).split(';')
                         ansi_color = {'foreground': None, 'background': None}
 
                         for part in ansi_params:
                             if part in ansi_to_hex_color_map:
                                 color_ = ansi_to_hex_color_map[part]
                                 ansi_color[color_[1]] = color_[0]
                             elif part == '0':
-                                ansi_color['foreground'] = self.LoggingWindow.default_foreground_color
-                                ansi_color['background'] = self.LoggingWindow.default_background_color
+                                ansi_color[
+                                    'foreground'
+                                ] = self.LoggingWindow.default_foreground_color
+                                ansi_color[
+                                    'background'
+                                ] = self.LoggingWindow.default_background_color
                             else:
                                 pass  # error condition ignored
                         if ansi_color['foreground'] or ansi_color['background']:
-                            tags.append({'name': str(_uuid4()), 'start': self.LoggingWindow.logs.index('end-1c'),
-                                         'config': ansi_color})
+                            tags.append(
+                                {
+                                    'name': str(_uuid4()),
+                                    'start': self.LoggingWindow.logs.index('end-1c'),
+                                    'config': ansi_color
+                                }
+                            )
 
                 # Applies the color tags
                 for tag in tags:
                     self.LoggingWindow.logs.tag_add(tag['name'], tag['start'], 'end')
                     self.LoggingWindow.logs.tag_config(tag['name'], **tag['config'])
 
                 if parts:
                     parts.pop(0)
                     self.__carriage_return = True
 
             self.LoggingWindow.logs.config(state=_tkinter.DISABLED)
             self.LoggingWindow.logs.see(_tkinter.END)
 
 
-class LoggingWindow(_Logger):
+class LoggingWindow(_Logger):  # pylint: disable=too-many-instance-attributes
     """
     Usage Example:
         >>> # Manual creation
         >>> # Imports the LoggingWindow and LoggingWindowHandler classes
         >>> from log21 import LoggingWindow, LoggingWindowHandler
         >>> # Creates a new LoggingWindow object
         >>> window = LoggingWindow('Test Window', level='DEBUG')
-        >>> # Creates a new LoggingWindowHandler object and adds it to the LoggingWindow object
+        >>> # Creates a new LoggingWindowHandler object and adds it to the LoggingWindow
+        >>> # we created earlier
         >>> window.addHandler(LoggingWindowHandler(window))
         >>> window.debug('A debug message')
         >>> window.info('An info message')
         >>> # Run these lines to see the messages in the window
         >>>
         >>> # Automatic creation
         >>> # Imports log21 and time modules
@@ -207,26 +255,37 @@
         >>> name: str = window.input('Enter your name: ')
         >>> window.print('Hello, ' + name + '!')
         >>> # Run these lines to see the messages in the window
         >>>
 
     """
 
-    def __init__(self, name, level=_NOTSET, width: int = 80, height: int = 20, default_foreground_color='white',
-                 default_background_color='black', font=('Courier', 10), allow_python: bool = False,
-                 allow_shell: bool = False, command_history_buffer_size: int = 100):
-        """
-        Creates a new LoggingWindow object.
+    def __init__(
+        self,
+        name,
+        level=_NOTSET,
+        width: int = 80,
+        height: int = 20,
+        default_foreground_color='white',
+        default_background_color='black',
+        font=('Courier', 10),
+        allow_python: bool = False,
+        allow_shell: bool = False,
+        command_history_buffer_size: int = 100
+    ):  # pylint: disable=too-many-statements
+        """Creates a new LoggingWindow object.
 
         :param name: The name of the logger.
         :param level: The level of the logger.
         :param width: The width of the LoggingWindow.
         :param height: The height of the LoggingWindow.
-        :param default_foreground_color: The default foreground color of the LoggingWindow.
-        :param default_background_color: The default background color of the LoggingWindow.
+        :param default_foreground_color: The default foreground color of
+            the LoggingWindow.
+        :param default_background_color: The default background color of
+            the LoggingWindow.
         :param font: The font of the LoggingWindow.
         """
         super().__init__(name, level)
         self.window = _tkinter.Tk()
         self.window.title(name)
         # Hides window instead of closing it
         self.window.protocol("WM_DELETE_WINDOW", self.hide)
@@ -244,29 +303,36 @@
         self.command_entry.bind('<Return>', self.execute_command)
         self.command_entry.bind('<Up>', self.history_up)
         self.command_entry.bind('<Down>', self.history_down)
         self.command_history = []
         self.command_history_index = 0
         if not isinstance(command_history_buffer_size, (int, float)):
             raise TypeError('command_history_buffer_size must be a number')
-        self.command_history_buffer_size = command_history_buffer_size if command_history_buffer_size > 0 else 0
+        self.command_history_buffer_size = (
+            command_history_buffer_size if command_history_buffer_size > 0 else 0
+        )
         # Hides the command entry if allow_python and allow_shell are False
         if not allow_python and not allow_shell:
             self.command_entry.grid_remove()
         if allow_python:
             raise NotImplementedError('Python commands are not supported yet!')
         self.__allow_python = False
         self.__allow_shell = allow_shell
 
         # Scroll bars
-        self.logs.config(xscrollcommand=_tkinter.Scrollbar(self.window, orient=_tkinter.HORIZONTAL).set)
+        self.logs.config(
+            xscrollcommand=_tkinter.Scrollbar(self.window, orient=_tkinter.HORIZONTAL
+                                              ).set
+        )
         self.logs.config(yscrollcommand=_tkinter.Scrollbar(self.window).set)
 
         # Input related lines
-        self.getting_input_status: GettingInputStatus = GettingInputStatus.NOT_GETTING_INPUT
+        self.getting_input_status: GettingInputStatus = (
+            GettingInputStatus.NOT_GETTING_INPUT
+        )
         self.getting_pass = False
         self.input_text = ''
         # cursor counter is used for making a nice blinking cursor
         self.__cursor_counter = 1
         self._cursor_position = None
         self.cursor_position = 0
         # KeyPress event for self.logs
@@ -285,24 +351,28 @@
         self.window.bind('<<log>>', self.__log)
         self.window.bind('<<input>>', self.__input)
         self.window.bind('<<type input>>', self.__type_input)
         self.window.bind('<<getpass>>', self.__getpass)
         self.window.bind('<<SetAllowPython>>', self.__set_allow_python)
         self.window.bind('<<SetAllowShell>>', self.__set_allow_shell)
         self.window.bind('<<SetCursorPosition>>', self.__set_cursor_position)
-        self.window.bind('<<SetDefaultForegroundColor>>', self.__set_default_foreground_color)
-        self.window.bind('<<SetDefaultBackgroundColor>>', self.__set_default_background_color)
+        self.window.bind(
+            '<<SetDefaultForegroundColor>>', self.__set_default_foreground_color
+        )
+        self.window.bind(
+            '<<SetDefaultBackgroundColor>>', self.__set_default_background_color
+        )
         self.window.bind('<<SetFont>>', self.__set_font)
         self.window.bind('<<SetWidth>>', self.__set_width)
         self.window.bind('<<SetHeight>>', self.__set_height)
 
-    def addHandler(self, handler: _Union[_FileHandler, LoggingWindowHandler]):
-        if not (isinstance(handler, LoggingWindowHandler) or isinstance(handler, _FileHandler)):
+    def addHandler(self, hdlr: _Union[_FileHandler, LoggingWindowHandler]):
+        if not isinstance(hdlr, LoggingWindowHandler, _FileHandler):
             raise TypeError("Handler must be a FileHandler or LoggingWindowHandler")
-        super().addHandler(handler)
+        super().addHandler(hdlr)
 
     def __hide(self, _):
         self.window.withdraw()
 
     def __show(self, _):
         self.window.deiconify()
 
@@ -310,21 +380,30 @@
         self.logs.config(state=_tkinter.NORMAL)
         self.logs.delete('1.0', _tkinter.END)
         self.logs.config(state=_tkinter.DISABLED)
 
     def __log(self, event):
         data = event.data
         if self.getting_input_status == GettingInputStatus.GETTING_INPUT:
-            raise RuntimeError('Cannot log while getting input from the user! Please cancel the input first.')
-        super()._log(data.level, data.msg, data.args, data.exc_info, data.extra, data.stack_info, data.stacklevel)
+            raise RuntimeError(
+                'Cannot log while getting input from the user! '
+                'Please cancel the input first.'
+            )
+        super()._log(
+            data.level, data.msg, data.args, data.exc_info, data.extra, data.stack_info,
+            data.stacklevel
+        )
 
     def __input(self, event):
         data = event.data
         msg = ' '.join([str(m) for m in data.msg]) + data.end
-        self._log(self.level if self.level >= _NOTSET else _NOTSET, msg, data.args, **data.kwargs)
+        self._log(
+            self.level if self.level >= _NOTSET else _NOTSET, msg, data.args,
+            **data.kwargs
+        )
         self.input_text = ''
         self.getting_input_status = GettingInputStatus.GETTING_INPUT
         self.cursor_position = 0
         self.logs.focus()
         try:
             while self.getting_input_status == GettingInputStatus.GETTING_INPUT:
                 self.cursor_position = self.cursor_position
@@ -335,35 +414,41 @@
             self.getting_input_status = GettingInputStatus.NOT_GETTING_INPUT
 
         if self.getting_input_status == GettingInputStatus.NOT_GETTING_INPUT:
             data.output = self.input_text
         elif self.getting_input_status == GettingInputStatus.CANCELLED:
             if data.raise_error:
                 raise CancelledInputError('Input cancelled!')
-            else:
-                data.output = ''
+            data.output = ''
 
     def __type_input(self, event):
         data = event.data
-        if (self.getting_input_status != GettingInputStatus.GETTING_INPUT) and data.wait <= 0:
-            raise RuntimeError('The logger must be getting input for this method to work! '
-                               'Use `input` method or set the `wait` argument to a value greater than 0.')
+        if (self.getting_input_status
+                != GettingInputStatus.GETTING_INPUT) and data.wait <= 0:
+            raise RuntimeError(
+                'The logger must be getting input for this method to work! '
+                'Use `input` method or set the `wait` argument to '
+                'a value greater than 0.'
+            )
         while self.getting_input_status != GettingInputStatus.GETTING_INPUT:
             _sleep(data.wait)
         self.input_text += data.text
         self.logs.config(state=_tkinter.NORMAL)
         self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
         self.logs.insert(_tkinter.END, self.input_text)
         self.logs.config(state=_tkinter.DISABLED)
         self.cursor_position = len(self.input_text) - 1
 
     def __getpass(self, event):
         data = event.data
         msg = ' '.join([str(m) for m in data.msg]) + data.end
-        self._log(self.level if self.level >= _NOTSET else _NOTSET, msg, data.args, **data.kwargs)
+        self._log(
+            self.level if self.level >= _NOTSET else _NOTSET, msg, data.args,
+            **data.kwargs
+        )
         self.input_text = ''
         self.getting_pass = True
         self.cursor_position = 0
         self.logs.focus()
         try:
             while self.getting_pass:
                 self.cursor_position = self.cursor_position
@@ -371,99 +456,131 @@
                 self.window.after(10)
         except KeyboardInterrupt:
             self.input_text = ''
             self.getting_pass = False
         data.output = self.input_text
 
     def hide(self):
-        """
-        Hides the LoggingWindow.
+        """Hides the LoggingWindow.
+
         :return:
         """
         self.window.event_generate('<<hide>>')
 
     def show(self):
-        """
-        Shows the LoggingWindow.
+        """Shows the LoggingWindow.
+
         :return:
         """
         self.window.event_generate('<<show>>')
 
     def clear(self):
-        """
-        Clears the LoggingWindow.
+        """Clears the LoggingWindow.
+
         :return:
         """
         self.window.event_generate('<<clear>>')
 
-    def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False, stacklevel=1):
+    def _log(
+        self,
+        level,
+        msg,
+        args,
+        exc_info=None,
+        extra=None,
+        stack_info=False,
+        stacklevel=1
+    ):
         _lock.acquire()
-        self.window.event_generate('<<log>>', when='tail',
-                                   data=_Namespace(level=level, msg=msg, args=args, exc_info=exc_info,
-                                                   extra=extra, stack_info=stack_info,
-                                                   stacklevel=stacklevel))
+        self.window.event_generate(
+            '<<log>>',
+            when='tail',
+            data=_Namespace(
+                level=level,
+                msg=msg,
+                args=args,
+                exc_info=exc_info,
+                extra=extra,
+                stack_info=stack_info,
+                stacklevel=stacklevel
+            )
+        )
         _lock.release()
 
-    def input(self, *msg, args: tuple = (), end='', raise_error: str = False, **kwargs) -> str:
-        """
-        Prints a message and waits for input.
+    def input(
+        self,
+        *msg,
+        args: tuple = (),
+        end='',
+        raise_error: str = False,
+        **kwargs
+    ) -> str:
+        """Prints a message and waits for input.
 
         :param msg: The message to print.
         :param args: The arguments to pass to the message.
         :param end: The end of the message.
-        :param raise_error: If True, raises an error instead of returning an empty string.
+        :param raise_error: If True, raises an error instead of
+            returning an empty string.
         :param kwargs:
         :return: The input.
         """
         _lock.acquire()
-        data = _Namespace(msg=msg, args=args, end=end, raise_error=raise_error, kwargs=kwargs)
+        data = _Namespace(
+            msg=msg, args=args, end=end, raise_error=raise_error, kwargs=kwargs
+        )
         self.window.event_generate('<<input>>', when='tail', data=data)
         _lock.release()
         return data.output
 
     def cancel_input(self) -> str:
-        """
-        Cancels the input.
+        """Cancels the input.
+
         :return: Part of the input that the user has typed
         """
         if self.getting_input_status != GettingInputStatus.GETTING_INPUT:
-            raise RuntimeError('The logger must be getting input for this method to work! Use `input` method.')
+            raise RuntimeError(
+                'The logger must be getting input for this method to work! '
+                'Use `input` method.'
+            )
         self.getting_input_status = GettingInputStatus.CANCELLED
         return self.input_text
 
     def type_input(self, text: str, wait: _Union[int, float, bool] = False):
-        """
-        Types some text as a part of the input that the user can edit and enter.
+        """Types some text as a part of the input that the user can edit and
+        enter.
+
         :param text: The text to type for the user
-        :param wait: Wait until the input function is called and then type the text
+        :param wait: Wait until the input function is called and then
+            type the text
         :return:
         """
-        self.window.event_generate('<<type input>>', when='tail', data=_Namespace(text=text, wait=wait))
+        self.window.event_generate(
+            '<<type input>>', when='tail', data=_Namespace(text=text, wait=wait)
+        )
 
     def getpass(self, *msg, args: tuple = (), end='', **kwargs) -> str:
-        """
-        Prints a message and waits for input.
+        """Prints a message and waits for input.
 
         :param msg: The message to print.
         :param args: The arguments to pass to the message.
         :param end: The end of the message.
         :param kwargs:
         :return: The input.
         """
         _lock.acquire()
         data = _Namespace(msg=msg, args=args, end=end, kwargs=kwargs)
         self.window.event_generate('<<getpass>>', when='tail', data=data)
         _lock.release()
         return data.output
 
-    def key_press(self, event):
-        """
-        KeyPress event callback for self.logs.
-        """
-        if self.getting_input_status == GettingInputStatus.GETTING_INPUT or self.getting_pass:
+    def key_press(self, event):  # pylint: disable=too-many-branches
+        """KeyPress event callback for self.logs."""
+        if (self.getting_input_status == GettingInputStatus.GETTING_INPUT
+                or self.getting_pass):
             # Handles Enter key
             if event.keysym == 'Return':
                 self.getting_input_status = GettingInputStatus.NOT_GETTING_INPUT
                 self.getting_pass = False
                 self.cursor_position = 0
                 self.logs.config(state=_tkinter.NORMAL)
                 self.logs.insert(_tkinter.END, '\n')
@@ -480,179 +597,186 @@
                         self.logs.insert(_tkinter.END, '*' * len(self.input_text))
                     else:
                         self.logs.insert(_tkinter.END, self.input_text)
                     self.logs.config(state=_tkinter.DISABLED)
                     self.cursor_position -= 1
             # Handles Right Arrow
             elif event.keysym == 'Right':
-                if self.cursor_position < len(self.input_text) and not self.getting_pass:
+                if self.cursor_position < len(self.input_text
+                                              ) and not self.getting_pass:
                     self.cursor_position += 1
             # Handles Left Arrow
             elif event.keysym == 'Left':
                 if self.cursor_position > 0 and not self.getting_pass:
                     self.cursor_position -= 1
             # Handles other keys
             elif event.char:
                 self.logs.config(state=_tkinter.NORMAL)
                 self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
-                self.input_text = self.input_text[:self.cursor_position] + event.char + \
-                                  self.input_text[self.cursor_position:]
+                self.input_text = (
+                    self.input_text[:self.cursor_position] + event.char +
+                    self.input_text[self.cursor_position:]
+                )
                 if self.getting_pass:
                     self.logs.insert(_tkinter.END, '*' * len(self.input_text))
                 else:
                     self.logs.insert(_tkinter.END, self.input_text)
                 self.logs.config(state=_tkinter.DISABLED)
                 self.cursor_position += 1
 
     def execute_command(self, _):
-        """
-        Executes the command in self.command_entry.
-        """
+        """Executes the command in self.command_entry."""
         command = self.command_entry.get()
         self.command_entry.delete(0, _tkinter.END)
         self.command_history.append(command)
         self.command_history = self.command_history[-self.command_history_buffer_size:]
         # FIXME: It doesn't support multiline commands yet
         # Shell commands:
         if command.startswith('!'):
             if self.allow_shell:
                 try:
-                    # TODO: Add the support of interactive programmes such as python shell and bash
+                    # TODO: Add the support of interactive programmes such as python
+                    # shell and bash
                     output = _subprocess.check_output(command[1:].strip(), shell=False)
                     self.print(output.decode('utf-8').strip('\r\n'))
-                except _subprocess.CalledProcessError as e:
-                    self.error('Error code:', e.returncode, e.output.decode('utf-8').strip('\r\n'))
+                except _subprocess.CalledProcessError as ex:
+                    self.error(
+                        'Error code:', ex.returncode,
+                        ex.output.decode('utf-8').strip('\r\n')
+                    )
                 except FileNotFoundError:
                     self.error('File not found: Unrecognized command.')
-                except Exception as e:
-                    self.error(e)
+                except Exception as ex:  # pylint: disable=broad-except
+                    self.error(ex)
             else:
                 self.error('Shell commands are not allowed!')
         # Python commands:
         else:
             if self.allow_python:
                 try:
                     # TODO: Add the support of python commands
                     raise NotImplementedError
-                except Exception as e:
-                    self.error(e)
+                except Exception as ex:  # pylint: disable=broad-except
+                    self.error(ex)
             else:
                 try:
                     output = _subprocess.check_output(command.strip(), shell=False)
                     self.print(output.decode('utf-8').strip('\r\n'))
-                except _subprocess.CalledProcessError as e:
-                    self.error('Error code:', e.returncode, e.output.decode('utf-8').strip('\r\n'))
+                except _subprocess.CalledProcessError as ex:
+                    self.error(
+                        'Error code:', ex.returncode,
+                        ex.output.decode('utf-8').strip('\r\n')
+                    )
                 except FileNotFoundError:
                     self.error('File not found: Unrecognized command.')
-                except Exception as e:
-                    self.error(e)
+                except Exception as ex: # pylint: disable=broad-except
+                    self.error(ex)
         self.command_history_index = len(self.command_history)
 
     def history_up(self, _):
-        """
-        Moves up the command history.
-        """
+        """Moves up the command history."""
         _lock.acquire()
         if self.command_history_index > 0:
             self.command_history_index -= 1
             self.command_entry.delete(0, _tkinter.END)
-            self.command_entry.insert(0, self.command_history[self.command_history_index])
+            self.command_entry.insert(
+                0, self.command_history[self.command_history_index]
+            )
         _lock.release()
 
     def history_down(self, _):
-        """
-        Moves down the command history.
-        """
+        """Moves down the command history."""
         _lock.acquire()
         if self.command_history_index < len(self.command_history) - 1:
             self.command_history_index += 1
             self.command_entry.delete(0, _tkinter.END)
-            self.command_entry.insert(0, self.command_history[self.command_history_index])
+            self.command_entry.insert(
+                0, self.command_history[self.command_history_index]
+            )
         else:
             self.command_entry.delete(0, _tkinter.END)
         _lock.release()
 
     def __set_allow_python(self, event):
-        """
-        Sets the allow_python attribute.
-        """
+        """Sets the allow_python attribute."""
         self.__allow_python = event.data
         # Hides the command entry if allow_python and allow_shell are False
         if not self.__allow_python and not self.__allow_shell:
             self.command_entry.grid_remove()
         # Shows the command entry if allow_python or allow_shell are True
         else:
             self.command_entry.grid(row=1, column=0, sticky='nsew')
 
     def __set_allow_shell(self, event):
-        """
-        Sets the allow_shell attribute.
-        """
+        """Sets the allow_shell attribute."""
         self.__allow_shell = event.data
         # Hides the command entry if allow_python and allow_shell are False
         if not self.__allow_python and not self.__allow_shell:
             self.command_entry.grid_remove()
         # Shows the command entry if allow_python or allow_shell are True
         else:
             self.command_entry.grid(row=1, column=0, sticky='nsew')
 
     def __set_cursor_position(self, event):
-        """
-        Sets the cursor_position attribute.
-        """
+        """Sets the cursor_position attribute."""
         new_value = self.cursor_position != event.data
 
         # Removes the cursor from the last position
-        if self.cursor_position is not None and (self.__cursor_counter % 50 == 0 or new_value):
-            index = self.logs.index(f'end-{len(self.input_text) - self.cursor_position + 2}c')
-            self.logs.tag_add(index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c')
-            self.logs.tag_config(index, background=self.default_background_color,
-                                 foreground=self.default_foreground_color)
+        if self.cursor_position is not None and (self.__cursor_counter % 50 == 0
+                                                 or new_value):
+            index = self.logs.index(
+                f'end-{len(self.input_text) - self.cursor_position + 2}c'
+            )
+            self.logs.tag_add(
+                index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c'
+            )
+            self.logs.tag_config(
+                index,
+                background=self.default_background_color,
+                foreground=self.default_foreground_color
+            )
         self._cursor_position = event.data
 
         self.__cursor_counter += 1
         # Places the new cursor
         if self.getting_input_status == GettingInputStatus.GETTING_INPUT and (
                 self.__cursor_counter % 100 == 0 or new_value):
             self.__cursor_counter = 1
-            index = self.logs.index(f'end-{len(self.input_text) - self.cursor_position + 2}c')
-            self.logs.tag_add(index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c')
-            self.logs.tag_config(index, background=self.default_foreground_color,
-                                 foreground=self.default_background_color)
+            index = self.logs.index(
+                f'end-{len(self.input_text) - self.cursor_position + 2}c'
+            )
+            self.logs.tag_add(
+                index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c'
+            )
+            self.logs.tag_config(
+                index,
+                background=self.default_foreground_color,
+                foreground=self.default_background_color
+            )
 
     def __set_default_foreground_color(self, event):
-        """
-        Sets the default_foreground_color attribute.
-        """
+        """Sets the default_foreground_color attribute."""
         self._default_foreground_color = event.data
         self.logs.config(foreground=event.data)
 
     def __set_default_background_color(self, event):
-        """
-        Sets the default_background_color attribute.
-        """
+        """Sets the default_background_color attribute."""
         self._default_background_color = event.data
         self.logs.config(background=event.data)
 
     def __set_font(self, event):
-        """
-        Sets the font attribute.
-        """
+        """Sets the font attribute."""
         self.logs.config(font=event.data)
 
     def __set_width(self, event):
-        """
-        Sets the width attribute.
-        """
+        """Sets the width attribute."""
         self.logs.config(width=event.data)
 
     def __set_height(self, event):
-        """
-        Sets the height attribute.
-        """
+        """Sets the height attribute."""
         self.logs.config(height=event.data)
 
     @property
     def allow_python(self):
         return self.__allow_python
 
     @allow_python.setter
@@ -678,23 +802,27 @@
 
     @property
     def default_foreground_color(self):
         return self._default_foreground_color
 
     @default_foreground_color.setter
     def default_foreground_color(self, value):
-        self.window.event_generate('<<SetDefaultForegroundColor>>', when='tail', data=value)
+        self.window.event_generate(
+            '<<SetDefaultForegroundColor>>', when='tail', data=value
+        )
 
     @property
     def default_background_color(self):
         return self._default_background_color
 
     @default_background_color.setter
     def default_background_color(self, value):
-        self.window.event_generate('<<SetDefaultBackgroundColor>>', when='tail', data=value)
+        self.window.event_generate(
+            '<<SetDefaultBackgroundColor>>', when='tail', data=value
+        )
 
     @property
     def font(self):
         return self.logs.config()['font']
 
     @font.setter
     def font(self, value):
@@ -715,27 +843,33 @@
     @height.setter
     def height(self, value):
         self.window.event_generate('<<SetHeight>>', when='tail', data=value)
 
     @property
     def progress_bar(self):
         if not self._progress_bar:
+            # Import here to avoid circular import
+            # pylint: disable=import-outside-toplevel
             from log21.ProgressBar import ProgressBar
             self._progress_bar = ProgressBar(logger=self, width=self.width)
         self.window.update()
         return self._progress_bar
 
     def __del__(self):
         self.window.withdraw()
         self.window.destroy()
         del self.window
 
 
 if not _tkinter:
-    class LoggingWindow:
+
+    class LoggingWindow:  # pylint: disable=function-redefined
+        """LoggingWindow requires tkinter to be installed."""
+
         def __init__(self, *args, **kwargs):
             raise ImportError('LoggingWindow requires tkinter to be installed.')
 
+    class LoggingWindowHandler:  # pylint: disable=function-redefined
+        """LoggingWindow requires tkinter to be installed."""
 
-    class LoggingWindowHandler:
         def __init__(self, *args, **kwargs):
             raise ImportError('LoggingWindow requires tkinter to be installed.')
```

### Comparing `log21-2.6.0/src/log21/Manager.py` & `log21-2.6.1/src/log21/Manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # log21.Manager.py
 # CodeWriter21
 
 import logging as _logging
 from typing import Union as _Union
-from log21.Logger import Logger as _loggerClass
+
 from log21.Levels import INFO as _INFO
+from log21.Logger import Logger as _loggerClass
 
 root = _logging.RootLogger(_INFO)
 
 
 class Manager(_logging.Manager):
+    """The Manager class is a subclass of the logging.Manager class. It
+    overrides the getLogger method to make it more compatible with the
+    log21.Logger class. It also overrides the constructor."""
+
     def __init__(self):
         self.root = root
         self.disable = 0
         self.emittedNoHandlerWarning = False
         self.loggerDict = {}
         self.loggerClass = None
         self.logRecordFactory = None
 
     def getLogger(self, name: str) -> _Union[_logging.Logger, _loggerClass, None]:
-        """
-        Takes the name of a logger and if there was a logger with that name in the loggerDict it will return the logger
-        otherwise it'll return None.
+        """Takes the name of a logger and if there was a logger with that name
+        in the loggerDict it will return the logger otherwise it'll return
+        None.
 
         :param name: The name of the logger.
         :raises TypeError: A logger name must be a string
         :return:
         """
         if not isinstance(name, str):
             raise TypeError('A logger name must be a string')
@@ -34,21 +39,20 @@
                 rv = self.loggerDict[name]
                 if isinstance(rv, _logging.PlaceHolder):
                     rv = (self.loggerClass or _loggerClass)(name)
                     rv.manager = self
                     self.loggerDict[name] = rv
             else:
                 return None
-        except Exception:
+        except Exception:  # pylint: disable=broad-except
             return None
         return rv
 
-    def addLogger(self, name: str, logger) -> None:
-        """
-        Adds a logger to the loggerDict dictionary.
+    def addLogger(self, name: str, logger) -> None:  # pylint: disable=invalid-name
+        """Adds a logger to the loggerDict dictionary.
 
         :param name: str: The name of the logger.
         :param logger: The logger to save.
         :raises TypeError: A logger name must be a string
         :return: None
         """
         if not isinstance(name, str):
```

### Comparing `log21-2.6.0/src/log21/PPrint.py` & `log21-2.6.1/src/log21/PPrint.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 # CodeWriter21
 
 import re as _re
 import sys as _sys
 import types as _types
 import collections as _collections
 import dataclasses as _dataclasses
-
 from pprint import PrettyPrinter as _PrettyPrinter
-from typing import Mapping as _Mapping, Optional as _Optional, Dict as _Dict
+from typing import Dict as _Dict, Mapping as _Mapping, Optional as _Optional
 
 from log21.Colors import get_colors as _gc
 
 _builtin_scalars = frozenset({str, bytes, bytearray, float, complex, bool, type(None)})
 
 
 def _recursion(obj):
     return f"<Recursion on {type(obj).__name__} with id={id(obj)}>"
 
 
 def _safe_tuple(t):
-    """Helper function for comparing 2-tuples"""
+    """Helper function for comparing 2-tuples."""
     return _SafeKey(t[0]), _SafeKey(t[1])
 
 
 def _wrap_bytes_repr(obj, width, allowance):
     current = b''
     last = len(obj) // 4 * 4
     for i in range(0, len(obj), 4):
-        part = obj[i: i + 4]
+        part = obj[i:i + 4]
         candidate = current + part
         if i == last:
             width -= allowance
         if len(repr(candidate)) > width:
             if current:
                 yield repr(current)
             current = part
@@ -45,33 +44,52 @@
 class _SafeKey:
     """Helper function for key functions when sorting unorderable objects.
 
     The wrapped-object will fallback to a Py2.x style comparison for
     unorderable types (sorting first comparing the type name and then by
     the obj ids).  Does not work recursively, so dict.items() must have
     _safe_key applied to both the key and the value.
-
     """
 
     __slots__ = ['obj']
 
     def __init__(self, obj):
         self.obj = obj
 
     def __lt__(self, other):
         try:
             return self.obj < other.obj
         except TypeError:
-            return (str(type(self.obj)), id(self.obj)) < (str(type(other.obj)), id(other.obj))
+            return (str(type(self.obj)), id(self.obj
+                                            )) < (str(type(other.obj)), id(other.obj))
 
 
 class PrettyPrinter(_PrettyPrinter):
-    def __init__(self, indent=1, width=80, depth=None, stream=None, sign_colors: _Optional[_Mapping[str, str]] = None,
-                 *, compact=False, sort_dicts=True, underscore_numbers=False, **kwargs):
-        super().__init__(indent=indent, width=width, depth=depth, stream=stream, compact=compact, **kwargs)
+
+    def __init__(
+        self,
+        indent=1,
+        width=80,
+        depth=None,
+        stream=None,
+        sign_colors: _Optional[_Mapping[str, str]] = None,
+        *,
+        compact=False,
+        sort_dicts=True,
+        underscore_numbers=False,
+        **kwargs
+    ):
+        super().__init__(
+            indent=indent,
+            width=width,
+            depth=depth,
+            stream=stream,
+            compact=compact,
+            **kwargs
+        )
         self._depth = depth
         self._indent_per_level = indent
         self._width = width
         if stream is not None:
             self._stream = stream
         else:
             self._stream = _sys.stdout
@@ -104,37 +122,39 @@
         if len(rep) > max_width:
             p = self._dispatch.get(type(obj).__repr__, None)
             if p is not None:
                 context[objid] = 1
                 p(self, obj, stream, indent, allowance, context, level + 1)
                 del context[objid]
                 return
-            elif (_dataclasses.is_dataclass(obj) and
-                  not isinstance(obj, type) and
-                  obj.__dataclass_params__.repr and
-                  # Check dataclass has generated repr method.
-                  hasattr(obj.__repr__, "__wrapped__") and
-                  "__create_fn__" in obj.__repr__.__wrapped__.__qualname__):
+            elif (_dataclasses.is_dataclass(obj) and not isinstance(obj, type)
+                  and obj.__dataclass_params__.repr
+                  and  # Check dataclass has generated repr method.
+                  hasattr(obj.__repr__, "__wrapped__")
+                  and "__create_fn__" in obj.__repr__.__wrapped__.__qualname__):
                 context[objid] = 1
-                self._pprint_dataclass(obj, stream, indent, allowance, context, level + 1)
+                self._pprint_dataclass(
+                    obj, stream, indent, allowance, context, level + 1
+                )
                 del context[objid]
                 return
         stream.write(rep)
 
     def _pprint_dataclass(self, obj, stream, indent, allowance, context, level):
         cls_name = obj.__class__.__name__
         indent += len(cls_name) + 1
-        items = [(f.name, getattr(obj, f.name)) for f in _dataclasses.fields(obj) if f.repr]
+        items = [
+            (f.name, getattr(obj, f.name)) for f in _dataclasses.fields(obj) if f.repr
+        ]
         stream.write(cls_name + '(')
         self._format_namespace_items(items, stream, indent, allowance, context, level)
         stream.write(')')
 
     def _repr(self, obj, context, level):
-        repr, readable, recursive = self.format(obj, context.copy(),
-                                                self._depth, level)
+        repr, readable, recursive = self.format(obj, context.copy(), self._depth, level)
         if not readable:
             self._readable = False
         if recursive:
             self._recursive = True
         return repr
 
     def _safe_repr(self, object_, context, max_levels, level):
@@ -149,15 +169,17 @@
             if self._underscore_numbers:
                 return f"{object_:_d}", True, False
             else:
                 return repr(object_), True, False
 
         if issubclass(type_, dict) and representation is dict.__repr__:
             if not object_:
-                return self.sign_colors.get('curly-braces') + "{}" + self.sign_colors.get('data'), True, False
+                return self.sign_colors.get(
+                    'curly-braces'
+                ) + "{}" + self.sign_colors.get('data'), True, False
             object_id = id(object_)
             if max_levels and level >= max_levels:
                 return self.sign_colors.get('curly-braces') + "{" + self.sign_colors.get('...') + "..." + \
                        self.sign_colors.get('curly-braces') + "}" + self.sign_colors.get('data'), \
                        False, object_id in context
             if object_id in context:
                 return _recursion(object_), False, True
@@ -170,42 +192,50 @@
             if self._sort_dicts:
                 items = sorted(object_.items(), key=_safe_tuple)
             else:
                 items = object_.items()
             for k, v in items:
                 krepr, kreadable, krecur = self.format(k, context, max_levels, level)
                 vrepr, vreadable, vrecur = self.format(v, context, max_levels, level)
-                append(f"{krepr}{self.sign_colors.get('colon')}:{self.sign_colors.get('data')} {vrepr}")
+                append(
+                    f"{krepr}{self.sign_colors.get('colon')}:{self.sign_colors.get('data')} {vrepr}"
+                )
                 readable = readable and kreadable and vreadable
                 if krecur or vrecur:
                     recursive = True
             del context[object_id]
             return self.sign_colors.get('curly-braces') + "{" + self.sign_colors.get('data') + \
                    (self.sign_colors.get('comma') + ", " + self.sign_colors.get('data')).join(components) + \
                    self.sign_colors.get('curly-braces') + "}", readable, recursive
 
         if (issubclass(type_, list) and representation is list.__repr__) or \
                 (issubclass(type_, tuple) and representation is tuple.__repr__):
             if issubclass(type_, list):
                 if not object_:
-                    return self.sign_colors.get('square-brackets') + "[]" + self.sign_colors.get('data'), True, False
+                    return self.sign_colors.get(
+                        'square-brackets'
+                    ) + "[]" + self.sign_colors.get('data'), True, False
                 format_ = self.sign_colors.get('square-brackets') + "[" + self.sign_colors.get('data') + "%s" + \
                           self.sign_colors.get('square-brackets') + "]" + self.sign_colors.get('data')
             elif len(object_) == 1:
                 format_ = self.sign_colors.get('parenthesis') + "(" + self.sign_colors.get('data') + "%s" + \
                           self.sign_colors.get('comma') + "," + self.sign_colors.get('parenthesis') + ")" + \
                           self.sign_colors.get('data')
             else:
                 if not object_:
-                    return self.sign_colors.get('parenthesis') + "()" + self.sign_colors.get('data'), True, False
+                    return self.sign_colors.get(
+                        'parenthesis'
+                    ) + "()" + self.sign_colors.get('data'), True, False
                 format_ = self.sign_colors.get('parenthesis') + "(" + self.sign_colors.get('data') + "%s" + \
                           self.sign_colors.get('parenthesis') + ")" + self.sign_colors.get('data')
             object_id = id(object_)
             if max_levels and level >= max_levels:
-                return format_ % self.sign_colors.get('...') + "...", False, object_id in context
+                return format_ % self.sign_colors.get(
+                    '...'
+                ) + "...", False, object_id in context
             if object_id in context:
                 return _recursion(object_), False, True
             context[object_id] = 1
             readable = True
             recursive = False
             components = []
             append = components.append
@@ -233,69 +263,92 @@
             write((self._indent_per_level - 1) * ' ')
         length = len(obj)
         if length:
             if self._sort_dicts:
                 items = sorted(obj.items(), key=_safe_tuple)
             else:
                 items = obj.items()
-            self._format_dict_items(items, stream, indent, allowance + 1,
-                                    context, level)
+            self._format_dict_items(
+                items, stream, indent, allowance + 1, context, level
+            )
         write(self.sign_colors.get('curly-braces') + '}' + self.sign_colors.get('data'))
 
     _dispatch[dict.__repr__] = _pprint_dict
 
     def _pprint_ordered_dict(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
-        self._format(list(obj.items()), stream,
-                     indent + len(cls.__name__) + 1, allowance + 1,
-                     context, level)
-        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data')
+        )
+        self._format(
+            list(obj.items()), stream, indent + len(cls.__name__) + 1, allowance + 1,
+            context, level
+        )
+        stream.write(
+            self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data')
+        )
 
     _dispatch[_collections.OrderedDict.__repr__] = _pprint_ordered_dict
 
     def _pprint_list(self, obj, stream, indent, allowance, context, level):
-        stream.write(self.sign_colors.get('square-brackets') + '[' + self.sign_colors.get('data'))
-        self._format_items(obj, stream, indent, allowance + 1,
-                           context, level)
-        stream.write(self.sign_colors.get('square-brackets') + ']' + self.sign_colors.get('data'))
+        stream.write(
+            self.sign_colors.get('square-brackets') + '[' +
+            self.sign_colors.get('data')
+        )
+        self._format_items(obj, stream, indent, allowance + 1, context, level)
+        stream.write(
+            self.sign_colors.get('square-brackets') + ']' +
+            self.sign_colors.get('data')
+        )
 
     _dispatch[list.__repr__] = _pprint_list
 
     def _pprint_tuple(self, obj, stream, indent, allowance, context, level):
-        stream.write(self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
+        stream.write(
+            self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data')
+        )
         endchar = self.sign_colors.get('comma') + ',' + self.sign_colors.get('parenthesis') + ')' + \
                   self.sign_colors.get('data') if len(obj) == 1 else self.sign_colors.get('parenthesis') + ')' + \
                                                                       self.sign_colors.get('data')
-        self._format_items(obj, stream, indent, allowance + len(endchar),
-                           context, level)
+        self._format_items(
+            obj, stream, indent, allowance + len(endchar), context, level
+        )
         stream.write(endchar)
 
     _dispatch[tuple.__repr__] = _pprint_tuple
 
     def _pprint_set(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         typ = obj.__class__
         if typ is set:
-            stream.write(self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data'))
-            endchar = self.sign_colors.get('curly-braces') + '}' + self.sign_colors.get('data')
+            stream.write(
+                self.sign_colors.get('curly-braces') + '{' +
+                self.sign_colors.get('data')
+            )
+            endchar = self.sign_colors.get('curly-braces'
+                                           ) + '}' + self.sign_colors.get('data')
         else:
-            stream.write(typ.__name__ + self.sign_colors.get('parenthesis') + '(' +
-                         self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data'))
+            stream.write(
+                typ.__name__ + self.sign_colors.get('parenthesis') + '(' +
+                self.sign_colors.get('curly-braces') + '{' +
+                self.sign_colors.get('data')
+            )
             endchar = self.sign_colors.get('curly-braces') + '}' + self.sign_colors.get('parenthesis') + ')' \
                       + self.sign_colors.get('data')
             indent += len(typ.__name__) + 1
         obj = sorted(obj, key=_SafeKey)
-        self._format_items(obj, stream, indent, allowance + len(endchar),
-                           context, level)
+        self._format_items(
+            obj, stream, indent, allowance + len(endchar), context, level
+        )
         stream.write(endchar)
 
     _dispatch[set.__repr__] = _pprint_set
     _dispatch[frozenset.__repr__] = _pprint_set
 
     def _pprint_str(self, object_, stream, indent, allowance, context, level):
         write = stream.write
@@ -335,116 +388,153 @@
                         current = candidate
                 if current:
                     chunks.append(repr(current))
         if len(chunks) == 1:
             write(representation)
             return
         if level == 1:
-            write(self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
+            write(
+                self.sign_colors.get('parenthesis') + '(' +
+                self.sign_colors.get('data')
+            )
         for i, representation in enumerate(chunks):
             if i > 0:
                 write('\n' + ' ' * indent)
             write(representation)
         if level == 1:
-            write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+            write(
+                self.sign_colors.get('parenthesis') + ')' +
+                self.sign_colors.get('data')
+            )
 
     _dispatch[str.__repr__] = _pprint_str
 
     def _pprint_bytes(self, obj, stream, indent, allowance, context, level):
         write = stream.write
         if len(obj) <= 4:
             write(repr(obj))
             return
         parens = level == 1
         if parens:
             indent += 1
             allowance += 1
-            write(self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
+            write(
+                self.sign_colors.get('parenthesis') + '(' +
+                self.sign_colors.get('data')
+            )
         delim = ''
         for rep in _wrap_bytes_repr(obj, self._width - indent, allowance):
             write(delim)
             write(rep)
             if not delim:
                 delim = '\n' + ' ' * indent
         if parens:
-            write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+            write(
+                self.sign_colors.get('parenthesis') + ')' +
+                self.sign_colors.get('data')
+            )
 
     _dispatch[bytes.__repr__] = _pprint_bytes
 
     def _pprint_bytearray(self, obj, stream, indent, allowance, context, level):
         write = stream.write
-        write('bytearray' + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
-        self._pprint_bytes(bytes(obj), stream, indent + 10,
-                           allowance + 1, context, level + 1)
+        write(
+            'bytearray' + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data')
+        )
+        self._pprint_bytes(
+            bytes(obj), stream, indent + 10, allowance + 1, context, level + 1
+        )
         write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
 
     _dispatch[bytearray.__repr__] = _pprint_bytearray
 
     def _pprint_mappingproxy(self, obj, stream, indent, allowance, context, level):
-        stream.write('mappingproxy' + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
-        self._format(obj.copy(), stream, indent + 13, allowance + 1,
-                     context, level)
-        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+        stream.write(
+            'mappingproxy' + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data')
+        )
+        self._format(obj.copy(), stream, indent + 13, allowance + 1, context, level)
+        stream.write(
+            self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data')
+        )
 
     _dispatch[_types.MappingProxyType.__repr__] = _pprint_mappingproxy
 
     def _pprint_simplenamespace(self, obj, stream, indent, allowance, context, level):
         if type(obj) is _types.SimpleNamespace:
             # The SimpleNamespace repr is "namespace" instead of the class
             # name, so we do the same here. For subclasses; use the class name.
             cls_name = 'namespace'
         else:
             cls_name = obj.__class__.__name__
         indent += len(cls_name) + 1
         items = obj.__dict__.items()
-        stream.write(cls_name + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
+        stream.write(
+            cls_name + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data')
+        )
         self._format_namespace_items(items, stream, indent, allowance, context, level)
-        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+        stream.write(
+            self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data')
+        )
 
     _dispatch[_types.SimpleNamespace.__repr__] = _pprint_simplenamespace
 
     def _format_dict_items(self, items, stream, indent, allowance, context, level):
         write = stream.write
         indent += self._indent_per_level
-        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent
+        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get(
+            'data'
+        ) + ' ' * indent
         last_index = len(items) - 1
         for i, (key, ent) in enumerate(items):
             last = i == last_index
             rep = self._repr(key, context, level)
             write(rep)
             write(self.sign_colors.get('colon') + ': ' + self.sign_colors.get('data'))
-            self._format(ent, stream, indent + len(rep) + 2,
-                         allowance if last else 1,
-                         context, level)
+            self._format(
+                ent, stream, indent + len(rep) + 2, allowance if last else 1, context,
+                level
+            )
             if not last:
                 write(delimnl)
 
     def _format_namespace_items(self, items, stream, indent, allowance, context, level):
         write = stream.write
-        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent
+        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get(
+            'data'
+        ) + ' ' * indent
         last_index = len(items) - 1
         for i, (key, ent) in enumerate(items):
             last = i == last_index
             write(key)
             write('=')
             if id(ent) in context:
                 # Special-case representation of recursion to match standard
                 # recursive dataclass repr.
-                write(self.sign_colors.get('...') + "..." + self.sign_colors.get('data'))
+                write(
+                    self.sign_colors.get('...') + "..." + self.sign_colors.get('data')
+                )
             else:
-                self._format(ent, stream, indent + len(key) + 1, allowance if last else 1, context, level)
+                self._format(
+                    ent, stream, indent + len(key) + 1, allowance if last else 1,
+                    context, level
+                )
             if not last:
                 write(delimnl)
 
     def _format_items(self, items, stream, indent, allowance, context, level):
         write = stream.write
         indent += self._indent_per_level
         if self._indent_per_level > 1:
             write((self._indent_per_level - 1) * ' ')
-        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent
+        delimnl = self.sign_colors.get('comma') + ',\n' + self.sign_colors.get(
+            'data'
+        ) + ' ' * indent
         delim = ''
         width = max_width = self._width - indent + 1
         it = iter(items)
         try:
             next_ent = next(it)
         except StopIteration:
             return
@@ -463,90 +553,120 @@
                 if width < w:
                     width = max_width
                     if delim:
                         delim = delimnl
                 if width >= w:
                     width -= w
                     write(delim)
-                    delim = self.sign_colors.get('comma') + ', ' + self.sign_colors.get('data')
+                    delim = self.sign_colors.get('comma') + ', ' + self.sign_colors.get(
+                        'data'
+                    )
                     write(rep)
                     continue
             write(delim)
             delim = delimnl
             self._format(ent, stream, indent, allowance if last else 1, context, level)
 
     def _pprint_default_dict(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         rdf = self._repr(obj.default_factory, context, level)
         cls = obj.__class__
         indent += len(cls.__name__) + 1
-        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data') + rdf +
-                     self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + (' ' * indent))
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data') + rdf + self.sign_colors.get('comma') + ',\n' +
+            self.sign_colors.get('data') + (' ' * indent)
+        )
         self._pprint_dict(obj, stream, indent, allowance + 1, context, level)
-        stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+        stream.write(
+            self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data')
+        )
 
     _dispatch[_collections.defaultdict.__repr__] = _pprint_default_dict
 
     def _pprint_counter(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
-                     self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data'))
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data')
+        )
         if self._indent_per_level > 1:
             stream.write((self._indent_per_level - 1) * ' ')
         items = obj.most_common()
-        self._format_dict_items(items, stream,
-                                indent + len(cls.__name__) + 1, allowance + 2,
-                                context, level)
-        stream.write(self.sign_colors.get('curly-braces') + '}' +
-                     self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+        self._format_dict_items(
+            items, stream, indent + len(cls.__name__) + 1, allowance + 2, context, level
+        )
+        stream.write(
+            self.sign_colors.get('curly-braces') + '}' +
+            self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data')
+        )
 
     _dispatch[_collections.Counter.__repr__] = _pprint_counter
 
     def _pprint_chain_map(self, obj, stream, indent, allowance, context, level):
         if not len(obj.maps):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data')
+        )
         indent += len(cls.__name__) + 1
         for i, m in enumerate(obj.maps):
             if i == len(obj.maps) - 1:
                 self._format(m, stream, indent, allowance + 1, context, level)
-                stream.write(self.sign_colors.get('parenthesis') + ')' + self.sign_colors.get('data'))
+                stream.write(
+                    self.sign_colors.get('parenthesis') + ')' +
+                    self.sign_colors.get('data')
+                )
             else:
                 self._format(m, stream, indent, 1, context, level)
-                stream.write(self.sign_colors.get('comma') + ',\n' + self.sign_colors.get('data') + ' ' * indent)
+                stream.write(
+                    self.sign_colors.get('comma') + ',\n' +
+                    self.sign_colors.get('data') + ' ' * indent
+                )
 
     _dispatch[_collections.ChainMap.__repr__] = _pprint_chain_map
 
     def _pprint_deque(self, obj, stream, indent, allowance, context, level):
         if not len(obj):
             stream.write(repr(obj))
             return
         cls = obj.__class__
-        stream.write(cls.__name__ + self.sign_colors.get('parenthesis') + '(' + self.sign_colors.get('data'))
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data')
+        )
         indent += len(cls.__name__) + 1
-        stream.write(self.sign_colors.get('square-brackets') + '[' + self.sign_colors.get('data'))
+        stream.write(
+            self.sign_colors.get('square-brackets') + '[' +
+            self.sign_colors.get('data')
+        )
         if obj.maxlen is None:
-            self._format_items(obj, stream, indent, allowance + 2,
-                               context, level)
-            stream.write(self.sign_colors.get('square-brackets') + ']' + self.sign_colors.get('parenthesis') + ')' +
-                         self.sign_colors.get('data'))
+            self._format_items(obj, stream, indent, allowance + 2, context, level)
+            stream.write(
+                self.sign_colors.get('square-brackets') + ']' +
+                self.sign_colors.get('parenthesis') + ')' +
+                self.sign_colors.get('data')
+            )
         else:
-            self._format_items(obj, stream, indent, 2,
-                               context, level)
+            self._format_items(obj, stream, indent, 2, context, level)
             rml = self._repr(obj.maxlen, context, level)
-            stream.write(self.sign_colors.get('square-brackets') + ']' + self.sign_colors.get('comma') +
-                         ',' + self.sign_colors.get('data') + '\n' + (' ' * indent) + 'maxlen=' + rml +
-                         self.sign_colors.get('parenthesis') + ')')
+            stream.write(
+                self.sign_colors.get('square-brackets') + ']' +
+                self.sign_colors.get('comma') + ',' + self.sign_colors.get('data') +
+                '\n' + (' ' * indent) + 'maxlen=' + rml +
+                self.sign_colors.get('parenthesis') + ')'
+            )
 
     _dispatch[_collections.deque.__repr__] = _pprint_deque
 
     def _pprint_user_dict(self, obj, stream, indent, allowance, context, level):
         self._format(obj.data, stream, indent, allowance, context, level - 1)
 
     _dispatch[_collections.UserDict.__repr__] = _pprint_user_dict
@@ -558,12 +678,30 @@
 
     def _pprint_user_string(self, obj, stream, indent, allowance, context, level):
         self._format(obj.data, stream, indent, allowance, context, level - 1)
 
     _dispatch[_collections.UserString.__repr__] = _pprint_user_string
 
 
-def pformat(obj, indent=1, width=80, depth=None, signs_colors: _Optional[_Mapping[str, str]] = None, *, compact=False,
-            sort_dicts=True, underscore_numbers=False, **kwargs):
+def pformat(
+    obj,
+    indent=1,
+    width=80,
+    depth=None,
+    signs_colors: _Optional[_Mapping[str, str]] = None,
+    *,
+    compact=False,
+    sort_dicts=True,
+    underscore_numbers=False,
+    **kwargs
+):
     """Format a Python object into a pretty-printed representation."""
-    return PrettyPrinter(indent=indent, width=width, depth=depth, compact=compact, sign_colors=signs_colors,
-                         sort_dicts=sort_dicts, underscore_numbers=underscore_numbers, **kwargs).pformat(obj)
+    return PrettyPrinter(
+        indent=indent,
+        width=width,
+        depth=depth,
+        compact=compact,
+        sign_colors=signs_colors,
+        sort_dicts=sort_dicts,
+        underscore_numbers=underscore_numbers,
+        **kwargs
+    ).pformat(obj)
```

### Comparing `log21-2.6.0/src/log21/ProgressBar.py` & `log21-2.6.1/src/log21/ProgressBar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # log21.ProgressBar.py
 # CodeWriter21
 
 from __future__ import annotations
 
 import shutil as _shutil
-
-from typing import Mapping as _Mapping, Any as _Any, Optional as _Optional
+from typing import Any as _Any, Mapping as _Mapping, Optional as _Optional
 
 import log21 as _log21
+from log21.Colors import get_colors as _gc
 from log21.Logger import Logger as _Logger
 from log21.StreamHandler import ColorizingStreamHandler as _ColorizingStreamHandler
-from log21.Colors import get_colors as _gc
 
 _logger = _Logger('ProgressBar')
 _logger.addHandler(_ColorizingStreamHandler())
 
 __all__ = ['ProgressBar']
 
 
-class ProgressBar:
+class ProgressBar:  # pylint: disable=too-many-instance-attributes, line-too-long
     """
     Usage Example:
         >>> pb = ProgressBar(width=20, show_percentage=False, prefix='[', suffix=']', fill='=', empty='-')
         >>> pb(0, 10)
         [/-----------------]
         >>> pb(1, 10)
         [==----------------]
@@ -37,33 +36,48 @@
         ...     time.sleep(0.01)
         ...
         |████████████████████████████████████████████████████████████████████████████████████████████| 100%
         >>> # Of course, You should try it yourself to see the progress! XD
         >>>
     """
 
-    def __init__(self, *, width: _Optional[int] = None, show_percentage: bool = True, prefix: str = '|',
-                 suffix: str = '|', fill: str = '█', empty: str = ' ', format_: _Optional[str] = None, style: str = '%',
-                 new_line_when_complete: bool = True, colors: _Optional[_Mapping[str, str]] = None, no_color: bool = False,
-                 logger: _log21.Logger = _logger, additional_variables: _Optional[_Mapping[str, _Any]] = None):
+    def __init__(
+        self,
+        *,
+        width: _Optional[int] = None,
+        show_percentage: bool = True,
+        prefix: str = '|',
+        suffix: str = '|',
+        fill: str = '█',
+        empty: str = ' ',
+        format_: _Optional[str] = None,
+        style: str = '%',
+        new_line_when_complete: bool = True,
+        colors: _Optional[_Mapping[str, str]] = None,
+        no_color: bool = False,
+        logger: _log21.Logger = _logger,
+        additional_variables: _Optional[_Mapping[str, _Any]] = None
+    ):  # pylint: disable=too-many-branches, too-many-statements
         """
         :param args: Prevents the use of positional arguments
         :param width: The width of the progress bar
         :param show_percentage: Whether to show the percentage of the progress
         :param prefix: The prefix of the progress bar
         :param suffix: The suffix of the progress bar
         :param fill: The fill character of the progress bar
         :param empty: The empty character of the progress bar
         :param format_: The format of the progress bar
         :param style: The style that is used to format the progress bar
-        :param new_line_when_complete: Whether to print a new line when the progress is complete or failed
+        :param new_line_when_complete: Whether to print a new line when the progress is
+            complete or failed
         :param colors: The colors of the progress bar
         :param no_color: If True, removes the colors of the progress bar
         :param logger: The logger to use
-        :param additional_variables: Additional variables to use in the format and their default values
+        :param additional_variables: Additional variables to use in the format and their
+            default values
         """
         # Sets a default value for the width
         if width is None:
             try:
                 width = _shutil.get_terminal_size().columns - 1
             except OSError:
                 width = 50
@@ -83,25 +97,29 @@
         if len(fill) != 1:
             raise ValueError('`fill` must be a single character')
         if len(empty) != 1:
             raise ValueError('`empty` must be a single character')
         if style not in ['%', '{']:
             raise ValueError('`style` must be either `%` or `{`')
         if colors and no_color:
-            raise PermissionError('You cannot use `no_color` and `colors` parameters together!')
+            raise PermissionError(
+                'You cannot use `no_color` and `colors` parameters together!'
+            )
         if additional_variables:
             if not isinstance(additional_variables, _Mapping):
-                raise TypeError('`additional_variables` must be a dictionary like object.')
+                raise TypeError(
+                    '`additional_variables` must be a dictionary like object.'
+                )
             for key, value in additional_variables.items():
                 if not isinstance(key, str):
                     raise TypeError('`additional_variables` keys must be strings')
                 if not isinstance(value, str):
                     additional_variables[key] = str(value)
         else:
-            additional_variables = dict()
+            additional_variables = {}
 
         self.colors = {
             'progress in-progress': _gc('LightYellow'),
             'progress complete': _gc('LightGreen'),
             'progress failed': _gc('LightRed'),
             'percentage in-progress': _gc('LightBlue'),
             'percentage complete': _gc('LightCyan'),
@@ -134,22 +152,45 @@
         if no_color:
             self.colors = {name: '' for name in self.colors}
         self.logger = logger
         self.additional_variables = additional_variables
         self.i = 0
 
     def get_bar(self, progress: float, total: float, **kwargs) -> str:
+        """Return the progress bar as a string.
+
+        :param progress: The current progress. (e.g. 21)
+        :param total: The total progress. (e.g. 100)
+        :param kwargs: Additional variables to be used in the format
+            string.
+        :raises ValueError: If the style is not supported.
+            Set the style to one of the following:
+            + '%'
+            + '{'
+            e.g. bar = ProgressBar(style='{')
+        :return: The progress bar as a string.
+        """
         if progress == total:
             return self.progress_complete(**kwargs)
-        elif progress > total or progress < 0:
+        if progress > total or progress < 0:
             return self.progress_failed(progress, total, **kwargs)
-        else:
-            return self.progress_in_progress(progress, total, **kwargs)
+        return self.progress_in_progress(progress, total, **kwargs)
 
-    def progress_in_progress(self, progress: float, total: float, **kwargs):
+    def progress_in_progress(self, progress: float, total: float, **kwargs) -> str:
+        """Return the progress bar as a string when the progress is in
+        progress.
+
+        :param progress: The current progress. (e.g. 21)
+        :param total: The total progress. (e.g. 100)
+        :param kwargs: Additional variables to be used in the format
+            string.
+        :raises ValueError: If the style is not supported. (supported
+            styles: '%', '{')
+        :return: The progress bar as a string.
+        """
         percentage = str(round(progress / total * 100, 2))
         progress_dict = {
             'prefix': self.prefix,
             'bar': '',
             'suffix': self.suffix,
             'percentage': percentage,
             **self.additional_variables
@@ -172,32 +213,47 @@
         if self.i >= 3:
             self.i = 0
         else:
             self.i += 1
         spinner_char = self.spinner[self.i] if empty_length > 0 else ''
 
         progress_dict = {
-            'prefix': self.colors['prefix-color in-progress'] + self.prefix + self.colors['reset-color'],
-            'bar': self.colors['progress in-progress'] + (self.fill * fill_length + spinner_char +
-                                                          self.empty * empty_length) + self.colors['reset-color'],
-            'suffix': self.colors['suffix-color in-progress'] + self.suffix + self.colors['reset-color'],
-            'percentage': self.colors["percentage in-progress"] + str(percentage) + self.colors['reset-color'],
+            'prefix':
+            self.colors['prefix-color in-progress'] + self.prefix +
+            self.colors['reset-color'],
+            'bar':
+            self.colors['progress in-progress'] +
+            (self.fill * fill_length + spinner_char + self.empty * empty_length) +
+            self.colors['reset-color'],
+            'suffix':
+            self.colors['suffix-color in-progress'] + self.suffix +
+            self.colors['reset-color'],
+            'percentage':
+            self.colors["percentage in-progress"] + str(percentage) +
+            self.colors['reset-color'],
             **self.additional_variables
         }
         for key, value in kwargs.items():
             progress_dict[key] = value
 
         if self.style == '%':
             return '\r' + self.format % progress_dict + self.colors['reset-color']
-        elif self.style == '{':
-            return '\r' + self.format.format(**progress_dict) + self.colors['reset-color']
-        else:
-            raise ValueError('`style` must be either `%` or `{`')
-
-    def progress_complete(self, **kwargs):
+        if self.style == '{':
+            return '\r' + self.format.format(**progress_dict
+                                             ) + self.colors['reset-color']
+        raise ValueError('`style` must be either `%` or `{`')
+
+    def progress_complete(self, **kwargs) -> str:
+        """Prints the progress bar as complete.
+
+        :param kwargs: Additional variables to be passed to the format
+            string.
+        :raises ValueError: If the style is not either `%` or `{`.
+        :return: The formatted progress bar.
+        """
         progress_dict = {
             'prefix': self.prefix,
             'bar': '',
             'suffix': self.suffix,
             'percentage': '100',
             **self.additional_variables
         }
@@ -210,33 +266,52 @@
             bar_length = self.width - len(self.format % progress_dict)
         elif self.style == '{':
             bar_length = self.width - len(self.format.format(**progress_dict))
         else:
             raise ValueError('`style` must be either `%` or `{`')
 
         progress_dict = {
-            'prefix': self.colors['prefix-color complete'] + self.prefix + self.colors['reset-color'],
-            'bar': self.colors['progress complete'] + (self.fill * bar_length) + self.colors['reset-color'],
-            'suffix': self.colors['suffix-color complete'] + self.suffix + self.colors['reset-color'],
-            'percentage': self.colors["percentage complete"] + '100' + self.colors['reset-color'],
+            'prefix':
+            self.colors['prefix-color complete'] + self.prefix +
+            self.colors['reset-color'],
+            'bar':
+            self.colors['progress complete'] + (self.fill * bar_length) +
+            self.colors['reset-color'],
+            'suffix':
+            self.colors['suffix-color complete'] + self.suffix +
+            self.colors['reset-color'],
+            'percentage':
+            self.colors["percentage complete"] + '100' + self.colors['reset-color'],
             **self.additional_variables
         }
         for key, value in kwargs.items():
             progress_dict[key] = value
 
         if self.style == '%':
-            return '\r' + self.format % progress_dict + self.colors['reset-color'] + \
-                   ('\n' if self.new_line_when_complete else '')
-        elif self.style == '{':
-            return '\r' + self.format.format(**progress_dict) + self.colors['reset-color'] + \
-                   ('\n' if self.new_line_when_complete else '')
-        else:
-            raise ValueError('`style` must be either `%` or `{`')
+            return (
+                '\r' + self.format % progress_dict + self.colors['reset-color'] +
+                ('\n' if self.new_line_when_complete else '')
+            )
+        if self.style == '{':
+            return (
+                '\r' + self.format.format(**progress_dict) +
+                self.colors['reset-color'] +
+                ('\n' if self.new_line_when_complete else '')
+            )
+        raise ValueError('`style` must be either `%` or `{`')
 
     def progress_failed(self, progress: float, total: float, **kwargs):
+        """Returns a progress bar with a failed state.
+
+        :param progress: The current progress.
+        :param total: The total progress.
+        :param kwargs: Additional variables to be passed to the format string.
+        :raises ValueError: If the style is not `%` or `{`.
+        :return: A progress bar with a failed state.
+        """
         progress_dict = {
             'prefix': self.prefix,
             'bar': '',
             'suffix': self.suffix,
             'percentage': str(round(progress / total * 100, 2)),
             **self.additional_variables
         }
@@ -254,33 +329,64 @@
 
         if progress > total:
             bar_char = self.fill
         else:
             bar_char = self.empty
 
         progress_dict = {
-            'prefix': self.colors['prefix-color failed'] + self.prefix + self.colors['reset-color'],
-            'bar': self.colors['progress failed'] + (bar_char * bar_length) + self.colors['reset-color'],
-            'suffix': self.colors['suffix-color failed'] + self.suffix + self.colors['reset-color'],
-            'percentage': self.colors["percentage failed"] + progress_dict['percentage'] + self.colors['reset-color'],
+            'prefix':
+            self.colors['prefix-color failed'] + self.prefix +
+            self.colors['reset-color'],
+            'bar':
+            self.colors['progress failed'] + (bar_char * bar_length) +
+            self.colors['reset-color'],
+            'suffix':
+            self.colors['suffix-color failed'] + self.suffix +
+            self.colors['reset-color'],
+            'percentage':
+            self.colors["percentage failed"] + progress_dict['percentage'] +
+            self.colors['reset-color'],
             **self.additional_variables
         }
         for key, value in kwargs.items():
             progress_dict[key] = value
 
         if self.style == '%':
-            bar = self.format % progress_dict
+            progress_bar = self.format % progress_dict
         elif self.style == '{':
-            bar = self.format.format(**progress_dict)
+            progress_bar = self.format.format(**progress_dict)
         else:
             raise ValueError('`style` must be either `%` or `{`')
 
-        return '\r' + bar + self.colors['reset-color'] + ('\n' if self.new_line_when_complete else '')
-
-    def __call__(self, progress: float, total: float, logger: _Optional[_log21.Logger] = None, **kwargs):
+        return '\r' + progress_bar + self.colors['reset-color'] + (
+            '\n' if self.new_line_when_complete else ''
+        )
+
+    def __call__(
+        self,
+        progress: float,
+        total: float,
+        logger: _Optional[_log21.Logger] = None,
+        **kwargs
+    ):
         if not logger:
             logger = self.logger
 
         logger.print(self.get_bar(progress, total, **kwargs), end='')
 
-    def update(self, progress: float, total: float, logger: _Optional[_log21.Logger] = None, **kwargs):
+    def update(
+        self,
+        progress: float,
+        total: float,
+        logger: _Optional[_log21.Logger] = None,
+        **kwargs
+    ):
+        """Update the progress bar.
+
+        :param progress: The current progress.
+        :param total: The total progress.
+        :param logger: The logger to use. If not specified, the logger
+            specified in the constructor will be used.
+        :param kwargs: Additional variables to be used in the format string.
+        :raises ValueError: If the style is not `%` or `{`.
+        """
         self(progress, total, logger, **kwargs)
```

### Comparing `log21-2.6.0/src/log21/StreamHandler.py` & `log21-2.6.1/src/log21/StreamHandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,82 @@
 # log21.StreamHandler.py
 # CodeWriter21
 
 import os as _os
 import re as _re
 import shutil as _shutil
-
-from logging import StreamHandler as _StreamHandler
 from typing import Optional as _Optional
-from log21.Colors import ansi_escape as _ansi_escape, get_colors as _gc, hex_escape as _hex_escape
+from logging import StreamHandler as _StreamHandler
+
+from log21.Colors import (get_colors as _gc, hex_escape as _hex_escape,
+                          ansi_escape as _ansi_escape)
 
 __all__ = ['IS_WINDOWS', 'ColorizingStreamHandler', 'StreamHandler']
 
 IS_WINDOWS = _os.name == 'nt'
 
 if IS_WINDOWS:
     import ctypes
 
 
 class StreamHandler(_StreamHandler):
+    """A StreamHandler that can handle carriage returns and new lines."""
     terminator = ''
 
-    def __init__(self, handle_carriage_return: bool = True, handle_new_line: bool = True, stream=None, formatter=None,
-                 level=None):
+    def __init__(
+        self,
+        handle_carriage_return: bool = True,
+        handle_new_line: bool = True,
+        stream=None,
+        formatter=None,
+        level=None
+    ):
+        """Initialize the StreamHandler.
+
+        :param handle_carriage_return: Whether to handle carriage
+            returns.
+        :param handle_new_line: Whether to handle new lines.
+        :param stream: The stream to write to.
+        :param formatter: The formatter to use.
+        :param level: The level to log at.
+        """
         self.HandleCR = handle_carriage_return
         self.HandleNL = handle_new_line
         super().__init__(stream=stream)
         if formatter is not None:
             self.setFormatter(formatter)
         if level is not None:
             self.setLevel(level)
 
     def check_cr(self, record):
+        """Check if the record contains a carriage return and handle it."""
         if record.msg:
-            msg = _hex_escape.sub('', _ansi_escape.sub('', record.msg.strip(' \t\n\x0b\x0c')))
+            msg = _hex_escape.sub(
+                '', _ansi_escape.sub('', record.msg.strip(' \t\n\x0b\x0c'))
+            )
             if '\r' in msg[1:-1]:
                 file_descriptor = getattr(self.stream, 'fileno', None)
                 if file_descriptor:
                     file_descriptor = file_descriptor()
                     if file_descriptor in (1, 2):  # stdout or stderr
                         self.stream.write(
-                            '\r' + (' ' * (_shutil.get_terminal_size(file_descriptor).columns - 1)) + '\r')
+                            '\r' + (
+                                ' ' * (
+                                    _shutil.get_terminal_size(file_descriptor).columns -
+                                    1
+                                )
+                            ) + '\r'
+                        )
                         index = record.msg.rfind('\r')
                         find = _re.compile(r'(\x1b\[(?:\d+(?:;(?:\d+))*)m)')
-                        record.msg = _gc(*find.split(record.msg[:index])) + record.msg[index + 1:]
+                        record.msg = _gc(*find.split(record.msg[:index])
+                                         ) + record.msg[index + 1:]
 
     def check_nl(self, record):
+        """Check if the record contains a newline and handle it."""
         while record.msg and record.msg[0] == '\n':
             file_descriptor = getattr(self.stream, 'fileno', None)
             if file_descriptor:
                 file_descriptor = file_descriptor()
                 if file_descriptor in (1, 2):  # stdout or stderr
                     self.stream.write('\n')
                     record.msg = record.msg[1:]
@@ -57,16 +85,15 @@
         if self.HandleCR:
             self.check_cr(record)
         if self.HandleNL:
             self.check_nl(record)
         super().emit(record)
 
     def clear_line(self, length: _Optional[int] = None):
-        """
-        Clear the current line.
+        """Clear the current line.
 
         :param length: The length of the line to clear.
         :return:
         """
         file_descriptor = getattr(self.stream, 'fileno', None)
         if file_descriptor:
             file_descriptor = file_descriptor()
@@ -74,33 +101,37 @@
                 if length is None:
                     length = _shutil.get_terminal_size(file_descriptor).columns
                 self.stream.write('\r' + (' ' * (length - 1)) + '\r')
 
 
 # A stream handler that supports colorizing.
 class ColorizingStreamHandler(StreamHandler):
+    """A stream handler that supports colorizing even in Windows."""
+
     def emit(self, record):
         try:
             if self.HandleCR:
                 self.check_cr(record)
             if self.HandleNL:
                 self.check_nl(record)
             msg = self.format(record)
             if IS_WINDOWS:
                 self.convert_and_write(msg)
                 self.convert_and_write(self.terminator)
             else:
                 self.write(msg)
                 self.write(self.terminator)
             self.flush()
-        except Exception:
+        except Exception:  # pylint: disable=broad-except
             self.handleError(record)
 
     # Writes colorized text to the Windows console.
     def convert_and_write(self, message):
+        """Convert the message to a Windows console colorized message and write
+        it to the stream."""
         nt_color_map = {
             30: 0,  # foreground: black   - 0b00000000
             31: 4,  # foreground: red     - 0b00000100
             32: 2,  # foreground: green   - 0b00000010
             33: 6,  # foreground: yellow  - 0b00000110
             34: 1,  # foreground: blue    - 0b00000001
             35: 5,  # foreground: magenta - 0b00000101
@@ -153,19 +184,20 @@
             if parts:
                 params = parts.pop(0)
 
                 if win_handle is not None:
                     params = [int(p) for p in params.split(';')]
                     color = 0
 
-                    for p in params:
-                        if p in nt_color_map:
-                            color |= nt_color_map[p]
+                    for param in params:
+                        if param in nt_color_map:
+                            color |= nt_color_map[param]
                         else:
                             pass  # error condition ignored
 
                     ctypes.windll.kernel32.SetConsoleTextAttribute(win_handle, color)
 
     # Writes the message to the console.
     def write(self, message):
+        """Write the message to the stream."""
         self.stream.write(message)
         self.flush()
```

### Comparing `log21-2.6.0/src/log21/TreePrint.py` & `log21-2.6.1/src/log21/TreePrint.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 # log21.TreePrint.py
 # CodeWriter21
 
 from __future__ import annotations
 
-from typing import (
-    List as _List, Union as _Union, Mapping as _Mapping, Optional as _Optional, Sequence
-    as _Sequence
-)
+from typing import (List as _List, Union as _Union, Mapping as _Mapping,
+                    Optional as _Optional, Sequence as _Sequence)
 
 from log21.Colors import get_colors as _gc
 
 
 class TreePrint:
+    """A class to help you print objects in a tree-like format."""
 
     class Node:
+        """A class to represent a node in a tree."""
 
         def __init__(
             self,
             value: _Union[str, int],
             children: _Optional[_List[TreePrint.Node]] = None,
             indent: int = 4,
             colors: _Optional[_Mapping[str, str]] = None,
             mode: str = '-'
         ):
+            """Initialize a node.
+
+            :param value: The value of the node.
+            :param children: The children of the node.
+            :param indent: Number of spaces to indent the node.
+            :param colors: Colors to use for the node.
+            :param mode: Choose between '-' and '='.
+            """
             self.value = str(value)
             if children:
                 self._children = children
             else:
                 self._children = []
             self.indent = indent
             self.colors = {
                 'branches': _gc('Green'),
                 'fruit': _gc('LightMagenta'),
             }
 
             if colors:
-                for key, value in colors.items():
+                for key, value_ in colors.items():
                     if key in self.colors:
-                        self.colors[key] = _gc(value)
+                        self.colors[key] = _gc(value_)
             if not mode:
                 self.mode = 1
             else:
                 self.mode = self._get_mode(mode)
                 if self.mode == -1:
                     raise ValueError('`mode` must be - or =')
 
@@ -76,60 +84,65 @@
             else:
                 text += chars[0]  # ─ OR ═
 
             text += ' ' + _gc(self.colors['fruit']) + str(self.value) + '\n'
 
             for i, child in enumerate(self._children):
                 prefix_ = ''
-                for j in range(len(prefix)):
-                    if prefix[j] in '┌│├┬╔║╠╦':
+                for part in prefix:
+                    if part in '┌│├┬╔║╠╦':
                         prefix_ += chars[2]  # │ OR ║
-                    elif prefix[j] in chars:
+                    elif part in chars:
                         prefix_ += ' '
                     else:
-                        prefix_ += prefix[j]
+                        prefix_ += part
 
                 if i + 1 == len(self._children):
                     prefix_ += chars[6]  # └ OR ╚
                 else:
                     prefix_ += chars[5]  # ├ OR ╠
                 prefix_ += chars[0] * (self.indent - 1)  # ─ OR ═
                 prefix_ = prefix_[:len(prefix)] + _gc(self.colors['branches']
                                                       ) + prefix_[len(prefix):]
                 text += child.__str__(level=level + 1, prefix=prefix_, mode=mode)
 
             return text
 
         def has_child(self):
+            """Return True if node has children, False otherwise."""
             return len(self._children) > 0
 
         def add_child(self, child: TreePrint.Node):
+            """Add a child to the node."""
             if not isinstance(child, TreePrint.Node):
                 raise TypeError('`child` must be TreePrint.Node')
             self._children.append(child)
 
         def get_child(self, value: _Optional[str] = None, index: _Optional[int] = None):
+            """Get a child by value or index."""
             if value and index:
                 raise ValueError('`value` and `index` can not be both set')
             if not value and not index:
                 raise ValueError('`value` or `index` must be set')
             if value:
                 for child in self._children:
                     if child.value == value:
                         return child
             if index:
                 return self._children[index]
+            raise ValueError(f'Failed to find child: {value = }, {index = }')
 
         def add_to(
             self: TreePrint.Node,
             data: _Union[_Mapping, _Sequence, str, int],
             indent: int = 4,
             colors: _Optional[_Mapping[str, str]] = None,
             mode='-'
-        ):
+        ):  # pylint: disable=too-many-branches
+            """Add data to the node."""
             if isinstance(data, _Mapping):
                 if len(data) == 1:
                     child = TreePrint.Node(
                         list(data.keys())[0], indent=indent, colors=colors, mode=mode
                     )
                     child.add_to(
                         list(data.values())[0], indent=indent, colors=colors, mode=mode
@@ -202,22 +215,31 @@
             self.root = self.Node(str(data), indent=indent, colors=colors)
 
     def add_to_root(
         self,
         data: _Union[_Mapping, _Sequence, str, int],
         colors: _Optional[_Mapping[str, str]] = None
     ):
+        """Add data to root node."""
         self.root.add_to(data, indent=self.indent, colors=colors, mode=self.mode)
 
     def __str__(self, mode=None):
         if not mode:
             mode = self.mode
         return self.root.__str__(mode=mode)
 
 
 def tree_format(
     data: _Union[_Mapping, _Sequence, str, int],
     indent: int = 4,
     mode='-',
     colors: _Optional[_Mapping[str, str]] = None
-):
+) -> str:
+    """Return a tree representation of data.
+
+    :param data: data to be represented as a tree (dict, list, str, int)
+    :param indent: number of spaces to indent each level of the tree
+    :param mode: mode of tree representation ('-', '=')
+    :param colors: colors to use for each level of the tree
+    :return: tree representation of data
+    """
     return str(TreePrint(data, indent=indent, colors=colors, mode=mode))
```

### Comparing `log21-2.6.0/src/log21/__init__.py` & `log21-2.6.1/src/log21/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Argumentify import argumentify
 from log21.FileHandler import DecolorizingFileHandler
 from log21.ProgressBar import ProgressBar
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import StreamHandler, ColorizingStreamHandler
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = [
     'ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter',
     'DecolorizingFormatter', 'get_logger', 'Logger', 'Colors', 'get_color',
     'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN', 'INFO', 'DEBUG',
     'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter',
@@ -114,24 +114,25 @@
     >>>
     >>> l = log21.get_logger()
     >>> l.warning('Pretty basic, huh?')
     [14:49:41] [WARNING] Pretty basic, huh?
     >>> l.critical('CONTINUE READING!! please...')
     [14:50:08] [CRITICAL] CONTINUE READING!! please...
     >>>
-    >>> my_logger = log21.get_logger(name='CodeWriter21', level=log21.INFO, fmt='{asctime} -> [{levelname}]: {message}',
-    ... style='{', override=True)
+    >>> my_logger = log21.get_logger(name='CodeWriter21', level=log21.INFO,
+    ... fmt='{asctime} -> [{levelname}]: {message}', style='{', override=True)
     >>>
     >>> my_logger.info('FYI: My name is Mehrad.')
     14:56:12 -> [INFO]: FYI: My name is Mehrad.
     >>> my_logger.error(log21.get_color('LightRed') + 'Oh no! Something went wrong D:')
     14:56:29 -> [ERROR]: Oh no! Something went wrong D:
     >>>
     >>> my_logger.debug(1 ,2 ,3)
-    >>> # It prints Nothing because our logger level is INFO and DEBUG level is less than INFO.
+    >>> # It prints Nothing because our logger level is INFO and DEBUG level is lower
+    >>> # than INFO.
     >>> # So let's modify the my_logger's level
     >>> my_logger.setLevel(log21.DEBUG)
     >>> # Now we try again...
     >>> my_logger.debug(1, 2, 3)
     14:57:34 -> [DEBUG]: 1 2 3
     >>> # Well Done. Right?
     >>> # Let's see more
@@ -150,26 +151,31 @@
     >>> # See you soon!
     >>>
 
     :param name: Optional[str]: The name of the logger
     :param level: Union[int, str] = logging.NOTSET: The logging level of the logger
     :param show_time: bool = True: Show the time in the log
     :param show_level: bool = True: Show the level of logging in the log
-    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default(show_time & show_level)
+    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default
+        (show_time & show_level)
     :param datefmt: str = "%H:%M:%S": Custom date-time formatting for the logger
-    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that you want to use one of
-        %-formatting, :meth:`str.format` (``{}``) formatting or :class:`string.Template` formatting in your format
-        string.
-    :param colorize_time_and_level: bool = True: Colorizes the time and level using the default colors
-    :param handle_carriage_return: bool = True: Adds a line of space characters to remove any text before the CR
-    :param handle_new_line: bool = True: Places the NewLine characters at the beginning of the text before everything
-        else
-    :param override: bool = True: Overrides the logger attributes even if it already exists
+    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that
+        you want to use one of %-formatting, :meth:`str.format` (``{}``) formatting or
+        :class:`string.Template` formatting in your format string.
+    :param colorize_time_and_level: bool = True: Colorizes the time and level using the
+        default colors
+    :param handle_carriage_return: bool = True: Adds a line of space characters to
+        remove any text before the CR
+    :param handle_new_line: bool = True: Places the NewLine characters at the beginning
+        of the text before everything else
+    :param override: bool = True: Overrides the logger attributes even if it already
+        exists.
     :param level_names: Mapping[int, str] = None: You can specify custom level names.
-    :param level_colors: Mapping[int, Tuple[str, ...]] = None: You can specify custom level colors.
+    :param level_colors: Mapping[int, Tuple[str, ...]] = None: You can specify custom
+        level colors.
     :param file: Union[os.PathLike, str] = None: The file to log to
     :return: log21.Logger
     """
     if not isinstance(name, str):
         raise TypeError('A logger name must be a string')
     logger = None
     if name:
@@ -233,15 +239,16 @@
     >>> # Creates a new LoggingWindow object
     >>> window = log21.get_logging_window('Test Window')
     >>> # Now use it without any additional steps to add handlers and formatters!
     >>> # It works just like a normal logger but with some extra features
     >>>
     >>> window.info('This works properly!')
     >>>
-    >>> # You can use HEX colors as well as the ANSI colors which are supported by normal loggers
+    >>> # You can use HEX colors as well as the ANSI colors which are supported by
+    >>> # normal loggers
     >>> # ANSI colors usage:
     >>> window.info('This is a \033[91mred\033[0m message.')
     >>> window.info('\033[102mThis is a message with green background.')
     >>> # HEX colors usage:
     >>> window.info('\033#00FFFFhfThis is a message with cyan foreground.')
     >>> window.info('\033#0000FFhbThis is a message with blue background.')
     >>>
@@ -257,24 +264,28 @@
     >>> # Run these lines to see the messages in the window
     >>>
 
     :param name: Optional[str]: The name of the logger
     :param level: Union[int, str] = logging.NOTSET: The logging level of the logger
     :param show_time: bool = True: Show the time in the log
     :param show_level: bool = True: Show the level of logging in the log
-    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default(show_time & show_level)
+    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default
+        (show_time & show_level)
     :param datefmt: str = "%H:%M:%S": Custom date-time formatting for the logger
-    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that you want to use one of
-        %-formatting, :meth:`str.format` (``{}``) formatting or :class:`string.Template` formatting in your format
-        string.
-    :param colorize_time_and_level: bool = True: Colorizes the time and level using the default colors
-    :param handle_carriage_return: bool = True: Adds a line of space characters to remove any text before the CR
-    :param handle_new_line: bool = True: Places the NewLine characters at the beginning of the text before everything
-        else
-    :param override: bool = True: Overrides the logger attributes even if it already exists
+    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that
+        you want to use one of %-formatting, :meth:`str.format` (``{}``) formatting or
+        :class:`string.Template` formatting in your format string.
+    :param colorize_time_and_level: bool = True: Colorizes the time and level using the
+        default colors
+    :param handle_carriage_return: bool = True: Adds a line of space characters to
+        remove any text before the CR
+    :param handle_new_line: bool = True: Places the NewLine characters at the beginning
+        of the text before everything else
+    :param override: bool = True: Overrides the logger attributes even if it already
+        exists
     :param level_names: Mapping[int, str] = None: You can specify custom level names.
     :param width: int = 80: The width of the window
     :param height: int = 20: The height of the window
     :param allow_shell: bool = False: Allow the user to use the shell
     :return: log21.LoggingWindow
     """
     if not isinstance(name, str):
@@ -302,25 +313,41 @@
         _manager.addLogger(name, logging_window)
     return logging_window
 
 
 getLogger = get_logger
 
 
-def print(*msg, args: tuple = (), end='\033[0m\n', **kwargs):
+def print(  # pylint: disable=redefined-builtin
+    *msg,
+    args: tuple = (),
+    end='\033[0m\n',
+    **kwargs
+):
+    """Works like the print function but ANSI colors are supported (even on
+    Windows) and it ends with a new line and a reset color by default."""
     logger = get_logger('log21.print', level=DEBUG, show_time=False, show_level=False)
     logger.print(*msg, args=args, end=end, **kwargs)
 
 
-def input(*msg, args: tuple = (), end='', **kwargs):
+def input(  # pylint: disable=redefined-builtin
+    *msg,
+    args: tuple = (),
+    end='',
+    **kwargs
+):
+    """Works like the input function but ANSI colors are supported (even on
+    Windows)."""
     logger = get_logger('log21.input', level=DEBUG, show_time=False, show_level=False)
     return logger.input(*msg, args=args, end=end, **kwargs)
 
 
 def getpass(*msg, args: tuple = (), end='', **kwargs):
+    """Works like the getpass.getpass function but ANSI colors are supported
+    (even on Windows)."""
     logger = get_logger('log21.getpass', level=DEBUG, show_time=False, show_level=False)
     return logger.getpass(*msg, args=args, end=end, **kwargs)
 
 
 def pprint(
     obj,
     indent=1,
@@ -330,14 +357,32 @@
     *,
     sort_dicts=True,
     underscore_numbers=False,
     compact=False,
     end='\033[0m\n',
     **kwargs
 ):
+    """A colorful version of the pprint.pprint function.
+
+    :param obj: The object to print.
+    :param indent: The amount of indentation to use.
+    :param width: The maximum width in characters of the output.
+    :param depth: The maximum depth to print nested structures. None
+        means unlimited.
+    :param signs_colors: A mapping that lets you specify the colors of
+        the supported signs.
+    :param sort_dicts: If True, dictionaries are sorted by key.
+    :param underscore_numbers: If True, numbers are printed with an
+        underscore between each group of three digits.
+    :param compact: If True, lists and tuples are displayed on a single
+        line.
+    :param end: The string to append at the end of the output.
+    :param kwargs: Additional keyword arguments passed to the
+        Logger.print function.
+    """
     logger = get_logger('log21.pprint', level=DEBUG, show_time=False, show_level=False)
     logger.print(
         pformat(
             obj=obj,
             indent=indent,
             width=width,
             depth=depth,
@@ -354,18 +399,29 @@
 pretty_print = pprint
 
 
 def tree_print(
     obj,
     indent: int = 4,
     mode='-',
-    colors: _Mapping[str, str] = None,
+    colors: _Optional[_Mapping[str, str]] = None,
     end='\033[0m\n',
     **kwargs
 ):
+    """Prints a tree representation of the given object. (e.g. a dictionary)
+
+    :param obj: The object to print.
+    :param indent: The number of spaces to indent each level.
+    :param mode: The mode to use for the tree. Can be '-' or '='.
+    :param colors: A mapping that lets you customize the colors of
+        branches and fruits.
+    :param end: The string to append at the end of the output.
+    :param kwargs: Additional keyword arguments passed to the
+        Logger.print function.
+    """
     logger = get_logger(
         'log21.tree_print', level=DEBUG, show_time=False, show_level=False
     )
     logger.print(
         tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs
     )
 
@@ -373,25 +429,25 @@
 tprint = tree_print
 
 root = Logger('root-logger', INFO)
 
 
 def basic_config(
     force: bool = False,
-    encoding: str = None,
+    encoding: _Optional[str] = None,
     errors: _Optional[str] = 'backslashreplace',
     handlers=None,
     stream=None,
     filename=None,
     filemode: str = 'a',
     date_format: str = "%H:%M:%S",
     style: str = '%',
-    format_: str = None,
-    level: _Union[int, str] = None
-):
+    format_: _Optional[str] = None,
+    level: _Optional[_Union[int, str]] = None
+):  # pylint: disable=too-many-branches
     """Do basic configuration for the logging system.
 
     This function does nothing if the root logger already has handlers
     configured, unless the keyword argument *force* is set to ``True``.
     It is a convenience method intended for use by simple scripts
     to do one-shot configuration of the logging package.
 
@@ -447,15 +503,16 @@
             if stream and filename:
                 raise ValueError(
                     "'stream' and 'filename' should not be specified together"
                 )
         else:
             if stream or filename:
                 raise ValueError(
-                    "'stream' or 'filename' should not be specified together with 'handlers'"
+                    "'stream' or 'filename' should not be specified together with "
+                    "'handlers'"
                 )
         if handlers is None:
             if filename:
                 if 'b' in filemode:
                     errors = None
                 else:
                     encoding = _io.text_encoding(encoding)
@@ -469,16 +526,14 @@
             raise ValueError('Style must be one of: %, {, $')
         if not format_:
             format_ = {
                 '%': '[%(asctime)s] [%(levelname)s] %(message)s',
                 '{': '[{asctime}] [{levelname}] {message}',
                 '$': '[${asctime}] [${levelname}] ${message}'
             }[style]
-        else:
-            format_ = format_
         formatter = ColorizingFormatter(format_, date_format, style=style)
         for handler in handlers:
             if handler.formatter is None:
                 handler.setFormatter(formatter)
             root.addHandler(handler)
         if level is not None:
             root.setLevel(level)
@@ -532,14 +587,15 @@
     """
     if len(root.handlers) == 0:
         basic_config()
     root.warning(*msg, args=args, **kwargs)
 
 
 def warn(*msg, args=(), **kwargs):
+    """An alias of warning()"""
     warning(*msg, args=args, **kwargs)
 
 
 def info(*msg, args=(), **kwargs):
     """Log a message with severity 'INFO' on the root logger.
 
     If the logger has no handlers, call basicConfig() to add a console
@@ -578,17 +634,17 @@
     width: _Optional[int] = None,
     prefix: str = '|',
     suffix: str = '|',
     show_percentage: bool = True
 ):
     """Print a progress bar to the console."""
 
-    bar = ProgressBar(
+    progress_bar_ = ProgressBar(
         width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage
     )
 
-    print(bar.get_bar(progress, total))
+    print(progress_bar_.get_bar(progress, total))
 
 
 console_reporter = CrashReporter.ConsoleReporter()
 
 file_reporter = CrashReporter.FileReporter(file='crash_report.log')
```

### Comparing `log21-2.6.0/src/log21.egg-info/PKG-INFO` & `log21-2.6.1/src/log21.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
 ![stars](https://img.shields.io/github/stars/MPCodeWriter21/log21)
@@ -79,17 +80,20 @@
 ```bash
 pip install git+https://github.com/MPCodeWriter21/log21
 ```
 
 Changes
 -------
 
-### 2.6.0
+### 2.6.1
 
-Added the `Argumentify` module. Check the examples.
+Added `encoding` to `log21.CrashReporter.FileReporter`.
+Added configs for `pylint`, `yapf` and `isort` to `pyproject.toml`.
+Added optional `dev` dependencies to `pyproject.toml`.
+Improved overall code quality.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
 
@@ -115,15 +119,15 @@
 logger.error(log21.get_colors('LightRed') + "I'm still here ;1")
 ```
 
 ![Basic Logging](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-1.png)
 
 ----------------
 
-### Argument Parsing (See Also: [Argumentify](https://github.com/MPCodeWriter21/log21#argumentify))
+### Argument Parsing (See Also: [Argumentify](https://github.com/MPCodeWriter21/log21#argumentify-check-out-the-manual-way))
 
 ```python
 import log21
 from log21 import ColorizingArgumentParser, get_logger, get_colors as gc
 
 parser = ColorizingArgumentParser(description="This is a simple example of a ColorizingArgumentParser.",
                                   colors={'help': 'LightCyan'})
@@ -273,15 +277,15 @@
 ```
 
 ![ProgressBar - Example 1](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.1.gif)
 ![ProgressBar - Example 2](https://github.com/MPCodeWriter21/log21/raw/master/screen-shots/example-5.2.gif)
 
 ------------------
 
-### Argumentify (Check out [the manual way](https://github.com/MPCodeWriter21/log21#argument-parsing))
+### Argumentify (Check out [the manual way](https://github.com/MPCodeWriter21/log21#argumentify-check-out-the-manual-way))
 
 ```python
 # Common Section
 import log21
 
 
 class ReversedText:
```

### Comparing `log21-2.6.0/src/log21.egg-info/SOURCES.txt` & `log21-2.6.1/src/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

