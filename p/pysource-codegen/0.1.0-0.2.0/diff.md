# Comparing `tmp/pysource_codegen-0.1.0.tar.gz` & `tmp/pysource_codegen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysource_codegen-0.1.0.tar", max compression
+gzip compressed data, was "pysource_codegen-0.2.0.tar", max compression
```

## Comparing `pysource_codegen-0.1.0.tar` & `pysource_codegen-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1190 2023-05-11 19:15:06.028387 pysource_codegen-0.1.0/README.md
--rw-r--r--   0        0        0      686 2023-05-10 15:22:04.070007 pysource_codegen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-10 15:18:01.250228 pysource_codegen-0.1.0/pysource_codegen/__init__.py
--rw-r--r--   0        0        0      264 2023-05-10 15:28:02.661203 pysource_codegen-0.1.0/pysource_codegen/__main__.py
--rw-r--r--   0        0        0    23491 2023-05-10 16:03:46.656254 pysource_codegen-0.1.0/pysource_codegen/_codegen.py
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 pysource_codegen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1556 2023-08-05 10:23:21.738583 pysource_codegen-0.2.0/README.md
+-rw-r--r--   0        0        0      757 2023-08-05 10:23:21.738583 pysource_codegen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-10 15:18:01.250228 pysource_codegen-0.2.0/pysource_codegen/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-10 15:28:02.661203 pysource_codegen-0.2.0/pysource_codegen/__main__.py
+-rw-r--r--   0        0        0    25872 2023-08-05 10:23:21.738583 pysource_codegen-0.2.0/pysource_codegen/_codegen.py
+-rw-r--r--   0        0        0    13751 2023-08-05 10:23:21.738583 pysource_codegen-0.2.0/pysource_codegen/static_type_info.py
+-rw-r--r--   0        0        0    13148 2023-08-05 10:23:21.738583 pysource_codegen-0.2.0/pysource_codegen/static_type_info37.py
+-rw-r--r--   0        0        0      555 2023-08-05 10:23:21.738583 pysource_codegen-0.2.0/pysource_codegen/types.py
+-rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 pysource_codegen-0.2.0/PKG-INFO
```

### Comparing `pysource_codegen-0.1.0/README.md` & `pysource_codegen-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![pypi version](https://img.shields.io/pypi/v/pysource-codegen.svg)](https://pypi.org/project/pysource-codegen/)
+![Python Versions](https://img.shields.io/pypi/pyversions/pysource-codegen)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/pysource-codegen)
+[![GitHub Sponsors](https://img.shields.io/github/sponsors/15r10nk)](https://github.com/sponsors/15r10nk)
+
 # Introduction
 
 
 `pysource_codegen` is able to generate random python code which can be compiled.
 The compiled code should no be executed.
 
 This is still a very early version, but it does its job.
@@ -39,9 +44,9 @@
 * https://github.com/psf/black/issues/3678
 * https://github.com/psf/black/issues/3677
 
 ## Todo:
 
 * [ ] refactor the existing code
 * [ ] use probabilities for the ast-nodes from existing python code (use markov chains)
-* [ ] support older python versions
+* [x] support older python versions
 * [ ] allow to customize the probabilities to generate code to test specific language features
```

### Comparing `pysource_codegen-0.1.0/pyproject.toml` & `pysource_codegen-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [tool.poetry]
 name = "pysource-codegen"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "pysource_codegen"}]
 
 [tool.poetry.scripts]
 pysource-codegen = "pysource_codegen.__main__:run"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.7"
+astunparse = "^1.6.3"
+typed-ast = "^1.5.5"
+typing-extensions = "^4.7.1"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3.4"
 pytest-xdist = {extras = ["psutil"], version = "^3.2.1"}
 pytest = "^7.2.1"
 mypy = "^1.2.0"
 coverage-enable-subprocess = "^1.0"
```

### Comparing `pysource_codegen-0.1.0/pysource_codegen/_codegen.py` & `pysource_codegen-0.2.0/pysource_codegen/_codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,94 @@
 import ast
 import inspect
+import itertools
 import re
 import sys
-from dataclasses import dataclass
 from typing import Dict
+from typing import Union
 
+from .types import BuiltinNodeType
+from .types import NodeType
+from .types import UnionNodeType
 
-@dataclass
-class NodeType:
-    fields: dict
-    ast_type: type
+if sys.version_info >= (3, 9):
+    from ast import unparse
+else:
+    from astunparse import unparse  # type: ignore
 
 
-@dataclass
-class BuiltinNodeType:
-    kind: str
+py38plus = (3, 8) <= sys.version_info
+py39plus = (3, 9) <= sys.version_info
+py310plus = (3, 10) <= sys.version_info
+py311plus = (3, 11) <= sys.version_info
 
+type_infos: Dict[str, Union[NodeType, BuiltinNodeType, UnionNodeType]] = {}
 
-@dataclass
-class UnionNodeType:
-    options: list
 
-
-type_infos: Dict[str, NodeType | BuiltinNodeType | UnionNodeType] = {}
+def all_args(args):
+    if py38plus:
+        return (args.posonlyargs, args.args, args.kwonlyargs)
+    else:
+        return (args.args, args.kwonlyargs)
 
 
 def get_info(name):
     if name in type_infos:
         return type_infos[name]
     elif name in ("identifier", "int", "string", "constant"):
         type_infos[name] = BuiltinNodeType(name)
 
     else:
         doc = inspect.getdoc(getattr(ast, name)) or ""
         doc = doc.replace("\n", " ")
 
         if doc:
-            if m := re.fullmatch(r"(\w*)", doc):
+            m = re.fullmatch(r"(\w*)", doc)
+            if m:
                 nt = NodeType(fields={}, ast_type=getattr(ast, name))
                 name = m.group(1)
                 type_infos[name] = nt
-            elif m := re.fullmatch(r"(\w*)\((.*)\)", doc):
-                nt = NodeType(fields={}, ast_type=getattr(ast, name))
-                name = m.group(1)
-                type_infos[name] = nt
-                for string_field in m.group(2).split(","):
-                    field_type, field_name = string_field.split()
-                    quantity = ""
-                    if (last := field_type[-1]) in "*?":
-                        quantity = last
-                        field_type = field_type[:-1]
-
-                    nt.fields[field_name] = (field_type, quantity)
-                    get_info(field_type)
-            elif doc.startswith(f"{name} = "):
-                doc = doc.split(" = ", 1)[1]
-                nt = UnionNodeType(options=[])
-                type_infos[name] = nt
-                nt.options = [d.split("(")[0] for d in doc.split(" | ")]
-                for o in nt.options:
-                    get_info(o)
-
             else:
-                assert False, "can not parse:" + doc
+                m = re.fullmatch(r"(\w*)\((.*)\)", doc)
+                if m:
+                    nt = NodeType(fields={}, ast_type=getattr(ast, name))
+                    name = m.group(1)
+                    type_infos[name] = nt
+                    for string_field in m.group(2).split(","):
+                        field_type, field_name = string_field.split()
+                        quantity = ""
+                        last = field_type[-1]
+                        if last in "*?":
+                            quantity = last
+                            field_type = field_type[:-1]
+
+                        nt.fields[field_name] = (field_type, quantity)
+                        get_info(field_type)
+                elif doc.startswith(f"{name} = "):
+                    doc = doc.split(" = ", 1)[1]
+                    nt = UnionNodeType(options=[])
+                    type_infos[name] = nt
+                    nt.options = [d.split("(")[0] for d in doc.split(" | ")]
+                    for o in nt.options:
+                        get_info(o)
+
+                else:
+                    assert False, "can not parse:" + doc
         else:
             assert False, "no doc"
 
     return type_infos[name]
 
 
+if sys.version_info < (3, 8):
+    from .static_type_info37 import type_infos  # type: ignore
+elif sys.version_info < (3, 9):
+    from .static_type_info import type_infos  # type: ignore
+
+
 get_info("Delete").fields = {"targets": ("_deleteTargets", "*")}
 type_infos["_deleteTargets"] = UnionNodeType(options=["Name", "Attribute", "Subscript"])
 
 
 import random
 
 
@@ -228,22 +244,43 @@
             ("FunctionDef.body", "AsyncFunctionDef.body", "Lambda.body"),
         )
         and child_name == "NamedExpr"
     ):
         # SyntaxError: assignment expression within a comprehension cannot be used in a class body
         return 0
 
+    if not py39plus and any(p[1] == "decorator_list" for p in parents):
+        # restricted decorators
+        # see https://peps.python.org/pep-0614/
+
+        deco_parents = list(
+            itertools.takewhile(lambda a: a[1] != "decorator_list", reversed(parents))
+        )[::-1]
+
+        def valid_deco_parents(parents):
+            # Call?,Attribute*
+            parents = list(parents)
+            if parents and parents[0] == ("Call", "func"):
+                parents.pop()
+            return all(p == ("Attribute", "value") for p in parents)
+
+        if valid_deco_parents(deco_parents) and child_name != "Name":
+            return 0
+
     if child_name == "Expr":
         return 30
 
     return 1
 
 
 def fix(node, parents):
     if isinstance(node, ast.ImportFrom):
+        if not py310plus and node.level is None:
+            node.level = 0
+
         if node.module == None and (node.level == None or node.level == 0):
             node.level = 1
 
     if isinstance(node, ast.ExceptHandler):
         if node.type is None:
             node.name = None
 
@@ -251,14 +288,16 @@
         # TODO: what is Constant.kind
         node.kind = None
         if parents[-1][0] == "JoinedStr":
             # TODO: better format string generation
             node.value = "text"
 
     if isinstance(node, ast.FormattedValue):
+        if not py310plus and node.conversion is None:
+            node.conversion = 5
         node.conversion = [-1, 115, 114, 97][node.conversion % 4]
 
     if hasattr(node, "ctx"):
         if parents[-1] == ("Delete", "targets"):
             node.ctx = ast.Del()
         elif [p for p in parents if p[0] not in ("Tuple", "List", "Starred")][-1] in (
             ("Assign", "targets"),
@@ -273,15 +312,15 @@
 
     if isinstance(node, (ast.List, ast.Tuple)) and isinstance(node.ctx, ast.Store):
         only_firstone(node.elts, lambda e: isinstance(e, ast.Starred))
 
     if isinstance(node, (ast.AsyncFunctionDef, ast.FunctionDef, ast.Lambda)):
         # unique argument names
         seen = set()
-        for args in (node.args.posonlyargs, node.args.args, node.args.kwonlyargs):
+        for args in all_args(node.args):
             for i, arg in reversed(list(enumerate(args))):
                 if arg.arg in seen:
                     del args[i]
                 seen.add(arg.arg)
 
         for arg_name in ("kwarg", "vararg"):
             arg = getattr(node.args, arg_name)
@@ -319,15 +358,17 @@
     if sys.version_info >= (3, 11) and isinstance(node, ast.TryStar):
         node.handlers = [
             handler for handler in node.handlers if handler.type is not None
         ]
         if not node.handlers:
             node.orelse = []
 
-    if isinstance(node, (ast.GeneratorExp, ast.ListComp, ast.DictComp, ast.SetComp)):
+    if sys.version_info >= (3, 8) and isinstance(
+        node, (ast.GeneratorExp, ast.ListComp, ast.DictComp, ast.SetComp)
+    ):
         # SyntaxError: assignment expression cannot rebind comprehension iteration variable 'name_3'
         names = {
             n.id
             for c in node.generators
             for n in ast.walk(c.target)
             if isinstance(n, ast.Name)
         } | {
@@ -344,15 +385,15 @@
                 return self.generic_visit(node)
 
         node = Transformer().visit(node)
 
     if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef, ast.Module)):
         while True:
             try:
-                code = ast.unparse(ast.fix_missing_locations(node))
+                code = unparse(ast.fix_missing_locations(node))
                 compile(code, "<string>", "exec")
                 break
             except ValueError:
                 break
             except SyntaxError as e:
                 m = re.match("name '(.*)' is used prior to global declaration", str(e))
 
@@ -409,186 +450,195 @@
 
                     node = Transformer().visit(node)
                     continue
 
                 break
 
     # pattern matching
+    if sys.version_info >= (3, 10):
 
-    def match_wildcard(node):
-        if isinstance(node, ast.MatchAs):
-            return (
-                node.pattern is None
-                or match_wildcard(node.pattern)
-                or node.name is None
-            )
-        if isinstance(node, ast.MatchOr):
-            return any(match_wildcard(p) for p in node.patterns)
-
-    if isinstance(node, ast.Match):
-        found = False
-        new_last = None
-        for i, case_ in reversed(list(enumerate(node.cases))):
-            p = case_.pattern
-            if match_wildcard(p):
-                if not found:
-                    new_last = node.cases[i]
-                    found = True
-                del node.cases[i]
-        if new_last:
-            node.cases.append(new_last)
-
-    # @lambda f:lambda pattern:set(f(pattern))
-    def names(node):
-        if isinstance(node, ast.MatchAs) and node.name:
-            yield node.name
-        elif isinstance(node, ast.MatchStar) and node.name:
-            yield node.name
-        elif isinstance(node, ast.MatchMapping) and node.rest:
-            yield node.rest
-        elif isinstance(node, ast.MatchOr):
-            yield from set.intersection(
-                *[set(names(pattern)) for pattern in node.patterns]
-            )
-        else:
-            for child in ast.iter_child_nodes(node):
-                yield from names(child)
+        def match_wildcard(node):
+            if isinstance(node, ast.MatchAs):
+                return (
+                    node.pattern is None
+                    or match_wildcard(node.pattern)
+                    or node.name is None
+                )
+            if isinstance(node, ast.MatchOr):
+                return any(match_wildcard(p) for p in node.patterns)
 
-    class RemoveName(ast.NodeVisitor):
-        def __init__(self, condition):
-            self.condition = condition
-
-        def visit_MatchAs(self, node):
-            if self.condition(node.name):
-                node.name = None
-
-        def visit_MatchMapping(self, node):
-            if self.condition(node.rest):
-                node.rest = None
-
-    class FixPatternNames(ast.NodeTransformer):
-        def __init__(self, used=None, allowed=None):
-            # variables which are already used
-            self.used = set() if used is None else used
-            # variables which are allowed in a MatchOr
-            self.allowed = allowed
-
-        def is_allowed(self, name):
-            return (
-                name is None
-                or name not in self.used
-                and (name in self.allowed if self.allowed is not None else True)
-            )
+        if isinstance(node, ast.Match):
+            found = False
+            new_last = None
+            for i, case_ in reversed(list(enumerate(node.cases))):
+                p = case_.pattern
+                if match_wildcard(p):
+                    if not found:
+                        new_last = node.cases[i]
+                        found = True
+                    del node.cases[i]
+            if new_last:
+                node.cases.append(new_last)
+
+        # @lambda f:lambda pattern:set(f(pattern))
+        def names(node):
+            if isinstance(node, ast.MatchAs) and node.name:
+                yield node.name
+            elif isinstance(node, ast.MatchStar) and node.name:
+                yield node.name
+            elif isinstance(node, ast.MatchMapping) and node.rest:
+                yield node.rest
+            elif isinstance(node, ast.MatchOr):
+                yield from set.intersection(
+                    *[set(names(pattern)) for pattern in node.patterns]
+                )
+            else:
+                for child in ast.iter_child_nodes(node):
+                    yield from names(child)
 
-        def visit_MatchAs(self, node):
-            if not self.is_allowed(node.name):
-                return ast.Constant(value=None)
-            elif node.name is not None:
-                self.used.add(node.name)
-            return self.generic_visit(node)
-
-        def visit_MatchStar(self, node):
-            if not self.is_allowed(node.name):
-                return ast.Constant(value=None)
-            elif node.name is not None:
-                self.used.add(node.name)
-            return self.generic_visit(node)
-
-        def visit_MatchMapping(self, node):
-            if not self.is_allowed(node.rest):
-                return ast.Constant(value=None)
-            elif node.rest is not None:
-                self.used.add(node.rest)
-            return self.generic_visit(node)
+        class RemoveName(ast.NodeVisitor):
+            def __init__(self, condition):
+                self.condition = condition
+
+            def visit_MatchAs(self, node):
+                if self.condition(node.name):
+                    node.name = None
+
+            def visit_MatchMapping(self, node):
+                if self.condition(node.rest):
+                    node.rest = None
+
+        class FixPatternNames(ast.NodeTransformer):
+            def __init__(self, used=None, allowed=None):
+                # variables which are already used
+                self.used = set() if used is None else used
+                # variables which are allowed in a MatchOr
+                self.allowed = allowed
+
+            def is_allowed(self, name):
+                return (
+                    name is None
+                    or name not in self.used
+                    and (name in self.allowed if self.allowed is not None else True)
+                )
 
-        def visit_MatchOr(self, node: ast.MatchOr):
-            allowed = set.intersection(
-                *[set(names(pattern)) for pattern in node.patterns]
-            )
-            allowed -= self.used
+            def visit_MatchAs(self, node):
+                if not self.is_allowed(node.name):
+                    return ast.Constant(value=None)
+                elif node.name is not None:
+                    self.used.add(node.name)
+                return self.generic_visit(node)
 
-            node.patterns = [
-                FixPatternNames(set(self.used), allowed).visit(child)
-                for child in node.patterns
-            ]
+            def visit_MatchStar(self, node):
+                if not self.is_allowed(node.name):
+                    return ast.Constant(value=None)
+                elif node.name is not None:
+                    self.used.add(node.name)
+                return self.generic_visit(node)
 
-            self.used |= allowed
+            def visit_MatchMapping(self, node):
+                if not self.is_allowed(node.rest):
+                    return ast.Constant(value=None)
+                elif node.rest is not None:
+                    self.used.add(node.rest)
+                return self.generic_visit(node)
 
-            return node
+            def visit_MatchOr(self, node: ast.MatchOr):
+                allowed = set.intersection(
+                    *[set(names(pattern)) for pattern in node.patterns]
+                )
+                allowed -= self.used
 
-    if isinstance(node, ast.match_case):
-        node.pattern = FixPatternNames().visit(node.pattern)
+                node.patterns = [
+                    FixPatternNames(set(self.used), allowed).visit(child)
+                    for child in node.patterns
+                ]
 
-    if isinstance(node, ast.MatchMapping):
-        node.keys = unique_by(node.keys, ast.literal_eval)
-        del node.patterns[len(node.keys) :]
+                self.used |= allowed
 
-        seen = set()
-        for pattern in node.patterns:
-            RemoveName(lambda name: name in seen).visit(pattern)
-            seen |= {*names(pattern)}
-
-    if isinstance(node, ast.MatchAs):
-        if node.name is None:
-            node.pattern = None
-
-    if isinstance(node, ast.MatchOr):
-        var_names = set.intersection(
-            *[set(names(pattern)) for pattern in node.patterns]
-        )
+                return node
 
-        RemoveName(lambda name: name not in var_names).visit(node)
+        if isinstance(node, ast.match_case):
+            node.pattern = FixPatternNames().visit(node.pattern)
 
-        for i, pattern in enumerate(node.patterns):
-            if match_wildcard(pattern):
-                node.patterns = node.patterns[: i + 1]
-                break
+        if isinstance(node, ast.MatchMapping):
+            node.keys = unique_by(node.keys, ast.literal_eval)
+            del node.patterns[len(node.keys) :]
 
-        if len(node.patterns) == 1:
-            return node.patterns[0]
+            seen = set()
+            for pattern in node.patterns:
+                RemoveName(lambda name: name in seen).visit(pattern)
+                seen |= {*names(pattern)}
 
-    if isinstance(node, ast.Match):
-        for i, case in enumerate(node.cases):
-            if (
-                isinstance(case.pattern, ast.MatchAs)
-                and case.pattern.name is None
-                or isinstance(case.pattern, ast.MatchOr)
-                and isinstance(case.pattern.patterns[-1], ast.MatchAs)
-                and case.pattern.patterns[-1].name is None
-            ):
-                node.cases = node.cases[: i + 1]
-                break
+        if isinstance(node, ast.MatchAs):
+            if node.name is None:
+                node.pattern = None
 
-    if isinstance(node, ast.MatchSequence):
-        only_firstone(node.patterns, lambda e: isinstance(e, ast.MatchStar))
+        if isinstance(node, ast.MatchOr):
+            var_names = set.intersection(
+                *[set(names(pattern)) for pattern in node.patterns]
+            )
 
-        seen = set()
-        for pattern in node.patterns:
-            RemoveName(lambda name: name in seen).visit(pattern)
-            seen |= {*names(pattern)}
-
-    if isinstance(node, ast.MatchClass):
-        node.kwd_attrs = list(set(node.kwd_attrs))
-        del node.kwd_patterns[len(node.kwd_attrs) :]
+            RemoveName(lambda name: name not in var_names).visit(node)
 
-        seen = set()
-        for pattern in [*node.patterns, *node.kwd_patterns]:
-            RemoveName(lambda name: name in seen).visit(pattern)
-            seen |= {*names(pattern)}
+            for i, pattern in enumerate(node.patterns):
+                if match_wildcard(pattern):
+                    node.patterns = node.patterns[: i + 1]
+                    break
+
+            if len(node.patterns) == 1:
+                return node.patterns[0]
+
+        if isinstance(node, ast.Match):
+            for i, case in enumerate(node.cases):
+                if (
+                    isinstance(case.pattern, ast.MatchAs)
+                    and case.pattern.name is None
+                    or isinstance(case.pattern, ast.MatchOr)
+                    and isinstance(case.pattern.patterns[-1], ast.MatchAs)
+                    and case.pattern.patterns[-1].name is None
+                ):
+                    node.cases = node.cases[: i + 1]
+                    break
+
+        if isinstance(node, ast.MatchSequence):
+            only_firstone(node.patterns, lambda e: isinstance(e, ast.MatchStar))
+
+            seen = set()
+            for pattern in node.patterns:
+                RemoveName(lambda name: name in seen).visit(pattern)
+                seen |= {*names(pattern)}
+
+        if isinstance(node, ast.MatchClass):
+            node.kwd_attrs = list(set(node.kwd_attrs))
+            del node.kwd_patterns[len(node.kwd_attrs) :]
+
+            seen = set()
+            for pattern in [*node.patterns, *node.kwd_patterns]:
+                RemoveName(lambda name: name in seen).visit(pattern)
+                seen |= {*names(pattern)}
 
     # async nodes
 
     in_async_code = False
     for parent, attr in reversed(parents):
         if parent == "AsyncFunctionDef" and attr == "body":
             in_async_code = True
             break
         if parent in ("FunctionDef", "Lambda", "ClassDef"):
             break
 
+        if not py311plus and parent in (
+            "ListComp",
+            "DictComp",
+            "SetComp",
+            "GeneratorExp",
+        ):
+            break
+
     if hasattr(node, "generators"):
         if not in_async_code:
             for comp in node.generators:
                 comp.is_async = 0
 
     in_excepthandler = False
     for parent, _ in reversed(parents):
@@ -603,15 +653,15 @@
             node.cause = None
 
         if not in_excepthandler and not node.exc:
             return ast.Pass()
 
     if isinstance(node, ast.Lambda):
         # no annotation for lambda arguments
-        for args in (node.args.posonlyargs, node.args.args, node.args.kwonlyargs):
+        for args in all_args(node.args):
             for arg in args:
                 arg.annotation = None
 
         if node.args.vararg:
             node.args.vararg.annotation = None
 
         if node.args.kwarg:
@@ -717,8 +767,14 @@
         assert False
 
 
 def generate(seed):
     generator = AstGenerator(seed)
     tree = generator.generate("Module")
     ast.fix_missing_locations(tree)
-    return ast.unparse(tree)
+    if 0:
+        from pathlib import Path
+
+        (Path(__file__).parent / "static_type_info.py").write_text(
+            "type_info=" + repr(type_infos)
+        )
+    return unparse(tree)
```

### Comparing `pysource_codegen-0.1.0/PKG-INFO` & `pysource_codegen-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: pysource-codegen
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astunparse (>=1.6.3,<2.0.0)
+Requires-Dist: typed-ast (>=1.5.5,<2.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Description-Content-Type: text/markdown
 
+[![pypi version](https://img.shields.io/pypi/v/pysource-codegen.svg)](https://pypi.org/project/pysource-codegen/)
+![Python Versions](https://img.shields.io/pypi/pyversions/pysource-codegen)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/pysource-codegen)
+[![GitHub Sponsors](https://img.shields.io/github/sponsors/15r10nk)](https://github.com/sponsors/15r10nk)
+
 # Introduction
 
 
 `pysource_codegen` is able to generate random python code which can be compiled.
 The compiled code should no be executed.
 
 This is still a very early version, but it does its job.
@@ -50,10 +62,10 @@
 * https://github.com/psf/black/issues/3678
 * https://github.com/psf/black/issues/3677
 
 ## Todo:
 
 * [ ] refactor the existing code
 * [ ] use probabilities for the ast-nodes from existing python code (use markov chains)
-* [ ] support older python versions
+* [x] support older python versions
 * [ ] allow to customize the probabilities to generate code to test specific language features
```

