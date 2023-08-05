# Comparing `tmp/nice65-0.1.1.tar.gz` & `tmp/nice65-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice65-0.1.1.tar", last modified: Sat Aug  5 10:43:38 2023, max compression
+gzip compressed data, was "nice65-0.1.2.tar", last modified: Sat Aug  5 10:49:42 2023, max compression
```

## Comparing `nice65-0.1.1.tar` & `nice65-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:43:38.137904 nice65-0.1.1/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.1/LICENSE
--rw-r--r--   0 anderson  (1000) anderson  (1000)     4027 2023-08-05 10:43:38.137904 nice65-0.1.1/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3607 2023-08-05 10:43:06.000000 nice65-0.1.1/README.md
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:43:38.137904 nice65-0.1.1/nice65/
--rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.1/nice65/__init__.py
--rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.1/nice65/__main__.py
--rwxr-xr-x   0 anderson  (1000) anderson  (1000)     8822 2023-08-05 10:40:00.000000 nice65-0.1.1/nice65/app.py
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:43:38.137904 nice65-0.1.1/nice65.egg-info/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     4027 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/SOURCES.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/dependency_links.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/entry_points.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/requires.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/top_level.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-05 10:43:29.000000 nice65-0.1.1/pyproject.toml
--rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-05 10:43:38.137904 nice65-0.1.1/setup.cfg
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:49:42.157905 nice65-0.1.2/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.2/LICENSE
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3997 2023-08-05 10:49:42.157905 nice65-0.1.2/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3577 2023-08-05 10:49:20.000000 nice65-0.1.2/README.md
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:49:42.154572 nice65-0.1.2/nice65/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.2/nice65/__init__.py
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.2/nice65/__main__.py
+-rwxr-xr-x   0 anderson  (1000) anderson  (1000)     8804 2023-08-05 10:48:46.000000 nice65-0.1.2/nice65/app.py
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:49:42.157905 nice65-0.1.2/nice65.egg-info/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3997 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/SOURCES.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/dependency_links.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/entry_points.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/requires.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-05 10:49:42.000000 nice65-0.1.2/nice65.egg-info/top_level.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-05 10:49:35.000000 nice65-0.1.2/pyproject.toml
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-05 10:49:42.157905 nice65-0.1.2/setup.cfg
```

### Comparing `nice65-0.1.1/LICENSE` & `nice65-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nice65-0.1.1/PKG-INFO` & `nice65-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.1.1
+Version: 0.1.2
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -65,31 +65,28 @@
 Before:
 ```asm
 .macro ldax aa, bb ; do stuff
 lda aa
 ldx bb ; load bb
 .endmacro
 
-.macro pushall
-    pha
-    phx
-    phy
+.macro push_all
+    phA
+    phX
+    PHy
 .endmacro
 
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
-PHa
-Phx
-
-start: pushall
-ldax #0, #0
+push_all
+start: ldax #0, #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
 bne @again  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
 cmp foo+2
@@ -105,31 +102,28 @@
 After:
 ```asm
 .macro  ldax aa, bb     ; do stuff
         LDA aa
         LDX bb          ; load bb
 .endmacro
 
-.macro  pushall
+.macro  push_all
         PHA
         PHX
         PHY
 .endmacro
 
 .data
 foo:    .byte 1
 
 .code
 ; Fill zeropage with zeroes
 fill:
-        PHA
-        PHX
-
-start:  pushall
-        ldax #0, #0
+        push_all
+start:  ldax #0, #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
         BNE @again      ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
```

### Comparing `nice65-0.1.1/README.md` & `nice65-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,31 +52,28 @@
 Before:
 ```asm
 .macro ldax aa, bb ; do stuff
 lda aa
 ldx bb ; load bb
 .endmacro
 
-.macro pushall
-    pha
-    phx
-    phy
+.macro push_all
+    phA
+    phX
+    PHy
 .endmacro
 
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
-PHa
-Phx
-
-start: pushall
-ldax #0, #0
+push_all
+start: ldax #0, #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
 bne @again  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
 cmp foo+2
@@ -92,31 +89,28 @@
 After:
 ```asm
 .macro  ldax aa, bb     ; do stuff
         LDA aa
         LDX bb          ; load bb
 .endmacro
 
-.macro  pushall
+.macro  push_all
         PHA
         PHX
         PHY
 .endmacro
 
 .data
 foo:    .byte 1
 
 .code
 ; Fill zeropage with zeroes
 fill:
-        PHA
-        PHX
-
-start:  pushall
-        ldax #0, #0
+        push_all
+start:  ldax #0, #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
         BNE @again      ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
```

### Comparing `nice65-0.1.1/nice65/app.py` & `nice65-0.1.2/nice65/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,41 +93,41 @@
 
     definition = (
         # fmt: off
         r"""
         %import common.NUMBER
         %import common.HEXDIGIT
         %import common.LETTER
-        %import common.WORD
         %import common.WS_INLINE -> _WS
         %ignore _WS
 
         start: line*
         line: (labeldef statement | statement | labeldef)? comment? "\n"
 
         labeldef: LABEL ":" """ + ('?' if args.colonless_labels else '') + r""" | ":"
 
         statement: asm_statement | macro_start | macro_end | control_command | constant_def
         asm_statement: INSTR (_WS+ operand ("," operand)?)?
-        macro_start: ".macro" WORD (WORD ("," WORD)*)?
+        macro_start: ".macro" IDENT (IDENT ("," IDENT)*)?
         macro_end: ".endmacro"
-        control_command: "." WORD (_WS+ /[^\n]+/)?
+        control_command: "." IDENT (_WS+ /[^\n]+/)?
         constant_def: LABEL "=" /[^\n]+/
 
         comment: ";" SENTENCE?
 
         ?operand: REGISTER | (/#/? /[<>]/? expr)
         ?expr: LITERAL (OP expr)?
             | /\(/ expr /\)/ -> expr
 
         SENTENCE: /[^\n]+/
-        INSTR: """ + (instructions_def if args.colonless_labels else 'WORD') + r"""
+        INSTR: """ + (instructions_def if args.colonless_labels else 'IDENT') + r"""
         REGISTER: "A"i | "X"i | "Y"i
         LITERAL: NUMBER | /\$/ HEXDIGIT+ | /%/ /[01]+/ | LABEL | LABEL_REL | /'.'/ | /\*/
-        LABEL: "@"? (LETTER | "_")+ (LETTER | "_" | NUMBER)*
+        LABEL: "@"? IDENT
+        IDENT: /[a-zA-Z_][a-zA-Z0-9_]*/
         LABEL_REL: /:[\+\-]+/
         OP: "+" | "-" | "*" | "/" | "|" | "^" | "&"
     """
         # fmt: on
     )
 
     grammar = Lark(definition)
```

### Comparing `nice65-0.1.1/nice65.egg-info/PKG-INFO` & `nice65-0.1.2/nice65.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.1.1
+Version: 0.1.2
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -65,31 +65,28 @@
 Before:
 ```asm
 .macro ldax aa, bb ; do stuff
 lda aa
 ldx bb ; load bb
 .endmacro
 
-.macro pushall
-    pha
-    phx
-    phy
+.macro push_all
+    phA
+    phX
+    PHy
 .endmacro
 
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
-PHa
-Phx
-
-start: pushall
-ldax #0, #0
+push_all
+start: ldax #0, #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
 bne @again  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
 cmp foo+2
@@ -105,31 +102,28 @@
 After:
 ```asm
 .macro  ldax aa, bb     ; do stuff
         LDA aa
         LDX bb          ; load bb
 .endmacro
 
-.macro  pushall
+.macro  push_all
         PHA
         PHX
         PHY
 .endmacro
 
 .data
 foo:    .byte 1
 
 .code
 ; Fill zeropage with zeroes
 fill:
-        PHA
-        PHX
-
-start:  pushall
-        ldax #0, #0
+        push_all
+start:  ldax #0, #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
         BNE @again      ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
```

### Comparing `nice65-0.1.1/pyproject.toml` & `nice65-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nice65"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Andrew Dunai", email="a@dun.ai" },
 ]
 description = "Code formatter for CC65 assembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

