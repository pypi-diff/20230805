# Comparing `tmp/nice65-0.1.0.tar.gz` & `tmp/nice65-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice65-0.1.0.tar", last modified: Fri Aug  4 21:24:30 2023, max compression
+gzip compressed data, was "nice65-0.1.1.tar", last modified: Sat Aug  5 10:43:38 2023, max compression
```

## Comparing `nice65-0.1.0.tar` & `nice65-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:24:30.327899 nice65-0.1.0/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.0/LICENSE
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:24:30.327899 nice65-0.1.0/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3210 2023-08-04 21:04:40.000000 nice65-0.1.0/README.md
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:24:30.324566 nice65-0.1.0/nice65/
--rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.0/nice65/__init__.py
--rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.0/nice65/__main__.py
--rwxr-xr-x   0 anderson  (1000) anderson  (1000)     8259 2023-08-04 21:23:43.000000 nice65-0.1.0/nice65/app.py
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:24:30.327899 nice65-0.1.0/nice65.egg-info/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:24:30.000000 nice65-0.1.0/nice65.egg-info/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-04 21:24:30.000000 nice65-0.1.0/nice65.egg-info/SOURCES.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-04 21:24:30.000000 nice65-0.1.0/nice65.egg-info/dependency_links.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-04 21:24:30.000000 nice65-0.1.0/nice65.egg-info/entry_points.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-04 21:24:30.000000 nice65-0.1.0/nice65.egg-info/requires.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-04 21:24:30.000000 nice65-0.1.0/nice65.egg-info/top_level.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-04 21:24:17.000000 nice65-0.1.0/pyproject.toml
--rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-04 21:24:30.327899 nice65-0.1.0/setup.cfg
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:43:38.137904 nice65-0.1.1/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.1/LICENSE
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     4027 2023-08-05 10:43:38.137904 nice65-0.1.1/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3607 2023-08-05 10:43:06.000000 nice65-0.1.1/README.md
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:43:38.137904 nice65-0.1.1/nice65/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.1/nice65/__init__.py
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.1/nice65/__main__.py
+-rwxr-xr-x   0 anderson  (1000) anderson  (1000)     8822 2023-08-05 10:40:00.000000 nice65-0.1.1/nice65/app.py
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 10:43:38.137904 nice65-0.1.1/nice65.egg-info/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     4027 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/SOURCES.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/dependency_links.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/entry_points.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/requires.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-05 10:43:38.000000 nice65-0.1.1/nice65.egg-info/top_level.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-05 10:43:29.000000 nice65-0.1.1/pyproject.toml
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-05 10:43:38.137904 nice65-0.1.1/setup.cfg
```

### Comparing `nice65-0.1.0/LICENSE` & `nice65-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nice65-0.1.0/PKG-INFO` & `nice65-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: nice65
-Version: 0.1.0
-Summary: Code formatter for CC65 assembly
-Author-email: Andrew Dunai <a@dun.ai>
-Project-URL: Homepage, https://github.com/and3rson/nice65
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nice65
 Code formatter for CC65 assembly (WIP).
 
 Requirements:
 
 - Python 3.x
 - [Lark](https://github.com/lark-parser/lark)
@@ -28,14 +15,17 @@
 - Tested with [C64 Kernal/Basic](https://github.com/mist64/c64rom) and [my 6502-based SBC ROM code](https://github.com/and3rson/deck65)
 
 Not implemented yet:
 - Complex macros
 - Proper formatting of arithmetic expressions
 - Better indentation of comments based on deduced context
 
+Notes:
+- Colon-less label mode (`-l`) breaks macros due to [ambiguity of the syntax](https://github.com/cc65/cc65/discussions/2158#discussioncomment-6644905). Use this option only with legacy code that contains no macros (such as C64 source code).
+
 # Installation
 
 ```sh
 pip install nice65
 ```
 
 ## Example usage
@@ -57,34 +47,39 @@
 
 # Recursively reformat all files in directory with extension ".asm"
 nice65 ./samples/ -r -p '*.asm'
 ```
 
 Before:
 ```asm
-.macro foobar aa, bb, cc
+.macro ldax aa, bb ; do stuff
 lda aa
-ldx bb
-ldy cc
+ldx bb ; load bb
+.endmacro
+
+.macro pushall
+    pha
+    phx
+    phy
 .endmacro
 
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
 PHa
 Phx
 
-start lDa  #0
-LdX #0
+start: pushall
+ldax #0, #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
-bne fill  ; Repeat
+bne @again  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
 cmp foo+2
 jmp :+
 : lda $1234
 
@@ -92,35 +87,40 @@
 pla
 
 end:rts
 ```
 
 After:
 ```asm
-.macro  foobar aa, bb, cc
+.macro  ldax aa, bb     ; do stuff
         LDA aa
-        LDX bb
-        LDY cc
+        LDX bb          ; load bb
+.endmacro
+
+.macro  pushall
+        PHA
+        PHX
+        PHY
 .endmacro
 
 .data
 foo:    .byte 1
 
 .code
 ; Fill zeropage with zeroes
 fill:
         PHA
         PHX
 
-start:  LDA #0
-        LDX #0
+start:  pushall
+        ldax #0, #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
-        BNE fill        ; Repeat
+        BNE @again      ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
         CMP foo+2
         JMP :+
     :   LDA $1234
```

### Comparing `nice65-0.1.0/README.md` & `nice65-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: nice65
+Version: 0.1.1
+Summary: Code formatter for CC65 assembly
+Author-email: Andrew Dunai <a@dun.ai>
+Project-URL: Homepage, https://github.com/and3rson/nice65
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nice65
 Code formatter for CC65 assembly (WIP).
 
 Requirements:
 
 - Python 3.x
 - [Lark](https://github.com/lark-parser/lark)
@@ -15,14 +28,17 @@
 - Tested with [C64 Kernal/Basic](https://github.com/mist64/c64rom) and [my 6502-based SBC ROM code](https://github.com/and3rson/deck65)
 
 Not implemented yet:
 - Complex macros
 - Proper formatting of arithmetic expressions
 - Better indentation of comments based on deduced context
 
+Notes:
+- Colon-less label mode (`-l`) breaks macros due to [ambiguity of the syntax](https://github.com/cc65/cc65/discussions/2158#discussioncomment-6644905). Use this option only with legacy code that contains no macros (such as C64 source code).
+
 # Installation
 
 ```sh
 pip install nice65
 ```
 
 ## Example usage
@@ -44,34 +60,39 @@
 
 # Recursively reformat all files in directory with extension ".asm"
 nice65 ./samples/ -r -p '*.asm'
 ```
 
 Before:
 ```asm
-.macro foobar aa, bb, cc
+.macro ldax aa, bb ; do stuff
 lda aa
-ldx bb
-ldy cc
+ldx bb ; load bb
+.endmacro
+
+.macro pushall
+    pha
+    phx
+    phy
 .endmacro
 
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
 PHa
 Phx
 
-start lDa  #0
-LdX #0
+start: pushall
+ldax #0, #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
-bne fill  ; Repeat
+bne @again  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
 cmp foo+2
 jmp :+
 : lda $1234
 
@@ -79,35 +100,40 @@
 pla
 
 end:rts
 ```
 
 After:
 ```asm
-.macro  foobar aa, bb, cc
+.macro  ldax aa, bb     ; do stuff
         LDA aa
-        LDX bb
-        LDY cc
+        LDX bb          ; load bb
+.endmacro
+
+.macro  pushall
+        PHA
+        PHX
+        PHY
 .endmacro
 
 .data
 foo:    .byte 1
 
 .code
 ; Fill zeropage with zeroes
 fill:
         PHA
         PHX
 
-start:  LDA #0
-        LDX #0
+start:  pushall
+        ldax #0, #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
-        BNE fill        ; Repeat
+        BNE @again      ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
         CMP foo+2
         JMP :+
     :   LDA $1234
```

### Comparing `nice65-0.1.0/nice65/app.py` & `nice65-0.1.1/nice65/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,56 +43,14 @@
 COL1_COMMANDS = {'segment', 'zeropage', 'data', 'code', 'bss'}
 
 instructions = INSTRUCTIONS + CMOS_INSTRUCTIONS
 
 instructions_def = " | ".join(['"' + instr + '"i' for instr in instructions])
 
 
-definition = (
-    # fmt: off
-    r"""
-    %import common.NUMBER
-    %import common.HEXDIGIT
-    %import common.LETTER
-    %import common.WORD
-    %import common.WS_INLINE -> _WS
-    %ignore _WS
-
-    start: line*
-    line: (labeldef statement | statement | labeldef)? comment? "\n"
-
-    labeldef: LABEL ":"? | ":"
-
-    statement: asm_statement | macro_start | macro_end | control_command | constant_def
-    asm_statement: INSTR (_WS+ operand ("," operand)?)?
-    macro_start: ".macro" WORD (_WS+ WORD ("," WORD)*)?
-    macro_end: ".endmacro"
-    control_command: "." WORD (_WS+ /[^\n]+/)?
-    constant_def: LABEL "=" /[^\n]+/
-
-    comment: ";" SENTENCE?
-
-    ?operand: REGISTER | (/#/? /[<>]/? expr)
-    ?expr: LITERAL (OP expr)?
-        | /\(/ expr /\)/ -> expr
-
-    SENTENCE: /[^\n]+/
-    INSTR: """ + instructions_def + r"""
-    REGISTER: "A"i | "X"i | "Y"i
-    LITERAL: NUMBER | /\$/ HEXDIGIT+ | /%/ /[01]+/ | LABEL | LABEL_REL | /'.'/ | /\*/
-    LABEL: "@"? (LETTER | "_")+ (LETTER | "_" | NUMBER)*
-    LABEL_REL: /:[\+\-]+/
-    OP: "+" | "-" | "*" | "/" | "|" | "^" | "&"
-"""
-    # fmt: on
-)
-
-grammar = Lark(definition)
-
-
 def main():
     parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
     parser.add_argument("infile", help='Input file, pass "-" to read from for stdin')
     group = parser.add_mutually_exclusive_group()
     group.add_argument(
         "-o",
         "--outfile",
@@ -115,40 +73,87 @@
     parser.add_argument(
         "-p",
         "--pattern",
         help="Match file names by Unix shell-style wildcard when used with -r",
         default='*.s',
     )
     parser.add_argument(
+        "-l",
+        "--colonless-labels",
+        help="Allow labels without a colon (this option breaks macros, use with legacy code only)",
+        action="store_true",
+    )
+    parser.add_argument(
         "-v",
         "--version",
         help="Show version",
         nargs=0,
         action=Version,
     )
     args = parser.parse_args()
 
+    definition = (
+        # fmt: off
+        r"""
+        %import common.NUMBER
+        %import common.HEXDIGIT
+        %import common.LETTER
+        %import common.WORD
+        %import common.WS_INLINE -> _WS
+        %ignore _WS
+
+        start: line*
+        line: (labeldef statement | statement | labeldef)? comment? "\n"
+
+        labeldef: LABEL ":" """ + ('?' if args.colonless_labels else '') + r""" | ":"
+
+        statement: asm_statement | macro_start | macro_end | control_command | constant_def
+        asm_statement: INSTR (_WS+ operand ("," operand)?)?
+        macro_start: ".macro" WORD (WORD ("," WORD)*)?
+        macro_end: ".endmacro"
+        control_command: "." WORD (_WS+ /[^\n]+/)?
+        constant_def: LABEL "=" /[^\n]+/
+
+        comment: ";" SENTENCE?
+
+        ?operand: REGISTER | (/#/? /[<>]/? expr)
+        ?expr: LITERAL (OP expr)?
+            | /\(/ expr /\)/ -> expr
+
+        SENTENCE: /[^\n]+/
+        INSTR: """ + (instructions_def if args.colonless_labels else 'WORD') + r"""
+        REGISTER: "A"i | "X"i | "Y"i
+        LITERAL: NUMBER | /\$/ HEXDIGIT+ | /%/ /[01]+/ | LABEL | LABEL_REL | /'.'/ | /\*/
+        LABEL: "@"? (LETTER | "_")+ (LETTER | "_" | NUMBER)*
+        LABEL_REL: /:[\+\-]+/
+        OP: "+" | "-" | "*" | "/" | "|" | "^" | "&"
+    """
+        # fmt: on
+    )
+
+    grammar = Lark(definition)
+
     if args.recursive:
         for root, _, files in os.walk(args.infile):
             for file in files:
                 if fnmatch.fnmatch(file, args.pattern):
                     path = os.path.join(root, file)
                     print("Fixing", path, file=sys.stderr)
-                    fix(path, None, True)
+                    fix(grammar, path, None, True, args.colonless_labels)
     else:
-        fix(args.infile, args.outfile, args.modify_in_place)
+        fix(grammar, args.infile, args.outfile, args.modify_in_place, args.colonless_labels)
 
 
 class Version(Action):
     def __call__(self, parser, namespace, values, option_string):
         print('nice65 version', metadata.version("nice65"), file=sys.stderr)
         parser.exit()
 
 
-def fix(infile, outfile, modify_in_place):
+def fix(grammar, infile, outfile, modify_in_place, colonless_labels):
     if infile == "-":
         content = sys.stdin.read()
     else:
         with open(infile, "r") as fobj:
             content = fobj.read()
             options_match = re.findall(r'^[ \t]*;\s*nice65:([^\n]+)$', content, re.MULTILINE)
             if options_match:
@@ -211,15 +216,15 @@
                 elif statement.data == "macro_start":
                     name = statement.children[0].strip()
                     string += ".macro ".ljust(8, ' ') + name + " " + ", ".join(map(str.strip, statement.children[1:]))
                 elif statement.data == "macro_end":
                     string += ".endmacro"
                 elif statement.data == "asm_statement":
                     mnemonic = statement.children[0]
-                    string += padding + mnemonic.upper()
+                    string += padding + (mnemonic.upper() if mnemonic.lower() in instructions else mnemonic)
                     operands = statement.children[1:]
                     if operands:
                         args = []
                         for operand in operands:
                             args.append(flatten_expr(operand))
                         string += " " + ", ".join(args)
                 elif statement.data == "constant_def":
```

### Comparing `nice65-0.1.0/nice65.egg-info/PKG-INFO` & `nice65-0.1.1/nice65.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.1.0
+Version: 0.1.1
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -28,14 +28,17 @@
 - Tested with [C64 Kernal/Basic](https://github.com/mist64/c64rom) and [my 6502-based SBC ROM code](https://github.com/and3rson/deck65)
 
 Not implemented yet:
 - Complex macros
 - Proper formatting of arithmetic expressions
 - Better indentation of comments based on deduced context
 
+Notes:
+- Colon-less label mode (`-l`) breaks macros due to [ambiguity of the syntax](https://github.com/cc65/cc65/discussions/2158#discussioncomment-6644905). Use this option only with legacy code that contains no macros (such as C64 source code).
+
 # Installation
 
 ```sh
 pip install nice65
 ```
 
 ## Example usage
@@ -57,34 +60,39 @@
 
 # Recursively reformat all files in directory with extension ".asm"
 nice65 ./samples/ -r -p '*.asm'
 ```
 
 Before:
 ```asm
-.macro foobar aa, bb, cc
+.macro ldax aa, bb ; do stuff
 lda aa
-ldx bb
-ldy cc
+ldx bb ; load bb
+.endmacro
+
+.macro pushall
+    pha
+    phx
+    phy
 .endmacro
 
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
 PHa
 Phx
 
-start lDa  #0
-LdX #0
+start: pushall
+ldax #0, #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
-bne fill  ; Repeat
+bne @again  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
 cmp foo+2
 jmp :+
 : lda $1234
 
@@ -92,35 +100,40 @@
 pla
 
 end:rts
 ```
 
 After:
 ```asm
-.macro  foobar aa, bb, cc
+.macro  ldax aa, bb     ; do stuff
         LDA aa
-        LDX bb
-        LDY cc
+        LDX bb          ; load bb
+.endmacro
+
+.macro  pushall
+        PHA
+        PHX
+        PHY
 .endmacro
 
 .data
 foo:    .byte 1
 
 .code
 ; Fill zeropage with zeroes
 fill:
         PHA
         PHX
 
-start:  LDA #0
-        LDX #0
+start:  pushall
+        ldax #0, #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
-        BNE fill        ; Repeat
+        BNE @again      ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
         CMP foo+2
         JMP :+
     :   LDA $1234
```

### Comparing `nice65-0.1.0/pyproject.toml` & `nice65-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nice65"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Andrew Dunai", email="a@dun.ai" },
 ]
 description = "Code formatter for CC65 assembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

