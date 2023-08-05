# Comparing `tmp/manageprojects-0.9.8.tar.gz` & `tmp/manageprojects-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manageprojects-0.9.8.tar", last modified: Tue Apr  4 10:00:18 2023, max compression
+gzip compressed data, was "manageprojects-0.9.9.tar", last modified: Tue Apr  4 17:17:50 2023, max compression
```

## Comparing `manageprojects-0.9.8.tar` & `manageprojects-0.9.9.tar`

### file list

```diff
@@ -1,68 +1,80 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-04 10:00:18.495540 manageprojects-0.9.8/
--rw-rw-r--   0 jens      (1000) users      (100)    35149 2023-01-12 16:49:28.000000 manageprojects-0.9.8/LICENSE
--rw-rw-r--   0 jens      (1000) users      (100)    18041 2023-04-04 10:00:18.495540 manageprojects-0.9.8/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    17647 2023-03-17 07:18:26.000000 manageprojects-0.9.8/README.md
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-04 10:00:18.491540 manageprojects-0.9.8/manageprojects/
--rw-rw-r--   0 jens      (1000) users      (100)      144 2023-04-04 09:58:15.000000 manageprojects-0.9.8/manageprojects/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      204 2023-01-12 16:48:16.000000 manageprojects-0.9.8/manageprojects/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-04 10:00:18.495540 manageprojects-0.9.8/manageprojects/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-01-12 16:48:16.000000 manageprojects-0.9.8/manageprojects/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    17456 2023-04-04 09:58:15.000000 manageprojects-0.9.8/manageprojects/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)      967 2023-03-17 07:22:16.000000 manageprojects-0.9.8/manageprojects/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     4066 2023-02-18 16:35:05.000000 manageprojects-0.9.8/manageprojects/cookiecutter_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     3011 2023-04-04 09:58:15.000000 manageprojects-0.9.8/manageprojects/cookiecutter_generator.py
--rw-rw-r--   0 jens      (1000) users      (100)     9910 2023-04-04 09:58:15.000000 manageprojects-0.9.8/manageprojects/cookiecutter_templates.py
--rw-rw-r--   0 jens      (1000) users      (100)     1541 2023-01-25 06:36:05.000000 manageprojects-0.9.8/manageprojects/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)      201 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)     8590 2023-02-28 15:32:24.000000 manageprojects-0.9.8/manageprojects/format_file.py
--rw-rw-r--   0 jens      (1000) users      (100)    11995 2023-02-21 09:20:07.000000 manageprojects-0.9.8/manageprojects/git.py
--rw-rw-r--   0 jens      (1000) users      (100)     3378 2023-01-25 09:03:33.000000 manageprojects-0.9.8/manageprojects/overwrite.py
--rw-rw-r--   0 jens      (1000) users      (100)     7011 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/patching.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-04 10:00:18.495540 manageprojects-0.9.8/manageprojects/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1819 2023-02-26 12:08:59.000000 manageprojects-0.9.8/manageprojects/test_utils/click_cli_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1153 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/test_utils/git_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1136 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/test_utils/logs.py
--rw-rw-r--   0 jens      (1000) users      (100)     4338 2023-02-19 17:03:43.000000 manageprojects-0.9.8/manageprojects/test_utils/project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2436 2023-02-21 09:20:07.000000 manageprojects-0.9.8/manageprojects/test_utils/subprocess.py
--rw-rw-r--   0 jens      (1000) users      (100)      577 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/test_utils/temp_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-04 10:00:18.495540 manageprojects-0.9.8/manageprojects/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      199 2023-03-17 07:22:20.000000 manageprojects-0.9.8/manageprojects/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2282 2023-02-21 09:20:07.000000 manageprojects-0.9.8/manageprojects/tests/base.py
--rw-rw-r--   0 jens      (1000) users      (100)     2788 2023-03-12 19:13:29.000000 manageprojects-0.9.8/manageprojects/tests/test_cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      840 2023-02-26 12:15:11.000000 manageprojects-0.9.8/manageprojects/tests/test_click_cli_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2020 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/tests/test_cookiecutter_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     2781 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/tests/test_cookiecutter_generator.py
--rw-rw-r--   0 jens      (1000) users      (100)    12989 2023-01-14 15:00:15.000000 manageprojects-0.9.8/manageprojects/tests/test_cookiecutter_templates.py
--rw-rw-r--   0 jens      (1000) users      (100)      223 2023-03-07 15:26:51.000000 manageprojects-0.9.8/manageprojects/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     9758 2023-02-21 09:20:07.000000 manageprojects-0.9.8/manageprojects/tests/test_format_file.py
--rw-rw-r--   0 jens      (1000) users      (100)    13633 2023-02-21 09:20:07.000000 manageprojects-0.9.8/manageprojects/tests/test_git.py
--rw-rw-r--   0 jens      (1000) users      (100)     7992 2023-01-25 09:05:18.000000 manageprojects-0.9.8/manageprojects/tests/test_overwrite.py
--rw-rw-r--   0 jens      (1000) users      (100)     5934 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/tests/test_patching.py
--rw-rw-r--   0 jens      (1000) users      (100)     2357 2023-03-17 07:25:07.000000 manageprojects-0.9.8/manageprojects/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2628 2023-02-19 10:05:35.000000 manageprojects-0.9.8/manageprojects/tests/test_readme.py
--rw-rw-r--   0 jens      (1000) users      (100)     6746 2023-03-12 19:11:17.000000 manageprojects-0.9.8/manageprojects/tests/test_utilities_publish.py
--rw-rw-r--   0 jens      (1000) users      (100)    10707 2023-02-18 16:16:04.000000 manageprojects-0.9.8/manageprojects/tests/test_utilities_pyproject_toml.py
--rw-rw-r--   0 jens      (1000) users      (100)      742 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/tests/test_utilities_temp_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1679 2023-02-18 19:30:44.000000 manageprojects-0.9.8/manageprojects/tests/test_version_info.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-04 10:00:18.495540 manageprojects-0.9.8/manageprojects/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-01-12 16:51:36.000000 manageprojects-0.9.8/manageprojects/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1237 2023-02-18 18:05:37.000000 manageprojects-0.9.8/manageprojects/utilities/code_style.py
--rw-rw-r--   0 jens      (1000) users      (100)      608 2023-01-12 16:51:37.000000 manageprojects-0.9.8/manageprojects/utilities/cookiecutter_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      490 2023-01-12 16:51:37.000000 manageprojects-0.9.8/manageprojects/utilities/gitignore.py
--rw-rw-r--   0 jens      (1000) users      (100)     1848 2023-01-12 16:51:37.000000 manageprojects-0.9.8/manageprojects/utilities/log_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     8653 2023-03-12 18:15:32.000000 manageprojects-0.9.8/manageprojects/utilities/publish.py
--rw-rw-r--   0 jens      (1000) users      (100)     4553 2023-02-19 09:48:09.000000 manageprojects-0.9.8/manageprojects/utilities/pyproject_toml.py
--rw-rw-r--   0 jens      (1000) users      (100)     6560 2023-02-21 09:20:07.000000 manageprojects-0.9.8/manageprojects/utilities/subprocess_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      999 2023-01-12 16:51:37.000000 manageprojects-0.9.8/manageprojects/utilities/temp_path.py
--rw-rw-r--   0 jens      (1000) users      (100)      827 2023-01-12 16:51:37.000000 manageprojects-0.9.8/manageprojects/utilities/user_config.py
--rw-rw-r--   0 jens      (1000) users      (100)     1052 2023-02-18 19:31:13.000000 manageprojects-0.9.8/manageprojects/utilities/version_info.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-04 10:00:18.495540 manageprojects-0.9.8/manageprojects.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    18041 2023-04-04 10:00:18.000000 manageprojects-0.9.8/manageprojects.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     2161 2023-04-04 10:00:18.000000 manageprojects-0.9.8/manageprojects.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-04 10:00:18.000000 manageprojects-0.9.8/manageprojects.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       64 2023-04-04 10:00:18.000000 manageprojects-0.9.8/manageprojects.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      235 2023-04-04 10:00:18.000000 manageprojects-0.9.8/manageprojects.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       15 2023-04-04 10:00:18.000000 manageprojects-0.9.8/manageprojects.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4901 2023-03-17 07:23:34.000000 manageprojects-0.9.8/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-04 10:00:18.495540 manageprojects-0.9.8/setup.cfg
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.837991 manageprojects-0.9.9/
+-rw-rw-r--   0 jens      (1000) jens      (1000)      301 2023-02-20 12:13:04.000000 manageprojects-0.9.9/.editorconfig
+-rw-rw-r--   0 jens      (1000) jens      (1000)      153 2023-01-27 10:23:32.000000 manageprojects-0.9.9/.flake8
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.829990 manageprojects-0.9.9/.github/
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.833990 manageprojects-0.9.9/.github/workflows/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1457 2023-04-04 17:05:07.000000 manageprojects-0.9.9/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) jens      (1000)      108 2023-03-09 18:18:40.000000 manageprojects-0.9.9/.gitignore
+-rw-rw-r--   0 jens      (1000) jens      (1000)    35149 2023-01-27 10:23:32.000000 manageprojects-0.9.9/LICENSE
+-rw-rw-r--   0 jens      (1000) jens      (1000)    18029 2023-04-04 17:17:50.837991 manageprojects-0.9.9/PKG-INFO
+-rw-rw-r--   0 jens      (1000) jens      (1000)    17635 2023-04-04 17:13:11.000000 manageprojects-0.9.9/README.md
+-rwxrwxr-x   0 jens      (1000) jens      (1000)     3053 2023-03-25 09:18:51.000000 manageprojects-0.9.9/cli.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.833990 manageprojects-0.9.9/manageprojects/
+-rw-rw-r--   0 jens      (1000) jens      (1000)      144 2023-04-04 17:10:57.000000 manageprojects-0.9.9/manageprojects/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      204 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/__main__.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.833990 manageprojects-0.9.9/manageprojects/cli/
+-rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    17443 2023-04-04 17:12:08.000000 manageprojects-0.9.9/manageprojects/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      967 2023-04-04 17:05:24.000000 manageprojects-0.9.9/manageprojects/constants.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     4066 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/cookiecutter_api.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     3011 2023-04-04 16:55:04.000000 manageprojects-0.9.9/manageprojects/cookiecutter_generator.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     9910 2023-04-04 16:55:04.000000 manageprojects-0.9.9/manageprojects/cookiecutter_templates.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1541 2023-04-04 16:54:27.000000 manageprojects-0.9.9/manageprojects/data_classes.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      201 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/exceptions.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     8590 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/format_file.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    11995 2023-02-20 23:21:01.000000 manageprojects-0.9.9/manageprojects/git.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     3378 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/overwrite.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     7011 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/patching.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.833990 manageprojects-0.9.9/manageprojects/test_utils/
+-rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1819 2023-02-28 17:21:26.000000 manageprojects-0.9.9/manageprojects/test_utils/click_cli_utils.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1153 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/test_utils/git_utils.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1136 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/test_utils/logs.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     4338 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/test_utils/project_setup.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2436 2023-02-20 23:05:54.000000 manageprojects-0.9.9/manageprojects/test_utils/subprocess.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      577 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/test_utils/temp_utils.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.837991 manageprojects-0.9.9/manageprojects/tests/
+-rw-rw-r--   0 jens      (1000) jens      (1000)      199 2023-04-04 17:05:27.000000 manageprojects-0.9.9/manageprojects/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2282 2023-04-04 16:54:27.000000 manageprojects-0.9.9/manageprojects/tests/base.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2787 2023-04-04 17:12:34.000000 manageprojects-0.9.9/manageprojects/tests/test_cli.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      840 2023-02-28 17:21:26.000000 manageprojects-0.9.9/manageprojects/tests/test_click_cli_utils.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2020 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/tests/test_cookiecutter_api.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2781 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/tests/test_cookiecutter_generator.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    12989 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/tests/test_cookiecutter_templates.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      223 2023-03-09 18:18:40.000000 manageprojects-0.9.9/manageprojects/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     9758 2023-02-20 23:07:31.000000 manageprojects-0.9.9/manageprojects/tests/test_format_file.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    13633 2023-02-20 21:20:17.000000 manageprojects-0.9.9/manageprojects/tests/test_git.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      405 2023-02-20 15:36:01.000000 manageprojects-0.9.9/manageprojects/tests/test_git_git_apply_patch_1.snapshot.patch
+-rw-rw-r--   0 jens      (1000) jens      (1000)      228 2023-02-20 15:36:01.000000 manageprojects-0.9.9/manageprojects/tests/test_git_git_diff_1.snapshot.patch
+-rw-rw-r--   0 jens      (1000) jens      (1000)     7992 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/tests/test_overwrite.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     5934 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/tests/test_patching.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      290 2023-02-20 15:36:01.000000 manageprojects-0.9.9/manageprojects/tests/test_patching_make_git_diff_1.snapshot.patch
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2357 2023-04-04 17:05:30.000000 manageprojects-0.9.9/manageprojects/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2628 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     6746 2023-03-25 09:18:51.000000 manageprojects-0.9.9/manageprojects/tests/test_utilities_publish.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    10707 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/tests/test_utilities_pyproject_toml.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      742 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/tests/test_utilities_temp_utils.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1679 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/tests/test_version_info.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.837991 manageprojects-0.9.9/manageprojects/utilities/
+-rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1237 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/utilities/code_style.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      608 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/utilities/cookiecutter_utils.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      490 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/utilities/gitignore.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1848 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/utilities/log_utils.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     8653 2023-03-25 09:18:51.000000 manageprojects-0.9.9/manageprojects/utilities/publish.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     4553 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/utilities/pyproject_toml.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     6560 2023-03-28 17:05:20.000000 manageprojects-0.9.9/manageprojects/utilities/subprocess_utils.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      999 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/utilities/temp_path.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      827 2023-01-27 10:23:32.000000 manageprojects-0.9.9/manageprojects/utilities/user_config.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1052 2023-02-20 12:13:04.000000 manageprojects-0.9.9/manageprojects/utilities/version_info.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-04-04 17:17:50.833990 manageprojects-0.9.9/manageprojects.egg-info/
+-rw-rw-r--   0 jens      (1000) jens      (1000)    18029 2023-04-04 17:17:50.000000 manageprojects-0.9.9/manageprojects.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2452 2023-04-04 17:17:50.000000 manageprojects-0.9.9/manageprojects.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)        1 2023-04-04 17:17:50.000000 manageprojects-0.9.9/manageprojects.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)       64 2023-04-04 17:17:50.000000 manageprojects-0.9.9/manageprojects.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)      206 2023-04-04 17:17:50.000000 manageprojects-0.9.9/manageprojects.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)       15 2023-04-04 17:17:50.000000 manageprojects-0.9.9/manageprojects.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)     4821 2023-04-04 17:09:29.000000 manageprojects-0.9.9/pyproject.toml
+-rw-rw-r--   0 jens      (1000) jens      (1000)    50579 2023-04-04 17:10:02.000000 manageprojects-0.9.9/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)    19057 2023-04-04 17:09:43.000000 manageprojects-0.9.9/requirements.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)       38 2023-04-04 17:17:50.837991 manageprojects-0.9.9/setup.cfg
```

### Comparing `manageprojects-0.9.8/LICENSE` & `manageprojects-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/PKG-INFO` & `manageprojects-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manageprojects
-Version: 0.9.8
+Version: 0.9.9
 Summary: Manage Python / Django projects
 Author-email: Jens Diemer <mamageprojects@jensdiemer.de>
 Project-URL: Documentation, https://github.com/jedie/manageprojects
 Project-URL: Source, https://github.com/jedie/manageprojects
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -122,23 +122,23 @@
 
 [comment]: <> (✂✂✂ auto generated update-project help start ✂✂✂)
 ```
 Usage: ./cli.py update-project [OPTIONS] PROJECT_PATH
 
  Update a existing project.
  e.g. update by overwrite (and merge changes manually via git):
- ./cli.py update-project --overwrite ~/foo/bar/
+ ./cli.py update-project ~/foo/bar/
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --overwrite/--no-overwrite          Overwrite all Cookiecutter template files to the last        │
 │                                     template state and do not apply the changes via git patches. │
 │                                     The developer is supposed to apply the differences manually  │
 │                                     via git. Will be aborted if the project git repro is not in  │
 │                                     a clean state.                                               │
-│                                     [default: no-overwrite]                                      │
+│                                     [default: overwrite]                                         │
 │ --password                    TEXT  Cookiecutter Option: Password to use when extracting the     │
 │                                     repository                                                   │
 │ --config-file                 FILE  Cookiecutter Option: Optional path to                        │
 │                                     "cookiecutter_config.yaml"                                   │
 │ --input/--no-input                  Cookiecutter Option: Do not prompt for parameters and only   │
 │                                     use cookiecutter.json file content                           │
 │                                     [default: no-input]                                          │
```

### Comparing `manageprojects-0.9.8/README.md` & `manageprojects-0.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -110,23 +110,23 @@
 
 [comment]: <> (✂✂✂ auto generated update-project help start ✂✂✂)
 ```
 Usage: ./cli.py update-project [OPTIONS] PROJECT_PATH
 
  Update a existing project.
  e.g. update by overwrite (and merge changes manually via git):
- ./cli.py update-project --overwrite ~/foo/bar/
+ ./cli.py update-project ~/foo/bar/
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --overwrite/--no-overwrite          Overwrite all Cookiecutter template files to the last        │
 │                                     template state and do not apply the changes via git patches. │
 │                                     The developer is supposed to apply the differences manually  │
 │                                     via git. Will be aborted if the project git repro is not in  │
 │                                     a clean state.                                               │
-│                                     [default: no-overwrite]                                      │
+│                                     [default: overwrite]                                         │
 │ --password                    TEXT  Cookiecutter Option: Password to use when extracting the     │
 │                                     repository                                                   │
 │ --config-file                 FILE  Cookiecutter Option: Optional path to                        │
 │                                     "cookiecutter_config.yaml"                                   │
 │ --input/--no-input                  Cookiecutter Option: Do not prompt for parameters and only   │
 │                                     use cookiecutter.json file content                           │
 │                                     [default: no-input]                                          │
```

### Comparing `manageprojects-0.9.8/manageprojects/cli/cli_app.py` & `manageprojects-0.9.9/manageprojects/cli/cli_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 cli.add_command(start_project)
 
 
 @click.command()
 @click.argument('project_path', **ARGUMENT_EXISTING_DIR)
 @click.option(
     '--overwrite/--no-overwrite',
-    **OPTION_ARGS_DEFAULT_FALSE,
+    **OPTION_ARGS_DEFAULT_TRUE,
     help=(
         'Overwrite all Cookiecutter template files to the last template state and'
         ' do not apply the changes via git patches.'
         ' The developer is supposed to apply the differences manually via git.'
         ' Will be aborted if the project git repro is not in a clean state.'
     ),
 )
@@ -294,15 +294,15 @@
     cleanup: bool,
 ):
     """
     Update a existing project.
 
     e.g. update by overwrite (and merge changes manually via git):
 
-    ./cli.py update-project --overwrite ~/foo/bar/
+    ./cli.py update-project ~/foo/bar/
     """
     log_config()
     print(f'Update project: "{project_path}"...')
     update_managed_project(
         project_path=project_path,
         overwrite=overwrite,
         password=password,
```

### Comparing `manageprojects-0.9.8/manageprojects/constants.py` & `manageprojects-0.9.9/manageprojects/constants.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/cookiecutter_api.py` & `manageprojects-0.9.9/manageprojects/cookiecutter_api.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/cookiecutter_generator.py` & `manageprojects-0.9.9/manageprojects/cookiecutter_generator.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/cookiecutter_templates.py` & `manageprojects-0.9.9/manageprojects/cookiecutter_templates.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/data_classes.py` & `manageprojects-0.9.9/manageprojects/data_classes.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/format_file.py` & `manageprojects-0.9.9/manageprojects/format_file.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/git.py` & `manageprojects-0.9.9/manageprojects/git.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/overwrite.py` & `manageprojects-0.9.9/manageprojects/overwrite.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/patching.py` & `manageprojects-0.9.9/manageprojects/patching.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/test_utils/click_cli_utils.py` & `manageprojects-0.9.9/manageprojects/test_utils/click_cli_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/test_utils/git_utils.py` & `manageprojects-0.9.9/manageprojects/test_utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/test_utils/logs.py` & `manageprojects-0.9.9/manageprojects/test_utils/logs.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/test_utils/project_setup.py` & `manageprojects-0.9.9/manageprojects/test_utils/project_setup.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/test_utils/subprocess.py` & `manageprojects-0.9.9/manageprojects/test_utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/test_utils/temp_utils.py` & `manageprojects-0.9.9/manageprojects/test_utils/temp_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/base.py` & `manageprojects-0.9.9/manageprojects/tests/base.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_cli.py` & `manageprojects-0.9.9/manageprojects/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         tempdir = tempfile.gettempdir()
 
         with mock.patch.object(cli_app, 'update_managed_project') as m:
             stdout = invoke_click(update_project, tempdir)
 
         m.assert_called_once_with(
             project_path=Path(tempdir),
-            overwrite=False,
+            overwrite=True,
             password=None,
             config_file=None,
             cleanup=True,
             input=False,
         )
         self.assert_in_content(
             got=stdout,
```

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_click_cli_utils.py` & `manageprojects-0.9.9/manageprojects/tests/test_click_cli_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_cookiecutter_api.py` & `manageprojects-0.9.9/manageprojects/tests/test_cookiecutter_api.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_cookiecutter_generator.py` & `manageprojects-0.9.9/manageprojects/tests/test_cookiecutter_generator.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_cookiecutter_templates.py` & `manageprojects-0.9.9/manageprojects/tests/test_cookiecutter_templates.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_format_file.py` & `manageprojects-0.9.9/manageprojects/tests/test_format_file.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_git.py` & `manageprojects-0.9.9/manageprojects/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_overwrite.py` & `manageprojects-0.9.9/manageprojects/tests/test_overwrite.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_patching.py` & `manageprojects-0.9.9/manageprojects/tests/test_patching.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_project_setup.py` & `manageprojects-0.9.9/manageprojects/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_readme.py` & `manageprojects-0.9.9/manageprojects/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_utilities_publish.py` & `manageprojects-0.9.9/manageprojects/tests/test_utilities_publish.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_utilities_pyproject_toml.py` & `manageprojects-0.9.9/manageprojects/tests/test_utilities_pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_utilities_temp_utils.py` & `manageprojects-0.9.9/manageprojects/tests/test_utilities_temp_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/tests/test_version_info.py` & `manageprojects-0.9.9/manageprojects/tests/test_version_info.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/code_style.py` & `manageprojects-0.9.9/manageprojects/utilities/code_style.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/cookiecutter_utils.py` & `manageprojects-0.9.9/manageprojects/utilities/cookiecutter_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/log_utils.py` & `manageprojects-0.9.9/manageprojects/utilities/log_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/publish.py` & `manageprojects-0.9.9/manageprojects/utilities/publish.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/pyproject_toml.py` & `manageprojects-0.9.9/manageprojects/utilities/pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/subprocess_utils.py` & `manageprojects-0.9.9/manageprojects/utilities/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/temp_path.py` & `manageprojects-0.9.9/manageprojects/utilities/temp_path.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/user_config.py` & `manageprojects-0.9.9/manageprojects/utilities/user_config.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects/utilities/version_info.py` & `manageprojects-0.9.9/manageprojects/utilities/version_info.py`

 * *Files identical despite different names*

### Comparing `manageprojects-0.9.8/manageprojects.egg-info/PKG-INFO` & `manageprojects-0.9.9/manageprojects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manageprojects
-Version: 0.9.8
+Version: 0.9.9
 Summary: Manage Python / Django projects
 Author-email: Jens Diemer <mamageprojects@jensdiemer.de>
 Project-URL: Documentation, https://github.com/jedie/manageprojects
 Project-URL: Source, https://github.com/jedie/manageprojects
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -122,23 +122,23 @@
 
 [comment]: <> (✂✂✂ auto generated update-project help start ✂✂✂)
 ```
 Usage: ./cli.py update-project [OPTIONS] PROJECT_PATH
 
  Update a existing project.
  e.g. update by overwrite (and merge changes manually via git):
- ./cli.py update-project --overwrite ~/foo/bar/
+ ./cli.py update-project ~/foo/bar/
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --overwrite/--no-overwrite          Overwrite all Cookiecutter template files to the last        │
 │                                     template state and do not apply the changes via git patches. │
 │                                     The developer is supposed to apply the differences manually  │
 │                                     via git. Will be aborted if the project git repro is not in  │
 │                                     a clean state.                                               │
-│                                     [default: no-overwrite]                                      │
+│                                     [default: overwrite]                                         │
 │ --password                    TEXT  Cookiecutter Option: Password to use when extracting the     │
 │                                     repository                                                   │
 │ --config-file                 FILE  Cookiecutter Option: Optional path to                        │
 │                                     "cookiecutter_config.yaml"                                   │
 │ --input/--no-input                  Cookiecutter Option: Do not prompt for parameters and only   │
 │                                     use cookiecutter.json file content                           │
 │                                     [default: no-input]                                          │
```

### Comparing `manageprojects-0.9.8/manageprojects.egg-info/SOURCES.txt` & `manageprojects-0.9.9/manageprojects.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+.editorconfig
+.flake8
+.gitignore
 LICENSE
 README.md
+cli.py
 pyproject.toml
+requirements.dev.txt
+requirements.txt
+.github/workflows/tests.yml
 manageprojects/__init__.py
 manageprojects/__main__.py
 manageprojects/constants.py
 manageprojects/cookiecutter_api.py
 manageprojects/cookiecutter_generator.py
 manageprojects/cookiecutter_templates.py
 manageprojects/data_classes.py
@@ -34,16 +41,19 @@
 manageprojects/tests/test_click_cli_utils.py
 manageprojects/tests/test_cookiecutter_api.py
 manageprojects/tests/test_cookiecutter_generator.py
 manageprojects/tests/test_cookiecutter_templates.py
 manageprojects/tests/test_doctests.py
 manageprojects/tests/test_format_file.py
 manageprojects/tests/test_git.py
+manageprojects/tests/test_git_git_apply_patch_1.snapshot.patch
+manageprojects/tests/test_git_git_diff_1.snapshot.patch
 manageprojects/tests/test_overwrite.py
 manageprojects/tests/test_patching.py
+manageprojects/tests/test_patching_make_git_diff_1.snapshot.patch
 manageprojects/tests/test_project_setup.py
 manageprojects/tests/test_readme.py
 manageprojects/tests/test_utilities_publish.py
 manageprojects/tests/test_utilities_pyproject_toml.py
 manageprojects/tests/test_utilities_temp_utils.py
 manageprojects/tests/test_version_info.py
 manageprojects/utilities/__init__.py
```

### Comparing `manageprojects-0.9.8/pyproject.toml` & `manageprojects-0.9.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -10,52 +10,52 @@
 dependencies = [
     "cookiecutter",
     "tomlkit",
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
-    "packaging",  # https://github.com/pypa/packaging
-    "darker>=1.7",  # https://github.com/akaihola/darker
+]
+[project.optional-dependencies]
+dev = [
+    "pip-tools",  # https://github.com/jazzband/pip-tools/
+    "tox>=4.4.5",  # https://github.com/tox-dev/tox
+    "coveralls",  # https://github.com/TheKevJames/coveralls-python
+    "twine",  # https://github.com/pypa/twine
+    "pdoc", # Because: https://github.com/boxine/bx_py_utils/issues/157
     "autopep8",  # https://github.com/hhatto/autopep8
     "pyupgrade",  # https://github.com/asottile/pyupgrade
-    "isort",  # https://github.com/pycqa/isort
-    "flynt",  # https://github.com/ikamensh/flynt
     "flake8",  # https://github.com/pycqa/flake8
     "pyflakes",  # https://github.com/PyCQA/pyflakes
     "codespell",  # https://github.com/codespell-project/codespell
     "EditorConfig",  # https://github.com/editorconfig/editorconfig-core-py
     "mypy",  # https://github.com/python/mypy
     "safety",  # https://github.com/pyupio/safety
+
+    # https://github.com/akaihola/darker
+    # https://github.com/ikamensh/flynt
+    # https://github.com/pycqa/isort
+    # https://github.com/pygments/pygments
+    "darker[flynt, isort, color]",
+
     "tomli",  # https://github.com/hukkin/tomli
-    #
     # tomli only needed for Python <3.11, but see bug:
     # https://github.com/pypa/pip/issues/9644#issuecomment-1456583402
     #"tomli;python_version<\"3.11\"",  # https://github.com/hukkin/tomli
 ]
-[project.optional-dependencies]
-dev = [
-    "pip-tools",  # https://github.com/jazzband/pip-tools/
-    "tox>=4.4.5",  # https://github.com/tox-dev/tox
-    "coveralls",  # https://github.com/TheKevJames/coveralls-python
-    "tomli",  # https://github.com/hukkin/tomli
-    "twine",  # https://github.com/pypa/twine
-    "poetry-publish",  # https://github.com/jedie/poetry-publish
-    "pdoc", # Because: https://github.com/boxine/bx_py_utils/issues/157
-]
 
 [project.urls]
 Documentation = "https://github.com/jedie/manageprojects"
 Source = "https://github.com/jedie/manageprojects"
 
 [project.scripts]
 manageprojects = "manageprojects.__main__:main"
 
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "setuptools_scm>=7.1"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["manageprojects*"]
 
 [tool.setuptools.dynamic]
@@ -89,14 +89,15 @@
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
@@ -132,33 +133,30 @@
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
 allow_redefinition = true  # https://github.com/python/mypy/issues/7165
 show_error_codes = true
 plugins = []
-exclude = [
-    '.venv',
-    'tests',
-    'manageprojects/project_templates',
-]
+exclude = ['.venv', 'tests']
 
 
 [manageprojects] # https://github.com/jedie/manageprojects
 initial_revision = "8438598"
 initial_date = 2022-11-20T20:01:37+01:00
 cookiecutter_template = "https://github.com/jedie/cookiecutter_templates"
 cookiecutter_directory = "piptools-python"
 applied_migrations = [
     "cf44769", # 2023-01-11T08:15:06+01:00
     "cd164cd", # 2023-02-18T11:55:57+01:00
     "d970456", # 2023-02-20T16:19:35+01:00
     "80d0a0c", # 2023-03-06T17:52:14+01:00
     "04d5a25", # 2023-03-07T16:25:36+01:00
     "be96b03", # 2023-03-17T08:17:11+01:00
+    "588caaa", # 2023-04-04T15:40:44+02:00
 ]
 
 [manageprojects.cookiecutter_context.cookiecutter]
 full_name = "Jens Diemer"
 github_username = "jedie"
 author_email = "mamageprojects@jensdiemer.de"
 package_name = "manageprojects"
```

