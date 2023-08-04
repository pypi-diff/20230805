# Comparing `tmp/edk2-pytool-library-0.9.1.tar.gz` & `tmp/edk2-pytool-library-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edk2-pytool-library-0.9.1.tar", last modified: Fri Aug  2 01:15:57 2019, max compression
+gzip compressed data, was "dist\edk2-pytool-library-0.9.2.tar", last modified: Mon Aug 12 05:15:51 2019, max compression
```

## Comparing `edk2-pytool-library-0.9.1.tar` & `edk2-pytool-library-0.9.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/
--rw-rw-rw-   0        0        0     2486 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/BasicDevTests.py
--rw-rw-rw-   0        0        0      788 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/ConfirmVersionAndTag.py
--rw-rw-rw-   0        0        0      137 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6654 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/docs/
--rw-rw-rw-   0        0        0     2734 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/docs/developing.md
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/docs/features/
--rw-rw-rw-   0        0        0     1469 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/docs/features/logging.ansi_handler.md
--rw-rw-rw-   0        0        0      868 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/docs/features/utility_functions.GetHostInfo.md
--rw-rw-rw-   0        0        0     1872 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/docs/publishing.md
--rw-rw-rw-   0        0        0      398 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/docs/using.md
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2_pytool_library.egg-info/
--rw-rw-rw-   0        0        0     6654 2019-08-02 01:15:56.000000 edk2-pytool-library-0.9.1/edk2_pytool_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2456 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2_pytool_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-08-02 01:15:56.000000 edk2-pytool-library-0.9.1/edk2_pytool_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2019-08-02 01:15:56.000000 edk2-pytool-library-0.9.1/edk2_pytool_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/__init__.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/acpi/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/acpi/__init__.py
--rw-rw-rw-   0        0        0    20065 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/acpi/dmar_parser.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/bin/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/bin/__init__.py
--rwxrwxrwx   0        0        0   458336 2019-08-02 01:15:11.000000 edk2-pytool-library-0.9.1/edk2toollib/bin/vswhere.exe
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/log/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/log/__init__.py
--rw-rw-rw-   0        0        0    16072 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/log/ansi_handler.py
--rw-rw-rw-   0        0        0     3240 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/log/ansi_handler_test.py
--rw-rw-rw-   0        0        0      928 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/log/file_handler.py
--rw-rw-rw-   0        0        0     5565 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/log/junit_report_format.py
--rw-rw-rw-   0        0        0     3714 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/log/markdown_handler.py
--rw-rw-rw-   0        0        0     1336 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/log/string_handler.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/__init__.py
--rw-rw-rw-   0        0        0    24751 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_defs.py
--rw-rw-rw-   0        0        0     1126 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_defs_test.py
--rw-rw-rw-   0        0        0     7508 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_policy_calc.py
--rw-rw-rw-   0        0        0     6345 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_policy_calc_test.py
--rw-rw-rw-   0        0        0     3357 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_simulator.py
--rw-rw-rw-   0        0        0     2623 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_stream.py
--rw-rw-rw-   0        0        0     1514 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_stream_test.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/__init__.py
--rw-rw-rw-   0        0        0    21894 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/authenticated_variables_structure_support.py
--rw-rw-rw-   0        0        0    12097 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/bmp_object.py
--rw-rw-rw-   0        0        0     7011 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/bmp_object_test.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/__init__.py
--rw-rw-rw-   0        0        0     5721 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/ftw_working_block_format.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/__init__.py
--rw-rw-rw-   0        0        0    10067 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/base_parser.py
--rw-rw-rw-   0        0        0    14053 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/buildreport_parser.py
--rw-rw-rw-   0        0        0     4207 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/dec_parser.py
--rw-rw-rw-   0        0        0    12419 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/dsc_parser.py
--rw-rw-rw-   0        0        0     7530 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/fdf_parser.py
--rw-rw-rw-   0        0        0     6325 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/inf_parser.py
--rw-rw-rw-   0        0        0     5390 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/override_parser.py
--rw-rw-rw-   0        0        0     6438 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/override_parser_test.py
--rw-rw-rw-   0        0        0     1287 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/targettxt_parser.py
--rw-rw-rw-   0        0        0     6172 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/path_utilities.py
--rw-rw-rw-   0        0        0     9438 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/variable_format.py
--rw-rw-rw-   0        0        0      794 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/variable_format_test.py
--rw-rw-rw-   0        0        0     4661 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/variablestore_manulipulations.py
--rw-rw-rw-   0        0        0     1961 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/pi_firmware_file.py
--rw-rw-rw-   0        0        0     4008 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/pi_firmware_volume.py
--rw-rw-rw-   0        0        0     1558 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/status_codes.py
--rw-rw-rw-   0        0        0      526 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/uefi_multi_phase.py
--rw-rw-rw-   0        0        0     7278 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/uefi/wincert.py
--rw-rw-rw-   0        0        0    15870 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/utility_functions.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/
--rw-rw-rw-   0        0        0      139 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/__init__.py
--rw-rw-rw-   0        0        0     3090 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/cat_generator.py
--rw-rw-rw-   0        0        0     2957 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/cat_generator_test.py
--rw-rw-rw-   0        0        0     6111 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/inf_generator.py
--rw-rw-rw-   0        0        0     3606 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/inf_generator_test.py
--rw-rw-rw-   0        0        0    11725 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/locate_tools.py
--rw-rw-rw-   0        0        0     4591 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/edk2toollib/windows/locate_tools_test.py
--rw-rw-rw-   0        0        0       42 2019-08-02 01:15:57.000000 edk2-pytool-library-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1969 2019-08-02 01:13:55.000000 edk2-pytool-library-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/
+-rw-rw-rw-   0        0        0     2486 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/BasicDevTests.py
+-rw-rw-rw-   0        0        0      788 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/ConfirmVersionAndTag.py
+-rw-rw-rw-   0        0        0      137 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6888 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/docs/
+-rw-rw-rw-   0        0        0     2734 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/docs/developing.md
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/docs/features/
+-rw-rw-rw-   0        0        0     1469 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/docs/features/logging.ansi_handler.md
+-rw-rw-rw-   0        0        0      868 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/docs/features/utility_functions.GetHostInfo.md
+-rw-rw-rw-   0        0        0     1872 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/docs/publishing.md
+-rw-rw-rw-   0        0        0      398 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/docs/using.md
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2_pytool_library.egg-info/
+-rw-rw-rw-   0        0        0     6888 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2_pytool_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2456 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2_pytool_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2_pytool_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2_pytool_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/__init__.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/acpi/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/acpi/__init__.py
+-rw-rw-rw-   0        0        0    20065 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/acpi/dmar_parser.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/bin/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/bin/__init__.py
+-rwxrwxrwx   0        0        0   458336 2019-08-12 05:15:01.000000 edk2-pytool-library-0.9.2/edk2toollib/bin/vswhere.exe
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/log/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/log/__init__.py
+-rw-rw-rw-   0        0        0    16072 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/log/ansi_handler.py
+-rw-rw-rw-   0        0        0     3240 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/log/ansi_handler_test.py
+-rw-rw-rw-   0        0        0      928 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/log/file_handler.py
+-rw-rw-rw-   0        0        0     5565 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/log/junit_report_format.py
+-rw-rw-rw-   0        0        0     3714 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/log/markdown_handler.py
+-rw-rw-rw-   0        0        0     1336 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/log/string_handler.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/__init__.py
+-rw-rw-rw-   0        0        0    24751 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_defs.py
+-rw-rw-rw-   0        0        0     1126 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_defs_test.py
+-rw-rw-rw-   0        0        0     7508 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_policy_calc.py
+-rw-rw-rw-   0        0        0     6345 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_policy_calc_test.py
+-rw-rw-rw-   0        0        0     3357 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_simulator.py
+-rw-rw-rw-   0        0        0     2623 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_stream.py
+-rw-rw-rw-   0        0        0     1514 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_stream_test.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/__init__.py
+-rw-rw-rw-   0        0        0    21894 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/authenticated_variables_structure_support.py
+-rw-rw-rw-   0        0        0    12097 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/bmp_object.py
+-rw-rw-rw-   0        0        0     7011 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/bmp_object_test.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/__init__.py
+-rw-rw-rw-   0        0        0     5721 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/ftw_working_block_format.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/__init__.py
+-rw-rw-rw-   0        0        0    10067 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/base_parser.py
+-rw-rw-rw-   0        0        0    14053 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/buildreport_parser.py
+-rw-rw-rw-   0        0        0     4207 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/dec_parser.py
+-rw-rw-rw-   0        0        0    12419 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/dsc_parser.py
+-rw-rw-rw-   0        0        0     7530 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/fdf_parser.py
+-rw-rw-rw-   0        0        0     6325 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/inf_parser.py
+-rw-rw-rw-   0        0        0     5390 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/override_parser.py
+-rw-rw-rw-   0        0        0     6438 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/override_parser_test.py
+-rw-rw-rw-   0        0        0     1287 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/targettxt_parser.py
+-rw-rw-rw-   0        0        0     6172 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/path_utilities.py
+-rw-rw-rw-   0        0        0     9438 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/variable_format.py
+-rw-rw-rw-   0        0        0      794 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/variable_format_test.py
+-rw-rw-rw-   0        0        0     4661 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/variablestore_manulipulations.py
+-rw-rw-rw-   0        0        0     1961 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/pi_firmware_file.py
+-rw-rw-rw-   0        0        0     4008 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/pi_firmware_volume.py
+-rw-rw-rw-   0        0        0     1558 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/status_codes.py
+-rw-rw-rw-   0        0        0      526 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/uefi_multi_phase.py
+-rw-rw-rw-   0        0        0     7278 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/uefi/wincert.py
+-rw-rw-rw-   0        0        0    16057 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/utility_functions.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/
+-rw-rw-rw-   0        0        0      139 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/__init__.py
+-rw-rw-rw-   0        0        0     3090 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/cat_generator.py
+-rw-rw-rw-   0        0        0     2957 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/cat_generator_test.py
+-rw-rw-rw-   0        0        0     6111 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/inf_generator.py
+-rw-rw-rw-   0        0        0     3606 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/inf_generator_test.py
+-rw-rw-rw-   0        0        0    11866 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/locate_tools.py
+-rw-rw-rw-   0        0        0     4591 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/edk2toollib/windows/locate_tools_test.py
+-rw-rw-rw-   0        0        0       42 2019-08-12 05:15:51.000000 edk2-pytool-library-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1978 2019-08-12 05:13:31.000000 edk2-pytool-library-0.9.2/setup.py
```

### Comparing `edk2-pytool-library-0.9.1/BasicDevTests.py` & `edk2-pytool-library-0.9.2/BasicDevTests.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/ConfirmVersionAndTag.py` & `edk2-pytool-library-0.9.2/ConfirmVersionAndTag.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/PKG-INFO` & `edk2-pytool-library-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: edk2-pytool-library
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library supporting UEFI EDK2 firmware development
 Home-page: https://github.com/tianocore/edk2-pytool-library
 Author: Tianocore Edk2-PyTool-Library team
 Author-email: sean.brogan@microsoft.com
-License: BSD+Patent
+License: BSD-2-Clause-Patent
 Description: # Tianocore Edk2 PyTool Library (edk2toollib)
         
         This is a Tianocore maintained project consisting of a python library supporting UEFI firmware development.  This package's intent is to provide an easy way to organize and share python code to facilitate reuse across environments, tools, and scripts.  Inclusion of this package and dependency management is best managed using Pip/Pypi.
         
         This is a supplemental package and is not required to be used for edk2 builds.  
         
         ## Content
@@ -38,14 +38,19 @@
         * To use in your python code
             ```python
             from edk2toollib.<module> import <class>
             ```
         
         ## Release Version History
         
+        ### Version 0.9.2
+        
+        * Bugs:
+          * Change QueryVcVariables so environment variable keys are not case sensitive.  On Windows these are not case sensitive and "Path" is not consistent.
+        
         ### Version 0.9.1
         
         * Features:
           * Add support for getting WinSdk tools on platforms without VS2017 or newer
           * FindToolInWinSdk in locate_tools.py throws a FileNotFoundException when it cannot find the tool requested, previouly it returned None
           * Add support for limiting vswhere to certain versions of visual studio (VS2017 and VS2019 supported)
```

### Comparing `edk2-pytool-library-0.9.1/docs/developing.md` & `edk2-pytool-library-0.9.2/docs/developing.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/docs/features/logging.ansi_handler.md` & `edk2-pytool-library-0.9.2/docs/features/logging.ansi_handler.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/docs/features/utility_functions.GetHostInfo.md` & `edk2-pytool-library-0.9.2/docs/features/utility_functions.GetHostInfo.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/docs/publishing.md` & `edk2-pytool-library-0.9.2/docs/publishing.md`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2_pytool_library.egg-info/PKG-INFO` & `edk2-pytool-library-0.9.2/edk2_pytool_library.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: edk2-pytool-library
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library supporting UEFI EDK2 firmware development
 Home-page: https://github.com/tianocore/edk2-pytool-library
 Author: Tianocore Edk2-PyTool-Library team
 Author-email: sean.brogan@microsoft.com
-License: BSD+Patent
+License: BSD-2-Clause-Patent
 Description: # Tianocore Edk2 PyTool Library (edk2toollib)
         
         This is a Tianocore maintained project consisting of a python library supporting UEFI firmware development.  This package's intent is to provide an easy way to organize and share python code to facilitate reuse across environments, tools, and scripts.  Inclusion of this package and dependency management is best managed using Pip/Pypi.
         
         This is a supplemental package and is not required to be used for edk2 builds.  
         
         ## Content
@@ -38,14 +38,19 @@
         * To use in your python code
             ```python
             from edk2toollib.<module> import <class>
             ```
         
         ## Release Version History
         
+        ### Version 0.9.2
+        
+        * Bugs:
+          * Change QueryVcVariables so environment variable keys are not case sensitive.  On Windows these are not case sensitive and "Path" is not consistent.
+        
         ### Version 0.9.1
         
         * Features:
           * Add support for getting WinSdk tools on platforms without VS2017 or newer
           * FindToolInWinSdk in locate_tools.py throws a FileNotFoundException when it cannot find the tool requested, previouly it returned None
           * Add support for limiting vswhere to certain versions of visual studio (VS2017 and VS2019 supported)
```

### Comparing `edk2-pytool-library-0.9.1/edk2_pytool_library.egg-info/SOURCES.txt` & `edk2-pytool-library-0.9.2/edk2_pytool_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/acpi/dmar_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/acpi/dmar_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/bin/vswhere.exe` & `edk2-pytool-library-0.9.2/edk2toollib/bin/vswhere.exe`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/log/ansi_handler.py` & `edk2-pytool-library-0.9.2/edk2toollib/log/ansi_handler.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/log/ansi_handler_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/log/ansi_handler_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/log/file_handler.py` & `edk2-pytool-library-0.9.2/edk2toollib/log/file_handler.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/log/junit_report_format.py` & `edk2-pytool-library-0.9.2/edk2toollib/log/junit_report_format.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/log/markdown_handler.py` & `edk2-pytool-library-0.9.2/edk2toollib/log/markdown_handler.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/log/string_handler.py` & `edk2-pytool-library-0.9.2/edk2toollib/log/string_handler.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_defs.py` & `edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_defs.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_defs_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_defs_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_policy_calc.py` & `edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_policy_calc.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_policy_calc_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_policy_calc_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_simulator.py` & `edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_simulator.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_stream.py` & `edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_stream.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/tpm/tpm2_stream_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/tpm/tpm2_stream_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/authenticated_variables_structure_support.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/authenticated_variables_structure_support.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/bmp_object.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/bmp_object.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/bmp_object_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/bmp_object_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/ftw_working_block_format.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/ftw_working_block_format.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/base_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/buildreport_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/buildreport_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/dec_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/dec_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/dsc_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/dsc_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/fdf_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/fdf_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/inf_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/inf_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/override_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/override_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/override_parser_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/override_parser_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/parsers/targettxt_parser.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/parsers/targettxt_parser.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/path_utilities.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/path_utilities.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/variable_format.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/variable_format.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/variable_format_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/variable_format_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/edk2/variablestore_manulipulations.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/edk2/variablestore_manulipulations.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/pi_firmware_file.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/pi_firmware_file.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/pi_firmware_volume.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/pi_firmware_volume.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/status_codes.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/status_codes.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/uefi_multi_phase.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/uefi_multi_phase.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/uefi/wincert.py` & `edk2-pytool-library-0.9.2/edk2toollib/uefi/wincert.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/utility_functions.py` & `edk2-pytool-library-0.9.2/edk2toollib/utility_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,16 @@
 # @param environ - shell environment variables dictionary that replaces the one inherited from the
 #                  current process.
 #
 # @return returncode of called cmd
 ####
 
 
-def RunPythonScript(pythonfile, params, capture=True, workingdir=None, outfile=None, outstream=None, environ=None):
+def RunPythonScript(pythonfile, params, capture=True, workingdir=None, outfile=None, outstream=None,
+                    environ=None, logging_level=logging.INFO, raise_exception_on_nonzero=False):
     # locate python file on path
     pythonfile.strip('"\'')
     if " " in pythonfile:
         pythonfile = '"' + pythonfile + '"'
     params.strip()
     logging.debug("RunPythonScript: {0} {1}".format(pythonfile, params))
     if(os.path.isabs(pythonfile)):
@@ -222,15 +223,16 @@
             a = os.path.normpath(a)
             if os.path.isfile(os.path.join(a, pythonfile)):
                 pythonfile = os.path.join(a, pythonfile)
                 logging.debug("Python Script was found on the path: %s" % pythonfile)
                 break
     params = pythonfile + " " + params
     return RunCmd(sys.executable, params, capture=capture, workingdir=workingdir, outfile=outfile,
-                  outstream=outstream, environ=environ)
+                  outstream=outstream, environ=environ, logging_level=logging_level,
+                  xraise_exception_on_nonzero=raise_exception_on_nonzero)
 ####
 # Locally Sign input file using Windows SDK signtool.  This will use a local Pfx file.
 # WARNING!!! : This should not be used for production signing as that process should follow stronger
 #               security practices (HSM / smart cards / etc)
 #
 #  Signing is in format specified by UEFI authentacted variables
 ####
```

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/cat_generator.py` & `edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/cat_generator.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/cat_generator_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/cat_generator_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/inf_generator.py` & `edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/inf_generator.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/windows/capsule/inf_generator_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/windows/capsule/inf_generator_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/windows/locate_tools.py` & `edk2-pytool-library-0.9.2/edk2toollib/windows/locate_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # Supported Versions that can be queried with vswhere
 # Use lower case for key as all comparisons will be lower case
 #
 supported_vs_versions = {"vs2017": "15.0,16.0", "vs2019": "16.0,17.0"}
 
 
 # Downloads VSWhere
-def _DownloadVsWhere(unpack_folder=None):
+def _DownloadVsWhere(unpack_folder: os.PathLike = None):
     if unpack_folder is None:
         unpack_folder = os.path.dirname(__VsWherePath())
 
     out_file_name = os.path.join(unpack_folder, "vswhere.exe")
     logging.info("Attempting to download vswhere to: {}. This may take a second.".format(unpack_folder))
     # check if we have the vswhere file already downloaded
     if not os.path.isfile(out_file_name):
@@ -81,15 +81,15 @@
 
 ####
 #
 # https://docs.microsoft.com/en-us/vswhere/install-vswhere-client-tools
 #
 # @return string "/PATH/TO/vswhere.exe" or None
 ####
-def GetVsWherePath(fail_on_not_found=True):
+def GetVsWherePath(fail_on_not_found: bool = True):
     vswhere_path = __VsWherePath()
     # check if we can't find it, look for vswhere in the path
     if not os.path.isfile(vswhere_path):
         for env_var in os.getenv("PATH").split(os.pathsep):
             env_var = os.path.join(os.path.normpath(env_var), "vswhere.exe")
             if os.path.isfile(env_var):
                 vswhere_path = env_var
@@ -151,22 +151,24 @@
 #  Inspiration taken from cpython for this method of env collection
 #
 # keys: enumerable list with names of env variables to collect after bat run
 # arch: arch to run.  amd64, x86, ??
 # product: value defined by vswhere.exe
 # vs_version: helper to find version of supported VS version (example vs2019).
 # returns a dictionary of the interesting environment variables
-def QueryVcVariables(keys: dict, arch: str = None, product: str = None, vs_version: str = None):
-    """Launch vcvarsall.bat and read the settings from its environment"""
+def QueryVcVariables(keys: list, arch: str = None, product: str = None, vs_version: str = None):
+    """Launch vcvarsall.bat and read the settings from its environment.  This is a windows only function
+    and Windows is case insensitive for the keys"""
+
     if product is None:
         product = "*"
     if arch is None:
         # TODO: look up host architecture?
         arch = "amd64"
-    interesting = set(keys)
+    interesting = set(x.upper() for x in keys)
     result = {}
     ret, vs_path = FindWithVsWhere(product, vs_version)
     if ret != 0 or vs_path is None:
         logging.warning("We didn't find VS path or otherwise failed to invoke vsWhere")
         raise ValueError("Bad VC")
     vcvarsall_path = os.path.join(vs_path, "VC", "Auxiliary", "Build", "vcvarsall.bat")
     logging.debug("Calling '%s %s'", vcvarsall_path, arch)
@@ -177,15 +179,15 @@
             raise Exception(stderr.decode("mbcs"))
         stdout = stdout.decode("mbcs")
         for line in stdout.split("\n"):
             if '=' not in line:
                 continue
             line = line.strip()
             key, value = line.split('=', 1)
-            if key in interesting:
+            if key.upper() in interesting:
                 if value.endswith(os.pathsep):
                     value = value[:-1]
                 result[key] = value
     finally:
         popen.stdout.close()
         popen.stderr.close()
 
@@ -258,15 +260,15 @@
     if isArm and (bits < 32 or arch != "ARM"):
         return False
     return True
 
 
 # does a glob in the folder that your sdk is
 # uses the environmental variable WindowsSdkDir and tries to use WindowsSDKVersion
-def FindToolInWinSdk(tool, product=None, arch=None):
+def FindToolInWinSdk(tool: str, product=None, arch=None):
     variables = ["WindowsSdkDir", "WindowsSDKVersion"]
     # get the value with QueryVcVariables
     try:
         results = QueryVcVariables(variables, product, arch)
         # Get the variables we care about
         sdk_dir = results["WindowsSdkDir"]
         sdk_ver = results["WindowsSDKVersion"]
```

### Comparing `edk2-pytool-library-0.9.1/edk2toollib/windows/locate_tools_test.py` & `edk2-pytool-library-0.9.2/edk2toollib/windows/locate_tools_test.py`

 * *Files identical despite different names*

### Comparing `edk2-pytool-library-0.9.1/setup.py` & `edk2-pytool-library-0.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     name="edk2-pytool-library",
     author="Tianocore Edk2-PyTool-Library team",
     author_email="sean.brogan@microsoft.com",
     description="Python library supporting UEFI EDK2 firmware development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tianocore/edk2-pytool-library",
-    license='BSD+Patent',
+    license='BSD-2-Clause-Patent',
     packages=setuptools.find_packages(),
     cmdclass={
         'sdist': PostSdistCommand,
         'install': PostInstallCommand,
         'develop': PostDevCommand,
     },
     include_package_data=True,
```

