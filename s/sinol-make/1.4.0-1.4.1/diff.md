# Comparing `tmp/sinol-make-1.4.0.tar.gz` & `tmp/sinol-make-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.4.0.tar", last modified: Fri Aug  4 21:38:22 2023, max compression
+gzip compressed data, was "sinol-make-1.4.1.tar", last modified: Fri Aug  4 21:44:49 2023, max compression
```

## Comparing `sinol-make-1.4.0.tar` & `sinol-make-1.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-04 21:38:09.000000 sinol-make-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 21:38:22.438460 sinol-make-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-04 21:38:09.000000 sinol-make-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-04 21:38:09.000000 sinol-make-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:38:22.438460 sinol-make-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.434460 sinol-make-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.434460 sinol-make-1.4.0/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.434460 sinol-make-1.4.0/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/commands/gen/
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/gen/gen_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/gen/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/inwer/inwer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/inwer/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    46043 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/helpers/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-08-04 21:38:09.000000 sinol-make-1.4.0/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 21:38:22.000000 sinol-make-1.4.0/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:38:22.438460 sinol-make-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-08-04 21:38:09.000000 sinol-make-1.4.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.941498 sinol-make-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-04 21:44:37.000000 sinol-make-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 21:44:49.941498 sinol-make-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-04 21:44:37.000000 sinol-make-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-04 21:44:37.000000 sinol-make-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:44:49.941498 sinol-make-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.933498 sinol-make-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.937498 sinol-make-1.4.1/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.933498 sinol-make-1.4.1/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.937498 sinol-make-1.4.1/src/sinol_make/commands/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/gen/gen_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/gen/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.941498 sinol-make-1.4.1/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/inwer/inwer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/inwer/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.941498 sinol-make-1.4.1/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    47142 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.941498 sinol-make-1.4.1/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/helpers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/helpers/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.941498 sinol-make-1.4.1/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.941498 sinol-make-1.4.1/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-08-04 21:44:37.000000 sinol-make-1.4.1/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.937498 sinol-make-1.4.1/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 21:44:49.000000 sinol-make-1.4.1/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 21:44:49.000000 sinol-make-1.4.1/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:44:49.000000 sinol-make-1.4.1/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 21:44:49.000000 sinol-make-1.4.1/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 21:44:49.000000 sinol-make-1.4.1/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 21:44:49.000000 sinol-make-1.4.1/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:44:49.941498 sinol-make-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-08-04 21:44:37.000000 sinol-make-1.4.1/tests/test_util.py
```

### Comparing `sinol-make-1.4.0/LICENSE` & `sinol-make-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/PKG-INFO` & `sinol-make-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.4.0
+Version: 1.4.1
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.4.0/README.md` & `sinol-make-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/pyproject.toml` & `sinol-make-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/__init__.py` & `sinol-make-1.4.1/src/sinol_make/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argcomplete
 import argparse
 import sys
 
 from sinol_make import util
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
     parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
```

### Comparing `sinol-make-1.4.0/src/sinol_make/commands/gen/__init__.py` & `sinol-make-1.4.1/src/sinol_make/commands/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/commands/gen/gen_util.py` & `sinol-make-1.4.1/src/sinol_make/commands/gen/gen_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/commands/inwer/__init__.py` & `sinol-make-1.4.1/src/sinol_make/commands/inwer/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/commands/inwer/inwer_util.py` & `sinol-make-1.4.1/src/sinol_make/commands/inwer/inwer_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/commands/inwer/structs.py` & `sinol-make-1.4.1/src/sinol_make/commands/inwer/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.4.1/src/sinol_make/commands/run/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,28 +311,41 @@
         return sorted(list(set([self.get_group(test) for test in tests])))
 
 
     def compile_solutions(self, solutions):
         os.makedirs(self.COMPILATION_DIR, exist_ok=True)
         os.makedirs(self.EXECUTABLES_DIR, exist_ok=True)
         print("Compiling %d solutions..." % len(solutions))
+        args = [(solution, True) for solution in solutions]
         with mp.Pool(self.cpus) as pool:
-            compilation_results = pool.map(self.compile, solutions)
+            compilation_results = pool.starmap(self.compile, args)
         return compilation_results
 
 
-    def compile(self, solution):
+    def compile(self, solution, use_extras = False):
         compile_log_file = os.path.join(
             self.COMPILATION_DIR, "%s.compile_log" % package_util.get_file_name(solution))
         source_file = os.path.join(os.getcwd(), "prog", self.get_solution_from_exe(solution))
         output = os.path.join(self.EXECUTABLES_DIR, package_util.get_executable(solution))
 
+        extra_compilation_args = []
+        extra_compilation_files = []
+        if use_extras:
+            if "extra_compilation_args" in self.config:
+                lang = os.path.splitext(source_file)[1][1:]
+                for file in self.config["extra_compilation_args"].get(lang, []):
+                    extra_compilation_args.append(os.path.join(os.getcwd(), "prog", file))
+
+            for file in self.config.get("extra_compilation_files", []):
+                extra_compilation_files.append(os.path.join(os.getcwd(), "prog", file))
+
         try:
-            compile.compile(source_file, output, self.compilers,
-                            open(compile_log_file, "w"), self.args.weak_compilation_flags)
+            with open(compile_log_file, "w") as compile_log:
+                compile.compile(source_file, output, self.compilers, compile_log, self.args.weak_compilation_flags,
+                                extra_compilation_args, extra_compilation_files)
             print(util.info("Compilation of file %s was successful."
                             % package_util.get_file_name(solution)))
             return True
         except CompilationError as e:
             print(util.error("Compilation of file %s was unsuccessful."
                              % package_util.get_file_name(solution)))
             compile.print_compile_log(compile_log_file)
@@ -372,18 +385,20 @@
 
     def check_output(self, name, input_file, output_file_path, output, answer_file_path):
         """
         Checks if the output file is correct.
         Returns a tuple (is correct, number of points).
         """
         if not hasattr(self, "checker") or self.checker is None:
-            correct = util.lines_diff(output, open(answer_file_path, "r").readlines())
+            with open(answer_file_path, "r") as answer_file:
+                correct = util.lines_diff(output, answer_file.readlines())
             return correct, 100 if correct else 0
         else:
-            open(output_file_path, "w").write("\n".join(output))
+            with open(output_file_path, "w") as output_file:
+                output_file.write("\n".join(output))
             return self.check_output_checker(name, input_file, output_file_path, answer_file_path)
 
 
     def execute_oiejq(self, command, name, result_file_path, input_file_path, output_file_path, answer_file_path,
                       time_limit, memory_limit, hard_time_limit):
         env = os.environ.copy()
         env["MEM_LIMIT"] = f'{memory_limit}K'
@@ -475,15 +490,16 @@
                 timeout = True
                 os.killpg(os.getpgid(process.pid), signal.SIGTERM)
 
         result = ExecutionResult()
         program_exit_code = None
         if not timeout:
             output = output.decode("utf-8").splitlines()
-            lines = open(result_file_path).readlines()
+            with open(result_file_path, "r") as result_file:
+                lines = result_file.readlines()
             if len(lines) == 3:
                 """
                 If programs runs successfully, the output looks like this:
                  - first line is CPU time in seconds
                  - second line is memory in KB
                  - third line is exit code
                 This format is defined by -f flag in time command.
@@ -963,15 +979,16 @@
         if len(self.tests) > 0:
             print(util.bold('Tests that will be run:'), ' '.join([self.extract_file_name(test) for test in self.tests]))
 
             example_tests = [test for test in self.tests if self.get_group(test) == 0]
             if len(example_tests) == len(self.tests):
                 print(util.warning('Running only on example tests.'))
 
-            self.validate_existence_of_outputs()
+            if not self.has_lib:
+                self.validate_existence_of_outputs()
         else:
             print(util.warning('There are no tests to run.'))
 
     def check_errors(self, results: dict[str, dict[str, dict[str, ExecutionResult]]]):
         error_msg = ""
         for solution in results:
             for group in results[solution]:
@@ -984,18 +1001,19 @@
     def run(self, args):
         if not util.check_if_project():
             print(util.warning('You are not in a project directory (couldn\'t find config.yml in current directory).'))
             exit(1)
 
         self.set_constants()
         self.args = args
-        try:
-            self.config = yaml.load(open("config.yml"), Loader=yaml.FullLoader)
-        except AttributeError:
-            self.config = yaml.load(open("config.yml"))
+        with open(os.path.join(os.getcwd(), "config.yml"), 'r') as config:
+            try:
+                self.config = yaml.load(config, Loader=yaml.FullLoader)
+            except AttributeError:
+                self.config = yaml.load(config)
 
         if not 'title' in self.config.keys():
             util.exit_with_error('Title was not defined in config.yml.')
         if not 'time_limit' in self.config.keys():
             util.exit_with_error('Time limit was not defined in config.yml.')
         if not 'memory_limit' in self.config.keys():
             util.exit_with_error('Memory limit was not defined in config.yml.')
@@ -1029,14 +1047,17 @@
 
             checker_compilation = self.compile_solutions([self.checker])
             if not checker_compilation[0]:
                 util.exit_with_error('Checker compilation failed.')
         else:
             self.checker = None
 
+        lib = glob.glob(os.path.join(os.getcwd(), "prog", f'{self.ID}lib.*'))
+        self.has_lib = len(lib) != 0
+
         self.set_scores()
         self.check_are_any_tests_to_run()
 
         self.failed_compilations = []
         solutions = self.get_solutions(self.args.solutions)
 
         results, all_results = self.compile_and_run(solutions)
```

### Comparing `sinol-make-1.4.0/src/sinol_make/commands/run/structs.py` & `sinol-make-1.4.1/src/sinol_make/commands/run/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/helpers/compile.py` & `sinol-make-1.4.1/src/sinol_make/helpers/compile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,65 @@
 from typing import Tuple
 import os
 import sys
+import shutil
 import stat
 import subprocess
 
 import sinol_make.helpers.compiler as compiler
 from sinol_make.interfaces.Errors import CompilationError
 from sinol_make.structs.compiler_structs import Compilers
 
 
-def compile(program, output, compilers: Compilers = None, compile_log = None, weak_compilation_flags = False):
-    """
-    Compile a program
-    compilers - A Compilers object with compilers to use. If None, default compilers will be used.
+def compile(program, output, compilers: Compilers = None, compile_log = None, weak_compilation_flags = False,
+            extra_compilation_args = None, extra_compilation_files = None):
     """
+    Compile a program.
+    :param program: Path to the program to compile
+    :param output: Path to the output file
+    :param compilers: Compilers object
+    :param compile_log: File to write the compilation log to
+    :param weak_compilation_flags: If True, disable all warnings
+    :param extra_compilation_args: Extra compilation arguments
+    :param extra_compilation_files: Extra compilation files
+    """
+    if extra_compilation_args is None:
+        extra_compilation_args = []
+    if extra_compilation_files is None:
+        extra_compilation_files = []
+
+    for file in extra_compilation_files:
+        shutil.copy(file, os.path.join(os.path.dirname(output), os.path.basename(file)))
+
     gcc_compilation_flags = '-Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'
     if weak_compilation_flags:
-        gcc_compilation_flags = '-w' # Disable all warnings
+        gcc_compilation_flags = '-w'  # Disable all warnings
 
     if compilers is None:
         compilers = Compilers()
 
     ext = os.path.splitext(program)[1]
     arguments = []
     if ext == '.cpp':
-        arguments = [compilers.cpp_compiler_path or compiler.get_cpp_compiler_path(), program, '-o', output] + \
+        arguments = [compilers.cpp_compiler_path or compiler.get_cpp_compiler_path(), program] + \
+                    extra_compilation_args + ['-o', output] + \
                     f'--std=c++17 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
     elif ext == '.c':
-        arguments = [compilers.c_compiler_path, program, '-o', output] + \
+        arguments = [compilers.c_compiler_path or compiler.get_c_compiler_path(), program] + \
+                    extra_compilation_args + ['-o', output] + \
                     f'--std=c17 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
     elif ext == '.py':
         if sys.platform == 'win32' or sys.platform == 'cygwin':
             # TODO: Make this work on Windows
             pass
         else:
-            open(output, 'w').write('#!/usr/bin/python3\n')
-            open(output, 'a').write(open(program, 'r').read())
+            with open(output, 'w') as output_file, open(program, 'r') as program_file:
+                output_file.write('#!/usr/bin/python3\n')
+                output_file.write(program_file.read())
+
             st = os.stat(output)
             os.chmod(output, st.st_mode | stat.S_IEXEC)
         arguments = [compilers.python_interpreter_path, '-m', 'py_compile', program]
     elif ext == '.java':
         raise NotImplementedError('Java compilation is not implemented')
     else:
         raise CompilationError('Unknown file extension: ' + ext)
@@ -72,29 +92,26 @@
     executable_dir = os.path.join(os.getcwd(), 'cache', 'executables')
     compile_log_dir = os.path.join(os.getcwd(), 'cache', 'compilation')
     os.makedirs(executable_dir, exist_ok=True)
     os.makedirs(compile_log_dir, exist_ok=True)
 
     output = os.path.join(executable_dir, name)
     compile_log_path = os.path.join(compile_log_dir, os.path.splitext(name)[0] + '.compile_log')
-    compile_log = open(compile_log_path, 'w')
-
-    try:
-        if compile(file_path, output, compilers, compile_log, weak_compilation_flags):
-            return output, compile_log_path
-        else:
-            return None, compile_log_path
-    except CompilationError:
+    with open(compile_log_path, 'w') as compile_log:
+        try:
+            if compile(file_path, output, compilers, compile_log, weak_compilation_flags):
+                return output, compile_log_path
+        except CompilationError:
+            pass
         return None, compile_log_path
 
 
 def print_compile_log(compile_log_path: str):
     """
     Print the first 500 lines of compilation log
     :param compile_log_path: path to the compilation log
     """
 
-    compile_log = open(compile_log_path, 'r')
-    lines = compile_log.readlines()
-    compile_log.close()
-    for line in lines[:500]:
-        print(line, end='')
+    with open(compile_log_path, 'r') as compile_log:
+        lines = compile_log.readlines()
+        for line in lines[:500]:
+            print(line, end='')
```

### Comparing `sinol-make-1.4.0/src/sinol_make/helpers/compiler.py` & `sinol-make-1.4.1/src/sinol_make/helpers/compiler.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/helpers/package_util.py` & `sinol-make-1.4.1/src/sinol_make/helpers/package_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/helpers/parsers.py` & `sinol-make-1.4.1/src/sinol_make/helpers/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
                         help=f'C compiler to use (default {gcc_versions})')
     parser.add_argument('--cpp-compiler-path', dest='cpp_compiler_path', type=str, default=compiler.get_cpp_compiler_path(),
                         help=f'C++ compiler to use (default {gpp_versions})')
     parser.add_argument('--python-interpreter-path', dest='python_interpreter_path', type=str, default=compiler.get_python_interpreter_path(),
                         help='Python interpreter to use (default: python3)')
     parser.add_argument('--java-compiler-path', dest='java_compiler_path', type=str, default=compiler.get_java_compiler_path(),
                         help='Java compiler to use (default: javac)')
-    parser.add_argument('--weak-compilation-flags', dest='weak_compilation_flags', action='store_true',
+    parser.add_argument('-W', '--weak-compilation-flags', dest='weak_compilation_flags', action='store_true',
                         help='use weaker compilation flags')
```

### Comparing `sinol-make-1.4.0/src/sinol_make/helpers/printer.py` & `sinol-make-1.4.1/src/sinol_make/helpers/printer.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/structs/compiler_structs.py` & `sinol-make-1.4.1/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/src/sinol_make/util.py` & `sinol-make-1.4.1/src/sinol_make/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import glob, importlib, os, sys, subprocess, requests, tarfile, yaml
+import tempfile
 import importlib.resources
 import threading
 
 
 def get_commands():
     """
     Function to get an array of all available commands.
@@ -75,27 +76,33 @@
 
     try:
         request = requests.get('https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz')
     except requests.exceptions.ConnectionError:
         raise Exception('Couldn\'t download oiejq (https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz couldn\'t connect)')
     if request.status_code != 200:
         raise Exception('Couldn\'t download oiejq (https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz returned status code: ' + str(request.status_code) + ')')
-    open('/tmp/oiejq.tar.gz', 'wb').write(request.content)
 
-    def strip(tar):
-        l = len('oiejq/')
-        for member in tar.getmembers():
-            member.name = member.name[l:]
-            yield member
-
-    tar = tarfile.open('/tmp/oiejq.tar.gz')
-    tar.extractall(path=os.path.expanduser('~/.local/bin'), members=strip(tar))
-    tar.close()
-    os.remove('/tmp/oiejq.tar.gz')
-    os.rename(os.path.expanduser('~/.local/bin/oiejq.sh'), os.path.expanduser('~/.local/bin/oiejq'))
+    # oiejq is downloaded to a temporary directory and not to the `cache` dir,
+    # as there is no guarantee that the current directory is the package directory.
+    # The `cache` dir is only used for files that are part of the package and those
+    # that the package creator might want to look into.
+    with tempfile.TemporaryDirectory() as tmpdir:
+        oiejq_path = os.path.join(tmpdir, 'oiejq.tar.gz')
+        with open(oiejq_path, 'wb') as oiejq_file:
+            oiejq_file.write(request.content)
+
+        def strip(tar):
+            l = len('oiejq/')
+            for member in tar.getmembers():
+                member.name = member.name[l:]
+                yield member
+
+        with tarfile.open(oiejq_path) as tar:
+            tar.extractall(path=os.path.expanduser('~/.local/bin'), members=strip(tar))
+        os.rename(os.path.expanduser('~/.local/bin/oiejq.sh'), os.path.expanduser('~/.local/bin/oiejq'))
 
     return check_oiejq()
 
 
 def get_oiejq_path():
     if not check_oiejq():
         return None
@@ -127,15 +134,22 @@
         "title_en",
         "memory_limit",
         "memory_limits",
         "time_limit",
         "time_limits",
         "override_limits",
         "scores",
-        "extra_compilation_files",
+        {
+            "key": "extra_compilation_files",
+            "default_flow_style": None
+        },
+        {
+            "key": "extra_compilation_args",
+            "default_flow_style": None
+        },
         {
             "key": "sinol_expected_scores",
             "default_flow_style": None
         }
     ]
 
     config = config.copy()
@@ -236,20 +250,21 @@
     for i in range(len(lines1)):
         if lines1[i].rstrip() != lines2[i].rstrip():
             return False
 
     return True
 
 
-def file_diff(file1, file2):
+def file_diff(file1_path, file2_path):
     """
     Function to compare two files.
     Returns True if they are the same, False otherwise.
     """
-    return lines_diff(open(file1).readlines(), open(file2).readlines())
+    with open(file1_path) as file1, open(file2_path) as file2:
+        return lines_diff(file1.readlines(), file2.readlines())
 
 
 def get_terminal_size():
     """
     Function to get the size of the terminal.
     :return: triple (has_terminal, width, height)
     """
```

### Comparing `sinol-make-1.4.0/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.4.1/src/sinol_make.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.4.0
+Version: 1.4.1
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.4.0/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.4.1/src/sinol_make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinol-make-1.4.0/tests/test_util.py` & `sinol-make-1.4.1/tests/test_util.py`

 * *Files identical despite different names*

