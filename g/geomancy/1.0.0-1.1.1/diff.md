# Comparing `tmp/geomancy-1.0.0.tar.gz` & `tmp/geomancy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-1.0.0.tar", last modified: Wed Aug  2 21:34:17 2023, max compression
+gzip compressed data, was "geomancy-1.1.1.tar", last modified: Sat Aug  5 17:13:58 2023, max compression
```

## Comparing `geomancy-1.0.0.tar` & `geomancy-1.1.1.tar`

### file list

```diff
@@ -1,112 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.514897 geomancy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 21:34:06.000000 geomancy-1.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 21:34:06.000000 geomancy-1.0.0/.geomancy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.494896 geomancy-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-02 21:34:06.000000 geomancy-1.0.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 21:34:06.000000 geomancy-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-02 21:34:06.000000 geomancy-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 21:34:06.000000 geomancy-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-02 21:34:06.000000 geomancy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-08-02 21:34:17.510897 geomancy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-08-02 21:34:06.000000 geomancy-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-02 21:34:06.000000 geomancy-1.0.0/Taskfile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-02 21:34:06.000000 geomancy-1.0.0/changelog/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    49829 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/_static/geomancy_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/_static/geomancy_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/about/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/about/api/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/about/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/about/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/checks/aws.md
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/checks/core.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/checks/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/checks/snippets/base_args.md
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/guides/tips_and_tricks.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/usage/cmd_checks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/usage/cmd_run.md
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/usage/format.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/examples/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/aws/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/aws/geomancy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/geomancy.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/geomancy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/geomancy/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/__description__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/checks/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/config/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/environment/dotenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/geomancy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-02 21:34:06.000000 geomancy-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:34:17.514897 geomancy-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/checks/aws/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.494896 geomancy-1.0.0/tests/checks/aws/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/config/config1.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/data/test.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/entrypoints/test_geo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/environment/test_dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.360191 geomancy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-05 17:13:44.000000 geomancy-1.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-05 17:13:44.000000 geomancy-1.1.1/.geomancy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.336192 geomancy-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-05 17:13:44.000000 geomancy-1.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-05 17:13:44.000000 geomancy-1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-05 17:13:44.000000 geomancy-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-05 17:13:44.000000 geomancy-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-05 17:13:44.000000 geomancy-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-05 17:13:58.360191 geomancy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-05 17:13:44.000000 geomancy-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-05 17:13:44.000000 geomancy-1.1.1/Taskfile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-05 17:13:44.000000 geomancy-1.1.1/changelog/_template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    49829 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/_static/geomancy_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/_static/geomancy_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/about/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/about/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/about/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/about/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/guides/tips_and_tricks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/iam.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/s3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/aws/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/snippets/common_args.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/env.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/exec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/path.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/platform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/python.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/snippets/common_args.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/cmd_checks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/cmd_run.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/format.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/examples/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/aws/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/geomancy.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/geomancy/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/__description__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/geomancy/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/environment/dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/geomancy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 17:13:44.000000 geomancy-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:13:58.360191 geomancy-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.352192 geomancy-1.1.1/tests/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.352192 geomancy-1.1.1/tests/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/tests/checks/aws/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.352192 geomancy-1.1.1/tests/checks/aws/cassettes/test_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/test_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/config/config1.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/data/test.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/entrypoints/test_geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/environment/test_dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/utils/sleep.yaml
```

### Comparing `geomancy-1.0.0/.geomancy.yaml` & `geomancy-1.1.1/.geomancy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/.github/workflows/publish-to-pypi.yml` & `geomancy-1.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Publish Python distributions to PyPI and TestPyPI
 
-#on:
-#  release:
-#    types: [published]
-on: push
+on:
+  push:
+    branches:
+      - main
 
 jobs:
   build-and-publish:
     name: Build and Publish Python distributions
     runs-on: ubuntu-latest
     environment:
       name: pypi
```

### Comparing `geomancy-1.0.0/.github/workflows/tests.yml` & `geomancy-1.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/.gitignore` & `geomancy-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/LICENSE` & `geomancy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/PKG-INFO` & `geomancy-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 1.0.0
+Version: 1.1.1
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Keywords: .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
@@ -62,15 +62,15 @@
 <strong><u>Validation of layered and combined environments</u></strong>
 </summary>
 
 Layered environments could include a _common_ or _base_ environment, with
 additional checks for settings of _test_, _development_ and _production_
 environments.
 
-In the following checks file, the existence of environment file and secrets
+In the following checks file, the existence of an environment file and a secrets
 file can be checked based on the ``$ENV`` environment variable. (See the
 [docker environment variable parameter expansion rules](https://docs.docker.com/compose/environment-variables/env-file/#parameter-expansion))
 
 ```yaml
 checks:
   Environment:
     desc: Check environment variables in different deployments
@@ -354,24 +354,28 @@
 ```
 </details>
 </p>
 
 <p>
 <details>
 <summary><strong><u>AWS</u></strong> resources exist and are securely setup
-  (<a href="https://geomancy.readthedocs.io/en/latest/usage/format.html#checkawss3">checkS3</a>)
+  (<a href="https://geomancy.readthedocs.io/en/latest/usage/checks/aws/index.html">AWS checks</a>)
 </summary>
 
 The following shows an example in yaml format. Checks can be formatted in
 toml format as well.
 
 ```yaml
 AWS:
+  IAM:
+    desc: Check the default authentication and security settings
+    checkIAM:
+
   TemplatesS3Bucket:
-    desc: The bucket for cloudformation templates
+    desc: Check the bucket for cloudformation templates
     checkS3: "myproject-cfn-templates"
 ```
 </details>
 </p>
 
 <!-- end features -->
 
@@ -411,22 +415,24 @@
           desc: Python interpreter ver 3.11 or higher
           checkExec: python3>=3.11
     ```
 
 2. Use ``geo`` to run the checks.
 
     ```shell
-    $ geo check
-    [✔] .geomancy.yaml...passed
+    [✔] test.yaml...passed
     [✔]   checks...passed
     [✔]     Environment...passed
-    [✔]       Check environment variable '$USER'......passed
+    [✔]       Check environment variable '$USER'...passed
     [✔]     Paths...passed
-    [✔]       Check path 'examples/geomancy.toml'......passed
-    [✔]       Check path 'examples/pyproject.toml'......passed
+    [✔]       Check path 'examples/geomancy.toml'...passed
+    [✔]       Check path 'examples/pyproject.toml'...passed
+    [✔]     Executables...passed
+    [✔]       Check executable 'python3>=3.11'...passed
+    ================================= 9 passed in 0.51s ==================================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 
@@ -435,13 +441,20 @@
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
 
 
 ## Bugs or Requests
 Please use the [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues)
 to submit bugs or request features.
 
+## Similar projects
+
+The following projects share some of the same goals in different contexts:
+
+- [Envalid](https://github.com/af/envalid)
+- [AWS Config](https://aws.amazon.com/config/)
+
 ## License
 
 Copyright Justin Lorieau and others, 2023.
 
 Distributed under the terms of the [MIT license](LICENSE).
 geomancy is free and open source software.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geomancy Version: 1.0.0 Summary: Geomancy validates
+Metadata-Version: 2.1 Name: geomancy Version: 1.1.1 Summary: Geomancy validates
 deployment and development environments Author: Justin Lorieau Keywords:
 .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: MIT License
@@ -26,29 +26,30 @@
 setting of environment variables, the installation and versions of installed
 executables, the state of external dependencies, like LaTeX packages, or cloud
 resources, or for checking environments that use the [12-factor](http://
 12factor.net/) principles.  ## Features  ### Capabilities
   Validation_of_layered_and_combined_environments  Layered environments could
 include a _common_ or _base_ environment, with additional checks for settings
 of _test_, _development_ and _production_ environments. In the following checks
-file, the existence of environment file and secrets file can be checked based
-on the ``$ENV`` environment variable. (See the [docker environment variable
-parameter expansion rules](https://docs.docker.com/compose/environment-
-variables/env-file/#parameter-expansion)) ```yaml checks: Environment: desc:
-Check environment variables in different deployments CheckEnvFile: desc: Check
-the existence of the environment file checkPath: "deployments/${ENV}/.env"
-CheckSecretsFile: desc: Check the existence of the secrets file checkPath:
-"deployments/${ENV}/.secrets" ``` This check file can be used to check multiple
-environments: ```shell # check "dev" environment $ geo -e deployments/base/.env
--e deployments/dev/.env checks.yaml ... # check "test" environment $ geo -
-e deployments/base/.env -e deployments/test/.env checks.yaml ... ``` In this
-case, ``deployments/dev/.env`` is an [environment file](https://
-docs.docker.com/compose/environment-variables/env-file/) that sets ``ENV=dev``,
-``deployments/test/.env`` is an [environment file](https://docs.docker.com/
-compose/environment-variables/env-file/) that sets ``ENV=test``.
+file, the existence of an environment file and a secrets file can be checked
+based on the ``$ENV`` environment variable. (See the [docker environment
+variable parameter expansion rules](https://docs.docker.com/compose/
+environment-variables/env-file/#parameter-expansion)) ```yaml checks:
+Environment: desc: Check environment variables in different deployments
+CheckEnvFile: desc: Check the existence of the environment file checkPath:
+"deployments/${ENV}/.env" CheckSecretsFile: desc: Check the existence of the
+secrets file checkPath: "deployments/${ENV}/.secrets" ``` This check file can
+be used to check multiple environments: ```shell # check "dev" environment $
+geo -e deployments/base/.env -e deployments/dev/.env checks.yaml ... # check
+"test" environment $ geo -e deployments/base/.env -e deployments/test/.env
+checks.yaml ... ``` In this case, ``deployments/dev/.env`` is an [environment
+file](https://docs.docker.com/compose/environment-variables/env-file/) that
+sets ``ENV=dev``, ``deployments/test/.env`` is an [environment file](https://
+docs.docker.com/compose/environment-variables/env-file/) that sets
+``ENV=test``.
   Full_environment_file_support of the docker env_file_syntax  Environment
 files are loaded using the ``-e/--env`` option, which can be layered for
 different environments. ```shell # Run checks for 'dev' environment $ geo -
 e deployments/base/.env -e deployments/dev/.env check ... # Run checks for
 'test' environment $ geo -e base.env -e test.env run -- echo "Test environment"
 ```
   Concurrent_checks_with_multiple_threads to quickly probe I/O bound resources
@@ -108,34 +109,39 @@
 Windows 10 or later (released 2015) checkOS: "Windows >= 10" Environment: desc:
 Check environment variables common to all development environments Path: decs:
 Paths to search for executables checkEnv: $PATH Username: subchecks: any
 UnixUsername: # Username on linux and macOS desc: The current username
 checkEnv: $USER regex: "[a-z_][a-z0-9_-]*[$]?" WindowsUsername: # Username on
 Windows desc: The current username checkEnv: $USERNAME regex: "[a-z_][a-z0-9_-
 ]*[$]?" ```
- AWS resources exist and are securely setup (checkS3)  The following shows an
-example in yaml format. Checks can be formatted in toml format as well. ```yaml
-AWS: TemplatesS3Bucket: desc: The bucket for cloudformation templates checkS3:
-"myproject-cfn-templates" ```
+ AWS resources exist and are securely setup (AWS_checks)  The following shows
+an example in yaml format. Checks can be formatted in toml format as well.
+```yaml AWS: IAM: desc: Check the default authentication and security settings
+checkIAM: TemplatesS3Bucket: desc: Check the bucket for cloudformation
+templates checkS3: "myproject-cfn-templates" ```
  ## Quickstart  1. Create a ``.geomancy.yaml`` file with checks. See [examples/
 geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/
 geomancy.yaml) for an example of all checks. ```yaml checks: Environment: desc:
 Check environment variables common to all development environments Username:
 desc: The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?"
 Paths: desc: Checks the existence of needed files and directories subchecks:
 "any" # at least one of the files must be present Geomancy: desc: Check for the
 'geomancy.toml' file checkPath: examples/geomancy.toml type: file Pyproject:
 desc: Check for 'pyproject.toml' file checkPath: examples/pyproject.toml type:
 file Executables: desc: Check the availability of commands and their versions
 Python: desc: Python interpreter ver 3.11 or higher checkExec: python3>=3.11
-``` 2. Use ``geo`` to run the checks. ```shell $ geo check [â]
-.geomancy.yaml...passed [â] checks...passed [â] Environment...passed [â]
-Check environment variable '$USER'......passed [â] Paths...passed [â] Check
-path 'examples/geomancy.toml'......passed [â] Check path 'examples/
-pyproject.toml'......passed ``` (By default, ``geomancy`` will search
+``` 2. Use ``geo`` to run the checks. ```shell [â] test.yaml...passed [â]
+checks...passed [â] Environment...passed [â] Check environment variable
+'$USER'...passed [â] Paths...passed [â] Check path 'examples/
+geomancy.toml'...passed [â] Check path 'examples/pyproject.toml'...passed
+[â] Executables...passed [â] Check executable 'python3>=3.11'...passed
+================================= 9 passed in 0.51s
+================================== ``` (By default, ``geomancy`` will search
 ``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``, ``geomancy.toml``
 and ``pyproject.toml``.)  ## Documentation For full documentation please see
 https://geomancy.readthedocs.io/en/latest. ## Bugs or Requests Please use the
 [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues) to submit
-bugs or request features. ## License Copyright Justin Lorieau and others, 2023.
-Distributed under the terms of the [MIT license](LICENSE). geomancy is free and
-open source software.
+bugs or request features. ## Similar projects The following projects share some
+of the same goals in different contexts: - [Envalid](https://github.com/af/
+envalid) - [AWS Config](https://aws.amazon.com/config/) ## License Copyright
+Justin Lorieau and others, 2023. Distributed under the terms of the [MIT
+license](LICENSE). geomancy is free and open source software.
```

### Comparing `geomancy-1.0.0/README.md` & `geomancy-1.1.1/geomancy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: geomancy
+Version: 1.1.1
+Summary: Geomancy validates deployment and development environments
+Author: Justin Lorieau
+Keywords: .env,dotenv,env,env var,environment,environment variable,deployment,validation
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Bug Tracking
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: aws
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
 <!-- start logo -->
 <img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/docs/_static/geomancy_logo.svg" alt="geomancy logo" height="150px"/>
 <!-- end logo -->
 
 <!-- start badges -->
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
@@ -31,15 +62,15 @@
 <strong><u>Validation of layered and combined environments</u></strong>
 </summary>
 
 Layered environments could include a _common_ or _base_ environment, with
 additional checks for settings of _test_, _development_ and _production_
 environments.
 
-In the following checks file, the existence of environment file and secrets
+In the following checks file, the existence of an environment file and a secrets
 file can be checked based on the ``$ENV`` environment variable. (See the
 [docker environment variable parameter expansion rules](https://docs.docker.com/compose/environment-variables/env-file/#parameter-expansion))
 
 ```yaml
 checks:
   Environment:
     desc: Check environment variables in different deployments
@@ -323,24 +354,28 @@
 ```
 </details>
 </p>
 
 <p>
 <details>
 <summary><strong><u>AWS</u></strong> resources exist and are securely setup
-  (<a href="https://geomancy.readthedocs.io/en/latest/usage/format.html#checkawss3">checkS3</a>)
+  (<a href="https://geomancy.readthedocs.io/en/latest/usage/checks/aws/index.html">AWS checks</a>)
 </summary>
 
 The following shows an example in yaml format. Checks can be formatted in
 toml format as well.
 
 ```yaml
 AWS:
+  IAM:
+    desc: Check the default authentication and security settings
+    checkIAM:
+
   TemplatesS3Bucket:
-    desc: The bucket for cloudformation templates
+    desc: Check the bucket for cloudformation templates
     checkS3: "myproject-cfn-templates"
 ```
 </details>
 </p>
 
 <!-- end features -->
 
@@ -380,22 +415,24 @@
           desc: Python interpreter ver 3.11 or higher
           checkExec: python3>=3.11
     ```
 
 2. Use ``geo`` to run the checks.
 
     ```shell
-    $ geo check
-    [✔] .geomancy.yaml...passed
+    [✔] test.yaml...passed
     [✔]   checks...passed
     [✔]     Environment...passed
-    [✔]       Check environment variable '$USER'......passed
+    [✔]       Check environment variable '$USER'...passed
     [✔]     Paths...passed
-    [✔]       Check path 'examples/geomancy.toml'......passed
-    [✔]       Check path 'examples/pyproject.toml'......passed
+    [✔]       Check path 'examples/geomancy.toml'...passed
+    [✔]       Check path 'examples/pyproject.toml'...passed
+    [✔]     Executables...passed
+    [✔]       Check executable 'python3>=3.11'...passed
+    ================================= 9 passed in 0.51s ==================================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 
@@ -404,13 +441,20 @@
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
 
 
 ## Bugs or Requests
 Please use the [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues)
 to submit bugs or request features.
 
+## Similar projects
+
+The following projects share some of the same goals in different contexts:
+
+- [Envalid](https://github.com/af/envalid)
+- [AWS Config](https://aws.amazon.com/config/)
+
 ## License
 
 Copyright Justin Lorieau and others, 2023.
 
 Distributed under the terms of the [MIT license](LICENSE).
 geomancy is free and open source software.
```

#### html2text {}

```diff
@@ -1,38 +1,55 @@
- [geomancy logo]   [![pypi version](https://img.shields.io/pypi/v/
-geomancy.svg)](https://pypi.org/project/geomancy/) [![python versions](https://
-img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/
-geomancy/) [![Black formatting](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) [![Documentation Status]
-(https://readthedocs.org/projects/geomancy/badge/?version=latest)](https://
-geomancy.readthedocs.io/en/latest/?badge=latest)   Geomancy makes it easy to
-check and validate environments, such as development, testing and production.
-Environment checks and tests are helpful for testing the correct setting of
-environment variables, the installation and versions of installed executables,
-the state of external dependencies, like LaTeX packages, or cloud resources, or
-for checking environments that use the [12-factor](http://12factor.net/
-) principles.  ## Features  ### Capabilities
+Metadata-Version: 2.1 Name: geomancy Version: 1.1.1 Summary: Geomancy validates
+deployment and development environments Author: Justin Lorieau Keywords:
+.env,dotenv,env,env var,environment,environment variable,deployment,validation
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Information Technology Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Bug Tracking Classifier: Topic ::
+Software Development :: Debuggers Classifier: Topic :: Software Development ::
+Quality Assurance Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance Classifier:
+Topic :: System :: Monitoring Classifier: Topic :: System :: Systems
+Administration Classifier: Topic :: Utilities Classifier: Development Status ::
+4 - Beta Requires-Python: >=3.11 Description-Content-Type: text/markdown
+Provides-Extra: all Provides-Extra: aws Provides-Extra: dev Provides-Extra:
+docs License-File: LICENSE  [geomancy logo]   [![pypi version](https://
+img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/) [!
+[python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https:/
+/pypi.org/project/geomancy/) [![Black formatting](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black) [![Documentation
+Status](https://readthedocs.org/projects/geomancy/badge/?version=latest)]
+(https://geomancy.readthedocs.io/en/latest/?badge=latest)   Geomancy makes it
+easy to check and validate environments, such as development, testing and
+production. Environment checks and tests are helpful for testing the correct
+setting of environment variables, the installation and versions of installed
+executables, the state of external dependencies, like LaTeX packages, or cloud
+resources, or for checking environments that use the [12-factor](http://
+12factor.net/) principles.  ## Features  ### Capabilities
   Validation_of_layered_and_combined_environments  Layered environments could
 include a _common_ or _base_ environment, with additional checks for settings
 of _test_, _development_ and _production_ environments. In the following checks
-file, the existence of environment file and secrets file can be checked based
-on the ``$ENV`` environment variable. (See the [docker environment variable
-parameter expansion rules](https://docs.docker.com/compose/environment-
-variables/env-file/#parameter-expansion)) ```yaml checks: Environment: desc:
-Check environment variables in different deployments CheckEnvFile: desc: Check
-the existence of the environment file checkPath: "deployments/${ENV}/.env"
-CheckSecretsFile: desc: Check the existence of the secrets file checkPath:
-"deployments/${ENV}/.secrets" ``` This check file can be used to check multiple
-environments: ```shell # check "dev" environment $ geo -e deployments/base/.env
--e deployments/dev/.env checks.yaml ... # check "test" environment $ geo -
-e deployments/base/.env -e deployments/test/.env checks.yaml ... ``` In this
-case, ``deployments/dev/.env`` is an [environment file](https://
-docs.docker.com/compose/environment-variables/env-file/) that sets ``ENV=dev``,
-``deployments/test/.env`` is an [environment file](https://docs.docker.com/
-compose/environment-variables/env-file/) that sets ``ENV=test``.
+file, the existence of an environment file and a secrets file can be checked
+based on the ``$ENV`` environment variable. (See the [docker environment
+variable parameter expansion rules](https://docs.docker.com/compose/
+environment-variables/env-file/#parameter-expansion)) ```yaml checks:
+Environment: desc: Check environment variables in different deployments
+CheckEnvFile: desc: Check the existence of the environment file checkPath:
+"deployments/${ENV}/.env" CheckSecretsFile: desc: Check the existence of the
+secrets file checkPath: "deployments/${ENV}/.secrets" ``` This check file can
+be used to check multiple environments: ```shell # check "dev" environment $
+geo -e deployments/base/.env -e deployments/dev/.env checks.yaml ... # check
+"test" environment $ geo -e deployments/base/.env -e deployments/test/.env
+checks.yaml ... ``` In this case, ``deployments/dev/.env`` is an [environment
+file](https://docs.docker.com/compose/environment-variables/env-file/) that
+sets ``ENV=dev``, ``deployments/test/.env`` is an [environment file](https://
+docs.docker.com/compose/environment-variables/env-file/) that sets
+``ENV=test``.
   Full_environment_file_support of the docker env_file_syntax  Environment
 files are loaded using the ``-e/--env`` option, which can be layered for
 different environments. ```shell # Run checks for 'dev' environment $ geo -
 e deployments/base/.env -e deployments/dev/.env check ... # Run checks for
 'test' environment $ geo -e base.env -e test.env run -- echo "Test environment"
 ```
   Concurrent_checks_with_multiple_threads to quickly probe I/O bound resources
@@ -92,34 +109,39 @@
 Windows 10 or later (released 2015) checkOS: "Windows >= 10" Environment: desc:
 Check environment variables common to all development environments Path: decs:
 Paths to search for executables checkEnv: $PATH Username: subchecks: any
 UnixUsername: # Username on linux and macOS desc: The current username
 checkEnv: $USER regex: "[a-z_][a-z0-9_-]*[$]?" WindowsUsername: # Username on
 Windows desc: The current username checkEnv: $USERNAME regex: "[a-z_][a-z0-9_-
 ]*[$]?" ```
- AWS resources exist and are securely setup (checkS3)  The following shows an
-example in yaml format. Checks can be formatted in toml format as well. ```yaml
-AWS: TemplatesS3Bucket: desc: The bucket for cloudformation templates checkS3:
-"myproject-cfn-templates" ```
+ AWS resources exist and are securely setup (AWS_checks)  The following shows
+an example in yaml format. Checks can be formatted in toml format as well.
+```yaml AWS: IAM: desc: Check the default authentication and security settings
+checkIAM: TemplatesS3Bucket: desc: Check the bucket for cloudformation
+templates checkS3: "myproject-cfn-templates" ```
  ## Quickstart  1. Create a ``.geomancy.yaml`` file with checks. See [examples/
 geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/
 geomancy.yaml) for an example of all checks. ```yaml checks: Environment: desc:
 Check environment variables common to all development environments Username:
 desc: The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?"
 Paths: desc: Checks the existence of needed files and directories subchecks:
 "any" # at least one of the files must be present Geomancy: desc: Check for the
 'geomancy.toml' file checkPath: examples/geomancy.toml type: file Pyproject:
 desc: Check for 'pyproject.toml' file checkPath: examples/pyproject.toml type:
 file Executables: desc: Check the availability of commands and their versions
 Python: desc: Python interpreter ver 3.11 or higher checkExec: python3>=3.11
-``` 2. Use ``geo`` to run the checks. ```shell $ geo check [â]
-.geomancy.yaml...passed [â] checks...passed [â] Environment...passed [â]
-Check environment variable '$USER'......passed [â] Paths...passed [â] Check
-path 'examples/geomancy.toml'......passed [â] Check path 'examples/
-pyproject.toml'......passed ``` (By default, ``geomancy`` will search
+``` 2. Use ``geo`` to run the checks. ```shell [â] test.yaml...passed [â]
+checks...passed [â] Environment...passed [â] Check environment variable
+'$USER'...passed [â] Paths...passed [â] Check path 'examples/
+geomancy.toml'...passed [â] Check path 'examples/pyproject.toml'...passed
+[â] Executables...passed [â] Check executable 'python3>=3.11'...passed
+================================= 9 passed in 0.51s
+================================== ``` (By default, ``geomancy`` will search
 ``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``, ``geomancy.toml``
 and ``pyproject.toml``.)  ## Documentation For full documentation please see
 https://geomancy.readthedocs.io/en/latest. ## Bugs or Requests Please use the
 [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues) to submit
-bugs or request features. ## License Copyright Justin Lorieau and others, 2023.
-Distributed under the terms of the [MIT license](LICENSE). geomancy is free and
-open source software.
+bugs or request features. ## Similar projects The following projects share some
+of the same goals in different contexts: - [Envalid](https://github.com/af/
+envalid) - [AWS Config](https://aws.amazon.com/config/) ## License Copyright
+Justin Lorieau and others, 2023. Distributed under the terms of the [MIT
+license](LICENSE). geomancy is free and open source software.
```

### Comparing `geomancy-1.0.0/Taskfile.yaml` & `geomancy-1.1.1/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/docs/_static/geomancy_logo.png` & `geomancy-1.1.1/docs/_static/geomancy_logo.png`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/docs/_static/geomancy_logo.svg` & `geomancy-1.1.1/docs/_static/geomancy_logo.svg`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/docs/about/api/index.rst` & `geomancy-1.1.1/docs/about/api/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     geomancy.checks.Result
     geomancy.checks.CheckException
     geomancy.checks.CheckEnv
     geomancy.checks.CheckExec
     geomancy.checks.CheckPath
     geomancy.checks.CheckPlatform
     geomancy.checks.CheckPythonPackage
-    geomancy.checks.CheckAWSS3
+    geomancy.checks.aws.CheckAwsS3
+    geomancy.checks.aws.CheckAwsIam
 
 Config
 ------
 
 .. autosummary::
     :toctree: generated
     :nosignatures:
```

### Comparing `geomancy-1.0.0/docs/conf.py` & `geomancy-1.1.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,22 +48,24 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "furo"
-html_title = " "
 html_logo = "_static/geomancy_logo.svg"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["custom.css"]
 
 # Other html variables (Furo)
 # https://pradyunsg.me/furo/customisation/colors/
-html_theme_options = {"light_css_variables": {"color-foreground-border": "#bfbfbf"}}
+html_theme_options = {
+    "light_css_variables": {"color-foreground-border": "#bfbfbf"},
+    "sidebar_hide_name": True,
+}
 
 # Remove the autosummary stub links from toctrees
 remove_from_toctrees = ["about/api/generated/*"]
```

### Comparing `geomancy-1.0.0/docs/usage/cmd_checks.md` & `geomancy-1.1.1/docs/usage/cmd_checks.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,310 +1,329 @@
-(running-checks)=
-# Running Checks
+.. _running-checks:
 
-## Specifying which checks to run
+Running Checks
+==============
+
+Specifying Checks to Run
+------------------------
 
 Geomancy can find checks from files in pre-defined locations, if file
 arguments aren't specified, or it can run checks from the files specified as
 arguments.
 
-The format of the checks file is specified in the [next section](#file-format).
+The format of the checks file is specified in the :ref:`file-format`.
+
+.. tab-set::
+
+    .. tab-item:: without arguments
+
+        When no arguments are specified, geo will search for checks in multiple
+        locations.
 
-::::{tab-set}
-:::{tab-item} With arguments
-The following evaluates the checks listed in ``examples/geomancy.yaml``, if
-this file exists.
-```shell
-$ geo examples/geomancy.yaml
- [✔] examples/geomancy.yaml...passed
- [✔]   checks...passed
- [✔]     OperatingSystem...passed
- [✔]       Check platform 'macOS >= 10.9'...passed
- [!]       Check platform 'Linux >= 3.0'...wrong platform
- [!]       Check platform 'Windows >= 10'...wrong platform
- [✔]     Environment...passed
- [✔]       Check environment variable '$PATH'...passed
- [✔]       Username...passed
- [✔]         Check environment variable '$USER'...passed
- [!]         Check environment variable '$USERNAME'...empty string
- [✔]     Paths...passed
- [✔]       ChecksFile...passed
- [✔]         Check path 'examples/geomancy.toml'...passed
- [✔]         Check path 'examples/pyproject.toml'...passed
- [!]         Check path '.missing__.txt'...missing
- [✔]     Executables...passed
- [✔]       Check executable 'python3>=3.11'...passed
- [✔]     PythonPackages...passed
- [✔]       Check python package 'geomancy>=0.8'...passed
-```
-:::
-:::{tab-item} Without arguments
-When no arguments are specified, geo will search for checks in multiple locations.
-```shell
-$ geo
- [✔] examples/geomancy.yaml...passed
- [✔]   checks...passed
- [✔]     OperatingSystem...passed
- [✔]       Check platform 'macOS >= 10.9'...passed
- [!]       Check platform 'Linux >= 3.0'...wrong platform
- [!]       Check platform 'Windows >= 10'...wrong platform
- [✔]     Environment...passed
- [✔]       Check environment variable '$PATH'...passed
- [✔]       Username...passed
- [✔]         Check environment variable '$USER'...passed
- [!]         Check environment variable '$USERNAME'...empty string
- [✔]     Paths...passed
- [✔]       ChecksFile...passed
- [✔]         Check path 'examples/geomancy.toml'...passed
- [✔]         Check path 'examples/pyproject.toml'...passed
- [!]         Check path '.missing__.txt'...missing
- [✔]     Executables...passed
- [✔]       Check executable 'python3>=3.11'...passed
- [✔]     PythonPackages...passed
- [✔]       Check python package 'geomancy>=0.8'...passed
-```
-:::
-::::
+        .. code-block:: shell
+
+            $ geo
+              [✔] examples/geomancy.yaml...passed
+              [✔]   checks...passed
+              [✔]     OperatingSystem...passed
+              [✔]       Check platform 'macOS >= 10.9'...passed
+              [!]       Check platform 'Linux >= 3.0'...failed (wrong platform)
+              [!]       Check platform 'Windows >= 10'...failed (wrong platform)
+              [✔]     Environment...passed
+              [✔]       Check environment variable '$PATH'...passed
+              [✔]       Username...passed
+              [✔]         Check environment variable '$USER'...passed
+              [!]         Check environment variable '$USERNAME'...failed (empty string)
+              [✔]     Paths...passed
+              [✔]       ChecksFile...passed
+              [✔]         Check path 'examples/geomancy.toml'...passed
+              [✔]         Check path 'examples/pyproject.toml'...passed
+              [!]         Check path '.missing__.txt'...failed (missing)
+              [✔]     Executables...passed
+              [✔]       Check executable 'python3>=3.11'...passed
+              [✔]     PythonPackages...passed
+              [✔]       Check python package 'geomancy>=0.8'...passed
+             ================================= 16 passed in 0.50s =================================
+
+    .. tab-item:: with arguments
+
+        The following evaluates the checks listed in ``examples/geomancy.yaml``, if
+        this file exists.
+
+        .. code-block:: shell
+
+            $ geo examples/geomancy.yaml
+              [✔] examples/geomancy.yaml...passed
+              [✔]   checks...passed
+              [✔]     OperatingSystem...passed
+              [✔]       Check platform 'macOS >= 10.9'...passed
+              [!]       Check platform 'Linux >= 3.0'...failed (wrong platform)
+              [!]       Check platform 'Windows >= 10'...failed (wrong platform)
+              [✔]     Environment...passed
+              [✔]       Check environment variable '$PATH'...passed
+              [✔]       Username...passed
+              [✔]         Check environment variable '$USER'...passed
+              [!]         Check environment variable '$USERNAME'...failed (empty string)
+              [✔]     Paths...passed
+              [✔]       ChecksFile...passed
+              [✔]         Check path 'examples/geomancy.toml'...passed
+              [✔]         Check path 'examples/pyproject.toml'...passed
+              [!]         Check path '.missing__.txt'...failed (missing)
+              [✔]     Executables...passed
+              [✔]       Check executable 'python3>=3.11'...passed
+              [✔]     PythonPackages...passed
+              [✔]       Check python package 'geomancy>=0.8'...passed
+             ================================= 16 passed in 0.50s =================================
 
 If no checks files are listed as arguments, geo will search the following file
 locations in the current directory, and it wil run all the checks in existing
 files: ``.geomancy.yaml``, ``.geomancy.yml``, ``.geomancy.toml``,
 ``geomancy.yaml``, ``geomancy.yml``, ``geomancy.toml``, ``pyproject.toml``
 
-:::{admonition} Layering and combining checks
-:class: tip
-Multiple checks files can be run together allowing the mixing and matching
-of test sets.
-
-For example, a ``dev`` environment and ``prod`` environment may have common
-checks, listed in ``base.yaml``, in addition to environment specific checks
-listed in ``dev.yaml`` and ``prod.yaml`` respectively.
-```shell
-$ geo base.yaml dev.yaml   # 'dev' environment
-...
-$ geo base.yaml prod.yaml  # 'prod environment
-....
-```
-:::
-
-:::{admonition} Wildcards and glob patterns
-:class: tip
-The check file arguments support wildcards and glob patterns to run checks from
-multiple files at once. For example, the following will run checks in all
-files that have the ``geomancy`` filename: ``$ geo geomancy.*``
-:::
+.. admonition:: Layering and combining checks
+    :class: tip
+
+    Multiple checks files can be run together allowing the mixing and matching
+    of test sets.
+
+    For example, a ``dev`` environment and ``prod`` environment may have common
+    checks, listed in ``base.yaml``, in addition to environment specific checks
+    listed in ``dev.yaml`` and ``prod.yaml`` respectively.
+
+    .. code-block:: shell
 
-(configuration)=
-## Configuration
+        $ geo base.yaml dev.yaml   # 'dev' environment
+        ...
+        $ geo base.yaml prod.yaml  # 'prod environment
+        ...
 
-As described in the [next section](#file-format), configuration options are
+.. admonition:: Wildcards and glob patterns
+    :class: tip
+
+    The check file arguments support wildcards and glob patterns to run checks
+    from multiple files at once. For example, the following will run checks in
+    all files that have the ``geomancy`` filename: ``$ geo geomancy.*``
+
+
+.. _configuration:
+
+Configuration
+-------------
+
+As described in the :ref:`file-format` section, configuration options are
 placed in the ``config`` section of checks files or the
 ``[tool.geomancy.config]`` section of the ``pyproject.toml`` file.
 
-The default configuration options can be listed in
-[yaml](https://yaml.org) or [toml](https://toml.io/en/) formats.
+The default configuration options can be listed in `yaml <http://yaml.org>`_
+or `toml <https://toml.io/en>`_ formats.
+
+.. tab-set::
+
+    .. tab-item:: config (yaml)
 
-::::{tab-set}
-:::{tab-item} config (yaml)
-```shell
-$ geo config --yaml
-config:
-  CHECKBASE:
-    ENV_SUBSTITUTE_DEFAULT: true
-    MAX_LEVEL: 10
-...
-```
-:::
-:::{tab-item} config (toml)
-```shell
-$ geo config ---toml
-[config]
-VERSION='0.9.2'
-
-  [config.CHECKBASE]
-  ENV_SUBSTITUTE_DEFAULT=true
-  MAX_LEVEL=10...
-```
-:::
-::::
+        .. code-block:: shell
 
-(environment-files)=
-## Environment Variables and Files
+            $ geo config --yaml
+            config:
+              CHECKBASE:
+                ENV_SUBSTITUTE_DEFAULT: true
+                MAX_LEVEL: 10
+            ...
+
+    .. tab-item:: config (toml)
+
+        .. code-block:: shell
+
+            $ geo config ---toml
+            [config]
+            VERSION='0.9.2'
+
+              [config.CHECKBASE]
+              ENV_SUBSTITUTE_DEFAULT=true
+              MAX_LEVEL=10...
+            ...
+
+
+.. _environment-files:
+
+Environment Variables and Files
+-------------------------------
 
 Environment variables can be loaded from one or more environment files
 (a.k.a dotenv files) with the ``-e``/``--env`` flag.
 
-```shell
-$ geo -e .base.env -e .dev.env
-```
+.. code-block:: shell
+
+    $ geo -e .base.env -e .dev.env
+
 
 By default, existing environment variables, or environment variables set
 by preceding env files, are not overwritten. To change this behavior,
 use the ``--overwrite`` flag.
 
-```shell
-$ geo -e .base.env -e .dev.env --overwrite
-```
-
-:::{admonition} Layering and combining environments
-:class: tip
-Layered environments can be created by splitting environment variables
-between multiple environment files and invoking the ``-e``/``--env`` flag
-multiple times. For example, a ``.base.env`` file could contain environment
-variables common to all environments, while a ``.dev.env`` file could
-contain environment variables for the 'dev' environment.
-:::
-
-:::{admonition} Geomancy within environments
-:class: attention
-Even though geomancy supports the loading of environment files, it is
-recommended that environments are validated using the environment file loading
-mechanism used in practice.
-
-For example, if an environment file is used within
-[docker compose](https://docs.docker.com/compose/), the geomancy checks should
-be tested within the docker compose container.
-:::
+.. code-block:: shell
+
+    $ geo -e .base.env -e .dev.env --overwrite
+
+.. admonition:: Layering and combining environments
+    :class: tip
+
+    Layered environments can be created by splitting environment variables
+    between multiple environment files and invoking the ``-e``/``--env`` flag
+    multiple times. For example, a ``.base.env`` file could contain environment
+    variables common to all environments, while a ``.dev.env`` file could
+    contain environment variables for the 'dev' environment.
+
+.. admonition:: Geomancy within environments
+    :class: attention
+
+    Even though geomancy supports the loading of environment files, it is
+    recommended that environments are validated using the environment file
+    loading mechanism used in practice.
 
-(environment-files-syntax)=
-### Syntax
+    For example, if an environment file is used within
+    `docker compose <https://docs.docker.com/compose/>`_, the geomancy checks
+    should be tested within the docker compose container.
+
+.. _environment-files-syntax:
+
+Syntax
+^^^^^^
 
 Environment files are a superset of the
-[docker compose](https://docs.docker.com/compose/environment-variables/env-file/#syntax)
-environment file rules. Specifically,
+`docker compose environment file syntax <https://docs.docker.com/compose/environment-variables/env-file/#syntax>`_.
+Specifically,
+
+#.  Environment variable names may contain letters (``A-Z`` or ``a-z``),
+    numbers (``0-9``) and underscores (``_``), but the first character must be a
+    letter (``A-Z`` or ``a-z``)
+
+#.  Lines beginning with a ``#`` are considered a comment and ignored
+
+#.  Blank lines are ignored
+
+#.  Each line represents an environment variable name-value pair. Values may
+    be quoted.
+
+    .. code-block:: shell
+
+        VAR=VAL    # -> VAL
+        VAR="VAL"  # -> VAL
+        VAR='VAL'  # -> VAL
+
+#.  Inline comments must be preceded by a space
+
+    .. code-block:: shell
+
+       VAR=VALUE # comment       # -> VALUE
+       VAR=VALUE# not a comment  # -> VALUE# not a comment
+
+#.  Comments for quoted values must follow the quote
+
+    .. code-block:: shell
+
+        VAR="VALUE # not a comment"  # -> VALUE # not a comment
+        VAR="VALUE"  # comment       # -> VALUE
+
+
+#.  Single-quoted values are taken literally
+
+    .. code-block:: shell
+
+        VAR='$OTHER'    # -> $OTHER
+        VAR='${OTHER}'  # -> ${OTHER}
+
+#.  Quotes can be escaped
+
+    .. code-block:: shell
+
+        VAR='Let\'s go!'             # -> Let's go!
+        VAR="{\"hello\": \"json\"}"  # -> {"hello": "json"}
+
+#.  Shell escape sequences (``\n``, ``\t``, ``\r``, ``\\``) are supported in
+    double-quoted values
+
+    .. code-block:: shell
+
+        VAR="some\tvalue"  # -> some    value
+        VAR='some\tvalue'  # -> some\tvalue
+        VAR=some\tvalue     # -> some\tvalue
+
+#.  Environment file values are substituted according to the
+    :ref:`substitution <environment-substitution>` rules.
+
+    .. code-block:: shell
+
+        MYVAR=MYVALUE
+        VAR1=$MYVAR      # VAR1=MYVALUE
 
-1. Environment variable names may contain letters (``A-Z`` or ``a-z``),
-   numbers (``0-9``) and underscores (``_``), but the first character must be a
-   letter (``A-Z`` or ``a-z``)
-
-2. Lines beginning with a ``#`` are considered a comment and ignored
-
-3. Blank lines are ignored
-
-4. Each line represents an environment variable name-value pair. Values may
-   be quoted.
-    ```shell
-    VAR=VAL    # -> VAL
-    VAR="VAL"  # -> VAL
-    VAR='VAL'  # -> VAL
-    ```
-
-5. Inline comments must be preceded by a space
-   ```shell
-   VAR=VALUE # comment       # -> VALUE
-   VAR=VALUE# not a comment  # -> VALUE# not a comment
-   ```
-
-6. Comments for quoted values must follow the quote
-    ```shell
-   VAR="VALUE # not a comment"  # -> VALUE # not a comment
-   VAR="VALUE"  # comment       # -> VALUE
-    ```
-
-7. Single-quoted values are taken literally
-    ```shell
-    VAR='$OTHER'    # -> $OTHER
-    VAR='${OTHER}'  # -> ${OTHER}
-    ```
-
-8. Quotes can be escaped
-    ```shell
-    VAR='Let\'s go!'             # -> Let's go!
-    VAR="{\"hello\": \"json\"}"  # -> {"hello": "json"}
-    ```
-
-9. Shell escape sequences (``\n``, ``\t``, ``\r``, ``\\``) are supported in
-   double-quoted values
-    ```shell
-    VAR="some\tvalue"  # -> some    value
-    VAR='some\tvalue'  # -> some\tvalue
-    VAR=some\tvalue     # -> some\tvalue
-    ```
-
-10. Environment file values are substituted according to the
-    [substitution](#environment-substitution) rules.
-    ```shell
-    MYVAR=MYVALUE
-    VAR1=$MYVAR      # VAR1=MYVALUE
-    ```
+.. _environment-substitution:
 
-(environment-substitution)=
-### Substitution
+Substitution
+^^^^^^^^^^^^
 
-The following rules are followed from
-[docker compose](https://docs.docker.com/compose/environment-variables/env-file/#syntax)
+The following rules follow the
+`docker compose environment substitution syntax <https://docs.docker.com/compose/environment-variables/env-file/#syntax>`_
 for substituting environment variables in values.
 
-1. Environment variables are substituted when preceded by a ``$`` and may or
-   may not contain braces. e.g. ``$USER`` or ``${USER}``
+#.  Environment variables are substituted when preceded by a ``$`` and may or
+    may not contain braces. e.g. ``$USER`` or ``${USER}``
 
-2. _Direct substitution_ of braced (``${VAR}``) and unbraced (``$VAR``)
-   variables may be done in unquoted or double-quoted values--not single-quoted
-   literals.
-    ```shell
-    MYVAR=MYVALUE
-    $MYVAR      # -> MYVALUE
-    "${MYVAR}"  # -> MYVALUE
-    '${MYVAR}'  # -> ${MYVAR}
-    ```
-3. _Default value substitution_ will return the default value if the variable
-   isn't set or is empty. Defaults can contain spaces in the braced version,
-   but not quotes.
-   ```shell
-   ${MISSING-my default value}   # -> my default value
-   ${MISSING:-my default value}  # -> my default value
-   $MISSING-default              # -> default
-   $MISSING:-default             # -> default
-   ```
-4. _Error value substitution_ will raise an exception with the given error
-   message if an environment variable isn't set or is empty. Errors can contain
-   spaces in the braced version, but not quotes
-   ```shell
-   ${MISSING?no value}   # -> raises EnvironmentError("no value")
-   ${MISSING:?no value}  # -> raises EnvironmentError("no value")
-   $MISSING?missing      # -> raises EnvironmentError("missing")
-   $MISSING:?missing     # -> raises EnvironmentError("missing")
-   ```
-5. _Replacement value substitution_ will replace a set environment variable
-   with the replacement value, otherwise it will produce an empty string.
-   Replacements can contain spaces in the braced version, but not quotes
-   ```shell
-   MYVAR=MYVALUE
-   ${MYVAR+replaced}   # -> replaced
-   ${MYVAR:+replaced}  # -> replaced
-   $MYVAR+replaced     # -> replaced
-   $MYVAR:+replaced    # -> replaced
-   ${MISSING+replaced} # ""
-   ${MISSING+replaced} # ""
-   ```
+#.  **Direct substitution** of braced (``${VAR}``) and unbraced (``$VAR``)
+    variables may be done in unquoted or double-quoted values--not single-quoted
+    literals.
+
+    .. code-block:: shell
+
+        MYVAR=MYVALUE
+        $MYVAR      # -> MYVALUE
+        "${MYVAR}"  # -> MYVALUE
+        '${MYVAR}'  # -> ${MYVAR}
+
+#.  **Default value substitution** will return the default value if the variable
+    isn't set or is empty. Defaults can contain spaces in the braced version,
+    but not quotes.
+
+    .. code-block:: shell
+
+        ${MISSING-my default value}   # -> my default value
+        ${MISSING:-my default value}  # -> my default value
+        $MISSING-default              # -> default
+        $MISSING:-default             # -> default
+
+#.  **Error value substitution** will raise an exception with the given error
+    message if an environment variable isn't set or is empty. Errors can contain
+    spaces in the braced version, but not quotes
+
+    .. code-block:: shell
+
+        ${MISSING?no value}   # -> raises EnvironmentError("no value")
+        ${MISSING:?no value}  # -> raises EnvironmentError("no value")
+        $MISSING?missing      # -> raises EnvironmentError("missing")
+        $MISSING:?missing     # -> raises EnvironmentError("missing")
+
+#.  **Replacement value substitution** will replace a set environment variable
+    with the replacement value, otherwise it will produce an empty string.
+    Replacements can contain spaces in the braced version, but not quotes
+
+    .. code-block:: shell
+
+        MYVAR=MYVALUE
+        ${MYVAR+replaced}   # -> replaced
+        ${MYVAR:+replaced}  # -> replaced
+        $MYVAR+replaced     # -> replaced
+        $MYVAR:+replaced    # -> replaced
+        ${MISSING+replaced} # ""
+        ${MISSING+replaced} # ""
 
-## Other Options
+Other Options
+-------------
 
 The following are options available to ``geo`` and``geo check``.
 
-`-e`/`--env`
-: Environment variable file(s) to load for checks
+``-e``/``--env``
+    Environment variable file(s) to load for checks
 
-`--overwrite`
-: Overwrite existing environment variables with those listed in environment
-  variable files. This option requires environment variable files to be
-  specified with `-e`/`--env`
-
-`-f`/`--fixture`
-: Load a fixture file (yaml format) for mocking network requests. If the
-  fixture does not exist, it will be created. This option is helpful for
-  testing checks files when checks require authentication.
-
-  :::{dropdown} Example
-  The following command runs the AWS checks in ``examples/aws/geomancy.yaml``,
-  which require proper authentication of the AWS client. To bypass network
-  requests, a fixture can be loaded to test this example.
-
-  ```shell
-  $ geo --fixture examples/aws/fixtures.yaml examples/aws/geomancy.yaml
-   [✔] examples/aws/geomancy.yaml...passed
-   [✔]   checks...passed
-   [✔]     CloudFormationTemplateS3...passed
-   [✔]       Check AWS S3 bucket access 'myproject-cfn-templates'......passed
-   [✔]       Check AWS S3 bucket private 'myproject-cfn-templates'......passed
-  ```
-  :::
+``--overwrite``
+    Overwrite existing environment variables with those listed in environment
+    variable files. This option requires environment variable files to be
+    specified with `-e`/`--env`
```

### Comparing `geomancy-1.0.0/docs/usage/cmd_run.md` & `geomancy-1.1.1/docs/usage/cmd_run.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,61 @@
-(running-environments)=
-# Running Environments
+.. _running-environments:
+
+Running Environments
+====================
 
 Geomancy can load [environment files](#environment-files) and run commands
 from within these environments.
 
 The ``run`` subcommand will run commands in a separate process, and environment
 files are loaded with the ``-e``/``-env`` option for each environment.
 See [Environment Files](#environment-files) for the syntax of environment files.
 
-```shell
-$ geo run -e [env_file] -- [cmd]
-```
+.. code-block:: shell
+
+    $ geo run -e [env_file] -- [cmd]
+
 
 The following examples shows commands with arguments.
 
-::::{tab-set}
-:::{tab-item} Example
-The following runs echo and grep in an environment loaded with the ``.env``
-file.
-```shell
-$ geo run -e .env -- echo "My first test" | grep -e "test"
-My first test
-```
-:::
-:::{tab-item} Example (abbreviated)
-The following is a command that does not produce option conflicts with geo--
-i.e. it does not use a `-e` flag, which could be captured by geo.
-```shell
-$ geo run -e .env uname
-Darwin
-```
-:::
-::::
-
-:::{admonition} Shell expansions
-:class: caution
-Including environment variable references in commands will expand them before
-running the command within the environment. For example, if the ``.env`` file
-specified ``ENV=dev``, then ``$ENV`` variable would not be printed to the
-shell with the following command.
-
-```shell
-$ geo run -e .env -- echo $ENV
-```
-
-Instead the value of ``ENV`` can be retrieve from the environment's ``env``
-command.
-
-```shell
-$ geo run -e .env -- env|grep ENV
-ENV=dev
-```
-:::
+.. tab-set::
+
+    .. tab-item:: Example
+
+        The following runs echo and grep in an environment loaded with the
+        ``.env`` file.
+
+        .. code-block:: shell
+
+            $ geo run -e .env -- echo "My first test" | grep -e "test"
+            My first test
+
+    .. tab-item:: Example (abbreviated)
+
+        The following is a command that does not produce option conflicts with
+        geo--i.e. it does not use a ``-e`` flag, which could be captured by geo.
+
+        .. code-block:: shell
+
+            $ geo run -e .env uname
+            Darwin
+
+.. admonition:: Shell expansions
+    :class: caution
+
+    Including environment variable references in commands will expand them
+    before running the command within the environment. For example, if the
+    ``.env`` file specified ``ENV=dev``, then ``$ENV`` variable would not be
+    printed to the shell with the following command.
+
+    .. code-block:: shell
+
+        $ geo run -e .env -- echo $ENV
+
+
+    Instead the value of ``ENV`` can be retrieve from the environment's ``env``
+    command.
+
+    .. code-block:: shell
 
+        $ geo run -e .env -- env|grep ENV
+        ENV=dev
```

### Comparing `geomancy-1.0.0/examples/aws/fixtures.yaml` & `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,66 @@
 interactions:
 - request:
     body: null
     headers: {}
     method: HEAD
-    uri: https://myproject-cfn-templates.s3.amazonaws.com/
+    uri: https://testbucket-valid.s3.amazonaws.com/
   response:
     body:
       string: ''
     headers:
       Content-Type:
       - application/xml
       Date:
-      - Wed, 02 Aug 2023 14:51:02 GMT
+      - Mon, 31 Jul 2023 10:31:58 GMT
+      Server:
+      - AmazonS3
+      x-amz-access-point-alias:
+      - 'false'
+      x-amz-bucket-region:
+      - us-east-1
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers: {}
+    method: HEAD
+    uri: https://testbucket-valid.s3.amazonaws.com/
+  response:
+    body:
+      string: ''
+    headers:
+      Content-Type:
+      - application/xml
+      Date:
+      - Mon, 31 Jul 2023 20:09:27 GMT
       Server:
       - AmazonS3
       x-amz-access-point-alias:
       - 'false'
       x-amz-bucket-region:
       - us-east-1
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers: {}
     method: GET
-    uri: https://myproject-cfn-templates.s3.amazonaws.com/?publicAccessBlock
+    uri: https://testbucket-valid.s3.amazonaws.com/?publicAccessBlock
   response:
     body:
       string: '<?xml version="1.0" encoding="UTF-8"?>
 
         <PublicAccessBlockConfiguration xmlns="http://s3.amazonaws.com/doc/2006-03-01/"><BlockPublicAcls>true</BlockPublicAcls><IgnorePublicAcls>true</IgnorePublicAcls><BlockPublicPolicy>true</BlockPublicPolicy><RestrictPublicBuckets>true</RestrictPublicBuckets></PublicAccessBlockConfiguration>'
     headers:
       Date:
-      - Wed, 02 Aug 2023 14:51:02 GMT
+      - Mon, 31 Jul 2023 20:09:28 GMT
       Server:
       - AmazonS3
       Transfer-Encoding:
       - chunked
     status:
       code: 200
       message: OK
+version: 1
```

### Comparing `geomancy-1.0.0/examples/geomancy.toml` & `geomancy-1.1.1/examples/geomancy.toml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/examples/geomancy.yaml` & `geomancy-1.1.1/examples/geomancy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/geomancy/checks/aws/s3.py` & `geomancy-1.1.1/geomancy/checks/aws/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,135 +1,137 @@
-"""Checks for AWS resources"""
+"""Check AWS `S3 buckets`_ and `security settings`_.
+
+- Existence and accessibility
+- Public access is disabled
+
+.. _S3 buckets: https://aws.amazon.com/s3/
+.. _security settings: https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html
+"""
 import typing as t
 import logging
 
-from ..base import Check, Result, Executor
+from .base import CheckAws
+from ..base import Result, Executor, CheckException
 from ..utils import pop_first
 from ...config import Parameter
 
-__all__ = ("CheckAWSS3",)
-
 logger = logging.getLogger(__name__)
 
-#: The error message to show when AWS modules can't be imported
-import_error_msg = (
-    "The 'aws' dependency is not installed: {exception}. "
-    "Please reinstall with the '[aws]' or '[all]' extra install "
-    '`python -m pip install "geomancy[aws]"` or '
-    '`python -m pip install "geomancy[all]"`'
-)
 
-
-class CheckAWSS3BucketAccess(Check):
+class CheckAwsS3BucketAccess(CheckAws):
     """Check AWS S3 bucket availability"""
 
     msg = Parameter(
-        "CHECKAWSS3BUCKETACCESS.MSG",
+        "CHECK_AWS_S3_BUCKET_ACCESS.MSG",
         default="Check AWS S3 bucket access '{check.value}'...",
     )
 
-    import_error_msg = import_error_msg
-
     def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check the availability and access to S3 Bucket"""
         msg = self.msg.format(check=self)
 
         # Get the needed modules, bucket name and boto3 client
-        boto3, exceptions = self.import_modules("boto3", "botocore.exceptions")
+        exceptions = self.import_modules("botocore.exceptions")
         bucket_name = self.value.strip()
-        s3 = boto3.client("s3")
+
+        # Retrieve the client
+        try:
+            s3 = self.client("s3")
+        except CheckException as exc:
+            return Result(status=exc.args[0], msg=msg)
 
         # Retrieve information on the bucket
         try:
             response = s3.head_bucket(Bucket=bucket_name)
-
         except exceptions.NoCredentialsError as e:
             # Unable to authenticate the client
-            return Result(msg=msg, status="Unable to locate credentials")
-
+            return Result(status="failed (unable to locate credentials)", msg=msg)
         except exceptions.ClientError as e:
             response = e.response
 
             # Retrieve error information from the response
             error = response["Error"] if "Error" in response else None
             error_code = error["Code"] if error and "Code" in error else ""
             error_msg = error["Message"] if error and "Message" in error else ""
 
             logger.debug(f"s3.head_bucket error: {error}")
 
             if error_msg in ("Not Found",) and error_code == "404":
                 # Couldn't find the bucket
-                return Result(msg=msg, status="not found")
+                return Result(status="failed (not found)", msg=msg)
             elif error_msg in ("Forbidden",) and error_code == "403":
                 # Do no have access to an existing bucket
-                return Result(msg=msg, status="access forbidden")
+                return Result(status="failed (access forbidden)", msg=msg)
             else:
-                return Result(msg=msg, status="unknown reason")
+                return Result(status="failed (unknown reason)", msg=msg)
 
         except exceptions.ParamValidationError as e:
             # The bucket name failed validation
             report = e.kwargs["report"] if "report" in e.kwargs else None
 
             if isinstance(report, str):
-                return Result(msg=msg, status=report)
-            else:
-                return Result(msg=msg, status="invalid bucket name")
+                return Result(
+                    status=f"failed (invalid bucket name '{self.value}')", msg=msg
+                )
 
         # Parse the response
         metadata = (
             response["ResponseMetadata"] if "ResponseMetadata" in response else None
         )
         return_code = (
             metadata["HTTPStatusCode"]
             if metadata and "HTTPStatusCode" in metadata
             else None
         )
 
         if return_code == 200:
             # Successfully probed S3 bucket
-            return Result(msg=msg, status="passed")
+            return Result(status="passed", msg=msg)
         else:
             # It failed, and I don't know why
-            return Result(msg=msg, status="unknown reason")
+            return Result(status="failed (unknown reason)", msg=msg)
 
 
-class CheckAWSS3BucketPrivate(Check):
+class CheckAwsS3BucketPrivate(CheckAws):
     """Check AWS S3 buck availability"""
 
     msg = Parameter(
-        "CHECKAWSS3BUCKETPRIVATE.MSG",
+        "CHECK_AWS_S3_BUCKET_PRIVATE.MSG",
         default="Check AWS S3 bucket private '{check.value}'...",
     )
 
-    import_error_msg = import_error_msg
-
     def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check the availability and access to S3 Bucket.
 
         See: https://stackoverflow.com/a/59002759/9099988
         """
         msg = self.msg.format(check=self)
 
         # Get the needed modules, bucket name and boto3 client
-        boto3, exceptions = self.import_modules("boto3", "botocore.exceptions")
+        exceptions = self.import_modules("botocore.exceptions")
         bucket_name = self.value.strip()
-        s3 = boto3.client("s3")
+
+        # Retrieve the client
+        try:
+            s3 = self.client("s3")
+        except CheckException as exc:
+            return Result(status=exc.args[0], msg=msg)
 
         # 1. Check the PublicAccessBlock
         try:
             response = s3.get_public_access_block(Bucket=bucket_name)
         except (exceptions.BotoCoreError, exceptions.ClientError):
-            return Result(msg=msg, status="Couldn't access PublicAccessBlock")
+            return Result(status="failed (couldn't get public access block)", msg=msg)
 
         section = response.get("PublicAccessBlockConfiguration", {})
         block_public_policy = section.get("BlockPublicPolicy")
         block_public_acls = section.get("BlockPublicAcls")
 
         if block_public_policy and block_public_acls:
-            return Result(msg=msg, status="passed")
+            return Result(status="passed", msg=msg)
 
         logger.debug(f"Bucket '{bucket_name}' does not block all public access")
 
         # 2. Check the Bucket policy to see if it allows public access
         try:
             response = s3.get_bucket_policy_status(Bucket=bucket_name)
         except exceptions.ClientError:
@@ -156,79 +158,60 @@
 
         logger.debug(f"Bucket '{bucket_name}' ACL to groups is: {public_acl}")
 
         # Summary
         # If the policy is false and the acl doesn't have a grantee type of 'group',
         # then it should be private
         if not public_policy and not public_acl:
-            return Result(msg=msg, status="passed")
+            return Result(status="passed", msg=msg)
 
         # At this stage, all the checks for private have failed, and it appears
         # that the s3 bucket is publicly accessible
-        return Result(msg=msg, status="publicly accessible")
+        return Result(status="failed (publicly accessible)", msg=msg)
 
 
-class CheckAWSS3(Check):
+class CheckAwsS3(CheckAws):
     """Check AWS the availability and permissions of S3 buckets.
 
     Notes
     -----
     The child checks are meant to verify the accessibility of the bucket as well
     as optionally test for the best security practices`. Current, these include:
 
-    - Default private access (CheckAWSS3BucketPrivate)
+    - Default private access (CheckAwsS3BucketPrivate)
 
     See: https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html
     """
 
-    #: Whether to check that the bucket is private
+    #: Check that a bucket is private and fail if it is publicly accessible
     private: bool = True
 
     #: Alternative parameter names for private
     private_aliases = ("private",)
 
     msg = Parameter(
-        "CHECKAWSS3.MSG",
-        default="Check AWS S3 bucket '{check.value}'...",
+        "CHECK_AWS_S3.MSG",
+        default="Check AWS S3 bucket '{check.value}'",
     )
 
-    aliases = ("checkAWSS3", "checkAwsS3", "CheckAwsS3", "checkS3", "CheckS3")
+    aliases = ("checkAWSS3", "CheckAWSS3", "checkS3", "CheckS3")
 
     def __init__(self, *args, **kwargs):
         # Set up keyword arguments
         self.private = pop_first(kwargs, *self.private_aliases, default=self.private)
 
         # Set up the rest of the class
         super().__init__(*args, **kwargs)
 
         # Replace children with bucket sub-checls
         self.children.clear()
 
         # Bucket accessibility check
-        self.children.append(
-            CheckAWSS3BucketAccess(name=f"{self.name}Access", value=self.value)
-        )
+        child = CheckAwsS3BucketAccess(*args, **kwargs)
+        child.name = f"{self.name}Access"
+        self.children.append(child)
 
         # Bucket public access
         if self.private:
-            self.children.append(
-                CheckAWSS3BucketPrivate(name=f"{self.name}Private", value=self.value)
-            )
-
-    def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
-        """Run sub-checks in sequence, rather the Check base default.
-
-        This is done because the results of latter checks depend on earlier checks.
-        """
-        # check children
-        child_results = []
-        for child in self.children:
-            result = child.check(executor=executor, level=level + 1)
-            child_results.append(result)
-            if result.status != "passed":
-                break
-
-        return Result(
-            msg=f"[bold]{self.name}[/bold]",
-            children=child_results,
-            condition=self.condition,
-        )
+            child = CheckAwsS3BucketPrivate(*args, **kwargs)
+            child.name = f"{self.name}Private"
+            self.children.append(child)
```

### Comparing `geomancy-1.0.0/geomancy/checks/base.py` & `geomancy-1.1.1/geomancy/checks/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 """
-Abstract base class for checks
+Check base class and check groups that contain one or more child checks.
 """
 import typing as t
 import importlib
+import re
 from concurrent.futures import Future, Executor
 from types import ModuleType
 from inspect import isabstract
 from dataclasses import dataclass, field
 
 from rich.table import Table
 from rich.padding import Padding
 
 from .utils import pop_first, all_subclasses
 from ..config import Parameter
 from ..environment import sub_env
 
-__all__ = ("Check", "CheckException", "Result", "Executor")
+__all__ = ("Check", "CheckException", "Result", "CheckException", "Executor")
 
 
 class CheckException(Exception):
     """Exception raised when an error is encountered in the setup of a check."""
 
 
 @dataclass(slots=True)
 class Result:
     """A Check's result with awareness of concurrent.futures and rich
     functionality"""
 
-    #: Result's status--e.g. 'passed', 'failed', 'not found'
-    #: Only a 'passed' status is considered a passed result
+    #: Result's status--e.g. 'passed', 'failed', 'pending
+    #: Only a status that **starts with** 'passed' is considered a passed result
+    #: By convention, this string should start with 'passed', 'failed', 'warning'
+    #: or 'pending'. e.g. 'failed to find file'
     status: str = "pending"
 
+    #: Regular expression to validate allowed statuses
+    _allowed_re: t.Pattern[str] = field(
+        repr=False, default=re.compile(r"^(passed|failed|pending)( \([^)\n]+\))?$")
+    )
+
     #: Result message used when displaying the result. This may include
     #: rich tags
     msg: str = ""
 
     #: The pass condition for children checks and their passed property values
-    condition: t.Callable = all
+    condition: t.Callable = field(repr=False, default=all)
 
     #: The flat list of Results or Futures from children checks
     children: t.List[t.Union["Result", t.Awaitable["Result"]]] = field(
-        default_factory=list
+        repr=False,
+        default_factory=list,
     )
 
+    def __post_init__(self):
+        # Validate (on creation) that the status starts with an allowed value
+        assert self._allowed_re.match(self.status), (
+            f"The '{self.status}' status should match the following regular "
+            f"expression: '{self._allowed_re}'"
+        )
+
     @property
     def passed(self) -> bool:
         """Whether the check that generated this result passed.
 
         Notes
         -----
         This function checks whether children results have passed, whether this
@@ -58,32 +74,32 @@
 
         # Get the pass conditions for children. This list should only comprise
         # bools (True/False)
         children_passed = []
         for child in self.children:
             if isinstance(child, Result):
                 # The child is a Result object
-                child_status = child.status == "passed"
+                child_status = child.status.startswith("passed")
                 children_passed.append(child_status)
             elif isinstance(child, Future) and child.done():
                 # The child is a future with a result
                 result = child.result()
-                child_status = result.status == "passed"
+                child_status = result.status.startswith("passed")
                 children_passed.append(child_status)
             else:
                 # The child is a future that isn't done evaluating
                 done = False
                 children_passed.append(False)
 
         # Update the status from "pending" if this result is done (finished)
-        if self.status.lower() == "pending" and done:
+        if self.status.startswith("pending") and done:
             self.status = "passed" if self.condition(children_passed) else "failed"
 
         # Only a 'passed' status is considered a passed result
-        return self.status.lower() == "passed"
+        return self.status.startswith("passed")
 
     @property
     def done(self) -> bool:
         """Whether the check that generated this result and children checks are
         done"""
         # Get the done status for children. This list should only comprise
         # bools (True/False)
@@ -97,26 +113,41 @@
                 # The child is a future with a result
                 result = child.result()
                 child_done = result.done  # This function
                 children_done.append(child_done)
             else:
                 children_done.append(False)
 
-        if all(children_done) and self.status.lower() != "pending":
+        if all(children_done) and not self.status.startswith("pending"):
             # All children are done and this result has a non-pending status
             return True
-        elif all(children_done) and self.status.lower() == "pending":
+        elif all(children_done) and self.status.startswith("pending"):
             # All the children are done and this result's pending. This result's
             # status can be updated/changed from 'pending'. The passed
             # property will do this
             _ = self.passed  # update status from "pending" to something else
             return True
         else:
             return False
 
+    @property
+    def finished(self) -> t.List["Result"]:
+        """Return a flat list of currently finished results"""
+        finished = []
+        for child in self.children:
+            if isinstance(child, Result):
+                finished += child.finished  # this function
+            elif isinstance(child, Future) and child.done():
+                result = child.result()
+                finished += result.finished  # this function
+
+        if self.done:
+            finished = [self] + finished
+        return finished
+
     def rich_table(
         self, table: t.Optional[Table] = None, warning: bool = False, level: int = 0
     ) -> Table:
         """Generate a table with rich to display this result and child results
 
         Parameters
         ----------
@@ -139,18 +170,18 @@
         if table is None:
             table = Table(show_header=False, box=None, collapse_padding=True)
             table.add_column("Status")
             table.add_column("Value")
 
         # Format the checkbox string, status string and warning option for
         # children results
-        if self.status.lower() == "pending":
+        if self.status.lower().startswith("pending"):
             checkbox = "[ ]"
             status = f"[yellow]{self.status}[/yellow]"
-        elif self.status.lower() == "passed":
+        elif self.status.lower().startswith("passed"):
             checkbox = "[[green]:heavy_check_mark:[/green]]"
             status = f"[green]{self.status}[/green]"
             warning |= True  # All children should be marked as warnings
         elif warning:
             checkbox = "[[yellow]![/yellow]]"
             status = f"[yellow]{self.status}[/yellow]"
         else:
```

### Comparing `geomancy-1.0.0/geomancy/checks/env.py` & `geomancy-1.1.1/geomancy/checks/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Checks for environment variables
+Check the existence and, optionally, the value of an environment variable.
 """
 import typing as t
 import re
 
 from .base import Check, Result, Executor
 from ..environment import sub_env
 from ..config import Parameter
@@ -12,15 +12,15 @@
 class CheckEnv(Check):
     """Check the current environment variables."""
 
     #: (Optional) regex to match the environment variable value
     regex: t.Optional[t.Tuple[str, ...]] = None
 
     msg = Parameter(
-        "CHECKENV.MSG",
+        "CHECK_ENV.MSG",
         default="Check environment variable '{check.raw_value}'",
     )
 
     aliases = ("checkEnv",)
 
     def __init__(self, *args, regex: t.Optional[str] = None, **kwargs):
         super().__init__(*args, **kwargs)
@@ -29,20 +29,20 @@
     def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check the environment variable value."""
         # Substitute environment variables, if needed
         value = sub_env(self.raw_value) if self.raw_value is not None else None
 
         if value is None:
             # If the value is None, the environment variable doesn't exist.
-            status = "missing"
+            status = "failed (missing)"
         elif value == "":
             # An empty string environment variable is considered not set
-            status = "empty string"
+            status = "failed (empty string)"
         elif isinstance(self.regex, str) and re.match(self.regex, value) is None:
             # Check the regex, if specified
-            status = f"does not match regex '{self.regex}'"
+            status = f"failed (does not match regex '{self.regex}')"
         else:
             # All checks passed!
             status = "passed"
 
         msg = self.msg.format(check=self, status=status)
         return Result(msg=msg, status=status)
```

### Comparing `geomancy-1.0.0/geomancy/checks/exec.py` & `geomancy-1.1.1/geomancy/checks/exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Checks for executables
+Check the existence and, optionally, the version of available executables or
+commands.
 """
 import typing as t
 from shutil import which
 import subprocess
 
 from .version import CheckVersion
 from .utils import version_to_tuple
@@ -16,15 +17,15 @@
     """Check for the presence and version of executables"""
 
     #: The executable may exist and be installed, but get_current_version
     #: may not be able to identify the current version
     require_current_version = False
 
     msg = Parameter(
-        "CHECKEXEC.MSG",
+        "CHECK_EXEC.MSG",
         default="Check executable '{check.raw_value}'",
     )
 
     aliases = ("checkExec",)
 
     @property
     def value(
```

### Comparing `geomancy-1.0.0/geomancy/checks/path.py` & `geomancy-1.1.1/geomancy/checks/path.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Checks for paths
+Check the existence and, optionally, the type of path.
 """
 import typing as t
 from pathlib import Path
 
 from .base import Check, Result, CheckException, Executor
 from ..config import Parameter
 
@@ -15,15 +15,15 @@
 
     #: (Optional) the type of path expected
     type: t.Optional[str] = None
 
     #: The valid values of path types
     type_options = (None, "dir", "file")
 
-    msg = Parameter("CHECKPATH.MSG", default="Check path '{check.value}'")
+    msg = Parameter("CHECK_PATH.MSG", default="Check path '{check.value}'")
 
     aliases = ("checkPath",)
 
     def __init__(self, *args, type: t.Optional[str] = None, **kwargs):
         super().__init__(*args, **kwargs)
         if type not in self.type_options:
             raise CheckException(
@@ -34,17 +34,17 @@
 
     def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check paths"""
         value = self.value
         path = Path(value)
 
         if not path.exists():
-            status = "missing"
+            status = "failed (missing)"
         elif self.type == "dir" and not path.is_dir():
-            status = "not dir"
+            status = "failed (not dir)"
         elif self.type == "file" and not path.is_file():
-            status = "not file"
+            status = "failed (not file)"
         else:
             status = "passed"
 
         msg = self.msg.format(check=self, status=status)
         return Result(msg=msg, status=status)
```

### Comparing `geomancy-1.0.0/geomancy/checks/platform.py` & `geomancy-1.1.1/geomancy/checks/platform.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Checks the platform (Operating System) and its version
+Check the current platform (operating system) and, optionally, its minimum version.
 """
 import typing as t
 import platform
 import logging
 
 from .base import Result, Executor
 from .version import CheckVersion
@@ -16,15 +16,15 @@
 
 
 class CheckPlatform(CheckVersion):
     """Check the availability and version of a python package"""
 
     # The message for checking python packages
     msg = Parameter(
-        "CHECKPLATFORM.MSG",
+        "CHECK_PLATFORM.MSG",
         default="Check platform '{check.raw_value}'",
     )
 
     aliases = ("checkOS", "checkPlatform")
 
     def get_current_platform(self) -> str:
         """Retrieve the OS platform name"""
@@ -66,11 +66,11 @@
 
         # Get the OS name checked against
         name, op, version = self.value
         current_platform = self.get_current_platform()
 
         if current_platform.lower() != name.lower():
             # Failed check if the platform doesn't match this check
-            return Result(msg=msg, status="wrong platform")
+            return Result(status="failed (wrong platform)", msg=msg)
 
         # Check the version, as usual
         return super().check(level=level)
```

### Comparing `geomancy-1.0.0/geomancy/checks/python.py` & `geomancy-1.1.1/geomancy/checks/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Checks for python environment and packages
+Checks whether the python package is installed and, optionally, check its
+version.
 """
 import typing as t
 import logging
 import importlib.metadata  # python >= 3.8
 
 from .version import CheckVersion
 from .utils import version_to_tuple
@@ -15,15 +16,15 @@
 
 
 class CheckPythonPackage(CheckVersion):
     """Check the availability and version of a python package"""
 
     # The message for checking python packages
     msg = Parameter(
-        "CHECKPYTHONPACKAGE.MSG",
+        "CHECK_PYTHON_PACKAGE.MSG",
         default="Check python package '{check.raw_value}'",
     )
 
     aliases = ("checkPythonPackage", "checkPythonPkg", "CheckPythonPkg")
 
     def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
         # Get the package name, operator and version to check against (the last
```

### Comparing `geomancy-1.0.0/geomancy/checks/utils.py` & `geomancy-1.1.1/geomancy/checks/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/geomancy/checks/version.py` & `geomancy-1.1.1/geomancy/checks/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,24 +42,27 @@
     def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check whether the current version is compatible with the version
         specified in the value."""
         name, op, version = self.value
         current_version = self.get_current_version()
 
         if name is None:
-            status = "missing"
+            status = "failed (missing)"
         elif self.require_current_version and current_version is None:
-            status = "missing"
+            status = "failed (missing)"
         else:
             if version is not None and current_version is None:
                 status = "present but current version unknown"
             elif (
                 version is not None
                 and current_version is not None
                 and op is not None
                 and not op(current_version, version)
             ):
-                status = f"incorrect version=" f"{'.'.join(map(str, current_version))}"
+                status = (
+                    f"failed (incorrect version="
+                    f"{'.'.join(map(str, current_version))})"
+                )
             else:
                 status = "passed"
 
         return Result(msg=self.msg.format(check=self), status=status)
```

### Comparing `geomancy-1.0.0/geomancy/config/config.py` & `geomancy-1.1.1/geomancy/config/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/geomancy/entrypoints/check.py` & `geomancy-1.1.1/geomancy/entrypoints/check.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 import logging
 import tomllib
 import time
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import ExitStack
 
 import click
-from rich.live import Live
 import yaml
-import vcr
+from rich.live import Live
+from rich.console import Group
+from rich.rule import Rule
+from rich.console import Console, Theme
+import rich.progress as progress
 
 from .environment import env_options
 from .utils import filepaths
 from ..checks import Check
 from ..config import Config
 
-__all__ = ("check",)
+__all__ = ("check_cmd",)
 
 # Setup logger and configuration
 logger = logging.getLogger(__name__)
 
 
 # Exception classes
 class MissingChecks(click.ClickException):
@@ -36,16 +39,14 @@
     ".geomancy.??ml",
     "geomancy.??ml",
     "geomancy.yml",
     ".geomancy.yml",
 ]
 config.CLI.TOML_EXTS = [".toml"]  # Default file extensions for TOML files
 config.CLI.YAML_EXTS = [".yml", ".yaml"]  # Default file extensions for YAML files
-config.CLI.VCR.RECORD_MODE = "ONCE"  # record fixtures if they don't exist
-config.CLI.VCR.ADDITIONAL_FILTER_HEADERS = []
 
 
 def validate_checks_files(
     ctx: click.Context, param: click.Parameter, values: t.Tuple[str]
 ):
     """Validate the checks files arguments and convert to valid paths"""
     # Convert filepath strings into Path objects. Use default locations if
@@ -60,27 +61,20 @@
             "Could not find a checks file.", ctx=ctx, param=param
         )
     logging.debug(f"Checking the following files: {existing_files}")
     return existing_files
 
 
 # Setup 'check' command
-@click.command
+@click.command(name="check")
 @env_options
-@click.option(
-    "-f",
-    "--fixture",
-    required=False,
-    type=click.Path(),
-    help="Fixture to replace network requests",
-)
 @click.argument("checks_files", nargs=-1, type=str, callback=validate_checks_files)
-def check(checks_files, env, fixture):
+def check_cmd(checks_files, env):
     """Run checks"""
-    logger.debug(f"check_files={checks_files}, env={env}, fixture={fixture}")
+    logger.debug(f"check_files={checks_files}, env={env}")
 
     # Convert the checks_files into checks
     checks = []
     for checks_file in checks_files:
         # Parse the file by filetype
         if checks_file.suffix in config.CLI.TOML_EXTS:
             with open(checks_file, "rb") as f:
@@ -117,45 +111,70 @@
     else:
         plural = True if len(checks_files) > 1 else False
         raise MissingChecks(
             f"No checks were found in the file{'s' if plural else ''}: "
             f"{', '.join(map(str, checks_files))}."
         )
 
+    # Set up a console for rendering to the terminal
+    console = Console(theme=Theme({"repr.number": ""}))
+
     with ExitStack() as stack:
-        # Set up the context managers
-        executor = stack.enter_context(ThreadPoolExecutor())  # concurrent.futures
-        live = stack.enter_context(Live(refresh_per_second=4))  # rich live display
-
-        if fixture is not None:
-            # Request header items to remove before saving
-            filter_headers = {
-                "Authorization",
-                "User-Agent",
-                "X-Amz-Content-SHA256",
-                "X-Amz-Date",
-                "amz-sdk-invocation-id",
-                "amz-sdk-request",
-            }
-            filter_headers.update(config.CLI.VCR.ADDITIONAL_FILTER_HEADERS)
-            kwargs = {
-                "record_mode": config.CLI.VCR.RECORD_MODE,
-                "filter_headers": list(filter_headers),
-            }
+        # Context manager for running checks in multiple threads
+        executor = stack.enter_context(ThreadPoolExecutor())
 
-            stack.enter_context(vcr.use_cassette(fixture, **kwargs))  # vcr fixtures
+        # Context manager for rendering live to the terminal (rich)
+        live = stack.enter_context(Live(refresh_per_second=4, console=console))
 
         # Run the checks, display the results to the terminal
         result = check.check(executor=executor)
 
+        # Get the total number of checks
+        check_total = len(check.flatten)
+
+        # Set up a progress bar and render group
+        pbar = progress.Progress(
+            progress.SpinnerColumn(),
+            progress.BarColumn(),
+            progress.TextColumn("checks"),
+            progress.MofNCompleteColumn(),
+            progress.TimeRemainingColumn(),
+        )
+        task1 = pbar.add_task("checking...", total=check_total)
+
         # Update the display until the checks are done
         while not result.done:
             time.sleep(0.5)
-            live.update(result.rich_table())
 
-        # Print the final table
-        live.update(result.rich_table())
+            # Update progress
+            pbar.update(task1, completed=len(result.finished))
+
+            # Update group
+            group = Group(
+                result.rich_table(),
+                pbar.make_tasks_table(tasks=pbar.tasks),
+            )
+            live.update(group)
+
+        # Create a summary line to render
+        passed_total = len([r for r in result.finished if r.passed])
+        failed_total = check_total - passed_total
+        elapsed = sum(task.elapsed for task in pbar.tasks if task.elapsed is not None)
+
+        if result.passed:
+            color = "green"
+            title = f"[{color}][bold]{passed_total} passed[/bold][/{color}]"
+        else:
+            color = "red"
+            title = f"[{color}][bold]{failed_total} failed[/bold][/{color}]"
+
+        title = f"{title}[{color}] in {elapsed:.2f}s[/{color}]"
+        status = Rule(title=title, characters="=", style=color)
+
+        # Print the final table and summary
+        group = Group(result.rich_table(), status)
+        live.update(group)
 
     if not result.passed:
         exit(1)
 
     return result.passed
```

### Comparing `geomancy-1.0.0/geomancy/entrypoints/environment.py` & `geomancy-1.1.1/geomancy/entrypoints/environment.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/geomancy/entrypoints/utils.py` & `geomancy-1.1.1/geomancy/entrypoints/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/geomancy/environment/dotenv.py` & `geomancy-1.1.1/geomancy/environment/dotenv.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/geomancy.egg-info/PKG-INFO` & `geomancy-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: geomancy
-Version: 1.0.0
-Summary: Geomancy validates deployment and development environments
-Author: Justin Lorieau
-Keywords: .env,dotenv,env,env var,environment,environment variable,deployment,validation
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Bug Tracking
-Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Classifier: Topic :: System :: Monitoring
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Utilities
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: aws
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 <!-- start logo -->
 <img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/docs/_static/geomancy_logo.svg" alt="geomancy logo" height="150px"/>
 <!-- end logo -->
 
 <!-- start badges -->
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
@@ -62,15 +31,15 @@
 <strong><u>Validation of layered and combined environments</u></strong>
 </summary>
 
 Layered environments could include a _common_ or _base_ environment, with
 additional checks for settings of _test_, _development_ and _production_
 environments.
 
-In the following checks file, the existence of environment file and secrets
+In the following checks file, the existence of an environment file and a secrets
 file can be checked based on the ``$ENV`` environment variable. (See the
 [docker environment variable parameter expansion rules](https://docs.docker.com/compose/environment-variables/env-file/#parameter-expansion))
 
 ```yaml
 checks:
   Environment:
     desc: Check environment variables in different deployments
@@ -354,24 +323,28 @@
 ```
 </details>
 </p>
 
 <p>
 <details>
 <summary><strong><u>AWS</u></strong> resources exist and are securely setup
-  (<a href="https://geomancy.readthedocs.io/en/latest/usage/format.html#checkawss3">checkS3</a>)
+  (<a href="https://geomancy.readthedocs.io/en/latest/usage/checks/aws/index.html">AWS checks</a>)
 </summary>
 
 The following shows an example in yaml format. Checks can be formatted in
 toml format as well.
 
 ```yaml
 AWS:
+  IAM:
+    desc: Check the default authentication and security settings
+    checkIAM:
+
   TemplatesS3Bucket:
-    desc: The bucket for cloudformation templates
+    desc: Check the bucket for cloudformation templates
     checkS3: "myproject-cfn-templates"
 ```
 </details>
 </p>
 
 <!-- end features -->
 
@@ -411,22 +384,24 @@
           desc: Python interpreter ver 3.11 or higher
           checkExec: python3>=3.11
     ```
 
 2. Use ``geo`` to run the checks.
 
     ```shell
-    $ geo check
-    [✔] .geomancy.yaml...passed
+    [✔] test.yaml...passed
     [✔]   checks...passed
     [✔]     Environment...passed
-    [✔]       Check environment variable '$USER'......passed
+    [✔]       Check environment variable '$USER'...passed
     [✔]     Paths...passed
-    [✔]       Check path 'examples/geomancy.toml'......passed
-    [✔]       Check path 'examples/pyproject.toml'......passed
+    [✔]       Check path 'examples/geomancy.toml'...passed
+    [✔]       Check path 'examples/pyproject.toml'...passed
+    [✔]     Executables...passed
+    [✔]       Check executable 'python3>=3.11'...passed
+    ================================= 9 passed in 0.51s ==================================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 
@@ -435,13 +410,20 @@
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
 
 
 ## Bugs or Requests
 Please use the [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues)
 to submit bugs or request features.
 
+## Similar projects
+
+The following projects share some of the same goals in different contexts:
+
+- [Envalid](https://github.com/af/envalid)
+- [AWS Config](https://aws.amazon.com/config/)
+
 ## License
 
 Copyright Justin Lorieau and others, 2023.
 
 Distributed under the terms of the [MIT license](LICENSE).
 geomancy is free and open source software.
```

#### html2text {}

```diff
@@ -1,54 +1,39 @@
-Metadata-Version: 2.1 Name: geomancy Version: 1.0.0 Summary: Geomancy validates
-deployment and development environments Author: Justin Lorieau Keywords:
-.env,dotenv,env,env var,environment,environment variable,deployment,validation
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
-Classifier: Environment :: Console Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Bug Tracking Classifier: Topic ::
-Software Development :: Debuggers Classifier: Topic :: Software Development ::
-Quality Assurance Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance Classifier:
-Topic :: System :: Monitoring Classifier: Topic :: System :: Systems
-Administration Classifier: Topic :: Utilities Classifier: Development Status ::
-4 - Beta Requires-Python: >=3.11 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: aws Provides-Extra: dev Provides-Extra:
-docs License-File: LICENSE  [geomancy logo]   [![pypi version](https://
-img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/) [!
-[python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https:/
-/pypi.org/project/geomancy/) [![Black formatting](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black) [![Documentation
-Status](https://readthedocs.org/projects/geomancy/badge/?version=latest)]
-(https://geomancy.readthedocs.io/en/latest/?badge=latest)   Geomancy makes it
-easy to check and validate environments, such as development, testing and
-production. Environment checks and tests are helpful for testing the correct
-setting of environment variables, the installation and versions of installed
-executables, the state of external dependencies, like LaTeX packages, or cloud
-resources, or for checking environments that use the [12-factor](http://
-12factor.net/) principles.  ## Features  ### Capabilities
+ [geomancy logo]   [![pypi version](https://img.shields.io/pypi/v/
+geomancy.svg)](https://pypi.org/project/geomancy/) [![python versions](https://
+img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/
+geomancy/) [![Black formatting](https://img.shields.io/badge/code%20style-
+black-000000.svg)](https://github.com/psf/black) [![Documentation Status]
+(https://readthedocs.org/projects/geomancy/badge/?version=latest)](https://
+geomancy.readthedocs.io/en/latest/?badge=latest)   Geomancy makes it easy to
+check and validate environments, such as development, testing and production.
+Environment checks and tests are helpful for testing the correct setting of
+environment variables, the installation and versions of installed executables,
+the state of external dependencies, like LaTeX packages, or cloud resources, or
+for checking environments that use the [12-factor](http://12factor.net/
+) principles.  ## Features  ### Capabilities
   Validation_of_layered_and_combined_environments  Layered environments could
 include a _common_ or _base_ environment, with additional checks for settings
 of _test_, _development_ and _production_ environments. In the following checks
-file, the existence of environment file and secrets file can be checked based
-on the ``$ENV`` environment variable. (See the [docker environment variable
-parameter expansion rules](https://docs.docker.com/compose/environment-
-variables/env-file/#parameter-expansion)) ```yaml checks: Environment: desc:
-Check environment variables in different deployments CheckEnvFile: desc: Check
-the existence of the environment file checkPath: "deployments/${ENV}/.env"
-CheckSecretsFile: desc: Check the existence of the secrets file checkPath:
-"deployments/${ENV}/.secrets" ``` This check file can be used to check multiple
-environments: ```shell # check "dev" environment $ geo -e deployments/base/.env
--e deployments/dev/.env checks.yaml ... # check "test" environment $ geo -
-e deployments/base/.env -e deployments/test/.env checks.yaml ... ``` In this
-case, ``deployments/dev/.env`` is an [environment file](https://
-docs.docker.com/compose/environment-variables/env-file/) that sets ``ENV=dev``,
-``deployments/test/.env`` is an [environment file](https://docs.docker.com/
-compose/environment-variables/env-file/) that sets ``ENV=test``.
+file, the existence of an environment file and a secrets file can be checked
+based on the ``$ENV`` environment variable. (See the [docker environment
+variable parameter expansion rules](https://docs.docker.com/compose/
+environment-variables/env-file/#parameter-expansion)) ```yaml checks:
+Environment: desc: Check environment variables in different deployments
+CheckEnvFile: desc: Check the existence of the environment file checkPath:
+"deployments/${ENV}/.env" CheckSecretsFile: desc: Check the existence of the
+secrets file checkPath: "deployments/${ENV}/.secrets" ``` This check file can
+be used to check multiple environments: ```shell # check "dev" environment $
+geo -e deployments/base/.env -e deployments/dev/.env checks.yaml ... # check
+"test" environment $ geo -e deployments/base/.env -e deployments/test/.env
+checks.yaml ... ``` In this case, ``deployments/dev/.env`` is an [environment
+file](https://docs.docker.com/compose/environment-variables/env-file/) that
+sets ``ENV=dev``, ``deployments/test/.env`` is an [environment file](https://
+docs.docker.com/compose/environment-variables/env-file/) that sets
+``ENV=test``.
   Full_environment_file_support of the docker env_file_syntax  Environment
 files are loaded using the ``-e/--env`` option, which can be layered for
 different environments. ```shell # Run checks for 'dev' environment $ geo -
 e deployments/base/.env -e deployments/dev/.env check ... # Run checks for
 'test' environment $ geo -e base.env -e test.env run -- echo "Test environment"
 ```
   Concurrent_checks_with_multiple_threads to quickly probe I/O bound resources
@@ -108,34 +93,39 @@
 Windows 10 or later (released 2015) checkOS: "Windows >= 10" Environment: desc:
 Check environment variables common to all development environments Path: decs:
 Paths to search for executables checkEnv: $PATH Username: subchecks: any
 UnixUsername: # Username on linux and macOS desc: The current username
 checkEnv: $USER regex: "[a-z_][a-z0-9_-]*[$]?" WindowsUsername: # Username on
 Windows desc: The current username checkEnv: $USERNAME regex: "[a-z_][a-z0-9_-
 ]*[$]?" ```
- AWS resources exist and are securely setup (checkS3)  The following shows an
-example in yaml format. Checks can be formatted in toml format as well. ```yaml
-AWS: TemplatesS3Bucket: desc: The bucket for cloudformation templates checkS3:
-"myproject-cfn-templates" ```
+ AWS resources exist and are securely setup (AWS_checks)  The following shows
+an example in yaml format. Checks can be formatted in toml format as well.
+```yaml AWS: IAM: desc: Check the default authentication and security settings
+checkIAM: TemplatesS3Bucket: desc: Check the bucket for cloudformation
+templates checkS3: "myproject-cfn-templates" ```
  ## Quickstart  1. Create a ``.geomancy.yaml`` file with checks. See [examples/
 geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/
 geomancy.yaml) for an example of all checks. ```yaml checks: Environment: desc:
 Check environment variables common to all development environments Username:
 desc: The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?"
 Paths: desc: Checks the existence of needed files and directories subchecks:
 "any" # at least one of the files must be present Geomancy: desc: Check for the
 'geomancy.toml' file checkPath: examples/geomancy.toml type: file Pyproject:
 desc: Check for 'pyproject.toml' file checkPath: examples/pyproject.toml type:
 file Executables: desc: Check the availability of commands and their versions
 Python: desc: Python interpreter ver 3.11 or higher checkExec: python3>=3.11
-``` 2. Use ``geo`` to run the checks. ```shell $ geo check [â]
-.geomancy.yaml...passed [â] checks...passed [â] Environment...passed [â]
-Check environment variable '$USER'......passed [â] Paths...passed [â] Check
-path 'examples/geomancy.toml'......passed [â] Check path 'examples/
-pyproject.toml'......passed ``` (By default, ``geomancy`` will search
+``` 2. Use ``geo`` to run the checks. ```shell [â] test.yaml...passed [â]
+checks...passed [â] Environment...passed [â] Check environment variable
+'$USER'...passed [â] Paths...passed [â] Check path 'examples/
+geomancy.toml'...passed [â] Check path 'examples/pyproject.toml'...passed
+[â] Executables...passed [â] Check executable 'python3>=3.11'...passed
+================================= 9 passed in 0.51s
+================================== ``` (By default, ``geomancy`` will search
 ``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``, ``geomancy.toml``
 and ``pyproject.toml``.)  ## Documentation For full documentation please see
 https://geomancy.readthedocs.io/en/latest. ## Bugs or Requests Please use the
 [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues) to submit
-bugs or request features. ## License Copyright Justin Lorieau and others, 2023.
-Distributed under the terms of the [MIT license](LICENSE). geomancy is free and
-open source software.
+bugs or request features. ## Similar projects The following projects share some
+of the same goals in different contexts: - [Envalid](https://github.com/af/
+envalid) - [AWS Config](https://aws.amazon.com/config/) ## License Copyright
+Justin Lorieau and others, 2023. Distributed under the terms of the [MIT
+license](LICENSE). geomancy is free and open source software.
```

### Comparing `geomancy-1.0.0/geomancy.egg-info/SOURCES.txt` & `geomancy-1.1.1/geomancy.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,34 +4,43 @@
 .readthedocs.yaml
 LICENSE
 README.md
 Taskfile.yaml
 pyproject.toml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/tests.yml
-changelog/changelog_template.jinja
+changelog/_template.rst
 docs/conf.py
-docs/index.md
-docs/quickstart.md
+docs/index.rst
+docs/quickstart.rst
 docs/_static/custom.css
 docs/_static/geomancy_logo.png
 docs/_static/geomancy_logo.svg
-docs/about/changelog.md
+docs/about/changelog.rst
 docs/about/api/index.rst
-docs/checks/aws.md
-docs/checks/core.md
-docs/checks/snippets/base_args.md
-docs/guides/tips_and_tricks.md
-docs/usage/cmd_checks.md
-docs/usage/cmd_run.md
-docs/usage/format.md
+docs/guides/tips_and_tricks.rst
+docs/usage/cmd_checks.rst
+docs/usage/cmd_run.rst
+docs/usage/format.rst
+docs/usage/checks/index.rst
+docs/usage/checks/aws/iam.rst
+docs/usage/checks/aws/index.rst
+docs/usage/checks/aws/s3.rst
+docs/usage/checks/aws/snippets/common_args.rst
+docs/usage/checks/core/base.rst
+docs/usage/checks/core/env.rst
+docs/usage/checks/core/exec.rst
+docs/usage/checks/core/index.rst
+docs/usage/checks/core/path.rst
+docs/usage/checks/core/platform.rst
+docs/usage/checks/core/python.rst
+docs/usage/checks/snippets/common_args.rst
 examples/geomancy.toml
 examples/geomancy.yaml
 examples/pyproject.toml
-examples/aws/fixtures.yaml
 examples/aws/geomancy.yaml
 geomancy/__description__.txt
 geomancy/__init__.py
 geomancy.egg-info/PKG-INFO
 geomancy.egg-info/SOURCES.txt
 geomancy.egg-info/dependency_links.txt
 geomancy.egg-info/entry_points.txt
@@ -40,41 +49,63 @@
 geomancy/checks/__init__.py
 geomancy/checks/base.py
 geomancy/checks/env.py
 geomancy/checks/exec.py
 geomancy/checks/path.py
 geomancy/checks/platform.py
 geomancy/checks/python.py
+geomancy/checks/test.py
 geomancy/checks/utils.py
 geomancy/checks/version.py
 geomancy/checks/aws/__init__.py
+geomancy/checks/aws/base.py
+geomancy/checks/aws/iam.py
 geomancy/checks/aws/s3.py
 geomancy/config/__init__.py
 geomancy/config/config.py
 geomancy/entrypoints/__init__.py
 geomancy/entrypoints/check.py
 geomancy/entrypoints/config.py
 geomancy/entrypoints/environment.py
 geomancy/entrypoints/geo.py
 geomancy/entrypoints/run.py
 geomancy/entrypoints/utils.py
 geomancy/environment/__init__.py
 geomancy/environment/dotenv.py
 tests/conftest.py
+tests/checks/__init__.py
 tests/checks/test_base.py
 tests/checks/test_env.py
 tests/checks/test_exec.py
 tests/checks/test_path.py
 tests/checks/test_platform.py
 tests/checks/test_python.py
+tests/checks/aws/__init__.py
+tests/checks/aws/conftest.py
+tests/checks/aws/test_base.py
+tests/checks/aws/test_iam.py
 tests/checks/aws/test_s3.py
+tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml
+tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml
+tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml
 tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
 tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
 tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
 tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
 tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
 tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
+tests/config/__init__.py
 tests/config/config1.toml
 tests/config/test_config.py
 tests/data/test.env
+tests/entrypoints/__init__.py
 tests/entrypoints/test_geo.py
-tests/environment/test_dotenv.py
+tests/environment/__init__.py
+tests/environment/test_dotenv.py
+tests/utils/sleep.yaml
```

### Comparing `geomancy-1.0.0/pyproject.toml` & `geomancy-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     ]
 dynamic = ["version", "description"]
 dependencies = [
     "pyyaml>=6.0",  # Parsing YAML for checks (CheckBase) and Config
     "click>=8.1",  # Tool to develop CLI
     "click-default-group",  # All default click subcommands. e.g. geo -> geo check
     "rich>=13",  # Platform-independent terminal rendering
-    "vcrpy<5.0",  # Mock http interactions and fixtures
 ]
 
 [tool.setuptools]
 packages = ["geomancy"]
 
 [tool.setuptools.dynamic]
 version = {attr = "geomancy.__version__"}
@@ -63,14 +62,15 @@
     "boto3>=1.28",  # AWS CDK for checking Amazon services
 ]
 dev = [  # For development
     "pytest>=7.4",  # Testing framework
     "twine>=4.0",  # Manage package uploads
     "build",  # Manage package builds
     "black[d]",  # Code formatter
+    "vcrpy<5.0",  # Mock http interactions and fixtures
     "pytest-recording"  # Implementation of vcrpy in pytest
     ]
 docs = [  # For building documentation
     "sphinx",  # Document generator
     "furo>=2023",  # Document theme
     "sphinx_design>=0.4",  # Extra document components
     "myst-parser>=2.0",  # Support for markdown in documentation
@@ -82,21 +82,19 @@
 geo = "geomancy.entrypoints:geo_cli"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
 [tool.towncrier]
 package = "geomancy"
-filename = "docs/about/changelog.md"
-directory = "changelog/"
-template = "changelog/changelog_template.jinja"
-start_string = "<!-- towncrier release notes start -->\n"
-underlines = ["", "", ""]
-title_format = "## [{version}](https://github.com/jlorieau/geomancy/tree/{version}) - {project_date}"
-issue_format = "[#{issue}](https://github.com/jlorieau/geomancy/issues/{issue})"
+filename = "docs/about/changelog.rst"
+directory = "changelog"
+template = "changelog/_template.rst"
+title_format = "`{name} {version} <https://github.com/jlorieau/geomancy/tree/{version}>`_ - {project_date}"
+issue_format = "`#{issue} <https://github.com/jlorieau/geomancy/issues/{issue}>`_"
 
     [[tool.towncrier.type]]
     directory = "breaking"
     name = "Breaking Changes"
     showcontent = true
 
     [[tool.towncrier.type]]
```

### Comparing `geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml` & `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,20 @@
       string: ''
     headers:
       Connection:
       - close
       Content-Type:
       - application/xml
       Date:
-      - Sun, 30 Jul 2023 23:03:39 GMT
+      - Fri, 04 Aug 2023 20:31:49 GMT
       Server:
       - AmazonS3
       x-amz-bucket-region:
       - eu-west-1
+      x-amzn-RequestId: 99999999-9999-9999-9999-999999999999
     status:
       code: 400
       message: Bad Request
 - request:
     body: null
     headers: {}
     method: HEAD
@@ -29,16 +30,17 @@
   response:
     body:
       string: ''
     headers:
       Content-Type:
       - application/xml
       Date:
-      - Sun, 30 Jul 2023 23:03:39 GMT
+      - Fri, 04 Aug 2023 20:31:49 GMT
       Server:
       - AmazonS3
       x-amz-bucket-region:
       - eu-west-1
+      x-amzn-RequestId: 99999999-9999-9999-9999-999999999999
     status:
       code: 403
       message: Forbidden
 version: 1
```

### Comparing `geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml` & `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml` & `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml` & `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/checks/test_base.py` & `geomancy-1.1.1/tests/checks/test_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,73 @@
 """
 Test the environment variable check class
 """
+import typing as t
 from concurrent.futures import ThreadPoolExecutor
 
 import pytest
 
-from geomancy.checks import Check, Result, CheckException
+from geomancy.checks.base import Check, Result, CheckException, Executor
 
 
 class CheckDummy(Check):
     """A dummy Check subclass for testing aliases"""
 
     aliases = ("checkDummy",)
 
 
 class HangCheck(Check):
     """A Check subclass that allows thread hanging"""
 
     locked = True
 
-    def check(self, executor, level: int = 0):
+    def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         # The following hangs the thread until self.locked is set to False
         while self.locked:
             pass
         return Result(msg=self.name, status="passed")
 
 
 class DefaultCheck(Check):
     """A Check subclass that reads the returned result status from an instance
     attribute"""
 
     default_status = "passed"
 
-    def check(self, executor, level: int = 0):
+    def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         return Result(msg=self.name, status=self.default_status)
 
 
+def test_result_status_validation():
+    """The Result validation of status"""
+    # These are ok
+    allowed = (
+        "passed",
+        "failed",
+        "pending",
+        "passed (it went well)",
+        "failed (it didn't go well)",
+    )
+    for status in allowed:
+        Result(status=status)
+
+    # These are not ok
+    not_allowed = (
+        "passed ",  # extra space
+        "passed (open",  # parenthesis not closed
+        "passed  (it went well)",  # extra space before parenthesis
+        "passed (it went well) ",  # extra space after parenthesis
+        "passed (This has\na new line)",  # new line
+    )
+
+    for status in not_allowed:
+        with pytest.raises(AssertionError):
+            Result(status=status)
+
+
 def test_check_init_env_subtitute():
     """Test the Check init with env_substitute specified"""
     for kwargs, expected in (
         ({"env_substitute": False}, False),
         ({"substitute": False}, False),
         ({}, True),  # default
     ):
@@ -220,40 +248,14 @@
     assert other_pytest == pytest
 
     # Try a missing module
     with pytest.raises(ImportError):
         Check.import_modules("nonexist-missing")
 
 
-# noinspection GrazieInspection
-def test_check_result_done():
-    """Test Check.check and Result.done methods together."""
-
-    # Create a check with a thread-locking sub-check
-    sub = HangCheck(name="HangCheck")
-    check = Check(name="root", children=[sub])
-
-    # Create an executor to run the checks
-    with ThreadPoolExecutor() as executor:
-        result = check.check(executor=executor)
-
-        # The 'sub' has the thread hanged and can't finish its check
-        assert not result.done
-
-        # Releasing the thread lock should allow 'sub' to finish its check
-        sub.locked = False
-
-        # The release might not be instantaneously after releasing the lock,
-        # so we wait until the 'sub' check is done
-        while not result.done:
-            pass
-        assert result.done
-
-
-# noinspection GrazieInspection
 @pytest.mark.parametrize("condition", ("all", "any"))
 def test_check_result_passed(condition):
     """Test Check.check and Result.passed methods together (all condition."""
 
     # Create a check with a thread-locking sub-check
     sub1 = DefaultCheck(name="DefaultCheck1")
     sub2 = DefaultCheck(name="DefaultCheck2")
@@ -293,7 +295,59 @@
         result = check.check(executor=executor)
 
         while not result.done:  # Wait for the thread to evaluate
             pass
 
         assert not result.passed  # all children checks fail
         assert result.status == "failed"
+
+
+def test_check_result_done():
+    """Test Check.check and Result.done methods together."""
+
+    # Create a check with a thread-locking sub-check
+    sub = HangCheck(name="HangCheck")
+    check = Check(name="root", children=[sub])
+
+    # Create an executor to run the checks
+    with ThreadPoolExecutor() as executor:
+        result = check.check(executor=executor)
+
+        # The 'sub' has the thread hanged and can't finish its check
+        assert not result.done
+
+        # Releasing the thread lock should allow 'sub' to finish its check
+        sub.locked = False
+
+        # The release might not be instantaneously after releasing the lock,
+        # so we wait until the 'sub' check is done
+        while not result.done:
+            pass
+        assert result.done
+
+
+def test_check_result_finished():
+    """Test Check.check and Result.finished methods together."""
+
+    # Create a check with a thread-locking sub-check
+    sub = HangCheck(name="HangCheck")
+    check = Check(name="root", children=[sub])
+
+    # Create an executor to run the checks
+    with ThreadPoolExecutor() as executor:
+        result = check.check(executor=executor)
+
+        # The 'sub1' and 'sub2 has the thread hanged and can't finish their checks
+        assert not result.done
+        assert result.finished == []  # nothing is finished
+
+        # Release thread locks and check that it's finished
+        sub.locked = False
+
+        # The release might not be instantaneously after releasing the lock,
+        # so we wait until the 'sub' check is done
+        while not result.done:
+            pass
+
+        assert result.done
+        assert len(result.finished) == 2
+        assert all(isinstance(r, Result) for r in result.finished)
```

### Comparing `geomancy-1.0.0/tests/checks/test_env.py` & `geomancy-1.1.1/tests/checks/test_env.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/checks/test_exec.py` & `geomancy-1.1.1/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/checks/test_path.py` & `geomancy-1.1.1/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/checks/test_platform.py` & `geomancy-1.1.1/tests/checks/test_platform.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/checks/test_python.py` & `geomancy-1.1.1/tests/checks/test_python.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/config/test_config.py` & `geomancy-1.1.1/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.0.0/tests/entrypoints/test_geo.py` & `geomancy-1.1.1/tests/entrypoints/test_geo.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,25 +70,14 @@
 
     # Check, for example, that environment variables were checked
     assert any(
         msg in result.output for msg in ("Check environment variable", "Check path")
     )
 
 
-@pytest.mark.parametrize(
-    "checks_file,fixture",
-    (("examples/aws/geomancy.yaml", "examples/aws/fixtures.yaml"),),
-)
-def test_cli_check_fixtures(run, checks_file, fixture):
-    """Test the CLI with checks that require network access and therefore use
-    fixtures."""
-    # Run the command and test that an 0 error code was received
-    result = run(("--fixture", fixture, checks_file))
-
-
 @pytest.mark.parametrize("flag", ("", "--toml", "--yaml"))
 def test_cli_config(run, flag):
     """Test the --config option"""
     if flag:
         result = run(("config", flag))
     else:
         result = run(("config",))
```

### Comparing `geomancy-1.0.0/tests/environment/test_dotenv.py` & `geomancy-1.1.1/tests/environment/test_dotenv.py`

 * *Files identical despite different names*

