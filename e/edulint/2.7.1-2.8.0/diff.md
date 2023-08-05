# Comparing `tmp/edulint-2.7.1.tar.gz` & `tmp/edulint-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-dbv3bqci/edulint-2.7.1.tar", last modified: Wed Aug  2 14:38:10 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-bo8c75cm/edulint-2.8.0.tar", last modified: Sat Aug  5 11:02:26 2023, max compression
```

## Comparing `edulint-2.7.1.tar` & `edulint-2.8.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 14:37:53.000000 edulint-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-02 14:38:10.000000 edulint-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-02 14:37:53.000000 edulint-2.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/config_translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/file_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/config/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/files/default.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/files/empty.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/duplication_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 14:37:53.000000 edulint-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 14:38:10.000000 edulint-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 14:37:53.000000 edulint-2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 11:02:14.000000 edulint-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-05 11:02:26.000000 edulint-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-05 11:02:14.000000 edulint-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/config_translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/file_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/config/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/files/default.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/files/empty.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/duplication_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-05 11:02:14.000000 edulint-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-05 11:02:26.000000 edulint-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-05 11:02:14.000000 edulint-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_visitors.py
```

### Comparing `edulint-2.7.1/LICENSE` & `edulint-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/PKG-INFO` & `edulint-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.7.1
+Version: 2.8.0
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.7.1/README.md` & `edulint-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/config/config.py` & `edulint-2.8.0/edulint/config/config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/config/config_translations.py` & `edulint-2.8.0/edulint/config/config_translations.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/config/file_config.py` & `edulint-2.8.0/edulint/config/file_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/config/files/default.toml` & `edulint-2.8.0/edulint/config/files/default.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/edulint.py` & `edulint-2.8.0/edulint/edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/explanations.toml` & `edulint-2.8.0/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linters.py` & `edulint-2.8.0/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/basic_checker.py` & `edulint-2.8.0/edulint/linting/checkers/basic_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/duplication_checker.py` & `edulint-2.8.0/edulint/linting/checkers/duplication_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/improper_loop.py` & `edulint-2.8.0/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/modified_listener.py` & `edulint-2.8.0/edulint/linting/checkers/modified_listener.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.8.0/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/short_problems.py` & `edulint-2.8.0/edulint/linting/checkers/short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.8.0/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/checkers/utils.py` & `edulint-2.8.0/edulint/linting/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/linting.py` & `edulint-2.8.0/edulint/linting/linting.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/overrides.py` & `edulint-2.8.0/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/problem.py` & `edulint-2.8.0/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/process_handler.py` & `edulint-2.8.0/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/linting/tweakers.py` & `edulint-2.8.0/edulint/linting/tweakers.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         v and v[0] == v[-1] and v[0] in "\"'" and len(v) == 3 for v in vals
     ):
         inner_quote = vals[0][0]
         return (
             start + inner_quote + "".join(v.strip("\"'") for v in vals) + inner_quote + outer_quote
         )
 
-    return problem.text
+    return start + f"({', '.join(vals)})" + outer_quote
 
 
 def unused_import_keep(self: Tweaker, problem: Problem, args: List[ImmutableArg]) -> bool:
     match = self.match(problem)
     return not match.group(1).startswith("ib111")
```

### Comparing `edulint-2.7.1/edulint/options.py` & `edulint-2.8.0/edulint/options.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/prepare_explanations/__init__.py` & `edulint-2.8.0/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.8.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.8.0/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.8.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.8.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/edulint.egg-info/PKG-INFO` & `edulint-2.8.0/edulint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.7.1
+Version: 2.8.0
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.7.1/edulint.egg-info/SOURCES.txt` & `edulint-2.8.0/edulint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/setup.cfg` & `edulint-2.8.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	flake8 ==4.0.1
+	flake8 >=3.8.4
 	flake8-json ==21.7.0
-	pylint ==2.14.5
+	pylint >=2.15.10
 	dataclasses-json
 	tomli
 	requests
 include_package_data = True
 
 [options.packages.find]
 where = .
```

### Comparing `edulint-2.7.1/setup.py` & `edulint-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/tests/test_config.py` & `edulint-2.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/tests/test_duplication.py` & `edulint-2.8.0/tests/test_duplication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from edulint.options import Option
 from edulint.config.arg import Arg
 from edulint.linting.problem import Problem
-from utils import lazy_problem, apply_and_lint, create_apply_and_lint
+from utils import lazy_problem, apply_and_lint
 from typing import List
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("013165-coins.py", [
         lazy_problem().set_line(9)
         .set_text("Identical code inside all if's branches, move 1 lines before the if.")
@@ -22,15 +22,15 @@
     ("023171-credit.py", [
         lazy_problem().set_line(26),
         lazy_problem().set_line(38)
     ]),
     ("024056-cards.py", [
         lazy_problem().set_line(7)
     ]),
-    ("024329-workdays.py", [ # TODO improve
+    ("024329-workdays.py", [  # TODO improve
         # lazy_problem().set_line(56)
     ]),
     ("024535-credit.py", [
         lazy_problem().set_line(23)
         .set_text("Identical code inside all if's branches, move 3 lines after the if."),
         lazy_problem().set_line(35),
     ]),
@@ -70,18 +70,19 @@
         .set_text("Identical code inside all if's branches, move 3 lines after the if.")
     ]),
     ("hw48505.py", []),
 ])
 def test_duplicate_if_branches(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=duplicate-if-branches")],
+        [Arg(Option.PYLINT, "--enable=duplicate-if-branches")],
         expected_output
     )
 
+
 @pytest.mark.parametrize("filename,expected_output", [
     ("012889-geometry.py", [
         lazy_problem().set_line(28).set_end_line(33)
         .set_text("Identical code inside 3 consecutive ifs, join their conditions using 'or'.")
     ]),
     ("012889-pythagorean.py", [
         lazy_problem().set_line(26).set_end_line(29)
@@ -102,41 +103,41 @@
         .set_text("Identical code inside 7 consecutive ifs, join their conditions using 'or'.")
     ]),
     ("052975-parse_time.py", []),
 ])
 def test_duplicate_seq_ifs(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=duplicate-seq-ifs")],
+        [Arg(Option.PYLINT, "--enable=duplicate-seq-ifs")],
         expected_output
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
-    ("012853-geometry.py", [ # TODO detect this
+    ("012853-geometry.py", [  # TODO detect this
         lazy_problem().set_line(8)
         .set_text("A complex expression 'not (a + b > c and b + c > a and c + a > b)' used repeatedly "
                   "(on lines 8, 18, 27). Extract it to a local variable or create a helper function.")
     ]),
     ("014024-pythagorean.py", [
         lazy_problem().set_line(19)
         .set_text("A complex expression 'sqrt(a**2 + b**2)' used repeatedly (on lines 19, 20). Extract it to a "
                   "local variable or create a helper function."),
         lazy_problem().set_line(21)
         .set_text("A complex expression 'a + b + c > result' used repeatedly (on lines 21, 27, 33). Extract it to a "
-        "local variable or create a helper function."),
+                  "local variable or create a helper function."),
         lazy_problem().set_line(25),
         lazy_problem().set_line(31),
     ]),
     ("042643-edge_detection.py", [])
 ])
 def test_duplicate_exprs(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=duplicate-exprs")],
+        [Arg(Option.PYLINT, "--enable=duplicate-exprs")],
         expected_output
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("013145-coins.py", [
         lazy_problem().set_line(5).set_end_line(7)
@@ -148,15 +149,15 @@
     ("024508-cards.py", [
         lazy_problem().set_line(61).set_end_line(66),
     ])
 ])
 def test_duplicate_blocks(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=duplicate-blocks")],
+        [Arg(Option.PYLINT, "--enable=duplicate-blocks")],
         expected_output
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("010666-coins.py", [
         lazy_problem().set_line(13).set_end_line(27)
@@ -175,10 +176,10 @@
         lazy_problem().set_line(25).set_end_line(36),
         lazy_problem().set_line(37).set_end_line(48),
     ]),
 ])
 def test_duplicate_sequence(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.NO_FLAKE8, "on"), Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=duplicate-sequence")],
+        [Arg(Option.PYLINT, "--enable=duplicate-sequence")],
         expected_output
     )
```

### Comparing `edulint-2.7.1/tests/test_improper_loop.py` & `edulint-2.8.0/tests/test_improper_loop.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,15 @@
         lazy_problem().set_line(2)
         .set_text("The while condition can be replaced with '<negated x>'")
     ]),
 ])
 def test_while_true_break(lines: List[str], expected_output: List[Problem]) -> None:
     create_apply_and_lint(
         lines,
-        [Arg(Option.PYLINT, "--disable=R1705"),
-            Arg(Option.FLAKE8, "--extend-ignore=E501,F841")],
+        [Arg(Option.PYLINT, "--enable=no-while-true")],
         [p.set_code("R6301") for p in expected_output]
     )
 
 
 @pytest.mark.parametrize("lines,expected_output", [
     ([
         "n = 10",
@@ -37,17 +36,15 @@
         lazy_problem().set_line(3)
         .set_text("Use for loop.")
     ]),
 ])
 def test_use_for_loop_custom(lines: List[str], expected_output: List[Problem]) -> None:
     create_apply_and_lint(
         lines,
-        [Arg(Option.PYLINT, "--disable=all"),
-            Arg(Option.PYLINT, "--enable=use-for-loop"),
-            Arg(Option.NO_FLAKE8, "on")],
+        [Arg(Option.PYLINT, "--enable=use-for-loop")],
         [p.set_code("R6305") for p in expected_output]
     )
 
 
 @pytest.mark.parametrize("lines,expected_output", [
     ([
         "for i in range(10):",
@@ -72,17 +69,15 @@
         "        _, rest = 'a,b,c,d'.split(',', 1)",
     ], [
     ])
 ])
 def test_changing_control_variable_custom(lines: List[str], expected_output: List[Problem]) -> None:
     create_apply_and_lint(
         lines,
-        [Arg(Option.PYLINT, "--disable=all"),
-            Arg(Option.PYLINT, "--enable=changing-control-variable"),
-            Arg(Option.NO_FLAKE8, "on")],
+        [Arg(Option.PYLINT, "--enable=changing-control-variable")],
         [p.set_code("R6304") for p in expected_output]
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("hw14062.py", [
         lazy_problem().set_code("R6302").set_line(29)
@@ -96,15 +91,15 @@
         lazy_problem().set_code("R6302").set_line(107)
         .set_text("Use tighter range boundaries, the last iteration never happens.")
     ]),
 ])
 def test_tighter_bounds_files(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=use-tighter-boundaries")],
+        [Arg(Option.PYLINT, "--enable=use-tighter-boundaries")],
         expected_output
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("010666-even.py", [lazy_problem().set_line(9)]),
     ("012630-next.py", []),
@@ -118,15 +113,15 @@
     ("017667-coins.py", []),
     ("023140-credit.py", []),
     ("043611-swap_columns.py", []),
 ])
 def test_use_for_loop_files(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=use-for-loop")],
+        [Arg(Option.PYLINT, "--enable=use-for-loop")],
         [problem.set_code("R6305") for problem in expected_output]
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("034636-right_cellular.py", []),
     ("104526-subset_sum.py", [
@@ -151,30 +146,29 @@
         .set_text("Iterated structure traders is being modified inside the for loop body. "
                   "Use while loop or iterate over a copy.")
     ]),
 ])
 def test_modifying_iterated_files(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=modifying-iterated-structure")],
+        [Arg(Option.PYLINT, "--enable=modifying-iterated-structure")],
         [problem.set_code("R6303") for problem in expected_output]
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("hw33176.py", []),
     ("m4521.py", [
         lazy_problem().set_line(117).set_text("Inner for loop shadows outer for loop's control variable i.")
     ])
 ])
 def test_shadowed_control_var_files(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=loop-shadows-control-variable"),
-            Arg(Option.NO_FLAKE8, "on")],
+        [Arg(Option.PYLINT, "--enable=loop-shadows-control-variable")],
         expected_output
     )
 
 
 @pytest.mark.parametrize("filename,expected_output", [
     ("014659-next.py", [
         lazy_problem().set_line(24).set_text("Changing the control variable i of a for loop has no effect.")
@@ -198,10 +192,10 @@
         lazy_problem().set_line(74),
         lazy_problem().set_line(77),
     ]),
 ])
 def test_changing_control_var_files(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=changing-control-variable")],
+        [Arg(Option.PYLINT, "--enable=changing-control-variable")],
         [problem.set_code("R6304") for problem in expected_output]
     )
```

### Comparing `edulint-2.7.1/tests/test_lint.py` & `edulint-2.8.0/tests/test_lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         lazy_problem().set_code("F401").set_line(1),
         lazy_problem().set_code("E501").set_line(1),
         lazy_problem().set_code("W293").set_line(19),
         lazy_problem().set_code("E303").set_line(22),
     ])
 ])
 def test_lint_basic(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
-    apply_and_lint(filename, args, expected_output)
+    apply_and_lint(filename, args + [Arg(Option.FLAKE8, "--extend-ignore=E721")], expected_output, from_empty=False)
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("z202817-zkouska.py", [Arg(Option.ENHANCEMENT, "on")], [
         lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6208").set_line(76),
@@ -76,15 +76,15 @@
         lazy_problem().set_line(343).set_code("R0915"),
         lazy_problem().set_line(387).set_code("R1702"),
         lazy_problem().set_line(387).set_code("R1702"),
         lazy_problem().set_line(387).set_code("R1702"),
     ])
 ])
 def test_translations(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
-    apply_and_lint(filename, args, expected_output)
+    apply_and_lint(filename, args + [Arg(Option.FLAKE8, "--extend-ignore=E721")], expected_output, from_empty=False)
 
 
 class TestIB111Week:
     @pytest.mark.parametrize("lines,args,expected_output", [
         ([
             "def swap(a, b):",
             "    tmp = a",
@@ -117,15 +117,15 @@
             "        return True",
             "    return False"
         ], [Arg(Option.PYTHON_SPECIFIC, "on"), Arg(Option.IB111_WEEK, "7"), Arg(Option.PYLINT, "--disable=R6201")], [
             lazy_problem().set_code("R1714").set_line(2),
         ])
     ])
     def test_ib111_week_custom(self, lines: List[str], args: List[Arg], expected_output: List[Problem]) -> None:
-        create_apply_and_lint(lines, args, expected_output)
+        create_apply_and_lint(lines, args, expected_output, from_empty=False)
 
 
 @pytest.mark.parametrize("lines,expected_output", [
     ([
         "class A:",
         "    pass"
     ], []),
@@ -211,15 +211,15 @@
     ([
         "global_variable = 1"
     ], [lazy_problem().set_line(1)]),
 ])
 def test_invalid_name_custom(lines: List[str], expected_output: List[Problem]) -> None:
     create_apply_and_lint(
         lines,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=invalid-name"), Arg(Option.NO_FLAKE8, "on")],
+        [Arg(Option.PYLINT, "--enable=invalid-name")],
         expected_output
     )
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("014186-p2_nested.py", [Arg(Option.PYTHON_SPECIFIC, "on")], [
         lazy_problem().set_code("C0103").set_line(20),
@@ -231,15 +231,15 @@
         lazy_problem().set_code("W0622").set_line(48),
     ]),
     ("custom_pep_assign.py", [Arg(Option.PYTHON_SPECIFIC, "on")], [
         lazy_problem().set_code("C0103").set_line(1),
     ])
 ])
 def test_invalid_name(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
-    apply_and_lint(filename, args, expected_output)
+    apply_and_lint(filename, args, expected_output, from_empty=False)
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("014180-p5_fibsum.py", [Arg(Option.ALLOWED_ONECHAR_NAMES, "")], [
         lazy_problem().set_code("C0104").set_line(6),
         lazy_problem().set_code("C0104").set_line(14)
     ]),
@@ -251,25 +251,25 @@
     ]),
     ("014180-p5_fibsum.py", [Arg(Option.ALLOWED_ONECHAR_NAMES, "in")], [
     ])
 ])
 def test_allowed_onechar_names(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=disallowed-name")] + args,
+        [Arg(Option.PYLINT, "--enable=disallowed-name")] + args,
         expected_output
     )
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
-    ("105119-p5_template.py", [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=R1714")], [
+    ("105119-p5_template.py", [Arg(Option.PYLINT, "--enable=R1714")], [
         lazy_problem().set_code("R1714").set_line(22)
-        .set_text("Consider merging these comparisons with \"in\" to \"i not in '[]'\""),
+        .set_text("Consider merging these comparisons with 'in' by using 'i not in '[]''"),
         lazy_problem().set_code("R1714").set_line(35)
-        .set_text("Consider merging these comparisons with \"in\" to 'i in (1, 2, 3)'"),
+        .set_text("Consider merging these comparisons with 'in' by using 'i in (1, 2, 3)'"),
     ]),
 ])
 def test_consider_using_in(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
     apply_and_lint(filename, args, expected_output)
 
 
 class TestImproveFor:
@@ -330,15 +330,15 @@
             "        B.append(A[x])"
         ], [
         ])
     ])
     def test_improve_for_custom(self, lines: List[str], expected_output: List[Problem]) -> None:
         create_apply_and_lint(
             lines,
-            [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=improve-for-loop")],
+            [Arg(Option.PYLINT, "--enable=improve-for-loop")],
             expected_output
         )
 
     @pytest.mark.parametrize("filename,args,expected_output", [
         ("105119-p5_template.py", [Arg(Option.PYLINT, "--enable=use-foreach")], [
         ]),
         ("015080-p4_geometry.py", [Arg(Option.PYLINT, "--enable=use-foreach"),
@@ -357,15 +357,15 @@
         ("umime_count_a.py", [Arg(Option.PYLINT, "--enable=improve-for-loop"),
                               Arg(Option.FLAKE8, "--extend-ignore=E225")], [
             lazy_problem().set_code("R6101").set_line(3)
             .set_text("Iterate directly: \"for var in text\" (with appropriate name for \"var\")"),
         ]),
     ])
     def test_improve_for(self, filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
-        apply_and_lint(filename, [Arg(Option.PYLINT, "--disable=all")] + args, expected_output)
+        apply_and_lint(filename, args, expected_output)
 
 
 class TestPyTA:
     @pytest.mark.parametrize("lines,expected_output", [
         ([
             "from typing import Tuple",
 
@@ -378,17 +378,15 @@
         ], [
             lazy_problem().set_line(1)
         ]),
     ])
     def test_forbidden_toplevel_code_custom(self, lines: List[str], expected_output: List[Problem]) -> None:
         create_apply_and_lint(
             lines,
-            [Arg(Option.PYLINT, "--disable=all"),
-             Arg(Option.PYLINT, "--enable=forbidden-top-level-code"),
-             Arg(Option.NO_FLAKE8, "on")],
+            [Arg(Option.PYLINT, "--enable=forbidden-top-level-code")],
             [p.set_code("E9992") for p in expected_output]
         )
 
 
 class TestNoGlobals:
     @pytest.mark.parametrize("lines,expected_output", [
         ([
@@ -440,17 +438,15 @@
             "    test = 2",
         ], [
         ]),
     ])
     def test_no_globals_custom(self, lines: List[str], expected_output: List[Problem]) -> None:
         create_apply_and_lint(
             lines,
-            [Arg(Option.PYLINT, "--disable=all"),
-             Arg(Option.PYLINT, "--enable=no-global-variables"),
-             Arg(Option.NO_FLAKE8, "on")],
+            [Arg(Option.PYLINT, "--enable=no-global-variables")],
             [p.set_code("R6401") for p in expected_output]
         )
 
     @pytest.mark.parametrize("filename,expected_output", [
         ("054141-p1_database.py", []),
         ("054103-p1_database.py", []),
         ("hw14699.py", []),
@@ -466,43 +462,43 @@
         ]),
         ("088952-p2_extremes.py", []),
         ("s10265-d_mancala.py", []),
     ])
     def test_no_globals_files(self, filename: str, expected_output: List[Problem]) -> None:
         apply_and_lint(
             filename,
-            [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=no-global-variables")],
+            [Arg(Option.PYLINT, "--enable=no-global-variables")],
             expected_output
         )
 
 
 class TestLongCode:
     @pytest.mark.parametrize("filename,expected_output", [
         ("hw48505.py", [
             lazy_problem().set_line(80),
             lazy_problem().set_line(196),
         ]),
     ])
     def test_long_function_files(self, filename: str, expected_output: List[Problem]) -> None:
         apply_and_lint(
             filename,
-            [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=long-function")],
+            [Arg(Option.PYLINT, "--enable=long-function")],
             expected_output
         )
 
     @pytest.mark.parametrize("filename,expected_output", [
         ("014422-next.py", [
             lazy_problem().set_line(19)
         ]),
         ("023240-cards.py", []),
     ])
     def test_use_early_return(self, filename: str, expected_output: List[Problem]) -> None:
         apply_and_lint(
             filename,
-            [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=use-early-return")],
+            [Arg(Option.PYLINT, "--enable=use-early-return")],
             expected_output
         )
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("umime_count_a.py", [
         Arg(Option.PYTHON_SPECIFIC, "on"),
@@ -523,25 +519,25 @@
         Arg(Option.PYTHON_SPECIFIC, "on"),
         Arg(Option.ALLOWED_ONECHAR_NAMES, ""),
         Arg(Option.ENHANCEMENT, "on"),
     ], [
         lazy_problem().set_code("R6201").set_line(2)
         .set_text("The if statement can be replaced with 'return ch == 'a' or ch == 'A''"),
         lazy_problem().set_code("R1714").set_line(2)
-        .set_text("Consider merging these comparisons with \"in\" to \"ch in 'aA'\""),
+        .set_text("Consider merging these comparisons with 'in' by using 'ch in 'aA''"),
         lazy_problem().set_code("C0104").set_line(9)
         .set_text("Disallowed single-character variable name \"a\", choose a more descriptive name"),
         lazy_problem().set_code("R6101").set_line(10)
         .set_text("Iterate directly: \"for var in text\" (with appropriate name for \"var\")"),
         lazy_problem().set_code("R6609").set_line(12)
         .set_text("Use augmenting assignment: 'a += 1'"),
     ])
 ])
 def test_umime_count_a(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
-    apply_and_lint(filename, args, expected_output)
+    apply_and_lint(filename, args, expected_output, from_empty=False)
 
 
 @pytest.mark.parametrize("lines,expected_output", [
     ([
         "def fun():",
         "    return 42",
         "    pass"
@@ -549,15 +545,16 @@
         lazy_problem().set_code("W0101")
     ]),
 ])
 def test_overrides_custom(lines: List[str], expected_output: List[Problem]) -> None:
     create_apply_and_lint(
         lines,
         [Arg(Option.NO_FLAKE8, "on")],
-        expected_output
+        expected_output,
+        from_empty=False
     )
 
 
 @pytest.mark.filterwarnings("ignore:The 'default' argument to fields is deprecated. Use 'dump_default' instead.")
 def test_problem_can_be_dumped_to_json() -> None:
     problem = Problem(source=Linter.FLAKE8, path='path', line=5, column=1, code='E303',
                       text='too many blank lines (3)', end_line=None, end_column=None)
```

### Comparing `edulint-2.7.1/tests/test_main.py` & `edulint-2.8.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.7.1/tests/test_short_problems.py` & `edulint-2.8.0/tests/test_short_problems.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,15 @@
             "    print('foobar')"
         ], [
         ]),
     ])
     def test_short_custom(self, lines: List[str], expected_output: List[Problem]) -> None:
         create_apply_and_lint(
             lines,
-            [Arg(Option.PYLINT, "--disable=all"),
-             Arg(Option.PYLINT, "--enable=short-problems"),
-             Arg(Option.NO_FLAKE8, "on")],
+            [Arg(Option.PYLINT, "--enable=short-problems")],
             expected_output
         )
 
     @pytest.mark.parametrize("lines,expected_output", [
         ([
             "def foo(a):",
             "    a = a + 1",
@@ -72,32 +70,28 @@
             "def foo(a):",
             "    a = a & {'a'}",
         ], []),
     ])
     def test_augassign_custom(self, lines: List[str], expected_output: List[Problem]) -> None:
         create_apply_and_lint(
             lines,
-            [Arg(Option.PYLINT, "--disable=all"),
-             Arg(Option.PYLINT, "--enable=use-augmenting-assignment"),
-             Arg(Option.NO_FLAKE8, "on")],
+            [Arg(Option.PYLINT, "--enable=use-augmenting-assignment")],
             [problem.set_code("R6609") for problem in expected_output]
         )
 
     @pytest.mark.parametrize("lines,expected_output", [
         (["1 is True"], [lazy_problem()]),
         (["1 is not True"], [lazy_problem()]),
         (["1 is None"], []),
         (["1 is not None"], []),
     ])
     def test_no_is_custom(self, lines: List[str], expected_output: List[Problem]) -> None:
         create_apply_and_lint(
             lines,
-            [Arg(Option.PYLINT, "--disable=all"),
-             Arg(Option.PYLINT, "--enable=no-is-bool"),
-             Arg(Option.NO_FLAKE8, "on")],
+            [Arg(Option.PYLINT, "--enable=no-is-bool")],
             [problem.set_code("R6613") for problem in expected_output]
         )
 
     @pytest.mark.parametrize("filename,expected_output", [
         ("044050-vigenere.py", [
             lazy_problem().set_code("R6614").set_line(38)
             .set_text("Use \"ord('A')\" instead of using the magical constant 65."),
@@ -142,16 +136,14 @@
             lazy_problem().set_code("R6614").set_line(178),
         ]),
     ])
     def test_ord_files(self, filename: str, expected_output: List[Problem]) -> None:
         apply_and_lint(
             filename,
             [
-                Arg(Option.NO_FLAKE8, "on"),
-                Arg(Option.PYLINT, "--disable=all"),
                 Arg(Option.PYLINT, "--enable=use-ord-letter,use-literal-letter")
             ],
             expected_output
         )
 
     @pytest.mark.parametrize("filename,expected_output", [
         ("010666-prime.py", [
@@ -302,14 +294,10 @@
             lazy_problem().set_code("R6608").set_line(64).set_text("Redundant arithmetic: valid += 0"),
         ]),
         ("ut_157_0762_16_47.py", []),
     ])
     def test_short_files(self, filename: str, expected_output: List[Problem]) -> None:
         apply_and_lint(
             filename,
-            [
-                Arg(Option.NO_FLAKE8, "on"),
-                Arg(Option.PYLINT, "--disable=all"),
-                Arg(Option.PYLINT, "--enable=short-problems")
-            ],
+            [Arg(Option.PYLINT, "--enable=short-problems")],
             expected_output
         )
```

### Comparing `edulint-2.7.1/tests/test_simplifiable_if.py` & `edulint-2.8.0/tests/test_simplifiable_if.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from utils import lazy_problem, apply_and_lint, create_apply_and_lint
 from typing import List
 
 
 def _test_simplify_if(lines: List[str], expected_output: List[Problem], code: str) -> None:
     create_apply_and_lint(
         lines,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, f"--enable={code}"), Arg(Option.NO_FLAKE8, "on")],
+        [Arg(Option.PYLINT, f"--enable={code}")],
         [p.set_code(code) for p in expected_output]
     )
 
 
 @pytest.mark.parametrize("lines,expected_output", [
     ([
         "def yyy(x):",
@@ -505,10 +505,10 @@
     ]),
     ("024423-p5_credit.py", []),
     ("044669-p3_person_id.py", [lazy_problem().set_code("R6206").set_line(30)])
 ])
 def test_simplify_if_files(filename: str, expected_output: List[Problem]) -> None:
     apply_and_lint(
         filename,
-        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=simplifiable-if")],
+        [Arg(Option.PYLINT, "--enable=simplifiable-if")],
         expected_output
     )
```

### Comparing `edulint-2.7.1/tests/test_visitors.py` & `edulint-2.8.0/tests/test_visitors.py`

 * *Files identical despite different names*

