# Comparing `tmp/mdit_py_hugo-0.1.0.tar.gz` & `tmp/mdit_py_hugo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdit_py_hugo-0.1.0.tar", max compression
+gzip compressed data, was "mdit_py_hugo-0.2.0.tar", max compression
```

## Comparing `mdit_py_hugo-0.1.0.tar` & `mdit_py_hugo-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
-drwxr-xr-x   0        0        0        0 2023-07-31 16:17:29.050884 mdit_py_hugo-0.1.0/LICENSES/
--rwxr-xr-x   0        0        0      332 2023-07-31 19:35:29.213034 mdit_py_hugo-0.1.0/README.md
--rwxr-xr-x   0        0        0        0 2023-07-31 13:57:13.449392 mdit_py_hugo-0.1.0/mdit_py_hugo/__init__.py
--rwxr-xr-x   0        0        0     3581 2023-08-01 10:13:39.216239 mdit_py_hugo-0.1.0/mdit_py_hugo/attribute.py
--rwxr-xr-x   0        0        0      196 2023-07-31 19:22:48.255216 mdit_py_hugo-0.1.0/mdit_py_hugo/renderer_localized_md.py
--rwxr-xr-x   0        0        0      332 2023-07-31 16:16:49.287483 mdit_py_hugo-0.1.0/mdit_py_hugo/shortcode.py
--rwxr-xr-x   0        0        0     1016 2023-07-31 19:35:29.387120 mdit_py_hugo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 mdit_py_hugo-0.1.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-31 16:17:29.050884 mdit_py_hugo-0.2.0/LICENSES/
+-rwxr-xr-x   0        0        0      332 2023-07-31 19:35:29.213034 mdit_py_hugo-0.2.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-08-05 04:18:37.211407 mdit_py_hugo-0.2.0/mdit_py_hugo/__init__.py
+-rwxr-xr-x   0        0        0     8724 2023-08-05 16:15:29.834882 mdit_py_hugo-0.2.0/mdit_py_hugo/_shortcode_parsing.py
+-rwxr-xr-x   0        0        0     3163 2023-08-01 20:38:50.977067 mdit_py_hugo-0.2.0/mdit_py_hugo/attribute.py
+-rwxr-xr-x   0        0        0      196 2023-07-31 19:22:48.255216 mdit_py_hugo-0.2.0/mdit_py_hugo/renderer_localized_md.py
+-rwxr-xr-x   0        0        0     1398 2023-08-05 04:28:39.164808 mdit_py_hugo-0.2.0/mdit_py_hugo/shortcode.py
+-rwxr-xr-x   0        0        0     1016 2023-08-05 16:54:51.291759 mdit_py_hugo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 mdit_py_hugo-0.2.0/PKG-INFO
```

### Comparing `mdit_py_hugo-0.1.0/mdit_py_hugo/attribute.py` & `mdit_py_hugo-0.2.0/mdit_py_hugo/attribute.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 - on the same line for titles (heading, lheading);
 - on a new line directly below for blocks (blockquote, hr, list, paragraph, table),
     - no effect for other blocks (code, fence, html_block, reference).
 """
 
 import logging
 import re
-from typing import List
 
 from markdown_it import MarkdownIt
 from markdown_it.rules_core import StateCore
-from markdown_it.token import Token
-from mdit_py_plugins.attrs.index import _attr_block_rule
+from mdit_py_plugins.attrs.index import _attr_block_rule, _find_opening
 from mdit_py_plugins.attrs.parse import parse, ParseError
 
 LOGGER = logging.getLogger(__name__)
 
 
 def attribute_plugin(mdi: MarkdownIt) -> None:
     # alt: list of rules which can be terminated by this one
@@ -29,57 +27,48 @@
                            'attribute_block',
                            _attr_block_rule,
                            {'alt': ['blockquote', 'lheading', 'list', 'paragraph', 'reference', 'table']})
     mdi.core.ruler.after('block', 'attribute_block', _attribute_resolve_block_rule)
     mdi.core.ruler.after('block', 'attribute_title', _attribute_resolve_title_rule)
 
 
-def _find_affected_open(tokens: List[Token], from_index: int) -> int:
-    affected_close_tokens = ['blockquote_close', 'hr', 'bullet_list_close', 'ordered_list_close',
-                             'paragraph_close', 'table_close']
-    # unaffected_tokens = ['code_block', 'fence', 'heading_close', 'html_block'] + ['attrs_block']
-    # Hugo doesn't stack attributes, only closest attribute block is used
-    if tokens[from_index].type == 'hr':
-        return from_index
-    if tokens[from_index].type in affected_close_tokens:
-        for i in range(from_index-1, -1, -1):
-            if (tokens[i].type == tokens[from_index].type.replace('close', 'open') and
-                    tokens[i].level == tokens[from_index].level):
-                return i
-    return -1
-
-
 def _attribute_resolve_block_rule(state: StateCore) -> None:
     """Find an attribute block, move its attributes to the previous affected block."""
+    affected_closing_tokens = ['blockquote_close', 'hr', 'bullet_list_close', 'ordered_list_close',
+                               'paragraph_close', 'table_close']
+    # unaffected_tokens = ['code_block', 'fence', 'heading_close', 'html_block'] + ['attrs_block']
+    # Hugo doesn't stack attributes, only closest attribute block is used
     tokens = state.tokens
     i = len(tokens) - 1
     while i > 0:
         if state.tokens[i].type != "attrs_block":
             i -= 1
             continue
 
-        affected_index = _find_affected_open(tokens, i-1)
-        if affected_index > -1:
-            if 'class' in tokens[i].attrs:
-                tokens[affected_index].attrs['class'] = tokens[i].attrs['class']
+        closing_index = i - 1
+        if tokens[closing_index].type == 'hr':
+            affected_index = closing_index
+        elif tokens[closing_index].type in affected_closing_tokens:
+            affected_index = _find_opening(tokens, closing_index)
+        else:
+            affected_index = None
+        if affected_index is not None:
             tokens[affected_index].attrs.update(tokens[i].attrs)
 
         state.tokens.pop(i)
         i -= 1
 
 
 def _attribute_resolve_title_rule(state: StateCore) -> None:
     """Find a heading block, move attributes left in its 'inline' to its 'heading_open' token."""
     tokens = state.tokens
-    pattern = re.compile(r'^(.+)({.+?}) *$')
+    attribute_pattern = re.compile(r'^(.+)({.+?}) *$')
     for i in range(0, len(tokens)-2):
         # after a 'heading_open' must be an 'inline'
-        if tokens[i].type == 'heading_open' and (match := pattern.fullmatch(tokens[i+1].content)):
+        if tokens[i].type == 'heading_open' and (match := attribute_pattern.fullmatch(tokens[i+1].content)):
             tokens[i+1].content = match.group(1)
             try:
                 _, attrs = parse(match.group(2))
             except ParseError:
                 LOGGER.error(f'Could not parse attributes "{match.group(2)}" in heading "{match.group(0)}"')
                 continue
-            if 'class' in attrs:
-                tokens[i].attrs['class'] = attrs['class']
             tokens[i].attrs.update(attrs)
```

### Comparing `mdit_py_hugo-0.1.0/pyproject.toml` & `mdit_py_hugo-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023 Phu Hung Nguyen <phuhnguyen@outlook.com>
 # SPDX-License-Identifier: CC0-1.0
 
 [tool.poetry]
 name = "mdit-py-hugo"
-version = "0.1.0"
+version = "0.2.0"
 description = "Collection of markdown-it-py plugins and extensions that add supports for Hugo syntaxes and functionalities"
 authors = ["Phu Hung Nguyen <phuhnguyen@outlook.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/phunh/mdit-py-hugo"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `mdit_py_hugo-0.1.0/PKG-INFO` & `mdit_py_hugo-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdit-py-hugo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Collection of markdown-it-py plugins and extensions that add supports for Hugo syntaxes and functionalities
 Home-page: https://github.com/phunh/mdit-py-hugo
 License: AGPL-3.0-or-later
 Author: Phu Hung Nguyen
 Author-email: phuhnguyen@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

