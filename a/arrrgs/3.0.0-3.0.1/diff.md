# Comparing `tmp/arrrgs-3.0.0.tar.gz` & `tmp/arrrgs-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrrgs-3.0.0.tar", last modified: Wed Aug  2 12:01:16 2023, max compression
+gzip compressed data, was "arrrgs-3.0.1.tar", last modified: Sat Aug  5 21:21:05 2023, max compression
```

## Comparing `arrrgs-3.0.0.tar` & `arrrgs-3.0.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.026501 arrrgs-3.0.0/
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.021976 arrrgs-3.0.0/.github/
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.023548 arrrgs-3.0.0/.github/workflows/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      302 2023-02-11 21:11:19.000000 arrrgs-3.0.0/.github/workflows/qa.yaml
--rw-r--r--   0 mishamyrt   (501) staff       (20)       66 2023-03-29 13:47:46.000000 arrrgs-3.0.0/.gitignore
--rw-r--r--   0 mishamyrt   (501) staff       (20)        6 2023-08-02 12:01:10.000000 arrrgs-3.0.0/.version
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1073 2023-03-29 13:12:20.000000 arrrgs-3.0.0/LICENSE
--rw-r--r--   0 mishamyrt   (501) staff       (20)      886 2023-08-02 12:00:21.000000 arrrgs-3.0.0/Makefile
--rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-08-02 12:01:16.026339 arrrgs-3.0.0/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)     3545 2023-03-29 13:53:36.000000 arrrgs-3.0.0/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.023682 arrrgs-3.0.0/assets/
--rw-r--r--   0 mishamyrt   (501) staff       (20)    15275 2023-02-11 21:11:19.000000 arrrgs-3.0.0/assets/logo@2x.png
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.024566 arrrgs-3.0.0/examples/
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)      446 2023-08-02 11:59:10.000000 arrrgs-3.0.0/examples/args.py
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)      252 2023-08-02 11:59:02.000000 arrrgs-3.0.0/examples/basic.py
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)      554 2023-08-02 11:58:59.000000 arrrgs-3.0.0/examples/context.py
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)      218 2023-08-02 11:58:56.000000 arrrgs-3.0.0/examples/custom_name.py
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)      505 2023-08-02 11:58:53.000000 arrrgs-3.0.0/examples/environment.py
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)      487 2023-08-02 11:57:33.000000 arrrgs-3.0.0/examples/root_command.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      963 2023-03-29 15:14:56.000000 arrrgs-3.0.0/pyproject.toml
--rw-r--r--   0 mishamyrt   (501) staff       (20)       56 2023-03-29 15:09:24.000000 arrrgs-3.0.0/requirements.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-08-02 12:01:16.026551 arrrgs-3.0.0/setup.cfg
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.022378 arrrgs-3.0.0/src/
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.025391 arrrgs-3.0.0/src/arrrgs/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      122 2023-08-02 11:17:14.000000 arrrgs-3.0.0/src/arrrgs/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      659 2023-03-29 14:50:37.000000 arrrgs-3.0.0/src/arrrgs/arguments.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      975 2023-08-02 11:57:26.000000 arrrgs-3.0.0/src/arrrgs/command.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      405 2023-03-29 13:41:43.000000 arrrgs-3.0.0/src/arrrgs/log.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      229 2023-08-02 11:49:49.000000 arrrgs-3.0.0/src/arrrgs/parser.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2238 2023-03-29 14:59:41.000000 arrrgs-3.0.0/src/arrrgs/run.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.026121 arrrgs-3.0.0/src/arrrgs.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      546 2023-08-02 12:01:16.000000 arrrgs-3.0.0/src/arrrgs.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        9 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        7 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/top_level.txt
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.790815 arrrgs-3.0.1/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.783200 arrrgs-3.0.1/.github/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.785532 arrrgs-3.0.1/.github/workflows/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      302 2023-02-11 21:11:19.000000 arrrgs-3.0.1/.github/workflows/qa.yaml
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       66 2023-03-29 13:47:46.000000 arrrgs-3.0.1/.gitignore
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        6 2023-08-05 21:21:00.000000 arrrgs-3.0.1/.version
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1073 2023-03-29 13:12:20.000000 arrrgs-3.0.1/LICENSE
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      886 2023-08-05 21:20:38.000000 arrrgs-3.0.1/Makefile
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-08-05 21:21:05.790637 arrrgs-3.0.1/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     3545 2023-03-29 13:53:36.000000 arrrgs-3.0.1/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.785801 arrrgs-3.0.1/assets/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)    15275 2023-02-11 21:11:19.000000 arrrgs-3.0.1/assets/logo@2x.png
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.788137 arrrgs-3.0.1/examples/
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      228 2023-08-05 16:40:04.000000 arrrgs-3.0.1/examples/aliases.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      446 2023-08-02 11:59:10.000000 arrrgs-3.0.1/examples/args.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      252 2023-08-02 11:59:02.000000 arrrgs-3.0.1/examples/basic.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      554 2023-08-02 11:58:59.000000 arrrgs-3.0.1/examples/context.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      218 2023-08-02 11:58:56.000000 arrrgs-3.0.1/examples/custom_name.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      505 2023-08-02 11:58:53.000000 arrrgs-3.0.1/examples/environment.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      604 2023-08-05 21:20:15.000000 arrrgs-3.0.1/examples/root_command.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      963 2023-03-29 15:14:56.000000 arrrgs-3.0.1/pyproject.toml
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       56 2023-03-29 15:09:24.000000 arrrgs-3.0.1/requirements.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-08-05 21:21:05.790872 arrrgs-3.0.1/setup.cfg
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.783852 arrrgs-3.0.1/src/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.789651 arrrgs-3.0.1/src/arrrgs/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      122 2023-08-02 11:17:14.000000 arrrgs-3.0.1/src/arrrgs/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      659 2023-03-29 14:50:37.000000 arrrgs-3.0.1/src/arrrgs/arguments.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1185 2023-08-05 16:39:02.000000 arrrgs-3.0.1/src/arrrgs/command.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      405 2023-03-29 13:41:43.000000 arrrgs-3.0.1/src/arrrgs/log.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      229 2023-08-02 11:49:49.000000 arrrgs-3.0.1/src/arrrgs/parser.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2206 2023-08-05 21:16:46.000000 arrrgs-3.0.1/src/arrrgs/run.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 21:21:05.790411 arrrgs-3.0.1/src/arrrgs.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-08-05 21:21:05.000000 arrrgs-3.0.1/src/arrrgs.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      566 2023-08-05 21:21:05.000000 arrrgs-3.0.1/src/arrrgs.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-08-05 21:21:05.000000 arrrgs-3.0.1/src/arrrgs.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        9 2023-08-05 21:21:05.000000 arrrgs-3.0.1/src/arrrgs.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        7 2023-08-05 21:21:05.000000 arrrgs-3.0.1/src/arrrgs.egg-info/top_level.txt
```

### Comparing `arrrgs-3.0.0/LICENSE` & `arrrgs-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrrgs-3.0.0/Makefile` & `arrrgs-3.0.1/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = 3.0.0
+VERSION = 3.0.1
 VENV_PATH = ./venv
 VENV = . $(VENV_PATH)/bin/activate;
 SRC := \
 	$(wildcard src/arrrgs/*.py)
 
 .PHONY: publish
 publish:
```

### Comparing `arrrgs-3.0.0/PKG-INFO` & `arrrgs-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrrgs
-Version: 3.0.0
+Version: 3.0.1
 Summary: The library for easily writing feature-rich Python scripts
 Author-email: Mikhael Khrustik <misha@myrt.co>
 License: MIT
 Keywords: cli,command-line-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `arrrgs-3.0.0/README.md` & `arrrgs-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arrrgs-3.0.0/assets/logo@2x.png` & `arrrgs-3.0.1/assets/logo@2x.png`

 * *Files identical despite different names*

### Comparing `arrrgs-3.0.0/examples/context.py` & `arrrgs-3.0.1/examples/context.py`

 * *Files identical despite different names*

### Comparing `arrrgs-3.0.0/pyproject.toml` & `arrrgs-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arrrgs-3.0.0/src/arrrgs/arguments.py` & `arrrgs-3.0.1/src/arrrgs/arguments.py`

 * *Files identical despite different names*

### Comparing `arrrgs-3.0.0/src/arrrgs/command.py` & `arrrgs-3.0.1/src/arrrgs/command.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Arrrgs command"""
 from argparse import ArgumentParser
-from typing import Callable, Tuple
+from typing import Callable, List, Tuple
 
 from .arguments import add_args
 from .parser import command_subparsers, parser
 
 
 def register_handler(
     parent: ArgumentParser,
@@ -17,17 +17,27 @@
         command_name = name
     else:
         command_name = func.__name__
     cmd_parser = parent.add_parser(command_name, description=func.__doc__)
     add_args(cmd_parser, args)
     cmd_parser.set_defaults(func=func)
 
-def command(*args, name:str=None, root=False, parent=command_subparsers, root_parser=parser):
+def command(
+        *args,
+        name:str=None,
+        root=False,
+        parent=command_subparsers,
+        root_parser=parser,
+        aliases:List[str]=None
+    ):
     """Decorator to define a new command"""
     def decorator(func):
         if root:
             root_parser.set_defaults(
                 root_command_handler=func,
                 root_command_args=list(args),
             )
         register_handler(parent, func, args, name)
+        if aliases is not None:
+            for alias in aliases:
+                register_handler(parent, func, args, alias)
     return decorator
```

### Comparing `arrrgs-3.0.0/src/arrrgs/run.py` & `arrrgs-3.0.1/src/arrrgs/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,33 +19,33 @@
 
 async def async_run(ctx: Any = None, prepare: Union[ContextPreparer, None] = None, debug=False):
     """Runs application asynchronously"""
     args, argv = parser.parse_known_args()
     if debug:
         log.setLevel(DEBUG)
         log.info("Running in debug mode")
+    if argv:
+        parser.error(f"unrecognized arguments: {' '.join(argv)}")
     handler: Callable
+    if prepare is not None:
+        log.info("Running 'prepare' callback")
+        (prepared_args, prepared_context) = await _run_safe(prepare, args, ctx)
+        # Updating values
+        args = prepared_args
+        ctx = prepared_context
     if args.cmd is None:
         if args.root_command_handler is None:
             log.info("root command handler is not found. Printing help")
             parser.print_help()
             return
         add_args(parser, args.root_command_args)
         args = parser.parse_args()
         handler = args.root_command_handler
     else:
-        if argv:
-            parser.error(f"unrecognized arguments: {' '.join(argv)}")
         handler = args.func
-        if prepare is not None:
-            log.info("Running 'prepare' callback")
-            (prepared_args, prepared_context) = await _run_safe(prepare, args, ctx)
-            # Updating values
-            args = prepared_args
-            ctx = prepared_context
     log.info(args)
     await _run_safe(handler, args, ctx)
 
 def _prepare_args(handler: Callable, parsed_args: Namespace, ctx: Any) -> List[str]:
     sig = signature(handler)
     params_count = len(sig.parameters)
     args = []
```

### Comparing `arrrgs-3.0.0/src/arrrgs.egg-info/PKG-INFO` & `arrrgs-3.0.1/src/arrrgs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrrgs
-Version: 3.0.0
+Version: 3.0.1
 Summary: The library for easily writing feature-rich Python scripts
 Author-email: Mikhael Khrustik <misha@myrt.co>
 License: MIT
 Keywords: cli,command-line-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `arrrgs-3.0.0/src/arrrgs.egg-info/SOURCES.txt` & `arrrgs-3.0.1/src/arrrgs.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 .github/workflows/qa.yaml
 assets/logo@2x.png
+examples/aliases.py
 examples/args.py
 examples/basic.py
 examples/context.py
 examples/custom_name.py
 examples/environment.py
 examples/root_command.py
 src/arrrgs/__init__.py
```

