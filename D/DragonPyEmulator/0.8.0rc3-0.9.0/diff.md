# Comparing `tmp/DragonPyEmulator-0.8.0rc3.tar.gz` & `tmp/DragonPyEmulator-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DragonPyEmulator-0.8.0rc3.tar", last modified: Tue Mar  7 16:05:50 2023, max compression
+gzip compressed data, was "DragonPyEmulator-0.9.0.tar", last modified: Sat Aug  5 19:57:44 2023, max compression
```

## Comparing `DragonPyEmulator-0.8.0rc3.tar` & `DragonPyEmulator-0.9.0.tar`

### file list

```diff
@@ -1,103 +1,266 @@
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/bleach/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/bleach/_vendor/
--rwxrwxr-x   0 jens      (1000) jens      (1000)      453 2023-03-07 15:54:00.000000 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/bleach/_vendor/vendor_install.sh
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/virtualenv/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/virtualenv/activation/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/virtualenv/activation/bash/
--rw-rw-r--   0 jens      (1000) jens      (1000)     2179 2023-03-07 15:53:59.000000 DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/bleach/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/bleach/_vendor/
--rwxrwxr-x   0 jens      (1000) jens      (1000)      453 2023-03-07 15:54:00.000000 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/bleach/_vendor/vendor_install.sh
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/virtualenv/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/virtualenv/activation/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/virtualenv/activation/bash/
--rw-rw-r--   0 jens      (1000) jens      (1000)     2179 2023-03-07 15:53:59.000000 DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/virtualenv/activation/bash/activate.sh
--rw-rw-r--   0 jens      (1000) jens      (1000)      937 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/AUTHORS
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/BASIC examples/
--rwxrwxr-x   0 jens      (1000) jens      (1000)     2623 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/DumpBasicProgram.bas
--rw-rw-r--   0 jens      (1000) jens      (1000)      717 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/ListVariables.bas
--rw-rw-r--   0 jens      (1000) jens      (1000)       90 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/display_all_chars.bas
--rw-rw-r--   0 jens      (1000) jens      (1000)       69 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/display_all_chars_loop.bas
--rw-rw-r--   0 jens      (1000) jens      (1000)     1448 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/hex_view01.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     4237 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/hustle.c10.bas
--rw-rw-r--   0 jens      (1000) jens      (1000)      494 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/mandelbrot1.bas
--rw-rw-r--   0 jens      (1000) jens      (1000)      707 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/mandelbrot2.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)       44 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/print_all_chars.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)       58 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/print_all_chars_loop.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)      105 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC examples/print_timer.bas
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/BASIC games/
--rwxrwxr-x   0 jens      (1000) jens      (1000)     6239 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC games/INVADER.bas
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/BASIC tools/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/BASIC tools/FloatingPoint/
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1601 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/FloatingPoint/test_FPA0.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1878 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/FloatingPoint/test_FPA0_02.bas
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/BASIC tools/HexViewer/
--rw-rw-r--   0 jens      (1000) jens      (1000)      231 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/HexViewer/README.creole
--rw-rw-r--   0 jens      (1000) jens      (1000)     1205 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/HexViewer/hex_view01.bas
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/BASIC tools/InputOutput/
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1220 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/InputOutput/keyboard.bas
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/
--rwxrwxr-x   0 jens      (1000) jens      (1000)     7660 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/README.creole
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1779 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1936 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_ADDA.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1872 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_DEC.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1872 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_INC.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1938 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_LSL.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1908 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_NEGA.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1935 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_SUBA.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)     1791 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_TST.bas
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/
--rw-rw-r--   0 jens      (1000) jens      (1000)    28477 2023-03-07 16:05:50.000000 DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) jens      (1000)     2200 2023-03-07 16:05:50.000000 DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)        1 2023-03-07 16:05:50.000000 DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)       52 2023-03-07 16:05:50.000000 DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)      286 2023-03-07 16:05:50.000000 DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)       27 2023-03-07 16:05:50.000000 DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)    35121 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/LICENSE
--rw-rw-r--   0 jens      (1000) jens      (1000)      296 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/MANIFEST.in
--rw-rw-r--   0 jens      (1000) jens      (1000)    28477 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/PKG-INFO
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/PyDC/
--rwxrwxr-x   0 jens      (1000) jens      (1000)     5031 2023-03-07 15:39:59.000000 DragonPyEmulator-0.8.0rc3/PyDC/PyDC_cli.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     5166 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/PyDC/README.creole
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.918342 DragonPyEmulator-0.8.0rc3/PyDC/test_files/
--rwxrwxr-x   0 jens      (1000) jens      (1000)       54 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/PyDC/test_files/HelloWorld1.bas
--rwxrwxr-x   0 jens      (1000) jens      (1000)      128 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/PyDC/test_files/LineNumberTest.bas
--rw-rw-r--   0 jens      (1000) jens      (1000)    27096 2023-03-07 15:49:58.000000 DragonPyEmulator-0.8.0rc3/README.md
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/basic_editor/
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/basic_editor/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)    11100 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/basic_editor/editor.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      611 2023-03-07 14:53:57.000000 DragonPyEmulator-0.8.0rc3/basic_editor/editor_base.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     5817 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/basic_editor/highlighting.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3610 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/basic_editor/scrolled_text.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      981 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/basic_editor/status_bar.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      584 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/basic_editor/tkinter_utils.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     4296 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/basic_editor/token_window.py
--rwxrwxr-x   0 jens      (1000) jens      (1000)     3034 2023-03-06 19:58:04.000000 DragonPyEmulator-0.8.0rc3/cli.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/dragonpy/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/dragonpy/Dragon64/
--rwxrwxr-x   0 jens      (1000) jens      (1000)   158695 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/dragonpy/Dragon64/dasm_asm_d64_rom.sh
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/dragonpy/Multicomp6809/
--rwxrwxr-x   0 jens      (1000) jens      (1000)      761 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/dragonpy/Multicomp6809/README.creole
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/dragonpy/Simple6809/
--rwxrwxr-x   0 jens      (1000) jens      (1000)      554 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/dragonpy/Simple6809/README.creole
--rw-rw-r--   0 jens      (1000) jens      (1000)     1521 2023-03-07 15:54:36.000000 DragonPyEmulator-0.8.0rc3/dragonpy/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      186 2023-03-06 19:20:05.000000 DragonPyEmulator-0.8.0rc3/dragonpy/__main__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      945 2023-03-07 15:31:45.000000 DragonPyEmulator-0.8.0rc3/dragonpy/constants.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/dragonpy/sbc09/
--rw-rw-r--   0 jens      (1000) jens      (1000)     2167 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/dragonpy/sbc09/README.creole
--rwxrwxr-x   0 jens      (1000) jens      (1000)    29929 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/dragonpy/sbc09/sbc09.creole
--rw-rw-r--   0 jens      (1000) jens      (1000)    32768 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/dragonpy/sbc09/v09.rom
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/dragonpy/vectrex/
--rw-rw-r--   0 jens      (1000) jens      (1000)     8192 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/dragonpy/vectrex/SYSTEM.IMG
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/misc/
--rw-rw-r--   0 jens      (1000) jens      (1000)    11745 2023-03-06 18:48:22.000000 DragonPyEmulator-0.8.0rc3/misc/README.creole
--rw-rw-r--   0 jens      (1000) jens      (1000)     5658 2023-03-07 16:03:26.000000 DragonPyEmulator-0.8.0rc3/pyproject.toml
--rw-rw-r--   0 jens      (1000) jens      (1000)       38 2023-03-07 16:05:50.922342 DragonPyEmulator-0.8.0rc3/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.127739 DragonPyEmulator-0.9.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1929 2023-08-05 19:50:00.000000 DragonPyEmulator-0.9.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      133 2023-08-05 18:21:43.000000 DragonPyEmulator-0.9.0/.gitignore
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.tox/py310/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.tox/py310/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/bleach/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/bleach/_vendor/
+-rwxrwxr-x   0 jens      (1000) users      (100)      453 2023-08-05 19:46:28.000000 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/bleach/_vendor/vendor_install.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.115739 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-08-05 19:46:27.000000 DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/bleach/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/bleach/_vendor/
+-rwxrwxr-x   0 jens      (1000) users      (100)      453 2023-08-05 19:46:08.000000 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/bleach/_vendor/vendor_install.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-08-05 19:46:07.000000 DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/bleach/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/bleach/_vendor/
+-rwxrwxr-x   0 jens      (1000) users      (100)      453 2023-08-05 19:46:50.000000 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/bleach/_vendor/vendor_install.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-08-05 19:46:49.000000 DragonPyEmulator-0.9.0/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/python3.10/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/bleach/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/bleach/_vendor/
+-rwxrwxr-x   0 jens      (1000) users      (100)      453 2023-03-07 15:54:00.000000 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/bleach/_vendor/vendor_install.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-08-05 18:37:20.000000 DragonPyEmulator-0.9.0/.venv/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/bleach/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/bleach/_vendor/
+-rwxrwxr-x   0 jens      (1000) users      (100)      453 2023-03-07 15:54:00.000000 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/bleach/_vendor/vendor_install.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-08-05 18:37:20.000000 DragonPyEmulator-0.9.0/.venv/lib64/python3.10/site-packages/virtualenv/activation/bash/activate.sh
+-rw-rw-r--   0 jens      (1000) users      (100)      937 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/AUTHORS
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/BASIC examples/
+-rwxrwxr-x   0 jens      (1000) users      (100)     2623 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/DumpBasicProgram.bas
+-rw-rw-r--   0 jens      (1000) users      (100)      717 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/ListVariables.bas
+-rw-rw-r--   0 jens      (1000) users      (100)       90 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/display_all_chars.bas
+-rw-rw-r--   0 jens      (1000) users      (100)       69 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/display_all_chars_loop.bas
+-rw-rw-r--   0 jens      (1000) users      (100)     1448 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/hex_view01.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     4237 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/hustle.c10.bas
+-rw-rw-r--   0 jens      (1000) users      (100)      494 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/mandelbrot1.bas
+-rw-rw-r--   0 jens      (1000) users      (100)      707 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/mandelbrot2.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)       44 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/print_all_chars.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)       58 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/print_all_chars_loop.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)      105 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC examples/print_timer.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/BASIC games/
+-rwxrwxr-x   0 jens      (1000) users      (100)     6239 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC games/INVADER.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/BASIC tools/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/BASIC tools/FloatingPoint/
+-rwxrwxr-x   0 jens      (1000) users      (100)     1601 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/FloatingPoint/test_FPA0.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1878 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/FloatingPoint/test_FPA0_02.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/BASIC tools/HexViewer/
+-rw-rw-r--   0 jens      (1000) users      (100)      231 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/HexViewer/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)     1205 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/HexViewer/hex_view01.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/BASIC tools/InputOutput/
+-rwxrwxr-x   0 jens      (1000) users      (100)     1220 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/InputOutput/keyboard.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/
+-rwxrwxr-x   0 jens      (1000) users      (100)     7660 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/README.creole
+-rwxrwxr-x   0 jens      (1000) users      (100)     1779 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1936 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_ADDA.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1872 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_DEC.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1872 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_INC.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1938 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_LSL.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1908 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_NEGA.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1935 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_SUBA.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1791 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_TST.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    29866 2023-08-05 19:57:42.000000 DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     6180 2023-08-05 19:57:44.000000 DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-08-05 19:57:42.000000 DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-08-05 19:57:42.000000 DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      213 2023-08-05 19:57:42.000000 DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       27 2023-08-05 19:57:42.000000 DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    35121 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/LICENSE
+-rw-rw-r--   0 jens      (1000) users      (100)      296 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/MANIFEST.in
+-rw-rw-r--   0 jens      (1000) users      (100)    29866 2023-08-05 19:57:44.127739 DragonPyEmulator-0.9.0/PKG-INFO
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/PyDC/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.119739 DragonPyEmulator-0.9.0/PyDC/PyDC/
+-rw-rw-r--   0 jens      (1000) users      (100)    26714 2023-03-07 15:38:05.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/CassetteObjects.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2999 2023-03-07 15:37:28.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3590 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/base_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3698 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/basic_tokens.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    11975 2023-03-07 15:38:27.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/bitstream_handler.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4858 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/configs.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    11290 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/tests.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    21278 2023-03-07 15:40:41.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)    23319 2023-03-07 15:37:50.000000 DragonPyEmulator-0.9.0/PyDC/PyDC/wave2bitstream.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     5031 2023-03-07 17:23:27.000000 DragonPyEmulator-0.9.0/PyDC/PyDC_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5166 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/README.creole
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/PyDC/test_files/
+-rwxrwxr-x   0 jens      (1000) users      (100)   225708 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/test_files/HelloWorld1 origin.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)    82204 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/test_files/HelloWorld1 xroar.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)       54 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/test_files/HelloWorld1.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)   264236 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/test_files/LineNumber Test 01.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)   401452 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/test_files/LineNumber Test 02.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)      128 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/PyDC/test_files/LineNumberTest.bas
+-rw-rw-r--   0 jens      (1000) users      (100)    29341 2023-08-05 19:53:35.000000 DragonPyEmulator-0.9.0/README.md
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/basic_editor/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/basic_editor/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    11100 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/basic_editor/editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)      611 2023-03-07 14:53:57.000000 DragonPyEmulator-0.9.0/basic_editor/editor_base.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5817 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/basic_editor/highlighting.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3610 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/basic_editor/scrolled_text.py
+-rw-rw-r--   0 jens      (1000) users      (100)      981 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/basic_editor/status_bar.py
+-rw-rw-r--   0 jens      (1000) users      (100)      584 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/basic_editor/tkinter_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4296 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/basic_editor/token_window.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3049 2023-08-05 18:21:05.000000 DragonPyEmulator-0.9.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3049 2023-08-05 18:21:05.000000 DragonPyEmulator-0.9.0/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/CoCo/
+-rw-rw-r--   0 jens      (1000) users      (100)      918 2023-03-07 14:18:17.000000 DragonPyEmulator-0.9.0/dragonpy/CoCo/CoCo2b_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/CoCo/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3796 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/CoCo/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      684 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/CoCo/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1828 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/CoCo/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1771 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/CoCo/periphery_coco.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/Dragon32/
+-rw-rw-r--   0 jens      (1000) users      (100)     1086 2023-03-07 06:59:50.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/Dragon32_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)    17337 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/MC6821_PIA.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4015 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/MC6847.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8435 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/MC6883_SAM.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      975 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/cassette.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5287 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7255 2023-03-06 19:37:02.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/dragon_charmap.py
+-rw-rw-r--   0 jens      (1000) users      (100)    30337 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/dragon_font.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10791 2023-03-06 19:37:02.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/gui_config.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    11074 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/keyboard_map.py
+-rw-rw-r--   0 jens      (1000) users      (100)      791 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)    46500 2023-03-06 19:35:33.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5407 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/periphery_dragon.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1517 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon32/speaker.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/Dragon64/
+-rwxrwxr-x   0 jens      (1000) users      (100)     2755 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/6809dasm_comments.py
+-rw-rw-r--   0 jens      (1000) users      (100)   138378 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/Dragon 64 in 32 mode.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1555 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/Dragon64_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2105 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      765 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/create_mem_info.py
+-rwxrwxr-x   0 jens      (1000) users      (100)   158695 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/dasm_asm_d64_rom.sh
+-rw-rw-r--   0 jens      (1000) users      (100)      708 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)   193693 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Dragon64/mem_info.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/
+-rw-rw-r--   0 jens      (1000) users      (100)     1876 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/Multicomp6809_rom.py
+-rwxrwxr-x   0 jens      (1000) users      (100)      761 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2017 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      443 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)      773 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2759 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/periphery_Multicomp6809.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/Simple6809/
+-rwxrwxr-x   0 jens      (1000) users      (100)      232 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/Grant's 6809 computer.URL
+-rwxrwxr-x   0 jens      (1000) users      (100)      554 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)     2003 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/Simple6809_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/__init__.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     1547 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/asm_lst2py_unittest.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2490 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      741 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/machine.py
+-rwxrwxr-x   0 jens      (1000) users      (100)      923 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/make_mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)   233609 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3281 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/periphery_simple6809.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2365 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/Simple6809/reformat_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1470 2023-08-05 19:50:00.000000 DragonPyEmulator-0.9.0/dragonpy/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.0/dragonpy/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.0/dragonpy/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5899 2023-08-05 18:31:25.000000 DragonPyEmulator-0.9.0/dragonpy/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-08-05 19:56:56.000000 DragonPyEmulator-0.9.0/dragonpy/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/components/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/components/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    13109 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/components/memory.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9857 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/components/periphery.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6073 2023-03-07 07:18:07.000000 DragonPyEmulator-0.9.0/dragonpy/components/rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)      942 2023-08-05 18:32:10.000000 DragonPyEmulator-0.9.0/dragonpy/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/core/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/core/__init__.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     1988 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/core/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3735 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/core/configs.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    16429 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/core/gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7721 2023-03-07 14:56:34.000000 DragonPyEmulator-0.9.0/dragonpy/core/gui_starter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6447 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/core/machine.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.123739 DragonPyEmulator-0.9.0/dragonpy/sbc09/
+-rw-rw-r--   0 jens      (1000) users      (100)     2167 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1676 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5818 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/create_trace.py
+-rw-rw-r--   0 jens      (1000) users      (100)      439 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)      687 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/machine.py
+-rwxrwxr-x   0 jens      (1000) users      (100)   142429 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/make_mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)    28291 2023-03-06 19:35:23.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4174 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/periphery.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    29929 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/sbc09.creole
+-rw-rw-r--   0 jens      (1000) users      (100)      712 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/sbc09_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)    32768 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/sbc09/v09.rom
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.127739 DragonPyEmulator-0.9.0/dragonpy/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      150 2023-08-05 18:21:05.000000 DragonPyEmulator-0.9.0/dragonpy/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1324 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/tests/project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3241 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_BASIC_Dragon32.py
+-rw-rw-r--   0 jens      (1000) users      (100)    25042 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_BASIC_simple09.py
+-rw-rw-r--   0 jens      (1000) users      (100)    15796 2023-03-07 16:21:59.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_base.py
+-rw-rw-r--   0 jens      (1000) users      (100)      749 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      280 2023-08-05 18:32:27.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2558 2023-08-05 18:21:05.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2148 2023-08-05 19:45:06.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1601 2023-03-07 16:22:09.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_rom_download.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6708 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/tests/test_sbc09.py
+-rw-rw-r--   0 jens      (1000) users      (100)      402 2023-03-07 15:36:28.000000 DragonPyEmulator-0.9.0/dragonpy/tests/utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.127739 DragonPyEmulator-0.9.0/dragonpy/utils/
+-rw-rw-r--   0 jens      (1000) users      (100)     4104 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/BASIC09_floating_point.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3214 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/bits.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1271 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/disable_logging.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     2321 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/hex2bin.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2341 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/humanize.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    17555 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/pager.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2107 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/simple_debugger.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     5553 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/utils/srecord_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.127739 DragonPyEmulator-0.9.0/dragonpy/vectrex/
+-rwxrwxr-x   0 jens      (1000) users      (100)    10241 2023-03-06 19:37:43.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/MOS6522.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8192 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/SYSTEM.IMG
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1746 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      750 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2429 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1725 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/periphery.py
+-rw-rw-r--   0 jens      (1000) users      (100)      367 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/vectrex_gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)      717 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/dragonpy/vectrex/vectrex_rom.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-05 19:57:44.127739 DragonPyEmulator-0.9.0/misc/
+-rw-rw-r--   0 jens      (1000) users      (100)    11745 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/misc/README.creole
+-rwxrwxr-x   0 jens      (1000) users      (100)     5407 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/misc/add_info_in_trace.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    10558 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/misc/filter_xroar_trace.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2196 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.0/misc/xroar_gdb_tests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4933 2023-08-05 19:50:00.000000 DragonPyEmulator-0.9.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    51703 2023-08-05 19:39:19.000000 DragonPyEmulator-0.9.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    19753 2023-08-05 19:39:02.000000 DragonPyEmulator-0.9.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-08-05 19:57:44.127739 DragonPyEmulator-0.9.0/setup.cfg
```

### Comparing `DragonPyEmulator-0.8.0rc3/.venv/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh` & `DragonPyEmulator-0.9.0/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh`

 * *Files 23% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     if ! [ -z "${_OLD_VIRTUAL_PS1+_}" ] ; then
         PS1="$_OLD_VIRTUAL_PS1"
         export PS1
         unset _OLD_VIRTUAL_PS1
     fi
 
     unset VIRTUAL_ENV
+    unset VIRTUAL_ENV_PROMPT
     if [ ! "${1-}" = "nondestructive" ] ; then
     # Self destruct!
         unset -f deactivate
     fi
 }
 
 # unset irrelevant variables
@@ -50,27 +51,30 @@
 fi
 export VIRTUAL_ENV
 
 _OLD_VIRTUAL_PATH="$PATH"
 PATH="$VIRTUAL_ENV/__BIN_NAME__:$PATH"
 export PATH
 
+if [ "x__VIRTUAL_PROMPT__" != x ] ; then
+    VIRTUAL_ENV_PROMPT="__VIRTUAL_PROMPT__"
+else
+    VIRTUAL_ENV_PROMPT=$(basename "$VIRTUAL_ENV")
+fi
+export VIRTUAL_ENV_PROMPT
+
 # unset PYTHONHOME if set
 if ! [ -z "${PYTHONHOME+_}" ] ; then
     _OLD_VIRTUAL_PYTHONHOME="$PYTHONHOME"
     unset PYTHONHOME
 fi
 
 if [ -z "${VIRTUAL_ENV_DISABLE_PROMPT-}" ] ; then
     _OLD_VIRTUAL_PS1="${PS1-}"
-    if [ "x__VIRTUAL_PROMPT__" != x ] ; then
-        PS1="(__VIRTUAL_PROMPT__) ${PS1-}"
-    else
-        PS1="(`basename \"$VIRTUAL_ENV\"`) ${PS1-}"
-    fi
+    PS1="(${VIRTUAL_ENV_PROMPT}) ${PS1-}"
     export PS1
 fi
 
 # Make sure to unalias pydoc if it's already there
 alias pydoc 2>/dev/null >/dev/null && unalias pydoc || true
 
 pydoc () {
```

### Comparing `DragonPyEmulator-0.8.0rc3/.venv/lib64/python3.10/site-packages/virtualenv/activation/bash/activate.sh` & `DragonPyEmulator-0.9.0/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh`

 * *Files 23% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     if ! [ -z "${_OLD_VIRTUAL_PS1+_}" ] ; then
         PS1="$_OLD_VIRTUAL_PS1"
         export PS1
         unset _OLD_VIRTUAL_PS1
     fi
 
     unset VIRTUAL_ENV
+    unset VIRTUAL_ENV_PROMPT
     if [ ! "${1-}" = "nondestructive" ] ; then
     # Self destruct!
         unset -f deactivate
     fi
 }
 
 # unset irrelevant variables
@@ -50,27 +51,30 @@
 fi
 export VIRTUAL_ENV
 
 _OLD_VIRTUAL_PATH="$PATH"
 PATH="$VIRTUAL_ENV/__BIN_NAME__:$PATH"
 export PATH
 
+if [ "x__VIRTUAL_PROMPT__" != x ] ; then
+    VIRTUAL_ENV_PROMPT="__VIRTUAL_PROMPT__"
+else
+    VIRTUAL_ENV_PROMPT=$(basename "$VIRTUAL_ENV")
+fi
+export VIRTUAL_ENV_PROMPT
+
 # unset PYTHONHOME if set
 if ! [ -z "${PYTHONHOME+_}" ] ; then
     _OLD_VIRTUAL_PYTHONHOME="$PYTHONHOME"
     unset PYTHONHOME
 fi
 
 if [ -z "${VIRTUAL_ENV_DISABLE_PROMPT-}" ] ; then
     _OLD_VIRTUAL_PS1="${PS1-}"
-    if [ "x__VIRTUAL_PROMPT__" != x ] ; then
-        PS1="(__VIRTUAL_PROMPT__) ${PS1-}"
-    else
-        PS1="(`basename \"$VIRTUAL_ENV\"`) ${PS1-}"
-    fi
+    PS1="(${VIRTUAL_ENV_PROMPT}) ${PS1-}"
     export PS1
 fi
 
 # Make sure to unalias pydoc if it's already there
 alias pydoc 2>/dev/null >/dev/null && unalias pydoc || true
 
 pydoc () {
```

### Comparing `DragonPyEmulator-0.8.0rc3/AUTHORS` & `DragonPyEmulator-0.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC examples/DumpBasicProgram.bas` & `DragonPyEmulator-0.9.0/BASIC examples/DumpBasicProgram.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC examples/ListVariables.bas` & `DragonPyEmulator-0.9.0/BASIC examples/ListVariables.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC examples/hex_view01.bas` & `DragonPyEmulator-0.9.0/BASIC examples/hex_view01.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC examples/hustle.c10.bas` & `DragonPyEmulator-0.9.0/BASIC examples/hustle.c10.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC examples/mandelbrot2.bas` & `DragonPyEmulator-0.9.0/BASIC examples/mandelbrot2.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC games/INVADER.bas` & `DragonPyEmulator-0.9.0/BASIC games/INVADER.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/FloatingPoint/test_FPA0.bas` & `DragonPyEmulator-0.9.0/BASIC tools/FloatingPoint/test_FPA0.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/FloatingPoint/test_FPA0_02.bas` & `DragonPyEmulator-0.9.0/BASIC tools/FloatingPoint/test_FPA0_02.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/HexViewer/hex_view01.bas` & `DragonPyEmulator-0.9.0/BASIC tools/HexViewer/hex_view01.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/InputOutput/keyboard.bas` & `DragonPyEmulator-0.9.0/BASIC tools/InputOutput/keyboard.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/README.creole` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_ADDA.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_ADDA.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_DEC.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_DEC.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_INC.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_INC.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_LSL.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_LSL.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_NEGA.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_NEGA.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_SUBA.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_SUBA.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/BASIC tools/TestCC_Registers/testCC_TST.bas` & `DragonPyEmulator-0.9.0/BASIC tools/TestCC_Registers/testCC_TST.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/DragonPyEmulator.egg-info/PKG-INFO` & `DragonPyEmulator-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,18 @@
-Metadata-Version: 2.1
-Name: DragonPyEmulator
-Version: 0.8.0rc3
-Summary: Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python...
-Author-email: Jens Diemer <git@jensdiemer.de>
-Project-URL: Documentation, https://github.com/jedie/DragonPy
-Project-URL: Source, https://github.com/jedie/DragonPy
-Keywords: Emulator,6809,Dragon,CoCo,Vectrex,tkinter,pypy
-Classifier: Development Status :: 5 - Production/Stable
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
-Requires-Python: <4,>=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-License-File: AUTHORS
-
 ## Dragon/CoCO emulator written in Python
 
 DragonPy is a Open source (GPL v3 or later) emulator for the old (1981) homecomputer `Dragon 32` and `Tandy TRS-80 Color Computer` (CoCo)...
 
 The [MC6809](https://github.com/6809/MC6809) project is used to emulate the 6809 CPU.
 
 [![tests](https://github.com/jedie/DragonPy/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/DragonPy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/dragonpy/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/dragonpy)
-[![dragonpy @ PyPi](https://img.shields.io/pypi/v/dragonpy?label=dragonpy%20%40%20PyPi)](https://pypi.org/project/dragonpy/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/dragonpy)](https://github.com/jedie/DragonPy/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/dragonpy)](https://github.com/jedie/DragonPy/blob/main/LICENSE)
+[![dragonpy @ PyPi](https://img.shields.io/pypi/v/DragonPyEmulator?label=dragonpy%20%40%20PyPi)](https://pypi.org/project/DragonPyEmulator/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/DragonPyEmulator)](https://github.com/jedie/DragonPy/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/DragonPyEmulator)](https://github.com/jedie/DragonPy/blob/main/LICENSE)
 
 
 Dragon 32 with CPython 3 under Linux:
 
 ![screenshot Dragon 32](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DragonPy/20150820_DragonPy_Dragon32_CPython3_Linux_01.png "screenshot Dragon 32")
 
 Tandy TRS-80 Color Computer 2b with CPython 2 under Windows:
@@ -133,32 +102,20 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ download-roms               Download/Test only ROM files                                         │
-│ editor                      Run only the BASIC editor                                            │
-│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
-│ gui                         Start the DragonPy tkinter starter GUI                               │
-│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
-│ log-list                    List all exiting loggers and exit.                                   │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
-│ publish                     Build and upload this project to PyPi                                │
-│ run                         Run a machine emulation                                              │
-│ safety                      Run safety check against current requirements files                  │
-│ test                        Run unittests                                                        │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
-│ version                     Print version and exit                                               │
+│ download-roms              Download/Test only ROM files                                          │
+│ editor                     Run only the BASIC editor                                             │
+│ gui                        Start the DragonPy tkinter starter GUI                                │
+│ log-list                   List all exiting loggers and exit.                                    │
+│ run                        Run a machine emulation                                               │
+│ version                    Print version and exit                                                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 The output of `./cli.py run --help` looks like:
 
@@ -205,24 +162,53 @@
 | Simple6809     | [http://searle.x10host.com/6809/Simple6809.html](http://searle.x10host.com/6809/Simple6809.html)                                                                                                                               |
 
 `sbc09` and `Vectrex` ROMs are included.
 
 All ROM files and download will be checked by `SHA1` value, before use.
 
 
-## run tests
+## development
 
-e.g.:
+Please use `dev-cli.py` for development.
 
-```bash
-~/DragonPy$ ./devshell.py pytest
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
+│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
+│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
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
 ```
-or
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+Run tests, e.g.:
+
 ```bash
-~/DragonPy$ ./devshell.py tox
+~/DragonPy$ ./dev-cli.py coverage
+# or just:
+~/DragonPy$ ./dev-cli.py test
+# or with different Python versions:
+~/DragonPy$ ./dev-cli.py tox
 ```
 
 ## more screenshots
 
 "sbc09" ROM in Tkinter window:
 
 ![screenshot sbc09](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DragonPy/DragonPy_sbc09_01.png "screenshot sbc09")
@@ -460,17 +446,27 @@
 * [pypi.org/project/Pygments](https://pypi.org/project/Pygments)
 * [http://pygments.org/](http://pygments.org/)
 * License: BSD License
 
 ## History
 
 
-* [*dev*](https://github.com/jedie/DragonPy/compare/v0.7.0...master):
-  * Replace Creole README with markdown.
+* [*dev*](https://github.com/jedie/DragonPy/compare/v0.9.0...master):
   * tbc
+* [07.03.2023 - v0.9.0](https://github.com/jedie/DragonPy/compare/v0.8.0...v0.9.0):
+  * Split CLI in app and dev
+  * Remove Python 3.9 support
+  * Update requirements
+* [07.03.2023 - v0.8.0](https://github.com/jedie/DragonPy/compare/v0.7.0...v0.8.0):
+  * Modernize project testing, CI pipeline, etc.
+  * Switch from poetry to pip-tools
+  * Replace devshell with click CLI
+  * Use https://github.com/jedie/manageprojects
+  * Min. Python Version is now v3.10
+  * Add BASIC examples `mandelbrot1.bas` and `mandelbrot2.bas` ;)
 * [01.10.2020 - v0.7.0](https://github.com/jedie/DragonPy/compare/v0.6.0...v0.7.0):
   * Modernize project testing, CI pipeline, usw poetry etc.
   * Many Code updates
   * Remove Python v2 fallback code parts
   * Update ROM Download Links
   * Bugfix "--max_ops" cli options
 * [19.06.2018 - v0.6.0](https://github.com/jedie/DragonPy/compare/v0.5.3...v0.6.0):
```

### Comparing `DragonPyEmulator-0.8.0rc3/LICENSE` & `DragonPyEmulator-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/PKG-INFO` & `DragonPyEmulator-0.9.0/DragonPyEmulator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 Metadata-Version: 2.1
 Name: DragonPyEmulator
-Version: 0.8.0rc3
+Version: 0.9.0
 Summary: Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python...
 Author-email: Jens Diemer <git@jensdiemer.de>
+License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/DragonPy
 Project-URL: Source, https://github.com/jedie/DragonPy
 Keywords: Emulator,6809,Dragon,CoCo,Vectrex,tkinter,pypy
-Classifier: Development Status :: 5 - Production/Stable
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
-Requires-Python: <4,>=3.9
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
 ## Dragon/CoCO emulator written in Python
 
 DragonPy is a Open source (GPL v3 or later) emulator for the old (1981) homecomputer `Dragon 32` and `Tandy TRS-80 Color Computer` (CoCo)...
 
 The [MC6809](https://github.com/6809/MC6809) project is used to emulate the 6809 CPU.
 
 [![tests](https://github.com/jedie/DragonPy/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/DragonPy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/dragonpy/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/dragonpy)
-[![dragonpy @ PyPi](https://img.shields.io/pypi/v/dragonpy?label=dragonpy%20%40%20PyPi)](https://pypi.org/project/dragonpy/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/dragonpy)](https://github.com/jedie/DragonPy/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/dragonpy)](https://github.com/jedie/DragonPy/blob/main/LICENSE)
+[![dragonpy @ PyPi](https://img.shields.io/pypi/v/DragonPyEmulator?label=dragonpy%20%40%20PyPi)](https://pypi.org/project/DragonPyEmulator/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/DragonPyEmulator)](https://github.com/jedie/DragonPy/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/DragonPyEmulator)](https://github.com/jedie/DragonPy/blob/main/LICENSE)
 
 
 Dragon 32 with CPython 3 under Linux:
 
 ![screenshot Dragon 32](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DragonPy/20150820_DragonPy_Dragon32_CPython3_Linux_01.png "screenshot Dragon 32")
 
 Tandy TRS-80 Color Computer 2b with CPython 2 under Windows:
@@ -133,32 +117,20 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ download-roms               Download/Test only ROM files                                         │
-│ editor                      Run only the BASIC editor                                            │
-│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
-│ gui                         Start the DragonPy tkinter starter GUI                               │
-│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
-│ log-list                    List all exiting loggers and exit.                                   │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
-│ publish                     Build and upload this project to PyPi                                │
-│ run                         Run a machine emulation                                              │
-│ safety                      Run safety check against current requirements files                  │
-│ test                        Run unittests                                                        │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
-│ version                     Print version and exit                                               │
+│ download-roms              Download/Test only ROM files                                          │
+│ editor                     Run only the BASIC editor                                             │
+│ gui                        Start the DragonPy tkinter starter GUI                                │
+│ log-list                   List all exiting loggers and exit.                                    │
+│ run                        Run a machine emulation                                               │
+│ version                    Print version and exit                                                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 The output of `./cli.py run --help` looks like:
 
@@ -205,24 +177,53 @@
 | Simple6809     | [http://searle.x10host.com/6809/Simple6809.html](http://searle.x10host.com/6809/Simple6809.html)                                                                                                                               |
 
 `sbc09` and `Vectrex` ROMs are included.
 
 All ROM files and download will be checked by `SHA1` value, before use.
 
 
-## run tests
+## development
 
-e.g.:
+Please use `dev-cli.py` for development.
 
-```bash
-~/DragonPy$ ./devshell.py pytest
+The output of `./dev-cli.py --help` looks like:
+
+[comment]: <> (✂✂✂ auto generated dev help start ✂✂✂)
 ```
-or
+Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help      Show this message and exit.                                                          │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+│ check-code-style            Check code style by calling darker + flake8                          │
+│ coverage                    Run and show coverage.                                               │
+│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
+│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
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
 ```bash
-~/DragonPy$ ./devshell.py tox
+~/DragonPy$ ./dev-cli.py coverage
+# or just:
+~/DragonPy$ ./dev-cli.py test
+# or with different Python versions:
+~/DragonPy$ ./dev-cli.py tox
 ```
 
 ## more screenshots
 
 "sbc09" ROM in Tkinter window:
 
 ![screenshot sbc09](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DragonPy/DragonPy_sbc09_01.png "screenshot sbc09")
@@ -460,17 +461,27 @@
 * [pypi.org/project/Pygments](https://pypi.org/project/Pygments)
 * [http://pygments.org/](http://pygments.org/)
 * License: BSD License
 
 ## History
 
 
-* [*dev*](https://github.com/jedie/DragonPy/compare/v0.7.0...master):
-  * Replace Creole README with markdown.
+* [*dev*](https://github.com/jedie/DragonPy/compare/v0.9.0...master):
   * tbc
+* [07.03.2023 - v0.9.0](https://github.com/jedie/DragonPy/compare/v0.8.0...v0.9.0):
+  * Split CLI in app and dev
+  * Remove Python 3.9 support
+  * Update requirements
+* [07.03.2023 - v0.8.0](https://github.com/jedie/DragonPy/compare/v0.7.0...v0.8.0):
+  * Modernize project testing, CI pipeline, etc.
+  * Switch from poetry to pip-tools
+  * Replace devshell with click CLI
+  * Use https://github.com/jedie/manageprojects
+  * Min. Python Version is now v3.10
+  * Add BASIC examples `mandelbrot1.bas` and `mandelbrot2.bas` ;)
 * [01.10.2020 - v0.7.0](https://github.com/jedie/DragonPy/compare/v0.6.0...v0.7.0):
   * Modernize project testing, CI pipeline, usw poetry etc.
   * Many Code updates
   * Remove Python v2 fallback code parts
   * Update ROM Download Links
   * Bugfix "--max_ops" cli options
 * [19.06.2018 - v0.6.0](https://github.com/jedie/DragonPy/compare/v0.5.3...v0.6.0):
```

### Comparing `DragonPyEmulator-0.8.0rc3/PyDC/PyDC_cli.py` & `DragonPyEmulator-0.9.0/PyDC/PyDC_cli.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/PyDC/README.creole` & `DragonPyEmulator-0.9.0/PyDC/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/README.md` & `DragonPyEmulator-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,33 @@
+Metadata-Version: 2.1
+Name: DragonPyEmulator
+Version: 0.9.0
+Summary: Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python...
+Author-email: Jens Diemer <git@jensdiemer.de>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://github.com/jedie/DragonPy
+Project-URL: Source, https://github.com/jedie/DragonPy
+Keywords: Emulator,6809,Dragon,CoCo,Vectrex,tkinter,pypy
+Requires-Python: <4,>=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS
+
 ## Dragon/CoCO emulator written in Python
 
 DragonPy is a Open source (GPL v3 or later) emulator for the old (1981) homecomputer `Dragon 32` and `Tandy TRS-80 Color Computer` (CoCo)...
 
 The [MC6809](https://github.com/6809/MC6809) project is used to emulate the 6809 CPU.
 
 [![tests](https://github.com/jedie/DragonPy/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/DragonPy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/dragonpy/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/dragonpy)
-[![dragonpy @ PyPi](https://img.shields.io/pypi/v/dragonpy?label=dragonpy%20%40%20PyPi)](https://pypi.org/project/dragonpy/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/dragonpy)](https://github.com/jedie/DragonPy/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/dragonpy)](https://github.com/jedie/DragonPy/blob/main/LICENSE)
+[![dragonpy @ PyPi](https://img.shields.io/pypi/v/DragonPyEmulator?label=dragonpy%20%40%20PyPi)](https://pypi.org/project/DragonPyEmulator/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/DragonPyEmulator)](https://github.com/jedie/DragonPy/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/DragonPyEmulator)](https://github.com/jedie/DragonPy/blob/main/LICENSE)
 
 
 Dragon 32 with CPython 3 under Linux:
 
 ![screenshot Dragon 32](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DragonPy/20150820_DragonPy_Dragon32_CPython3_Linux_01.png "screenshot Dragon 32")
 
 Tandy TRS-80 Color Computer 2b with CPython 2 under Windows:
@@ -102,32 +117,20 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ download-roms               Download/Test only ROM files                                         │
-│ editor                      Run only the BASIC editor                                            │
-│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
-│ gui                         Start the DragonPy tkinter starter GUI                               │
-│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
-│ log-list                    List all exiting loggers and exit.                                   │
-│ mypy                        Run Mypy (configured in pyproject.toml)                              │
-│ publish                     Build and upload this project to PyPi                                │
-│ run                         Run a machine emulation                                              │
-│ safety                      Run safety check against current requirements files                  │
-│ test                        Run unittests                                                        │
-│ tox                         Run tox                                                              │
-│ update                      Update "requirements*.txt" dependencies files                        │
-│ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
-│                             files)                                                               │
-│ version                     Print version and exit                                               │
+│ download-roms              Download/Test only ROM files                                          │
+│ editor                     Run only the BASIC editor                                             │
+│ gui                        Start the DragonPy tkinter starter GUI                                │
+│ log-list                   List all exiting loggers and exit.                                    │
+│ run                        Run a machine emulation                                               │
+│ version                    Print version and exit                                                │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 The output of `./cli.py run --help` looks like:
 
@@ -174,24 +177,53 @@
 | Simple6809     | [http://searle.x10host.com/6809/Simple6809.html](http://searle.x10host.com/6809/Simple6809.html)                                                                                                                               |
 
 `sbc09` and `Vectrex` ROMs are included.
 
 All ROM files and download will be checked by `SHA1` value, before use.
 
 
-## run tests
+## development
 
-e.g.:
+Please use `dev-cli.py` for development.
 
-```bash
-~/DragonPy$ ./devshell.py pytest
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
+│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
+│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
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
 ```
-or
+[comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
+
+Run tests, e.g.:
+
 ```bash
-~/DragonPy$ ./devshell.py tox
+~/DragonPy$ ./dev-cli.py coverage
+# or just:
+~/DragonPy$ ./dev-cli.py test
+# or with different Python versions:
+~/DragonPy$ ./dev-cli.py tox
 ```
 
 ## more screenshots
 
 "sbc09" ROM in Tkinter window:
 
 ![screenshot sbc09](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/DragonPy/DragonPy_sbc09_01.png "screenshot sbc09")
@@ -429,17 +461,27 @@
 * [pypi.org/project/Pygments](https://pypi.org/project/Pygments)
 * [http://pygments.org/](http://pygments.org/)
 * License: BSD License
 
 ## History
 
 
-* [*dev*](https://github.com/jedie/DragonPy/compare/v0.7.0...master):
-  * Replace Creole README with markdown.
+* [*dev*](https://github.com/jedie/DragonPy/compare/v0.9.0...master):
   * tbc
+* [07.03.2023 - v0.9.0](https://github.com/jedie/DragonPy/compare/v0.8.0...v0.9.0):
+  * Split CLI in app and dev
+  * Remove Python 3.9 support
+  * Update requirements
+* [07.03.2023 - v0.8.0](https://github.com/jedie/DragonPy/compare/v0.7.0...v0.8.0):
+  * Modernize project testing, CI pipeline, etc.
+  * Switch from poetry to pip-tools
+  * Replace devshell with click CLI
+  * Use https://github.com/jedie/manageprojects
+  * Min. Python Version is now v3.10
+  * Add BASIC examples `mandelbrot1.bas` and `mandelbrot2.bas` ;)
 * [01.10.2020 - v0.7.0](https://github.com/jedie/DragonPy/compare/v0.6.0...v0.7.0):
   * Modernize project testing, CI pipeline, usw poetry etc.
   * Many Code updates
   * Remove Python v2 fallback code parts
   * Update ROM Download Links
   * Bugfix "--max_ops" cli options
 * [19.06.2018 - v0.6.0](https://github.com/jedie/DragonPy/compare/v0.5.3...v0.6.0):
```

### Comparing `DragonPyEmulator-0.8.0rc3/basic_editor/editor.py` & `DragonPyEmulator-0.9.0/basic_editor/editor.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/basic_editor/editor_base.py` & `DragonPyEmulator-0.9.0/basic_editor/editor_base.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/basic_editor/highlighting.py` & `DragonPyEmulator-0.9.0/basic_editor/highlighting.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/basic_editor/scrolled_text.py` & `DragonPyEmulator-0.9.0/basic_editor/scrolled_text.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/basic_editor/status_bar.py` & `DragonPyEmulator-0.9.0/basic_editor/status_bar.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/basic_editor/tkinter_utils.py` & `DragonPyEmulator-0.9.0/basic_editor/tkinter_utils.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/basic_editor/token_window.py` & `DragonPyEmulator-0.9.0/basic_editor/token_window.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/cli.py` & `DragonPyEmulator-0.9.0/dev-cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
 PIP_SYNC_PATH = BIN_PATH / f'pip-sync{FILE_EXT}'
 
 DEP_LOCK_PATH = BASE_PATH / 'requirements.dev.txt'
 DEP_HASH_PATH = VENV_PATH / '.dep_hash'
 
 # script file defined in pyproject.toml as [console_scripts]
 # (Under Windows: ".exe" not added!)
-PROJECT_SHELL_SCRIPT = BIN_PATH / 'dragonpy'
+PROJECT_SHELL_SCRIPT = BIN_PATH / 'dragonpy_dev'
 
 
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

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/Dragon64/dasm_asm_d64_rom.sh` & `DragonPyEmulator-0.9.0/dragonpy/Dragon64/dasm_asm_d64_rom.sh`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/Multicomp6809/README.creole` & `DragonPyEmulator-0.9.0/dragonpy/Multicomp6809/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/Simple6809/README.creole` & `DragonPyEmulator-0.9.0/dragonpy/Simple6809/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/__init__.py` & `DragonPyEmulator-0.9.0/dragonpy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-"""dragonpy - Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python..."""
+"""
+    dragonpy
+    Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python...
+"""
 
-from importlib.metadata import version
 
 from dragonpy import constants
 from dragonpy.CoCo.config import CoCo2bCfg
 from dragonpy.CoCo.machine import run_CoCo2b
 from dragonpy.core.configs import machine_dict
 from dragonpy.Dragon32.config import Dragon32Cfg
 from dragonpy.Dragon32.machine import run_Dragon32
@@ -16,15 +18,15 @@
 from dragonpy.sbc09.machine import run_sbc09
 from dragonpy.Simple6809.config import Simple6809Cfg
 from dragonpy.Simple6809.machine import run_Simple6809
 from dragonpy.vectrex.config import VectrexCfg
 from dragonpy.vectrex.machine import run_Vectrex
 
 
-__version__ = version('DragonPyEmulator')
+__version__ = '0.9.0'
 __author__ = 'Jens Diemer <git@jensdiemer.de>'
 
 
 machine_dict.register(constants.DRAGON32, (run_Dragon32, Dragon32Cfg), default=True)
 machine_dict.register(constants.DRAGON64, (run_Dragon64, Dragon64Cfg))
 machine_dict.register(constants.COCO2B, (run_CoCo2b, CoCo2bCfg))
 machine_dict.register(constants.SBC09, (run_sbc09, SBC09Cfg))
```

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/constants.py` & `DragonPyEmulator-0.9.0/dragonpy/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CLI_EPILOG = 'Project Homepage: https://github.com/john-doh/dragonpy'
+CLI_EPILOG = 'Project Homepage: https://github.com/jedie/DragonPy'
 
 DRAGON32 = "Dragon32"
 DRAGON64 = "Dragon64"
 COCO2B = "CoCo2b"
 SBC09 = "sbc09"
 SIMPLE6809 = "Simple6809"
 MULTICOMP6809 = "Multicomp6809"
```

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/sbc09/README.creole` & `DragonPyEmulator-0.9.0/dragonpy/sbc09/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/sbc09/sbc09.creole` & `DragonPyEmulator-0.9.0/dragonpy/sbc09/sbc09.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/sbc09/v09.rom` & `DragonPyEmulator-0.9.0/dragonpy/sbc09/v09.rom`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/dragonpy/vectrex/SYSTEM.IMG` & `DragonPyEmulator-0.9.0/dragonpy/vectrex/SYSTEM.IMG`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/misc/README.creole` & `DragonPyEmulator-0.9.0/misc/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.8.0rc3/pyproject.toml` & `DragonPyEmulator-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,74 @@
 [project]
 name = "DragonPyEmulator"
-version = "0.8.0rc3"
+dynamic = ["version"]
 description = "Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python..."
 keywords=["Emulator","6809","Dragon","CoCo","Vectrex","tkinter","pypy"]
-classifiers = [
-    # http://pypi.python.org/pypi?%3Aaction=list_classifiers
-    "Development Status :: 5 - Production/Stable",
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
+license = {text = "GPL-3.0-or-later"}
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'git@jensdiemer.de'}
 ]
-requires-python = ">=3.9,<4"
+requires-python = ">=3.10,<4"
 dependencies = [
-    "MC6809>=0.7.0rc0",  # https://github.com/6809/MC6809
+    "MC6809",  # https://github.com/6809/MC6809
     "dragonlib",  # https://github.com/6809/dragonlib
+    "manageprojects",  # https://github.com/jedie/manageprojects
     "pygments",  # https://pygments.org/
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
 ]
 [project.optional-dependencies]
 dev = [
-    "manageprojects>=0.9.3rc1",  # https://github.com/jedie/manageprojects
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
 Documentation = "https://github.com/jedie/DragonPy"
 Source = "https://github.com/jedie/DragonPy"
 
 [project.scripts]
-dragonpy = "dragonpy.__main__:main"
+dragonpy_app = "dragonpy.__main__:main"
+dragonpy_dev = "dragonpy.cli.dev:main"
+
+[build-system]
+requires = ["setuptools>=61.0", "setuptools_scm>=7.1"]
+build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["basic_editor", "dragonpy", "PyDC"]
 
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+[tool.setuptools.dynamic]
+version = {attr = "dragonpy.__version__"}
 
 
 [tool.darker]
 src = ['.']
 revision = "origin/main..."
 line_length = 119
 verbose = true
@@ -109,14 +94,15 @@
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
@@ -129,15 +115,15 @@
 ]
 
 
 [tool.tox]  # https://tox.wiki/en/latest/config.html#pyproject-toml
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py{311,310,39}
+envlist = py{311,310}
 skip_missing_interpreters = True
 
 [testenv]
 passenv = *
 skip_install = true
 commands_pre =
     pip install -U pip-tools
@@ -174,8 +160,9 @@
 package_description = "Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python..."
 package_url = "https://github.com/jedie/DragonPy"
 issues_url = "https://github.com/jedie/DragonPy/issues"
 license = "GPL-3.0-or-later"
 _template = "https://github.com/jedie/cookiecutter_templates/"
 applied_migrations = [
     "04d5a25", # 2023-03-07T16:25:36+01:00
+    "da054d6", # 2023-08-04T17:39:02+02:00
 ]
```

