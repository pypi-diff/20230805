# Comparing `tmp/nice65-0.1.2.tar.gz` & `tmp/nice65-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice65-0.1.2.tar", last modified: Sat Aug  5 10:49:42 2023, max compression
+gzip compressed data, was "nice65-0.1.3.tar", last modified: Sat Aug  5 17:43:13 2023, max compression
```

## Comparing `nice65-0.1.2.tar` & `nice65-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:49:42.157905 nice65-0.1.2/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.2/LICENSE
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3997 2023-08-05 10:49:42.157905 nice65-0.1.2/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3577 2023-08-05 10:49:20.000000 nice65-0.1.2/README.md
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:49:42.154572 nice65-0.1.2/nice65/
--rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.2/nice65/__init__.py
--rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.2/nice65/__main__.py
--rwxr-xr-x   0 anderson  (1000) anderson  (1000)     8804 2023-08-05 10:48:46.000000 nice65-0.1.2/nice65/app.py
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:49:42.157905 nice65-0.1.2/nice65.egg-info/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3997 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/SOURCES.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/dependency_links.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/entry_points.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/requires.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/top_level.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-05 10:49:35.000000 nice65-0.1.2/pyproject.toml
--rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-05 10:49:42.157905 nice65-0.1.2/setup.cfg
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 17:43:13.567893 nice65-0.1.3/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.3/LICENSE
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3997 2023-08-05 17:43:13.567893 nice65-0.1.3/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3577 2023-08-05 10:49:20.000000 nice65-0.1.3/README.md
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 17:43:13.567893 nice65-0.1.3/nice65/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.3/nice65/__init__.py
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.3/nice65/__main__.py
+-rwxr-xr-x   0 anderson  (1000) anderson  (1000)     9194 2023-08-05 17:41:29.000000 nice65-0.1.3/nice65/app.py
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 17:43:13.567893 nice65-0.1.3/nice65.egg-info/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3997 2023-08-05 17:43:13.000000 nice65-0.1.3/nice65.egg-info/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-05 17:43:13.000000 nice65-0.1.3/nice65.egg-info/SOURCES.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-05 17:43:13.000000 nice65-0.1.3/nice65.egg-info/dependency_links.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-05 17:43:13.000000 nice65-0.1.3/nice65.egg-info/entry_points.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-05 17:43:13.000000 nice65-0.1.3/nice65.egg-info/requires.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-05 17:43:13.000000 nice65-0.1.3/nice65.egg-info/top_level.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-05 17:43:05.000000 nice65-0.1.3/pyproject.toml
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-05 17:43:13.567893 nice65-0.1.3/setup.cfg
```

### Comparing `nice65-0.1.2/LICENSE` & `nice65-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nice65-0.1.2/PKG-INFO` & `nice65-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.1.2
+Version: 0.1.3
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `nice65-0.1.2/README.md` & `nice65-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nice65-0.1.2/nice65/app.py` & `nice65-0.1.3/nice65/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,24 +97,25 @@
         %import common.NUMBER
         %import common.HEXDIGIT
         %import common.LETTER
         %import common.WS_INLINE -> _WS
         %ignore _WS
 
         start: line*
-        line: (labeldef statement | statement | labeldef)? comment? "\n"
+        line: (labeldef statement | statement | labeldef | numeric_var | constant_def)? comment? "\n"
 
         labeldef: LABEL ":" """ + ('?' if args.colonless_labels else '') + r""" | ":"
 
-        statement: asm_statement | macro_start | macro_end | control_command | constant_def
+        statement: asm_statement | macro_start | macro_end | control_command
         asm_statement: INSTR (_WS+ operand ("," operand)?)?
         macro_start: ".macro" IDENT (IDENT ("," IDENT)*)?
         macro_end: ".endmacro"
         control_command: "." IDENT (_WS+ /[^\n]+/)?
-        constant_def: LABEL "=" /[^\n]+/
+        constant_def: LABEL /=|:=/ /[^\n]+/
+        numeric_var: IDENT control_command
 
         comment: ";" SENTENCE?
 
         ?operand: REGISTER | (/#/? /[<>]/? expr)
         ?expr: LITERAL (OP expr)?
             | /\(/ expr /\)/ -> expr
 
@@ -223,18 +224,24 @@
                     string += padding + (mnemonic.upper() if mnemonic.lower() in instructions else mnemonic)
                     operands = statement.children[1:]
                     if operands:
                         args = []
                         for operand in operands:
                             args.append(flatten_expr(operand))
                         string += " " + ", ".join(args)
-                elif statement.data == "constant_def":
-                    string += padding + " = ".join(map(str.strip, statement.children))
                 else:
                     raise NotImplementedError("Unknown statement type: " + child.children[0].data)
+            elif child.data == "numeric_var":
+                name, cmd = child.children
+                string = name.strip().ljust(8, ' ') + '.' + ' '.join(map(str.strip, cmd.children))
+            elif child.data == "constant_def":
+                name, assign, value = child.children
+                string += name.strip() + " " + assign.strip() + " " + value.strip()
+            else:
+                raise NotImplementedError("Unknown child in line: " + child.data)
         print(string.rstrip(), file=outfile)
 
     outfile.close()
 
 
 def flatten_expr(operand):
     parts = []
```

### Comparing `nice65-0.1.2/nice65.egg-info/PKG-INFO` & `nice65-0.1.3/nice65.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.1.2
+Version: 0.1.3
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `nice65-0.1.2/pyproject.toml` & `nice65-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nice65"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Andrew Dunai", email="a@dun.ai" },
 ]
 description = "Code formatter for CC65 assembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

