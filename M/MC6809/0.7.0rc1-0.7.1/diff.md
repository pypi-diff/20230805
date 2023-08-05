# Comparing `tmp/MC6809-0.7.0rc1.tar.gz` & `tmp/MC6809-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MC6809-0.7.0rc1.tar", last modified: Tue Mar  7 17:20:51 2023, max compression
+gzip compressed data, was "MC6809-0.7.1.tar", last modified: Sat Aug  5 18:19:28 2023, max compression
```

## Comparing `MC6809-0.7.0rc1.tar` & `MC6809-0.7.1.tar`

### file list

```diff
@@ -1,86 +1,100 @@
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/
--rw-rw-r--   0 jens      (1000) jens      (1000)      891 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/AUTHORS
--rw-rw-r--   0 jens      (1000) jens      (1000)    35121 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/LICENSE
--rw-rw-r--   0 jens      (1000) jens      (1000)      125 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MANIFEST.in
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/
--rw-rw-r--   0 jens      (1000) jens      (1000)      174 2023-03-07 17:03:09.000000 MC6809-0.7.0rc1/MC6809/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      180 2023-03-06 18:58:20.000000 MC6809-0.7.0rc1/MC6809/__main__.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/cli/
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:58:20.000000 MC6809-0.7.0rc1/MC6809/cli/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     8684 2023-03-07 17:09:44.000000 MC6809-0.7.0rc1/MC6809/cli/cli_app.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/components/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/components/MC6809data/
--rwxrwxr-x   0 jens      (1000) jens      (1000)     4014 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/MC6809data/CPU6809_HTML_export.py
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1826 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/MC6809data/CPU6809csv_export.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      975 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/MC6809data/MC6809_data_utils.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    94239 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/MC6809data/MC6809_op_data.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    53563 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/MC6809data/MC6809_op_docs.py
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/MC6809data/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/__init__.py
--rwxrwxr-x   0 jens      (1000) jens      (1000)     2359 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu6809.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2417 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu6809_html_debug.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3698 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu6809_trace.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/components/cpu_utils/
--rw-rw-r--   0 jens      (1000) jens      (1000)     6066 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu_utils/Instruction_generator.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     4031 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu_utils/MC6809_registers.py
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu_utils/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      488 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu_utils/instruction_base.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    16001 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu_utils/instruction_call.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3214 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/cpu_utils/instruction_caller.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     9452 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_addressing.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    32047 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_base.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     7111 2023-03-06 19:10:18.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_cc_register.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     7921 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_interrupt.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    18636 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_ops_branches.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     4063 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_ops_load_store.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    10968 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_ops_logic.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     5063 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_ops_test.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1650 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_speedlimited.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     6580 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_stack.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     4123 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/mc6809_tools.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    13128 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/components/memory.py
--rw-rw-r--   0 jens      (1000) jens      (1000)       68 2023-03-06 18:58:20.000000 MC6809-0.7.0rc1/MC6809/constants.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/core/
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/core/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2325 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/core/bechmark.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     4188 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/core/configs.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     7924 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/core/cpu_control_server.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1835 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/core/memory_info.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     6690 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/example6809.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/tests/
--rw-rw-r--   0 jens      (1000) jens      (1000)     3581 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/LST2Unittest.py
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2261 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_6809_StoreLoad.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     9355 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_6809_address_modes.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    23255 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_6809_arithmetic.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    11918 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_6809_arithmetic_shift.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     9954 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_6809_branch_instructions.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    18623 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_6809_program.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     6151 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_6809_register_changes.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1468 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_accumulators.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     5208 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_base.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3735 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_condition_code_register.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      686 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_config.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    21089 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_cpu6809.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      207 2023-03-07 17:01:35.000000 MC6809-0.7.0rc1/MC6809/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      171 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/tests/test_example.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2257 2023-03-07 17:03:09.000000 MC6809-0.7.0rc1/MC6809/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2049 2023-03-07 17:18:24.000000 MC6809-0.7.0rc1/MC6809/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809/utils/
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/utils/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3212 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/utils/bits.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3509 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/utils/byte_word_values.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2337 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/utils/humanize.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2127 2023-03-06 18:49:14.000000 MC6809-0.7.0rc1/MC6809/utils/simple_debugger.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/MC6809.egg-info/
--rw-rw-r--   0 jens      (1000) jens      (1000)    13657 2023-03-07 17:20:51.000000 MC6809-0.7.0rc1/MC6809.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) jens      (1000)     2405 2023-03-07 17:20:51.000000 MC6809-0.7.0rc1/MC6809.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)        1 2023-03-07 17:20:51.000000 MC6809-0.7.0rc1/MC6809.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)       48 2023-03-07 17:20:51.000000 MC6809-0.7.0rc1/MC6809.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)      240 2023-03-07 17:20:51.000000 MC6809-0.7.0rc1/MC6809.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)        7 2023-03-07 17:20:51.000000 MC6809-0.7.0rc1/MC6809.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)    13657 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/PKG-INFO
--rw-rw-r--   0 jens      (1000) jens      (1000)    12354 2023-03-07 17:17:24.000000 MC6809-0.7.0rc1/README.md
--rwxrwxr-x   0 jens      (1000) jens      (1000)     3032 2023-03-06 18:58:20.000000 MC6809-0.7.0rc1/cli.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     5297 2023-03-07 17:17:24.000000 MC6809-0.7.0rc1/pyproject.toml
--rw-rw-r--   0 jens      (1000) jens      (1000)       38 2023-03-07 17:20:51.684783 MC6809-0.7.0rc1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.497591 MC6809-0.7.1/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-03-06 18:58:20.000000 MC6809-0.7.1/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      152 2023-08-05 15:38:29.000000 MC6809-0.7.1/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-08-05 18:12:02.000000 MC6809-0.7.1/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-08-04 16:04:23.000000 MC6809-0.7.1/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      891 2023-03-06 18:49:14.000000 MC6809-0.7.1/AUTHORS
+-rw-rw-r--   0 jens      (1000) users      (100)    44002 2023-08-05 18:19:22.000000 MC6809-0.7.1/CPU6809_opcodes.html
+-rw-rw-r--   0 jens      (1000) users      (100)    35121 2023-03-06 18:49:14.000000 MC6809-0.7.1/LICENSE
+-rw-rw-r--   0 jens      (1000) users      (100)      125 2023-03-06 18:49:14.000000 MC6809-0.7.1/MANIFEST.in
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/MC6809/
+-rw-rw-r--   0 jens      (1000) users      (100)      120 2023-08-05 18:16:08.000000 MC6809-0.7.1/MC6809/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      180 2023-03-06 18:58:20.000000 MC6809-0.7.1/MC6809/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/MC6809/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:58:20.000000 MC6809-0.7.1/MC6809/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2657 2023-08-05 15:39:42.000000 MC6809-0.7.1/MC6809/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7840 2023-08-05 18:18:01.000000 MC6809-0.7.1/MC6809/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/MC6809/components/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/MC6809/components/MC6809data/
+-rwxrwxr-x   0 jens      (1000) users      (100)     4014 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/CPU6809_HTML_export.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    29721 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/CPU6809_opcodes.csv
+-rw-rw-r--   0 jens      (1000) users      (100)    44002 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/CPU6809_opcodes.html
+-rwxrwxr-x   0 jens      (1000) users      (100)     1826 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/CPU6809csv_export.py
+-rw-rw-r--   0 jens      (1000) users      (100)      975 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/MC6809_data_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)    94239 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/MC6809_op_data.py
+-rw-rw-r--   0 jens      (1000) users      (100)    53563 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/MC6809_op_docs.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/MC6809data/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/__init__.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     2359 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu6809.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2417 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu6809_html_debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3698 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu6809_trace.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/MC6809/components/cpu_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)     6066 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu_utils/Instruction_generator.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4031 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu_utils/MC6809_registers.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      488 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu_utils/instruction_base.py
+-rw-rw-r--   0 jens      (1000) users      (100)    16001 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu_utils/instruction_call.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3214 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/cpu_utils/instruction_caller.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9452 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_addressing.py
+-rw-rw-r--   0 jens      (1000) users      (100)    32047 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_base.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7111 2023-03-06 19:10:18.000000 MC6809-0.7.1/MC6809/components/mc6809_cc_register.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7921 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_interrupt.py
+-rw-rw-r--   0 jens      (1000) users      (100)    18636 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_ops_branches.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4063 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_ops_load_store.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10968 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_ops_logic.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5063 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_ops_test.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1650 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_speedlimited.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6580 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_stack.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4123 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/mc6809_tools.py
+-rw-rw-r--   0 jens      (1000) users      (100)    13128 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/components/memory.py
+-rw-rw-r--   0 jens      (1000) users      (100)       64 2023-08-04 16:04:23.000000 MC6809-0.7.1/MC6809/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/MC6809/core/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/core/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2325 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/core/bechmark.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4188 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/core/configs.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7924 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/core/cpu_control_server.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1835 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/core/memory_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6690 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/example6809.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.497591 MC6809-0.7.1/MC6809/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)    44002 2023-03-07 17:05:39.000000 MC6809-0.7.1/MC6809/tests/CPU6809_opcodes.html
+-rw-rw-r--   0 jens      (1000) users      (100)     3581 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/LST2Unittest.py
+-rw-rw-r--   0 jens      (1000) users      (100)      150 2023-08-04 16:04:23.000000 MC6809-0.7.1/MC6809/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2261 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_6809_StoreLoad.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9355 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_6809_address_modes.py
+-rw-rw-r--   0 jens      (1000) users      (100)    23255 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_6809_arithmetic.py
+-rw-rw-r--   0 jens      (1000) users      (100)    11918 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_6809_arithmetic_shift.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9954 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_6809_branch_instructions.py
+-rw-rw-r--   0 jens      (1000) users      (100)    18623 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_6809_program.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6151 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_6809_register_changes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1468 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_accumulators.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5208 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_base.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3735 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_condition_code_register.py
+-rw-rw-r--   0 jens      (1000) users      (100)      686 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_config.py
+-rw-rw-r--   0 jens      (1000) users      (100)    21089 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_cpu6809.py
+-rw-rw-r--   0 jens      (1000) users      (100)      207 2023-03-07 17:01:35.000000 MC6809-0.7.1/MC6809/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)      171 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/tests/test_example.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2550 2023-08-04 16:04:23.000000 MC6809-0.7.1/MC6809/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2525 2023-08-05 18:10:44.000000 MC6809-0.7.1/MC6809/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.497591 MC6809-0.7.1/MC6809/utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3212 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/utils/bits.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3509 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/utils/byte_word_values.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2337 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/utils/humanize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2127 2023-03-06 18:49:14.000000 MC6809-0.7.1/MC6809/utils/simple_debugger.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 18:19:28.493591 MC6809-0.7.1/MC6809.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    14509 2023-08-05 18:19:28.000000 MC6809-0.7.1/MC6809.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     2687 2023-08-05 18:19:28.000000 MC6809-0.7.1/MC6809.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-08-05 18:19:28.000000 MC6809-0.7.1/MC6809.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       85 2023-08-05 18:19:28.000000 MC6809-0.7.1/MC6809.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      187 2023-08-05 18:19:28.000000 MC6809-0.7.1/MC6809.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        7 2023-08-05 18:19:28.000000 MC6809-0.7.1/MC6809.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    14509 2023-08-05 18:19:28.497591 MC6809-0.7.1/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    14098 2023-08-05 18:16:08.000000 MC6809-0.7.1/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-08-04 16:04:23.000000 MC6809-0.7.1/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-08-04 16:04:23.000000 MC6809-0.7.1/dev-cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4558 2023-08-05 15:38:29.000000 MC6809-0.7.1/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    50934 2023-08-05 15:38:29.000000 MC6809-0.7.1/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1663 2023-08-05 15:38:29.000000 MC6809-0.7.1/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-08-05 18:19:28.497591 MC6809-0.7.1/setup.cfg
```

### Comparing `MC6809-0.7.0rc1/AUTHORS` & `MC6809-0.7.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/LICENSE` & `MC6809-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/cli/cli_app.py` & `MC6809-0.7.1/MC6809/cli/dev.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,56 @@
-import cProfile
+"""
+    CLI for development
+"""
 import logging
-import pstats
 import sys
 from pathlib import Path
 
 import rich_click as click
 from bx_py_utils.path import assert_is_file
 from manageprojects.utilities import code_style
 from manageprojects.utilities.publish import publish_package
 from manageprojects.utilities.subprocess_utils import verbose_check_call
 from manageprojects.utilities.version_info import print_version
-from rich import print  # noqa
+from rich import print  # noqa; noqa
 from rich_click import RichGroup
 
 import MC6809
 from MC6809 import constants
-from MC6809.core.bechmark import run_benchmark
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(MC6809.__file__).parent.parent
 assert_is_file(PACKAGE_ROOT / 'pyproject.toml')
 
 OPTION_ARGS_DEFAULT_TRUE = dict(is_flag=True, show_default=True, default=True)
 OPTION_ARGS_DEFAULT_FALSE = dict(is_flag=True, show_default=True, default=False)
 ARGUMENT_EXISTING_DIR = dict(
     type=click.Path(exists=True, file_okay=False, dir_okay=True, readable=True, path_type=Path)
 )
 ARGUMENT_NOT_EXISTING_DIR = dict(
-    type=click.Path(exists=False, file_okay=False, dir_okay=True, readable=False, writable=True, path_type=Path)
+    type=click.Path(
+        exists=False,
+        file_okay=False,
+        dir_okay=True,
+        readable=False,
+        writable=True,
+        path_type=Path,
+    )
 )
 ARGUMENT_EXISTING_FILE = dict(
     type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True, path_type=Path)
 )
 
 
 class ClickGroup(RichGroup):  # FIXME: How to set the "info_name" easier?
     def make_context(self, info_name, *args, **kwargs):
-        info_name = './cli.py'
+        info_name = './dev-cli.py'
         return super().make_context(info_name, *args, **kwargs)
 
 
 @click.group(
     cls=ClickGroup,
     epilog=constants.CLI_EPILOG,
 )
@@ -79,15 +86,15 @@
 
 @click.command()
 def install():
     """
     Run pip-sync and install 'MC6809' via pip as editable.
     """
     verbose_check_call('pip-sync', PACKAGE_ROOT / 'requirements.dev.txt')
-    verbose_check_call('pip', 'install', '-e', '.')
+    verbose_check_call('pip', 'install', '--no-deps', '-e', '.')
 
 
 cli.add_command(install)
 
 
 @click.command()
 def safety():
@@ -138,18 +145,18 @@
         'pyproject.toml',
         '--extra=dev',
         '--output-file',
         'requirements.dev.txt',
         extra_env=extra_env,
     )
 
-    verbose_check_call('safety', 'check', '-r', 'requirements.dev.txt')
+    verbose_check_call(bin_path / 'safety', 'check', '-r', 'requirements.dev.txt')
 
     # Install new dependencies in current .venv:
-    verbose_check_call('pip-sync', 'requirements.dev.txt')
+    verbose_check_call(bin_path / 'pip-sync', 'requirements.dev.txt')
 
 
 cli.add_command(update)
 
 
 @click.command()
 def publish():
@@ -157,14 +164,15 @@
     Build and upload this project to PyPi
     """
     _run_unittest_cli(verbose=False, exit_after_run=False)  # Don't publish a broken state
 
     publish_package(
         module=MC6809,
         package_path=PACKAGE_ROOT,
+        distribution_name='MC6809',
     )
 
 
 cli.add_command(publish)
 
 
 @click.command()
@@ -290,49 +298,20 @@
     # Pseudo command, because the version always printed on every CLI call ;)
     sys.exit(0)
 
 
 cli.add_command(version)
 
 
-@click.command()
-@click.option('--loops', type=int, default=6, show_default=True, help='How many benchmark loops should be run?')
-@click.option('--multiply', type=int, default=15, show_default=True, help='est data multiplier')
-def benchmark(loops, multiply):
-    """
-    Run a MC6809 emulation benchmark
-    """
-    run_benchmark(loops=loops, multiply=multiply)
-
-
-cli.add_command(benchmark)
-
-
-@click.command()
-@click.option('--loops', type=int, default=6, show_default=True, help='How many benchmark loops should be run?')
-@click.option('--multiply', type=int, default=15, show_default=True, help='est data multiplier')
-def profile(loops, multiply):
-    """
-    Profile the MC6809 emulation benchmark
-    """
-    with cProfile.Profile() as pr:
-        run_benchmark(loops=loops, multiply=multiply)
-    pstats.Stats(pr).sort_stats('tottime', 'cumulative', 'calls').print_stats(20)
-
-
-cli.add_command(profile)
-
-
 def main():
     print_version(MC6809)
 
     if len(sys.argv) >= 2:
         # Check if we just pass a command call
         command = sys.argv[1]
         if command == 'test':
             _run_unittest_cli()
         elif command == 'tox':
             _run_tox()
 
     # Execute Click CLI:
-    cli.name = './cli.py'
     cli()
```

### Comparing `MC6809-0.7.0rc1/MC6809/components/MC6809data/CPU6809_HTML_export.py` & `MC6809-0.7.1/MC6809/components/MC6809data/CPU6809_HTML_export.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/MC6809data/CPU6809csv_export.py` & `MC6809-0.7.1/MC6809/components/MC6809data/CPU6809csv_export.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/MC6809data/MC6809_data_utils.py` & `MC6809-0.7.1/MC6809/components/MC6809data/MC6809_data_utils.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/MC6809data/MC6809_op_data.py` & `MC6809-0.7.1/MC6809/components/MC6809data/MC6809_op_data.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/MC6809data/MC6809_op_docs.py` & `MC6809-0.7.1/MC6809/components/MC6809data/MC6809_op_docs.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/cpu6809.py` & `MC6809-0.7.1/MC6809/components/cpu6809.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/cpu6809_html_debug.py` & `MC6809-0.7.1/MC6809/components/cpu6809_html_debug.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/cpu6809_trace.py` & `MC6809-0.7.1/MC6809/components/cpu6809_trace.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/cpu_utils/Instruction_generator.py` & `MC6809-0.7.1/MC6809/components/cpu_utils/Instruction_generator.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/cpu_utils/MC6809_registers.py` & `MC6809-0.7.1/MC6809/components/cpu_utils/MC6809_registers.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/cpu_utils/instruction_call.py` & `MC6809-0.7.1/MC6809/components/cpu_utils/instruction_call.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/cpu_utils/instruction_caller.py` & `MC6809-0.7.1/MC6809/components/cpu_utils/instruction_caller.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_addressing.py` & `MC6809-0.7.1/MC6809/components/mc6809_addressing.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_base.py` & `MC6809-0.7.1/MC6809/components/mc6809_base.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_cc_register.py` & `MC6809-0.7.1/MC6809/components/mc6809_cc_register.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_interrupt.py` & `MC6809-0.7.1/MC6809/components/mc6809_interrupt.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_ops_branches.py` & `MC6809-0.7.1/MC6809/components/mc6809_ops_branches.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_ops_load_store.py` & `MC6809-0.7.1/MC6809/components/mc6809_ops_load_store.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_ops_logic.py` & `MC6809-0.7.1/MC6809/components/mc6809_ops_logic.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_ops_test.py` & `MC6809-0.7.1/MC6809/components/mc6809_ops_test.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_speedlimited.py` & `MC6809-0.7.1/MC6809/components/mc6809_speedlimited.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_stack.py` & `MC6809-0.7.1/MC6809/components/mc6809_stack.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/mc6809_tools.py` & `MC6809-0.7.1/MC6809/components/mc6809_tools.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/components/memory.py` & `MC6809-0.7.1/MC6809/components/memory.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/core/bechmark.py` & `MC6809-0.7.1/MC6809/core/bechmark.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/core/configs.py` & `MC6809-0.7.1/MC6809/core/configs.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/core/cpu_control_server.py` & `MC6809-0.7.1/MC6809/core/cpu_control_server.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/core/memory_info.py` & `MC6809-0.7.1/MC6809/core/memory_info.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/example6809.py` & `MC6809-0.7.1/MC6809/example6809.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/LST2Unittest.py` & `MC6809-0.7.1/MC6809/tests/LST2Unittest.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_6809_StoreLoad.py` & `MC6809-0.7.1/MC6809/tests/test_6809_StoreLoad.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_6809_address_modes.py` & `MC6809-0.7.1/MC6809/tests/test_6809_address_modes.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_6809_arithmetic.py` & `MC6809-0.7.1/MC6809/tests/test_6809_arithmetic.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_6809_arithmetic_shift.py` & `MC6809-0.7.1/MC6809/tests/test_6809_arithmetic_shift.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_6809_branch_instructions.py` & `MC6809-0.7.1/MC6809/tests/test_6809_branch_instructions.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_6809_program.py` & `MC6809-0.7.1/MC6809/tests/test_6809_program.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_6809_register_changes.py` & `MC6809-0.7.1/MC6809/tests/test_6809_register_changes.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_accumulators.py` & `MC6809-0.7.1/MC6809/tests/test_accumulators.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_base.py` & `MC6809-0.7.1/MC6809/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_condition_code_register.py` & `MC6809-0.7.1/MC6809/tests/test_condition_code_register.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_config.py` & `MC6809-0.7.1/MC6809/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_cpu6809.py` & `MC6809-0.7.1/MC6809/tests/test_cpu6809.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_project_setup.py` & `MC6809-0.7.1/MC6809/tests/test_project_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 import subprocess
-from pathlib import Path
 from unittest import TestCase
 
-
-try:
-    import tomllib  # New in Python 3.11
-except ImportError:
-    import tomli as tomllib
-
 from bx_py_utils.path import assert_is_file
 from manageprojects.test_utils.click_cli_utils import subprocess_cli
+from manageprojects.test_utils.project_setup import check_editor_config, get_py_max_line_length
 from manageprojects.utilities import code_style
+from packaging.version import Version
 
 from MC6809 import __version__
 from MC6809.cli.cli_app import PACKAGE_ROOT
 
 
 class ProjectSetupTestCase(TestCase):
     def test_version(self):
-        pyproject_toml_path = Path(PACKAGE_ROOT, 'pyproject.toml')
-        assert_is_file(pyproject_toml_path)
-
         self.assertIsNotNone(__version__)
 
-        pyproject_toml = tomllib.loads(pyproject_toml_path.read_text(encoding='UTF-8'))
-        pyproject_version = pyproject_toml['project']['version']
-
-        self.assertEqual(__version__, pyproject_version)
+        version = Version(__version__)  # Will raise InvalidVersion() if wrong formatted
+        self.assertEqual(str(version), __version__)
 
         cli_bin = PACKAGE_ROOT / 'cli.py'
         assert_is_file(cli_bin)
 
         output = subprocess.check_output([cli_bin, 'version'], text=True)
         self.assertIn(f'MC6809 v{__version__}', output)
 
+        dev_cli_bin = PACKAGE_ROOT / 'dev-cli.py'
+        assert_is_file(dev_cli_bin)
+
+        output = subprocess.check_output([dev_cli_bin, 'version'], text=True)
+        self.assertIn(f'MC6809 v{__version__}', output)
+
     def test_code_style(self):
-        cli_bin = PACKAGE_ROOT / 'cli.py'
-        assert_is_file(cli_bin)
+        dev_cli_bin = PACKAGE_ROOT / 'dev-cli.py'
+        assert_is_file(dev_cli_bin)
 
         try:
             output = subprocess_cli(
-                cli_bin=cli_bin,
+                cli_bin=dev_cli_bin,
                 args=('check-code-style',),
                 exit_on_error=False,
             )
         except subprocess.CalledProcessError as err:
             self.assertIn('.venv/bin/darker', err.stdout)  # darker was called?
         else:
             if 'Code style: OK' in output:
                 self.assertIn('.venv/bin/darker', output)  # darker was called?
                 return  # Nothing to fix -> OK
 
         # Try to "auto" fix code style:
 
         try:
             output = subprocess_cli(
-                cli_bin=cli_bin,
+                cli_bin=dev_cli_bin,
                 args=('fix-code-style',),
                 exit_on_error=False,
             )
         except subprocess.CalledProcessError as err:
             output = err.stdout
 
         self.assertIn('.venv/bin/darker', output)  # darker was called?
 
         # Check again and display the output:
 
         try:
             code_style.check(package_root=PACKAGE_ROOT)
         except SystemExit as err:
             self.assertEqual(err.code, 0, 'Code style error, see output above!')
+
+    def test_check_editor_config(self):
+        check_editor_config(package_root=PACKAGE_ROOT)
+
+        max_line_length = get_py_max_line_length(package_root=PACKAGE_ROOT)
+        self.assertEqual(max_line_length, 119)
```

### Comparing `MC6809-0.7.0rc1/MC6809/tests/test_readme.py` & `MC6809-0.7.1/MC6809/tests/test_readme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from bx_py_utils.auto_doc import assert_readme_block
 from bx_py_utils.path import assert_is_file
 from manageprojects.test_utils.click_cli_utils import invoke_click
 from manageprojects.tests.base import BaseTestCase
 
 from MC6809 import constants
 from MC6809.cli.cli_app import PACKAGE_ROOT, cli
+from MC6809.cli.dev import cli as dev_cli
 
 
 def assert_cli_help_in_readme(text_block: str, marker: str):
     README_PATH = PACKAGE_ROOT / 'README.md'
     assert_is_file(README_PATH)
 
     text_block = text_block.replace(constants.CLI_EPILOG, '')
@@ -31,14 +32,27 @@
                 ' benchmark ',
                 ' profile ',
                 constants.CLI_EPILOG,
             ),
         )
         assert_cli_help_in_readme(text_block=stdout, marker='main help')
 
+    def test_dev_cli_main_help(self):
+        stdout = invoke_click(dev_cli, '--help')
+        self.assert_in_content(
+            got=stdout,
+            parts=(
+                'Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...',
+                ' check-code-style ',
+                ' coverage ',
+                constants.CLI_EPILOG,
+            ),
+        )
+        assert_cli_help_in_readme(text_block=stdout, marker='dev help')
+
     def test_benchmark_help(self):
         stdout = invoke_click(cli, 'benchmark', '--help')
         self.assert_in_content(
             got=stdout,
             parts=(
                 'Usage: ./cli.py benchmark [OPTIONS]',
                 ' --loops ',
```

### Comparing `MC6809-0.7.0rc1/MC6809/utils/bits.py` & `MC6809-0.7.1/MC6809/utils/bits.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/utils/byte_word_values.py` & `MC6809-0.7.1/MC6809/utils/byte_word_values.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/utils/humanize.py` & `MC6809-0.7.1/MC6809/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809/utils/simple_debugger.py` & `MC6809-0.7.1/MC6809/utils/simple_debugger.py`

 * *Files identical despite different names*

### Comparing `MC6809-0.7.0rc1/MC6809.egg-info/PKG-INFO` & `MC6809-0.7.1/MC6809.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 Metadata-Version: 2.1
 Name: MC6809
-Version: 0.7.0rc1
+Version: 0.7.1
 Summary: MC6809 CPU emulator written in Python
 Author-email: Jens Diemer <git@jensdiemer.de>
+License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/6809/MC6809
 Project-URL: Source, https://github.com/6809/MC6809
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Environment :: X11 Applications
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: System :: Emulators
-Classifier: Topic :: Software Development :: Assemblers
-Classifier: Topic :: Software Development :: Testing
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
 ## MC6809 CPU emulator written in Python
@@ -47,53 +30,32 @@
 Getting started:
 ```bash
 ~$ git clone https://github.com/6809/MC6809.git
 ~$ cd MC6809
 ~/MC6809 $ ./cli.py --help
 ```
 
-```bash
-~$ git clone https://github.com/jedie/DragonPy.git
-~$ cd DragonPy/
-~/DragonPy$ ./cli.py --help
-```
-
 The output of `./cli.py --help` looks like:
 
 [comment]: <> (✂✂✂ auto generated main help start ✂✂✂)
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ benchmark                   Run a MC6809 emulation benchmark                                     │
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ fix-code-style              Fix code style of all MC6809 source code files via darker            │
-│ install                     Run pip-sync and install 'MC6809' via pip as editable.               │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
-│ profile                     Profile the MC6809 emulation benchmark                               │
-│ publish                     Build and upload this project to PyPi                                │
-│ safety                      Run safety check against current requirements files                  │
-│ test                        Run unittests                                                        │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
-│ version                     Print version and exit                                               │
+│ benchmark            Run a MC6809 emulation benchmark                                            │
+│ profile              Profile the MC6809 emulation benchmark                                      │
+│ version              Print version and exit                                                      │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
-
-
-You can use the devshell as a CLI, too, e.g.:
 There is a simple benchmark. Run e.g.:
 ```bash
 ~/MC6809$ ./cli.py benchmark --help
 ```
 
 The output of `./cli.py benchmark --help` looks like:
 
@@ -108,25 +70,14 @@
 │ --multiply    INTEGER  est data multiplier [default: 15]                                         │
 │ --help                 Show this message and exit.                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated benchmark help end ✂✂✂)
 
 
-
-### tests
-
-```bash
-~/DragonPy$ ./cli.py coverage
-# or just:
-~/DragonPy$ ./cli.py test
-# or with different Python versions:
-~/DragonPy$ ./cli.py tox
-```
-
 ### profile
 
 You can run the Python profiler against the benchmark, e.g.:
 
 ```bash
 ~/MC6809$ ./cli.py profile --help
 ```
@@ -144,14 +95,62 @@
 │ --multiply    INTEGER  est data multiplier [default: 15]                                         │
 │ --help                 Show this message and exit.                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated profile help end ✂✂✂)
 
 
+### development
+
+For development exists `dev-cli`, e.g.:
+
+```bash
+~/MC6809$ ./dev-cli.py --help
+```
+
+The output of `./dev-cli.py --help` looks like:
+
+[comment]: <> (✂✂✂ auto generated dev help start ✂✂✂)
+```
+Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help      Show this message and exit.                                                          │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+│ check-code-style            Check code style by calling darker + flake8                          │
+│ coverage                    Run and show coverage.                                               │
+│ fix-code-style              Fix code style of all MC6809 source code files via darker            │
+│ install                     Run pip-sync and install 'MC6809' via pip as editable.               │
+│ mypy                        Run Mypy (configured in pyproject.toml)                              │
+│ publish                     Build and upload this project to PyPi                                │
+│ safety                      Run safety check against current requirements files                  │
+│ test                        Run unittests                                                        │
+│ tox                         Run tox                                                              │
+│ update                      Update "requirements*.txt" dependencies files                        │
+│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
+│                             files)                                                               │
+│ version                     Print version and exit                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+Run tests, e.g.:
+
+```bash
+~/DragonPy$ ./dev-cli.py coverage
+# or just:
+~/DragonPy$ ./dev-cli.py test
+# or with different Python versions:
+~/DragonPy$ ./dev-cli.py tox
+```
+
+
+
+
 ### TODO
 
 
 * Update 'cpu6809_html_debug.py'
 * Use bottle for http control server part
 * unimplemented OPs:
   * RESET
@@ -160,16 +159,19 @@
 
 
 ## History
 
 (Some of the points are related to [DragonPy Emulator](https://github.com/jedie/DragonPy))
 
 
-* [*dev*](https://github.com/6809/MC6809/compare/v0.7.0...main)
+* [*dev*](https://github.com/6809/MC6809/compare/v0.7.1...main)
   * TBC
+* 05.08.2023 - [v0.7.1](https://github.com/6809/MC6809/compare/v0.7.0...v0.7.1)
+  * Split CLI in a app and dev version with different venvs.
+  * Update requirements
 * 07.03.2023 - [v0.7.0](https://github.com/6809/MC6809/compare/v0.6.0...v0.7.0)
   * Replace the `Makefile` with a click CLI
   * Use pip-tools and https://github.com/jedie/manageprojects
   * Rename git `master` to `main` branch
   * Run CI tests against Python 3.9, 3.10 and 3.11
   * Replace Creole README with markdown
 * 10.02.2020 - [v0.6.0](https://github.com/6809/MC6809/compare/v0.5.0...v0.6.0)
```

### Comparing `MC6809-0.7.0rc1/MC6809.egg-info/SOURCES.txt` & `MC6809-0.7.1/MC6809.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,34 @@
+.editorconfig
+.flake8
+.gitignore
 AUTHORS
+CPU6809_opcodes.html
 LICENSE
 MANIFEST.in
 README.md
 cli.py
+dev-cli.py
 pyproject.toml
+requirements.dev.txt
+requirements.txt
+.github/workflows/tests.yml
 MC6809/__init__.py
 MC6809/__main__.py
 MC6809/constants.py
 MC6809/example6809.py
 MC6809.egg-info/PKG-INFO
 MC6809.egg-info/SOURCES.txt
 MC6809.egg-info/dependency_links.txt
 MC6809.egg-info/entry_points.txt
 MC6809.egg-info/requires.txt
 MC6809.egg-info/top_level.txt
 MC6809/cli/__init__.py
 MC6809/cli/cli_app.py
+MC6809/cli/dev.py
 MC6809/components/__init__.py
 MC6809/components/cpu6809.py
 MC6809/components/cpu6809_html_debug.py
 MC6809/components/cpu6809_trace.py
 MC6809/components/mc6809_addressing.py
 MC6809/components/mc6809_base.py
 MC6809/components/mc6809_cc_register.py
@@ -29,14 +38,16 @@
 MC6809/components/mc6809_ops_logic.py
 MC6809/components/mc6809_ops_test.py
 MC6809/components/mc6809_speedlimited.py
 MC6809/components/mc6809_stack.py
 MC6809/components/mc6809_tools.py
 MC6809/components/memory.py
 MC6809/components/MC6809data/CPU6809_HTML_export.py
+MC6809/components/MC6809data/CPU6809_opcodes.csv
+MC6809/components/MC6809data/CPU6809_opcodes.html
 MC6809/components/MC6809data/CPU6809csv_export.py
 MC6809/components/MC6809data/MC6809_data_utils.py
 MC6809/components/MC6809data/MC6809_op_data.py
 MC6809/components/MC6809data/MC6809_op_docs.py
 MC6809/components/MC6809data/__init__.py
 MC6809/components/cpu_utils/Instruction_generator.py
 MC6809/components/cpu_utils/MC6809_registers.py
@@ -45,14 +56,15 @@
 MC6809/components/cpu_utils/instruction_call.py
 MC6809/components/cpu_utils/instruction_caller.py
 MC6809/core/__init__.py
 MC6809/core/bechmark.py
 MC6809/core/configs.py
 MC6809/core/cpu_control_server.py
 MC6809/core/memory_info.py
+MC6809/tests/CPU6809_opcodes.html
 MC6809/tests/LST2Unittest.py
 MC6809/tests/__init__.py
 MC6809/tests/test_6809_StoreLoad.py
 MC6809/tests/test_6809_address_modes.py
 MC6809/tests/test_6809_arithmetic.py
 MC6809/tests/test_6809_arithmetic_shift.py
 MC6809/tests/test_6809_branch_instructions.py
```

### Comparing `MC6809-0.7.0rc1/PKG-INFO` & `MC6809-0.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 Metadata-Version: 2.1
 Name: MC6809
-Version: 0.7.0rc1
+Version: 0.7.1
 Summary: MC6809 CPU emulator written in Python
 Author-email: Jens Diemer <git@jensdiemer.de>
+License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/6809/MC6809
 Project-URL: Source, https://github.com/6809/MC6809
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Environment :: X11 Applications
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: System :: Emulators
-Classifier: Topic :: Software Development :: Assemblers
-Classifier: Topic :: Software Development :: Testing
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
 ## MC6809 CPU emulator written in Python
@@ -47,53 +30,32 @@
 Getting started:
 ```bash
 ~$ git clone https://github.com/6809/MC6809.git
 ~$ cd MC6809
 ~/MC6809 $ ./cli.py --help
 ```
 
-```bash
-~$ git clone https://github.com/jedie/DragonPy.git
-~$ cd DragonPy/
-~/DragonPy$ ./cli.py --help
-```
-
 The output of `./cli.py --help` looks like:
 
 [comment]: <> (✂✂✂ auto generated main help start ✂✂✂)
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ benchmark                   Run a MC6809 emulation benchmark                                     │
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ fix-code-style              Fix code style of all MC6809 source code files via darker            │
-│ install                     Run pip-sync and install 'MC6809' via pip as editable.               │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
-│ profile                     Profile the MC6809 emulation benchmark                               │
-│ publish                     Build and upload this project to PyPi                                │
-│ safety                      Run safety check against current requirements files                  │
-│ test                        Run unittests                                                        │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
-│ version                     Print version and exit                                               │
+│ benchmark            Run a MC6809 emulation benchmark                                            │
+│ profile              Profile the MC6809 emulation benchmark                                      │
+│ version              Print version and exit                                                      │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
-
-
-You can use the devshell as a CLI, too, e.g.:
 There is a simple benchmark. Run e.g.:
 ```bash
 ~/MC6809$ ./cli.py benchmark --help
 ```
 
 The output of `./cli.py benchmark --help` looks like:
 
@@ -108,25 +70,14 @@
 │ --multiply    INTEGER  est data multiplier [default: 15]                                         │
 │ --help                 Show this message and exit.                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated benchmark help end ✂✂✂)
 
 
-
-### tests
-
-```bash
-~/DragonPy$ ./cli.py coverage
-# or just:
-~/DragonPy$ ./cli.py test
-# or with different Python versions:
-~/DragonPy$ ./cli.py tox
-```
-
 ### profile
 
 You can run the Python profiler against the benchmark, e.g.:
 
 ```bash
 ~/MC6809$ ./cli.py profile --help
 ```
@@ -144,14 +95,62 @@
 │ --multiply    INTEGER  est data multiplier [default: 15]                                         │
 │ --help                 Show this message and exit.                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated profile help end ✂✂✂)
 
 
+### development
+
+For development exists `dev-cli`, e.g.:
+
+```bash
+~/MC6809$ ./dev-cli.py --help
+```
+
+The output of `./dev-cli.py --help` looks like:
+
+[comment]: <> (✂✂✂ auto generated dev help start ✂✂✂)
+```
+Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help      Show this message and exit.                                                          │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+│ check-code-style            Check code style by calling darker + flake8                          │
+│ coverage                    Run and show coverage.                                               │
+│ fix-code-style              Fix code style of all MC6809 source code files via darker            │
+│ install                     Run pip-sync and install 'MC6809' via pip as editable.               │
+│ mypy                        Run Mypy (configured in pyproject.toml)                              │
+│ publish                     Build and upload this project to PyPi                                │
+│ safety                      Run safety check against current requirements files                  │
+│ test                        Run unittests                                                        │
+│ tox                         Run tox                                                              │
+│ update                      Update "requirements*.txt" dependencies files                        │
+│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
+│                             files)                                                               │
+│ version                     Print version and exit                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+Run tests, e.g.:
+
+```bash
+~/DragonPy$ ./dev-cli.py coverage
+# or just:
+~/DragonPy$ ./dev-cli.py test
+# or with different Python versions:
+~/DragonPy$ ./dev-cli.py tox
+```
+
+
+
+
 ### TODO
 
 
 * Update 'cpu6809_html_debug.py'
 * Use bottle for http control server part
 * unimplemented OPs:
   * RESET
@@ -160,16 +159,19 @@
 
 
 ## History
 
 (Some of the points are related to [DragonPy Emulator](https://github.com/jedie/DragonPy))
 
 
-* [*dev*](https://github.com/6809/MC6809/compare/v0.7.0...main)
+* [*dev*](https://github.com/6809/MC6809/compare/v0.7.1...main)
   * TBC
+* 05.08.2023 - [v0.7.1](https://github.com/6809/MC6809/compare/v0.7.0...v0.7.1)
+  * Split CLI in a app and dev version with different venvs.
+  * Update requirements
 * 07.03.2023 - [v0.7.0](https://github.com/6809/MC6809/compare/v0.6.0...v0.7.0)
   * Replace the `Makefile` with a click CLI
   * Use pip-tools and https://github.com/jedie/manageprojects
   * Rename git `master` to `main` branch
   * Run CI tests against Python 3.9, 3.10 and 3.11
   * Replace Creole README with markdown
 * 10.02.2020 - [v0.6.0](https://github.com/6809/MC6809/compare/v0.5.0...v0.6.0)
```

### Comparing `MC6809-0.7.0rc1/README.md` & `MC6809-0.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,53 +16,32 @@
 Getting started:
 ```bash
 ~$ git clone https://github.com/6809/MC6809.git
 ~$ cd MC6809
 ~/MC6809 $ ./cli.py --help
 ```
 
-```bash
-~$ git clone https://github.com/jedie/DragonPy.git
-~$ cd DragonPy/
-~/DragonPy$ ./cli.py --help
-```
-
 The output of `./cli.py --help` looks like:
 
 [comment]: <> (✂✂✂ auto generated main help start ✂✂✂)
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ benchmark                   Run a MC6809 emulation benchmark                                     │
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ fix-code-style              Fix code style of all MC6809 source code files via darker            │
-│ install                     Run pip-sync and install 'MC6809' via pip as editable.               │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
-│ profile                     Profile the MC6809 emulation benchmark                               │
-│ publish                     Build and upload this project to PyPi                                │
-│ safety                      Run safety check against current requirements files                  │
-│ test                        Run unittests                                                        │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
-│ version                     Print version and exit                                               │
+│ benchmark            Run a MC6809 emulation benchmark                                            │
+│ profile              Profile the MC6809 emulation benchmark                                      │
+│ version              Print version and exit                                                      │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
-
-
-You can use the devshell as a CLI, too, e.g.:
 There is a simple benchmark. Run e.g.:
 ```bash
 ~/MC6809$ ./cli.py benchmark --help
 ```
 
 The output of `./cli.py benchmark --help` looks like:
 
@@ -77,25 +56,14 @@
 │ --multiply    INTEGER  est data multiplier [default: 15]                                         │
 │ --help                 Show this message and exit.                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated benchmark help end ✂✂✂)
 
 
-
-### tests
-
-```bash
-~/DragonPy$ ./cli.py coverage
-# or just:
-~/DragonPy$ ./cli.py test
-# or with different Python versions:
-~/DragonPy$ ./cli.py tox
-```
-
 ### profile
 
 You can run the Python profiler against the benchmark, e.g.:
 
 ```bash
 ~/MC6809$ ./cli.py profile --help
 ```
@@ -113,14 +81,62 @@
 │ --multiply    INTEGER  est data multiplier [default: 15]                                         │
 │ --help                 Show this message and exit.                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated profile help end ✂✂✂)
 
 
+### development
+
+For development exists `dev-cli`, e.g.:
+
+```bash
+~/MC6809$ ./dev-cli.py --help
+```
+
+The output of `./dev-cli.py --help` looks like:
+
+[comment]: <> (✂✂✂ auto generated dev help start ✂✂✂)
+```
+Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help      Show this message and exit.                                                          │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+│ check-code-style            Check code style by calling darker + flake8                          │
+│ coverage                    Run and show coverage.                                               │
+│ fix-code-style              Fix code style of all MC6809 source code files via darker            │
+│ install                     Run pip-sync and install 'MC6809' via pip as editable.               │
+│ mypy                        Run Mypy (configured in pyproject.toml)                              │
+│ publish                     Build and upload this project to PyPi                                │
+│ safety                      Run safety check against current requirements files                  │
+│ test                        Run unittests                                                        │
+│ tox                         Run tox                                                              │
+│ update                      Update "requirements*.txt" dependencies files                        │
+│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
+│                             files)                                                               │
+│ version                     Print version and exit                                               │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+Run tests, e.g.:
+
+```bash
+~/DragonPy$ ./dev-cli.py coverage
+# or just:
+~/DragonPy$ ./dev-cli.py test
+# or with different Python versions:
+~/DragonPy$ ./dev-cli.py tox
+```
+
+
+
+
 ### TODO
 
 
 * Update 'cpu6809_html_debug.py'
 * Use bottle for http control server part
 * unimplemented OPs:
   * RESET
@@ -129,16 +145,19 @@
 
 
 ## History
 
 (Some of the points are related to [DragonPy Emulator](https://github.com/jedie/DragonPy))
 
 
-* [*dev*](https://github.com/6809/MC6809/compare/v0.7.0...main)
+* [*dev*](https://github.com/6809/MC6809/compare/v0.7.1...main)
   * TBC
+* 05.08.2023 - [v0.7.1](https://github.com/6809/MC6809/compare/v0.7.0...v0.7.1)
+  * Split CLI in a app and dev version with different venvs.
+  * Update requirements
 * 07.03.2023 - [v0.7.0](https://github.com/6809/MC6809/compare/v0.6.0...v0.7.0)
   * Replace the `Makefile` with a click CLI
   * Use pip-tools and https://github.com/jedie/manageprojects
   * Rename git `master` to `main` branch
   * Run CI tests against Python 3.9, 3.10 and 3.11
   * Replace Creole README with markdown
 * 10.02.2020 - [v0.6.0](https://github.com/6809/MC6809/compare/v0.5.0...v0.6.0)
```

### Comparing `MC6809-0.7.0rc1/cli.py` & `MC6809-0.7.1/dev-cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,19 +52,19 @@
 PIP_SYNC_PATH = BIN_PATH / f'pip-sync{FILE_EXT}'
 
 DEP_LOCK_PATH = BASE_PATH / 'requirements.dev.txt'
 DEP_HASH_PATH = VENV_PATH / '.dep_hash'
 
 # script file defined in pyproject.toml as [console_scripts]
 # (Under Windows: ".exe" not added!)
-PROJECT_SHELL_SCRIPT = BIN_PATH / 'MC6809'
+PROJECT_SHELL_SCRIPT = BIN_PATH / 'MC6809_dev'
 
 
 def get_dep_hash():
-    """Get SHA512 hash from poetry.lock content."""
+    """Get SHA512 hash from lock file content."""
     return hashlib.sha512(DEP_LOCK_PATH.read_bytes()).hexdigest()
 
 
 def store_dep_hash():
     """Generate .venv/.dep_hash"""
     DEP_HASH_PATH.write_text(get_dep_hash())
 
@@ -97,15 +97,15 @@
         verbose_check_call(PYTHON_PATH, '-m', 'pip', 'install', '-U', 'pip-tools')
 
     if not PROJECT_SHELL_SCRIPT.is_file() or not venv_up2date():
         # install requirements via "pip-sync"
         verbose_check_call(PIP_SYNC_PATH, str(DEP_LOCK_PATH))
 
         # install project
-        verbose_check_call(PIP_PATH, 'install', '-e', '.')
+        verbose_check_call(PIP_PATH, 'install', '--no-deps', '-e', '.')
         store_dep_hash()
 
     # Call our entry point CLI:
     try:
         verbose_check_call(PROJECT_SHELL_SCRIPT, *sys.argv[1:])
     except subprocess.CalledProcessError as err:
         sys.exit(err.returncode)
```

### Comparing `MC6809-0.7.0rc1/pyproject.toml` & `MC6809-0.7.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,70 @@
 [project]
 name = "MC6809"
-version = "0.7.0rc1"
+dynamic = ["version"]
 description = "MC6809 CPU emulator written in Python"
+license = {text = "GPL-3.0-or-later"}
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'git@jensdiemer.de'}
 ]
-classifiers = [
-    # http://pypi.python.org/pypi?%3Aaction=list_classifiers
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Console",
-    "Environment :: MacOS X",
-    "Environment :: Win32 (MS Windows)",
-    "Environment :: X11 Applications",
-    "Environment :: Other Environment",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Education",
-    "Intended Audience :: End Users/Desktop",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-    "Topic :: System :: Emulators",
-    "Topic :: Software Development :: Assemblers",
-    "Topic :: Software Development :: Testing",
-]
 requires-python = ">=3.9,<4"
 dependencies = [
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
 ]
 [project.optional-dependencies]
 dev = [
     "manageprojects",  # https://github.com/jedie/manageprojects
     "pip-tools",  # https://github.com/jazzband/pip-tools/
     "tox",  # https://github.com/tox-dev/tox
     "coverage",  # https://github.com/nedbat/coveragepy
-    "darker>=1.7",  # https://github.com/akaihola/darker
     "autopep8",  # https://github.com/hhatto/autopep8
     "pyupgrade",  # https://github.com/asottile/pyupgrade
-    "isort",  # https://github.com/pycqa/isort
-    "flynt",  # https://github.com/ikamensh/flynt
     "flake8",  # https://github.com/pycqa/flake8
     "pyflakes",  # https://github.com/PyCQA/pyflakes
     "codespell",  # https://github.com/codespell-project/codespell
     "EditorConfig",  # https://github.com/editorconfig/editorconfig-core-py
     "safety",  # https://github.com/pyupio/safety
     "mypy",  # https://github.com/python/mypy
     "twine",  # https://github.com/pypa/twine
 
+    # https://github.com/akaihola/darker
+    # https://github.com/ikamensh/flynt
+    # https://github.com/pycqa/isort
+    # https://github.com/pygments/pygments
+    "darker[flynt, isort, color]",
+
     "tomli",  # https://github.com/hukkin/tomli
-    # tomli only needed for Python <3.11, but see bug:
-    # https://github.com/pypa/pip/issues/9644#issuecomment-1456583402
-    #"tomli;python_version<\"3.11\"",  # https://github.com/hukkin/tomli
-
-    # Work-a-round for:
-    # https://github.com/jazzband/pip-tools/issues/994#issuecomment-1321226661
-    "typing-extensions>=3.10;python_version<\"3.10\"",
+    #
+    # tomli only needed for Python <3.11, but see pip bug:
+    # https://github.com/pypa/pip/issues/9644 / https://github.com/jazzband/pip-tools/issues/1866
+    #'tomli;python_version<"3.11"',  # https://github.com/hukkin/tomli
 ]
 
 [project.urls]
 Documentation = "https://github.com/6809/MC6809"
 Source = "https://github.com/6809/MC6809"
 
 [project.scripts]
-MC6809 = "MC6809.__main__:main"
+MC6809_app = "MC6809.__main__:main"
+MC6809_dev = "MC6809.cli.dev:main"
+
+[build-system]
+requires = ["setuptools>=61.0", "setuptools_scm>=7.1"]
+build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["MC6809*"]
 
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+[tool.setuptools.dynamic]
+version = {attr = "MC6809.__version__"}
 
 
 [tool.darker]
 src = ['.']
 revision = "origin/main..."
 line_length = 119
 verbose = true
@@ -106,14 +90,15 @@
 line_length=119
 lines_after_imports=2
 
 
 [tool.coverage.run]
 branch = true
 parallel = true
+concurrency = ["multiprocessing"]
 source = ['.']
 command_line = '-m unittest --verbose --locals --buffer'
 
 [tool.coverage.report]
 omit = ['.*', '*/tests/*']
 skip_empty = true
 fail_under = 30
@@ -171,8 +156,9 @@
 package_description = "MC6809 CPU emulator written in Python"
 package_url = "https://github.com/6809/MC6809"
 issues_url = "https://github.com/6809/MC6809/issues"
 license = "GPL-3.0-or-later"
 _template = "https://github.com/jedie/cookiecutter_templates/"
 applied_migrations = [
     "04d5a25", # 2023-03-07T16:25:36+01:00
+    "da054d6", # 2023-08-04T17:39:02+02:00
 ]
```

