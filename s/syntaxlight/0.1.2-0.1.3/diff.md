# Comparing `tmp/syntaxlight-0.1.2.tar.gz` & `tmp/syntaxlight-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.1.2.tar", max compression
+gzip compressed data, was "syntaxlight-0.1.3.tar", max compression
```

## Comparing `syntaxlight-0.1.2.tar` & `syntaxlight-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.2/LICENSE
--rw-r--r--   0        0        0      463 2023-08-03 09:09:19.351998 syntaxlight-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.2/README.md
--rw-r--r--   0        0        0      225 2023-07-29 15:28:20.515491 syntaxlight-0.1.2/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.2/syntaxlight/ast.py
--rw-r--r--   0        0        0     2244 2023-07-30 03:01:17.999345 syntaxlight-0.1.2/syntaxlight/css/all.css
--rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.2/syntaxlight/css/asm.css
--rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.2/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.2/syntaxlight/css/c.css
--rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.2/syntaxlight/css/css.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.2/syntaxlight/css/index.css
--rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.2/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.2/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.2/syntaxlight/css/makefile.css
--rw-r--r--   0        0        0      876 2023-08-01 01:05:24.169127 syntaxlight-0.1.2/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     2907 2023-08-02 06:45:18.634086 syntaxlight-0.1.2/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.2/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.2/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.2/syntaxlight/error.py
--rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.2/syntaxlight/example.py
--rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.2/syntaxlight/export.py
--rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.2/syntaxlight/gdt.py
--rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.2/syntaxlight/language.py
--rw-r--r--   0        0        0      567 2023-08-02 08:37:35.901602 syntaxlight-0.1.2/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.2/syntaxlight/lexers/asm_lexer.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.2/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.2/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.2/syntaxlight/lexers/css_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.2/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    24348 2023-08-02 05:55:13.541695 syntaxlight-0.1.2/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.2/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.2/syntaxlight/lexers/makefile_lexer.py
--rw-r--r--   0        0        0     4457 2023-08-02 08:39:10.819146 syntaxlight-0.1.2/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.2/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.2/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.2/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.2/syntaxlight/parsers/asm_parser.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.2/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0   104738 2023-08-03 08:51:42.795428 syntaxlight-0.1.2/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.2/syntaxlight/parsers/css_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.2/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.2/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.2/syntaxlight/parsers/makefile_parser.py
--rw-r--r--   0        0        0    13420 2023-08-02 07:49:45.535569 syntaxlight-0.1.2/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     4619 2023-08-02 08:26:36.227646 syntaxlight-0.1.2/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.2/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.2/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.2/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.2/syntaxlight/template.html
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.3/LICENSE
+-rw-r--r--   0        0        0      463 2023-08-05 13:52:25.613007 syntaxlight-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.3/README.md
+-rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.3/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.3/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2244 2023-07-30 03:01:17.999345 syntaxlight-0.1.3/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.3/syntaxlight/css/asm.css
+-rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.3/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.3/syntaxlight/css/c.css
+-rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.3/syntaxlight/css/css.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.3/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.3/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.3/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.3/syntaxlight/css/makefile.css
+-rw-r--r--   0        0        0      876 2023-08-01 01:05:24.169127 syntaxlight-0.1.3/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     2907 2023-08-02 06:45:18.634086 syntaxlight-0.1.3/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.3/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.3/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.3/syntaxlight/error.py
+-rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.3/syntaxlight/example.py
+-rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.3/syntaxlight/export.py
+-rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.3/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.3/syntaxlight/language.py
+-rw-r--r--   0        0        0      579 2023-08-05 06:18:01.794963 syntaxlight-0.1.3/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.3/syntaxlight/lexers/asm_lexer.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.3/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.3/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.3/syntaxlight/lexers/css_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.3/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.3/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.3/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.3/syntaxlight/lexers/makefile_lexer.py
+-rw-r--r--   0        0        0     4457 2023-08-02 08:39:10.819146 syntaxlight-0.1.3/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.3/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.3/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.3/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.3/syntaxlight/parsers/asm_parser.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.3/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   106244 2023-08-05 13:51:29.921960 syntaxlight-0.1.3/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.3/syntaxlight/parsers/css_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.3/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.3/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.3/syntaxlight/parsers/makefile_parser.py
+-rw-r--r--   0        0        0    13418 2023-08-05 02:43:25.809482 syntaxlight-0.1.3/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     4619 2023-08-02 08:26:36.227646 syntaxlight-0.1.3/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.3/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.3/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.3/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.3/syntaxlight/template.html
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.3/PKG-INFO
```

### Comparing `syntaxlight-0.1.2/LICENSE` & `syntaxlight-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/README.md` & `syntaxlight-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/ast.py` & `syntaxlight-0.1.3/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/all.css` & `syntaxlight-0.1.3/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/asm.css` & `syntaxlight-0.1.3/syntaxlight/css/asm.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/bnf.css` & `syntaxlight-0.1.3/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/c.css` & `syntaxlight-0.1.3/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/css.css` & `syntaxlight-0.1.3/syntaxlight/css/css.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/index.css` & `syntaxlight-0.1.3/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/json.css` & `syntaxlight-0.1.3/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/lua.css` & `syntaxlight-0.1.3/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/makefile.css` & `syntaxlight-0.1.3/syntaxlight/css/makefile.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/shell.css` & `syntaxlight-0.1.3/syntaxlight/css/shell.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/themes.json` & `syntaxlight-0.1.3/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/css/toml.css` & `syntaxlight-0.1.3/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/error.py` & `syntaxlight-0.1.3/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/example.py` & `syntaxlight-0.1.3/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/export.py` & `syntaxlight-0.1.3/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/gdt.py` & `syntaxlight-0.1.3/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/language.py` & `syntaxlight-0.1.3/syntaxlight/language.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/__init__.py` & `syntaxlight-0.1.3/syntaxlight/lexers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .lexer import Lexer, TokenType, Token
+from .lexer import Lexer, TokenType, Token, TokenSet
 from .c_lexer import CLexer, CTokenType, CTokenSet
 from .lua_lexer import LuaLexer, LuaTokenType, LuaTokenSet
 from .json_lexer import JsonLexer, JsonTokenType
 from .toml_lexer import TomlLexer, TomlTokenType
 from .xml_lexer import XmlLexer, XmlTokenType
 from .shell_lexer import ShellLexer, ShellTokenType
 from .bnf_lexer import BNFLexer, BNFTokenType
 from .asm_lexer import AssemblyLexer, AssemblyTokenType
 from .css_lexer import CSSLexer, CSSTokenType
-from .makefile_lexer import MakefileLexer, MakefileTokenType
+from .makefile_lexer import MakefileLexer, MakefileTokenType
```

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/asm_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/asm_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/css_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/css_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,7 +693,10 @@
                 for token_type in arg._token_set:
                     self._token_set.add(token_type)
             else:
                 raise TypeError(args)
 
     def __contains__(self, item):
         return item in self._token_set
+
+    def __eq__(self, __value: object) -> bool:
+        return self.__contains__(__value)
```

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/makefile_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/makefile_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.1.3/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/asm_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/asm_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/c_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,28 +737,29 @@
         else:
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN, "should be StorageType or BaseType or QualifyType"
             )
 
         return node
 
-    def _unknown_typedef_id_guess(self):
+    def _unknown_typedef_id_guess(self, next_token_types=[TokenType.ID, TokenType.MUL]):
         """
         @扩展文法
 
         对于未知符号, 判断下一个 token 类型, 更正为 TYPEDEF_ID
 
         - static clock_t ticks = 10;                  ID
         - static clock_t *ticks = 10;                 *
+
+        下面这种情况没有办法匹配, 唯一的解决措施是在前面手动声明 uint64 的 typedef 或 define
         - static uint64 (*syscalls[])(void)           (
         """
-        if self.current_token.type == TokenType.ID and self.peek_next_token().type in (
-            TokenType.ID,
-            TokenType.MUL,
-            # TokenType.LPAREN
+        if (
+            self.current_token.type == TokenType.ID
+            and self.peek_next_token().type in next_token_types
         ):
             self.current_token.type = CTokenType.TYPEDEF_ID
             GDT.register_id(self.current_token.value, CSS.TYPEDEF)
 
     def storage_class_specifier(self):
         """
         <storage-class-specifier> ::= 'auto'
@@ -1266,41 +1267,72 @@
             [TokenType.MUL, TokenType.DIV, TokenType.MOD], self.cast_expression
         )
 
     def cast_expression(self):
         """
         <cast-expression> ::= ("(" <type-name> ")")* <unary-expression>
 
-        @修改文法?
+        @修改文法
         个人感觉这里存在问题, 对于 Person* ptr = &(Person) { "Bob", 30, { 50, 60 } }; 这里的 <type-name> 会被优先匹配到, 而不是匹配后面 <primary-expression> => "(" <type-name> ")" "{" <initializer-list> (",")? "}"
 
         所以这里做了一个对于 <initializer-list> 的补充
         """
         node = CastExpression()
         type_names = []
-        while (
-            self.current_token.type == TokenType.LPAREN
-            and self.peek_next_token().type in self.cfirst_set.type_name
+        
+        '''
+        @扩展文法
+        对于强制类型转换 (uint64)trampoline (见 test/c/40.c)
+        '''
+        while self.current_token.type == TokenType.LPAREN and (
+            self.peek_next_token().type in self.cfirst_set.type_name or self._type_cast_check()
         ):
-            node.register_token(self.eat(TokenType.LPAREN))
-            type_names.append(self.type_name())
-            node.register_token(self.eat(TokenType.RPAREN))
+            if self.peek_next_token().type in self.cfirst_set.type_name:
+                node.register_token(self.eat(TokenType.LPAREN))
+                type_names.append(self.type_name())
+                node.register_token(self.eat(TokenType.RPAREN))
+            else:
+                node.register_token(self.eat(TokenType.LPAREN))
+                self.current_token.type = CTokenType.TYPEDEF_ID
+                GDT.register_id(self.current_token.value, CSS.TYPEDEF)
+                type_names.append(self.type_name())
+                node.register_token(self.eat(TokenType.RPAREN))
         node.update(type_names=type_names)
         if self.current_token.type in self.cfirst_set.unary_expression:
             node.update(expr=self.unary_expression())
         elif self.current_token.type == TokenType.LCURLY_BRACE:
             node.register_token(self.eat(TokenType.LCURLY_BRACE))
             node.update(initializer_list=self.initializer_list())
             if self.current_token.type == TokenType.COMMA:
                 node.register_token(self.eat())
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be unary expression or (")
         return node
 
+    def _type_cast_check(self):
+        '''
+        强制类型转换的情况
+
+        (uint8) <unary-expression>
+        (uint8 *) <unary-expression>
+        (uint8 ****) <unary-expression>
+        '''
+        if self.peek_next_token().type == TokenType.ID:
+            if self.peek_next_token(2).type == TokenType.RPAREN and self.peek_next_token(3).type in self.cfirst_set.unary_expression:
+                return True
+            elif self.peek_next_token(2).type == TokenType.MUL:
+                n = 3
+                while self.peek_next_token(n).type == TokenType.MUL:
+                    n += 1
+                if self.peek_next_token(n).type == TokenType.RPAREN and self.peek_next_token(n+1).type in self.cfirst_set.unary_expression:
+                    return True
+
+        return False
+
     def unary_expression(self):
         """
         <unary-expression> ::= <postfix-expression>
                              | "++" <unary-expression>
                              | "--" <unary-expression>
                              | <unary-operator> <cast-expression>
                              | sizeof <unary-expression>
@@ -1533,46 +1565,44 @@
             node.update(type_name=self.type_name())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be default or type-name")
         node.register_token(self.eat(TokenType.COLON))
         node.update(assignment_expr=self.assignment_expression())
         return node
 
-    def _match_macro_function(self, macro_name:str):
+    def _match_macro_function(self, macro_name: str):
         """
         匹配不符合 C 文法的宏定义函数
 
         1. 对于全大写 ID 的会被认为是宏函数
 
            XBOX_ARG_BOOLEAN(NULL, [-h][--help][help = "show help information"])
 
         2. 对于前面定义过的宏函数会被匹配
 
            #define container_of()
 
            struct ipc_namespace *ns = container_of(table->data, struct ipc_namespace, shm_rmid_forced);
         """
-        
+
         assert self.current_token.type == TokenType.LPAREN
         self.eat(TokenType.LPAREN)
         brace_number = 1
 
         while self.current_token.type != TokenType.EOF:
             if self.current_token.type == TokenType.RPAREN:
                 brace_number -= 1
                 if brace_number == 0:
                     self.eat()
                     return
             elif self.current_token.type == TokenType.LPAREN:
                 brace_number += 1
             self.pp_token()
 
-        self.error(ErrorCode.BRACE_MISS_MATCH, f'in macro define function {macro_name}')
-
-
+        self.error(ErrorCode.BRACE_MISS_MATCH, f"in macro define function {macro_name}")
 
     def expression(self):
         """
         <expression> ::= <assignment-expression> ("," <assignment-expression>)*
         """
         node = Expression()
         exprs = [self.assignment_expression()]
```

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/css_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/css_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/makefile_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/makefile_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import html
 import traceback
 import re
 from ..gdt import CSS
 
 
 DEBUG = False
-# DEBUG = True
+DEBUG = True
 
 
 class Parser:
     def __init__(
         self, lexer, skip_invisible_characters=True, skip_space=True, display_warning=True
     ):
         self.lexer: Lexer = lexer
```

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/shell_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/shell_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.1.3/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/syntaxlight/syntax_parse.py` & `syntaxlight-0.1.3/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.2/PKG-INFO` & `syntaxlight-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.1.2
+Version: 0.1.3
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

