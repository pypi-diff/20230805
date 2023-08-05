# Comparing `tmp/geomancy-1.1.1.tar.gz` & `tmp/geomancy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-1.1.1.tar", last modified: Sat Aug  5 17:13:58 2023, max compression
+gzip compressed data, was "geomancy-1.1.2.tar", last modified: Sat Aug  5 21:37:12 2023, max compression
```

## Comparing `geomancy-1.1.1.tar` & `geomancy-1.1.2.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.360191 geomancy-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-05 17:13:44.000000 geomancy-1.1.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-05 17:13:44.000000 geomancy-1.1.1/.geomancy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.336192 geomancy-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-05 17:13:44.000000 geomancy-1.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-05 17:13:44.000000 geomancy-1.1.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-05 17:13:44.000000 geomancy-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-05 17:13:44.000000 geomancy-1.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-05 17:13:44.000000 geomancy-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-05 17:13:58.360191 geomancy-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-05 17:13:44.000000 geomancy-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-05 17:13:44.000000 geomancy-1.1.1/Taskfile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-05 17:13:44.000000 geomancy-1.1.1/changelog/_template.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    49829 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/_static/geomancy_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/_static/geomancy_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/about/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/about/api/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/about/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/about/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/guides/tips_and_tricks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/iam.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/s3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/aws/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/aws/snippets/common_args.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/env.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/exec.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/path.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/platform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/core/python.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/docs/usage/checks/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/checks/snippets/common_args.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/cmd_checks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/cmd_run.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-05 17:13:44.000000 geomancy-1.1.1/docs/usage/format.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/examples/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/aws/geomancy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/geomancy.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/geomancy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-05 17:13:44.000000 geomancy-1.1.1/examples/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/geomancy/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/__description__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/geomancy/checks/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/checks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/config/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/entrypoints/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/geomancy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-05 17:13:44.000000 geomancy-1.1.1/geomancy/environment/dotenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.344192 geomancy-1.1.1/geomancy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 17:13:58.000000 geomancy-1.1.1/geomancy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 17:13:44.000000 geomancy-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:13:58.360191 geomancy-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.348192 geomancy-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.352192 geomancy-1.1.1/tests/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.352192 geomancy-1.1.1/tests/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.340191 geomancy-1.1.1/tests/checks/aws/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.352192 geomancy-1.1.1/tests/checks/aws/cassettes/test_base/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/test_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/aws/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/checks/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/config/config1.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/data/test.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/entrypoints/test_geo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/environment/test_dotenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:13:58.356191 geomancy-1.1.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-05 17:13:44.000000 geomancy-1.1.1/tests/utils/sleep.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-05 21:37:01.000000 geomancy-1.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-05 21:37:01.000000 geomancy-1.1.2/.geomancy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.552366 geomancy-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-05 21:37:01.000000 geomancy-1.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-05 21:37:01.000000 geomancy-1.1.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-05 21:37:01.000000 geomancy-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-05 21:37:01.000000 geomancy-1.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-05 21:37:01.000000 geomancy-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-08-05 21:37:12.568366 geomancy-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-05 21:37:01.000000 geomancy-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-05 21:37:01.000000 geomancy-1.1.2/Taskfile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-05 21:37:01.000000 geomancy-1.1.2/changelog/48.bugfix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-05 21:37:01.000000 geomancy-1.1.2/changelog/_template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    49829 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/_static/geomancy_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/_static/geomancy_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/about/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/about/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/about/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/about/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/guides/tips_and_tricks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/iam.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/s3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/aws/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/aws/snippets/common_args.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/env.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/exec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/path.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/platform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/core/python.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/docs/usage/checks/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/checks/snippets/common_args.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/cmd_checks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/cmd_run.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-05 21:37:01.000000 geomancy-1.1.2/docs/usage/format.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/examples/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/aws/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/geomancy.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-05 21:37:01.000000 geomancy-1.1.2/examples/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.556366 geomancy-1.1.2/geomancy/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/__description__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19392 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/checks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/entrypoints/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/geomancy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-05 21:37:01.000000 geomancy-1.1.2/geomancy/environment/dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.560366 geomancy-1.1.2/geomancy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 21:37:12.000000 geomancy-1.1.2/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 21:37:01.000000 geomancy-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 21:37:12.568366 geomancy-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.552366 geomancy-1.1.2/tests/checks/aws/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/aws/cassettes/test_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.564366 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/test_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/aws/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/checks/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/config/config1.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/data/test.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/entrypoints/test_geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/environment/test_dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:37:12.568366 geomancy-1.1.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-05 21:37:01.000000 geomancy-1.1.2/tests/utils/sleep.yaml
```

### Comparing `geomancy-1.1.1/.geomancy.yaml` & `geomancy-1.1.2/.geomancy.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-checks:
-  desc: Check for the local development environment
+Executables:
+  Python3:
+    desc: Python version >=3.11 needed (https://www.python.org)
+    checkExec: python3 >= 3.11
+  Task:
+    desc: Task runner and build tool (Taskfile.yaml)
+    checkExec: task >= 3
+  Sphinx:
+    desc: Documentation building tool (https://www.sphinx-doc.org/en/master/)
+    checkExec: sphinx-build >= 6.2
+  Towncrier:
+    desc: Changelog building tool (https://pypi.org/project/towncrier/)
+    checkExec: towncrier >= 23
+  Twine:
+    desc: Build and upload packages on PyPI (https://pypi.org/project/twine/)
+    checkExec: twine >= 4
+  Pytest:
+    desc: Test python packages (https://github.com/pytest-dev/pytest)
+    checkExec: pytest >= 7
+  Black:
+    desc: Python code formatter (https://github.com/psf/black)
+    checkExec: black >= 23
 
-  Executables:
-    Python3:
-      desc: Python version >=3.11 needed (https://www.python.org)
-      checkExec: python3 >= 3.11
-    Task:
-      desc: Task runner and build tool (Taskfile.yaml)
-      checkExec: task >= 3
-    Sphinx:
-      desc: Documentation building tool (https://www.sphinx-doc.org/en/master/)
-      checkExec: sphinx-build >= 6.2
-    Towncrier:
-      desc: Changelog building tool (https://pypi.org/project/towncrier/)
-      checkExec: towncrier >= 23
-    Twine:
-      desc: Build and upload packages on PyPI (https://pypi.org/project/twine/)
-      checkExec: twine >= 4
-    Pytest:
-      desc: Test python packages (https://github.com/pytest-dev/pytest)
-      checkExec: pytest >= 7
-    Black:
-      desc: Python code formatter (https://github.com/psf/black)
-      checkExec: black >= 23
+Paths:
+  GeomancyYaml:
+    desc: Check development requirements
+    checkPath: .geomancy.yaml
+    type: file
 
-  Paths:
-    GeomancyYaml:
-      desc: Check development requirements
-      checkPath: .geomancy.yaml
-      type: file
-
-  PythonPackages:  # This section is redundant with pyproject.toml
-    PyYaml:
-      desc: YAML parser for Python (https://pypi.org/project/PyYAML/)
-      checkPythonPkg: pyyaml >= 6.0
-    Click:
-      desc: Command-line interface tool (https://pypi.org/project/click/)
-      checkPythonPkg: click >= 8.1
-    ClickDefaultGroup:
-      desc: Allow default commands for click (https://pypi.org/project/click-default-group/)
-      checkPythonPkg: click-default-group
-    Rich:
-      desc: CLI terminal renderer (https://pypi.org/project/rich/)
-      checkPythonPkg: rich >= 13
+PythonPackages:  # This section is redundant with pyproject.toml
+  PyYaml:
+    desc: YAML parser for Python (https://pypi.org/project/PyYAML/)
+    checkPythonPkg: pyyaml >= 6.0
+  Click:
+    desc: Command-line interface tool (https://pypi.org/project/click/)
+    checkPythonPkg: click >= 8.1
+  ClickDefaultGroup:
+    desc: Allow default commands for click (https://pypi.org/project/click-default-group/)
+    checkPythonPkg: click-default-group
+  Rich:
+    desc: CLI terminal renderer (https://pypi.org/project/rich/)
+    checkPythonPkg: rich >= 13
```

### Comparing `geomancy-1.1.1/.github/workflows/publish-to-pypi.yml` & `geomancy-1.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/.github/workflows/tests.yml` & `geomancy-1.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/.gitignore` & `geomancy-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/LICENSE` & `geomancy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/PKG-INFO` & `geomancy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Keywords: .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
@@ -382,57 +382,55 @@
 ## Quickstart
 <!-- start quickstart -->
 1. Create a ``.geomancy.yaml`` file with checks. See
    [examples/geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/geomancy.yaml)
    for an example of all checks.
 
     ```yaml
-    checks:
-      Environment:
-        desc: Check environment variables common to all development environments
-
-        Username:
-          desc: The current username
-          checkEnv: "$USER"
-          regex: "[a-z_][a-z0-9_-]*[$]?"
-
-      Paths:
-        desc: Checks the existence of needed files and directories
-        subchecks: "any" # at least one of the files must be present
-
-        Geomancy:
-          desc: Check for the 'geomancy.toml' file
-          checkPath: examples/geomancy.toml
-          type: file
-        Pyproject:
-          desc: Check for 'pyproject.toml' file
-          checkPath: examples/pyproject.toml
-          type: file
-
-      Executables:
-        desc: Check the availability of commands and their versions
-
-        Python:
-          desc: Python interpreter ver 3.11 or higher
-          checkExec: python3>=3.11
+    Environment:
+      desc: Check environment variables common to all development environments
+
+      Username:
+        desc: The current username
+        checkEnv: "$USER"
+        regex: "[a-z_][a-z0-9_-]*[$]?"
+
+    Paths:
+      desc: Checks the existence of needed files and directories
+      subchecks: "any" # at least one of the files must be present
+
+      Geomancy:
+        desc: Check for the 'geomancy.toml' file
+        checkPath: examples/geomancy.toml
+        type: file
+      Pyproject:
+        desc: Check for 'pyproject.toml' file
+        checkPath: examples/pyproject.toml
+        type: file
+
+    Executables:
+      desc: Check the availability of commands and their versions
+
+      Python:
+        desc: Python interpreter ver 3.11 or higher
+        checkExec: python3>=3.11
     ```
 
 2. Use ``geo`` to run the checks.
 
     ```shell
-    [✔] test.yaml...passed
-    [✔]   checks...passed
-    [✔]     Environment...passed
-    [✔]       Check environment variable '$USER'...passed
-    [✔]     Paths...passed
-    [✔]       Check path 'examples/geomancy.toml'...passed
-    [✔]       Check path 'examples/pyproject.toml'...passed
-    [✔]     Executables...passed
-    [✔]       Check executable 'python3>=3.11'...passed
-    ================================= 9 passed in 0.51s ==================================
+     [✔] test.yaml...passed
+     [✔]   Environment...passed
+     [✔]     Check environment variable '$USER'...passed
+     [✔]   Paths...passed
+     [✔]     Check path 'examples/geomancy.toml'...passed
+     [✔]     Check path 'examples/pyproject.toml'...passed
+     [✔]   Executables...passed
+     [✔]     Check executable 'python3>=3.11'...passed
+    ================================= 8 passed in 0.50s ==================================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geomancy Version: 1.1.1 Summary: Geomancy validates
+Metadata-Version: 2.1 Name: geomancy Version: 1.1.2 Summary: Geomancy validates
 deployment and development environments Author: Justin Lorieau Keywords:
 .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: MIT License
@@ -116,32 +116,32 @@
  AWS resources exist and are securely setup (AWS_checks)  The following shows
 an example in yaml format. Checks can be formatted in toml format as well.
 ```yaml AWS: IAM: desc: Check the default authentication and security settings
 checkIAM: TemplatesS3Bucket: desc: Check the bucket for cloudformation
 templates checkS3: "myproject-cfn-templates" ```
  ## Quickstart  1. Create a ``.geomancy.yaml`` file with checks. See [examples/
 geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/
-geomancy.yaml) for an example of all checks. ```yaml checks: Environment: desc:
-Check environment variables common to all development environments Username:
-desc: The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?"
-Paths: desc: Checks the existence of needed files and directories subchecks:
-"any" # at least one of the files must be present Geomancy: desc: Check for the
+geomancy.yaml) for an example of all checks. ```yaml Environment: desc: Check
+environment variables common to all development environments Username: desc:
+The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?" Paths:
+desc: Checks the existence of needed files and directories subchecks: "any" #
+at least one of the files must be present Geomancy: desc: Check for the
 'geomancy.toml' file checkPath: examples/geomancy.toml type: file Pyproject:
 desc: Check for 'pyproject.toml' file checkPath: examples/pyproject.toml type:
 file Executables: desc: Check the availability of commands and their versions
 Python: desc: Python interpreter ver 3.11 or higher checkExec: python3>=3.11
 ``` 2. Use ``geo`` to run the checks. ```shell [â] test.yaml...passed [â]
-checks...passed [â] Environment...passed [â] Check environment variable
-'$USER'...passed [â] Paths...passed [â] Check path 'examples/
-geomancy.toml'...passed [â] Check path 'examples/pyproject.toml'...passed
-[â] Executables...passed [â] Check executable 'python3>=3.11'...passed
-================================= 9 passed in 0.51s
-================================== ``` (By default, ``geomancy`` will search
-``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``, ``geomancy.toml``
-and ``pyproject.toml``.)  ## Documentation For full documentation please see
-https://geomancy.readthedocs.io/en/latest. ## Bugs or Requests Please use the
-[GitHub issue tracker](https://github.com/jlorieau/geomancy/issues) to submit
-bugs or request features. ## Similar projects The following projects share some
-of the same goals in different contexts: - [Envalid](https://github.com/af/
-envalid) - [AWS Config](https://aws.amazon.com/config/) ## License Copyright
-Justin Lorieau and others, 2023. Distributed under the terms of the [MIT
-license](LICENSE). geomancy is free and open source software.
+Environment...passed [â] Check environment variable '$USER'...passed [â]
+Paths...passed [â] Check path 'examples/geomancy.toml'...passed [â] Check
+path 'examples/pyproject.toml'...passed [â] Executables...passed [â] Check
+executable 'python3>=3.11'...passed ================================= 8 passed
+in 0.50s ================================== ``` (By default, ``geomancy`` will
+search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``,
+``geomancy.toml`` and ``pyproject.toml``.)  ## Documentation For full
+documentation please see https://geomancy.readthedocs.io/en/latest. ## Bugs or
+Requests Please use the [GitHub issue tracker](https://github.com/jlorieau/
+geomancy/issues) to submit bugs or request features. ## Similar projects The
+following projects share some of the same goals in different contexts: -
+[Envalid](https://github.com/af/envalid) - [AWS Config](https://aws.amazon.com/
+config/) ## License Copyright Justin Lorieau and others, 2023. Distributed
+under the terms of the [MIT license](LICENSE). geomancy is free and open source
+software.
```

### Comparing `geomancy-1.1.1/README.md` & `geomancy-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -351,57 +351,55 @@
 ## Quickstart
 <!-- start quickstart -->
 1. Create a ``.geomancy.yaml`` file with checks. See
    [examples/geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/geomancy.yaml)
    for an example of all checks.
 
     ```yaml
-    checks:
-      Environment:
-        desc: Check environment variables common to all development environments
-
-        Username:
-          desc: The current username
-          checkEnv: "$USER"
-          regex: "[a-z_][a-z0-9_-]*[$]?"
-
-      Paths:
-        desc: Checks the existence of needed files and directories
-        subchecks: "any" # at least one of the files must be present
-
-        Geomancy:
-          desc: Check for the 'geomancy.toml' file
-          checkPath: examples/geomancy.toml
-          type: file
-        Pyproject:
-          desc: Check for 'pyproject.toml' file
-          checkPath: examples/pyproject.toml
-          type: file
-
-      Executables:
-        desc: Check the availability of commands and their versions
-
-        Python:
-          desc: Python interpreter ver 3.11 or higher
-          checkExec: python3>=3.11
+    Environment:
+      desc: Check environment variables common to all development environments
+
+      Username:
+        desc: The current username
+        checkEnv: "$USER"
+        regex: "[a-z_][a-z0-9_-]*[$]?"
+
+    Paths:
+      desc: Checks the existence of needed files and directories
+      subchecks: "any" # at least one of the files must be present
+
+      Geomancy:
+        desc: Check for the 'geomancy.toml' file
+        checkPath: examples/geomancy.toml
+        type: file
+      Pyproject:
+        desc: Check for 'pyproject.toml' file
+        checkPath: examples/pyproject.toml
+        type: file
+
+    Executables:
+      desc: Check the availability of commands and their versions
+
+      Python:
+        desc: Python interpreter ver 3.11 or higher
+        checkExec: python3>=3.11
     ```
 
 2. Use ``geo`` to run the checks.
 
     ```shell
-    [✔] test.yaml...passed
-    [✔]   checks...passed
-    [✔]     Environment...passed
-    [✔]       Check environment variable '$USER'...passed
-    [✔]     Paths...passed
-    [✔]       Check path 'examples/geomancy.toml'...passed
-    [✔]       Check path 'examples/pyproject.toml'...passed
-    [✔]     Executables...passed
-    [✔]       Check executable 'python3>=3.11'...passed
-    ================================= 9 passed in 0.51s ==================================
+     [✔] test.yaml...passed
+     [✔]   Environment...passed
+     [✔]     Check environment variable '$USER'...passed
+     [✔]   Paths...passed
+     [✔]     Check path 'examples/geomancy.toml'...passed
+     [✔]     Check path 'examples/pyproject.toml'...passed
+     [✔]   Executables...passed
+     [✔]     Check executable 'python3>=3.11'...passed
+    ================================= 8 passed in 0.50s ==================================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
```

#### html2text {}

```diff
@@ -100,32 +100,32 @@
  AWS resources exist and are securely setup (AWS_checks)  The following shows
 an example in yaml format. Checks can be formatted in toml format as well.
 ```yaml AWS: IAM: desc: Check the default authentication and security settings
 checkIAM: TemplatesS3Bucket: desc: Check the bucket for cloudformation
 templates checkS3: "myproject-cfn-templates" ```
  ## Quickstart  1. Create a ``.geomancy.yaml`` file with checks. See [examples/
 geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/
-geomancy.yaml) for an example of all checks. ```yaml checks: Environment: desc:
-Check environment variables common to all development environments Username:
-desc: The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?"
-Paths: desc: Checks the existence of needed files and directories subchecks:
-"any" # at least one of the files must be present Geomancy: desc: Check for the
+geomancy.yaml) for an example of all checks. ```yaml Environment: desc: Check
+environment variables common to all development environments Username: desc:
+The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?" Paths:
+desc: Checks the existence of needed files and directories subchecks: "any" #
+at least one of the files must be present Geomancy: desc: Check for the
 'geomancy.toml' file checkPath: examples/geomancy.toml type: file Pyproject:
 desc: Check for 'pyproject.toml' file checkPath: examples/pyproject.toml type:
 file Executables: desc: Check the availability of commands and their versions
 Python: desc: Python interpreter ver 3.11 or higher checkExec: python3>=3.11
 ``` 2. Use ``geo`` to run the checks. ```shell [â] test.yaml...passed [â]
-checks...passed [â] Environment...passed [â] Check environment variable
-'$USER'...passed [â] Paths...passed [â] Check path 'examples/
-geomancy.toml'...passed [â] Check path 'examples/pyproject.toml'...passed
-[â] Executables...passed [â] Check executable 'python3>=3.11'...passed
-================================= 9 passed in 0.51s
-================================== ``` (By default, ``geomancy`` will search
-``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``, ``geomancy.toml``
-and ``pyproject.toml``.)  ## Documentation For full documentation please see
-https://geomancy.readthedocs.io/en/latest. ## Bugs or Requests Please use the
-[GitHub issue tracker](https://github.com/jlorieau/geomancy/issues) to submit
-bugs or request features. ## Similar projects The following projects share some
-of the same goals in different contexts: - [Envalid](https://github.com/af/
-envalid) - [AWS Config](https://aws.amazon.com/config/) ## License Copyright
-Justin Lorieau and others, 2023. Distributed under the terms of the [MIT
-license](LICENSE). geomancy is free and open source software.
+Environment...passed [â] Check environment variable '$USER'...passed [â]
+Paths...passed [â] Check path 'examples/geomancy.toml'...passed [â] Check
+path 'examples/pyproject.toml'...passed [â] Executables...passed [â] Check
+executable 'python3>=3.11'...passed ================================= 8 passed
+in 0.50s ================================== ``` (By default, ``geomancy`` will
+search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``,
+``geomancy.toml`` and ``pyproject.toml``.)  ## Documentation For full
+documentation please see https://geomancy.readthedocs.io/en/latest. ## Bugs or
+Requests Please use the [GitHub issue tracker](https://github.com/jlorieau/
+geomancy/issues) to submit bugs or request features. ## Similar projects The
+following projects share some of the same goals in different contexts: -
+[Envalid](https://github.com/af/envalid) - [AWS Config](https://aws.amazon.com/
+config/) ## License Copyright Justin Lorieau and others, 2023. Distributed
+under the terms of the [MIT license](LICENSE). geomancy is free and open source
+software.
```

### Comparing `geomancy-1.1.1/Taskfile.yaml` & `geomancy-1.1.2/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/changelog/_template.rst` & `geomancy-1.1.2/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/_static/custom.css` & `geomancy-1.1.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/_static/geomancy_logo.png` & `geomancy-1.1.2/docs/_static/geomancy_logo.png`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/_static/geomancy_logo.svg` & `geomancy-1.1.2/docs/_static/geomancy_logo.svg`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/about/api/index.rst` & `geomancy-1.1.2/docs/about/api/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/about/changelog.rst` & `geomancy-1.1.2/docs/about/changelog.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/conf.py` & `geomancy-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/guides/tips_and_tricks.rst` & `geomancy-1.1.2/docs/guides/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/index.rst` & `geomancy-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/aws/iam.rst` & `geomancy-1.1.2/docs/usage/checks/aws/iam.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/aws/index.rst` & `geomancy-1.1.2/docs/usage/checks/aws/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/aws/s3.rst` & `geomancy-1.1.2/docs/usage/checks/aws/s3.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/core/base.rst` & `geomancy-1.1.2/docs/usage/checks/core/base.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/core/env.rst` & `geomancy-1.1.2/docs/usage/checks/core/env.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/core/exec.rst` & `geomancy-1.1.2/docs/usage/checks/core/exec.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/core/index.rst` & `geomancy-1.1.2/docs/usage/checks/core/index.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/core/path.rst` & `geomancy-1.1.2/docs/usage/checks/core/path.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/core/platform.rst` & `geomancy-1.1.2/docs/usage/checks/core/platform.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/checks/core/python.rst` & `geomancy-1.1.2/docs/usage/checks/core/python.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/cmd_checks.rst` & `geomancy-1.1.2/docs/usage/cmd_checks.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/cmd_run.rst` & `geomancy-1.1.2/docs/usage/cmd_run.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/docs/usage/format.rst` & `geomancy-1.1.2/docs/usage/format.rst`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/examples/geomancy.toml` & `geomancy-1.1.2/examples/geomancy.toml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/examples/geomancy.yaml` & `geomancy-1.1.2/examples/geomancy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/aws/base.py` & `geomancy-1.1.2/geomancy/checks/aws/base.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/aws/iam.py` & `geomancy-1.1.2/geomancy/checks/aws/iam.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/aws/s3.py` & `geomancy-1.1.2/geomancy/checks/aws/s3.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/base.py` & `geomancy-1.1.2/geomancy/checks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     #: Only a status that **starts with** 'passed' is considered a passed result
     #: By convention, this string should start with 'passed', 'failed', 'warning'
     #: or 'pending'. e.g. 'failed to find file'
     status: str = "pending"
 
     #: Regular expression to validate allowed statuses
     _allowed_re: t.Pattern[str] = field(
-        repr=False, default=re.compile(r"^(passed|failed|pending)( \([^)\n]+\))?$")
+        repr=False, default=re.compile(r"^(passed|failed|pending)( \([^\n]+\))?$")
     )
 
     #: Result message used when displaying the result. This may include
     #: rich tags
     msg: str = ""
 
     #: The pass condition for children checks and their passed property values
```

### Comparing `geomancy-1.1.1/geomancy/checks/env.py` & `geomancy-1.1.2/geomancy/checks/env.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/exec.py` & `geomancy-1.1.2/geomancy/checks/exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/path.py` & `geomancy-1.1.2/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/platform.py` & `geomancy-1.1.2/geomancy/checks/platform.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/python.py` & `geomancy-1.1.2/geomancy/checks/python.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/test.py` & `geomancy-1.1.2/geomancy/checks/test.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/utils.py` & `geomancy-1.1.2/geomancy/checks/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/checks/version.py` & `geomancy-1.1.2/geomancy/checks/version.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/config/config.py` & `geomancy-1.1.2/geomancy/config/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/entrypoints/check.py` & `geomancy-1.1.2/geomancy/entrypoints/check.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/entrypoints/config.py` & `geomancy-1.1.2/geomancy/entrypoints/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/entrypoints/environment.py` & `geomancy-1.1.2/geomancy/entrypoints/environment.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/entrypoints/geo.py` & `geomancy-1.1.2/geomancy/entrypoints/geo.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/entrypoints/utils.py` & `geomancy-1.1.2/geomancy/entrypoints/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy/environment/dotenv.py` & `geomancy-1.1.2/geomancy/environment/dotenv.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/geomancy.egg-info/PKG-INFO` & `geomancy-1.1.2/geomancy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Keywords: .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
@@ -382,57 +382,55 @@
 ## Quickstart
 <!-- start quickstart -->
 1. Create a ``.geomancy.yaml`` file with checks. See
    [examples/geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/geomancy.yaml)
    for an example of all checks.
 
     ```yaml
-    checks:
-      Environment:
-        desc: Check environment variables common to all development environments
-
-        Username:
-          desc: The current username
-          checkEnv: "$USER"
-          regex: "[a-z_][a-z0-9_-]*[$]?"
-
-      Paths:
-        desc: Checks the existence of needed files and directories
-        subchecks: "any" # at least one of the files must be present
-
-        Geomancy:
-          desc: Check for the 'geomancy.toml' file
-          checkPath: examples/geomancy.toml
-          type: file
-        Pyproject:
-          desc: Check for 'pyproject.toml' file
-          checkPath: examples/pyproject.toml
-          type: file
-
-      Executables:
-        desc: Check the availability of commands and their versions
-
-        Python:
-          desc: Python interpreter ver 3.11 or higher
-          checkExec: python3>=3.11
+    Environment:
+      desc: Check environment variables common to all development environments
+
+      Username:
+        desc: The current username
+        checkEnv: "$USER"
+        regex: "[a-z_][a-z0-9_-]*[$]?"
+
+    Paths:
+      desc: Checks the existence of needed files and directories
+      subchecks: "any" # at least one of the files must be present
+
+      Geomancy:
+        desc: Check for the 'geomancy.toml' file
+        checkPath: examples/geomancy.toml
+        type: file
+      Pyproject:
+        desc: Check for 'pyproject.toml' file
+        checkPath: examples/pyproject.toml
+        type: file
+
+    Executables:
+      desc: Check the availability of commands and their versions
+
+      Python:
+        desc: Python interpreter ver 3.11 or higher
+        checkExec: python3>=3.11
     ```
 
 2. Use ``geo`` to run the checks.
 
     ```shell
-    [✔] test.yaml...passed
-    [✔]   checks...passed
-    [✔]     Environment...passed
-    [✔]       Check environment variable '$USER'...passed
-    [✔]     Paths...passed
-    [✔]       Check path 'examples/geomancy.toml'...passed
-    [✔]       Check path 'examples/pyproject.toml'...passed
-    [✔]     Executables...passed
-    [✔]       Check executable 'python3>=3.11'...passed
-    ================================= 9 passed in 0.51s ==================================
+     [✔] test.yaml...passed
+     [✔]   Environment...passed
+     [✔]     Check environment variable '$USER'...passed
+     [✔]   Paths...passed
+     [✔]     Check path 'examples/geomancy.toml'...passed
+     [✔]     Check path 'examples/pyproject.toml'...passed
+     [✔]   Executables...passed
+     [✔]     Check executable 'python3>=3.11'...passed
+    ================================= 8 passed in 0.50s ==================================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geomancy Version: 1.1.1 Summary: Geomancy validates
+Metadata-Version: 2.1 Name: geomancy Version: 1.1.2 Summary: Geomancy validates
 deployment and development environments Author: Justin Lorieau Keywords:
 .env,dotenv,env,env var,environment,environment variable,deployment,validation
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: MIT License
@@ -116,32 +116,32 @@
  AWS resources exist and are securely setup (AWS_checks)  The following shows
 an example in yaml format. Checks can be formatted in toml format as well.
 ```yaml AWS: IAM: desc: Check the default authentication and security settings
 checkIAM: TemplatesS3Bucket: desc: Check the bucket for cloudformation
 templates checkS3: "myproject-cfn-templates" ```
  ## Quickstart  1. Create a ``.geomancy.yaml`` file with checks. See [examples/
 geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/
-geomancy.yaml) for an example of all checks. ```yaml checks: Environment: desc:
-Check environment variables common to all development environments Username:
-desc: The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?"
-Paths: desc: Checks the existence of needed files and directories subchecks:
-"any" # at least one of the files must be present Geomancy: desc: Check for the
+geomancy.yaml) for an example of all checks. ```yaml Environment: desc: Check
+environment variables common to all development environments Username: desc:
+The current username checkEnv: "$USER" regex: "[a-z_][a-z0-9_-]*[$]?" Paths:
+desc: Checks the existence of needed files and directories subchecks: "any" #
+at least one of the files must be present Geomancy: desc: Check for the
 'geomancy.toml' file checkPath: examples/geomancy.toml type: file Pyproject:
 desc: Check for 'pyproject.toml' file checkPath: examples/pyproject.toml type:
 file Executables: desc: Check the availability of commands and their versions
 Python: desc: Python interpreter ver 3.11 or higher checkExec: python3>=3.11
 ``` 2. Use ``geo`` to run the checks. ```shell [â] test.yaml...passed [â]
-checks...passed [â] Environment...passed [â] Check environment variable
-'$USER'...passed [â] Paths...passed [â] Check path 'examples/
-geomancy.toml'...passed [â] Check path 'examples/pyproject.toml'...passed
-[â] Executables...passed [â] Check executable 'python3>=3.11'...passed
-================================= 9 passed in 0.51s
-================================== ``` (By default, ``geomancy`` will search
-``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``, ``geomancy.toml``
-and ``pyproject.toml``.)  ## Documentation For full documentation please see
-https://geomancy.readthedocs.io/en/latest. ## Bugs or Requests Please use the
-[GitHub issue tracker](https://github.com/jlorieau/geomancy/issues) to submit
-bugs or request features. ## Similar projects The following projects share some
-of the same goals in different contexts: - [Envalid](https://github.com/af/
-envalid) - [AWS Config](https://aws.amazon.com/config/) ## License Copyright
-Justin Lorieau and others, 2023. Distributed under the terms of the [MIT
-license](LICENSE). geomancy is free and open source software.
+Environment...passed [â] Check environment variable '$USER'...passed [â]
+Paths...passed [â] Check path 'examples/geomancy.toml'...passed [â] Check
+path 'examples/pyproject.toml'...passed [â] Executables...passed [â] Check
+executable 'python3>=3.11'...passed ================================= 8 passed
+in 0.50s ================================== ``` (By default, ``geomancy`` will
+search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml`` ``.geomancy.toml``,
+``geomancy.toml`` and ``pyproject.toml``.)  ## Documentation For full
+documentation please see https://geomancy.readthedocs.io/en/latest. ## Bugs or
+Requests Please use the [GitHub issue tracker](https://github.com/jlorieau/
+geomancy/issues) to submit bugs or request features. ## Similar projects The
+following projects share some of the same goals in different contexts: -
+[Envalid](https://github.com/af/envalid) - [AWS Config](https://aws.amazon.com/
+config/) ## License Copyright Justin Lorieau and others, 2023. Distributed
+under the terms of the [MIT license](LICENSE). geomancy is free and open source
+software.
```

### Comparing `geomancy-1.1.1/geomancy.egg-info/SOURCES.txt` & `geomancy-1.1.2/geomancy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 .readthedocs.yaml
 LICENSE
 README.md
 Taskfile.yaml
 pyproject.toml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/tests.yml
+changelog/48.bugfix.rst
 changelog/_template.rst
 docs/conf.py
 docs/index.rst
 docs/quickstart.rst
 docs/_static/custom.css
 docs/_static/geomancy_logo.png
 docs/_static/geomancy_logo.svg
```

### Comparing `geomancy-1.1.1/pyproject.toml` & `geomancy-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_base/test_check_aws_username_invalid_keys.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[120].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_access_key_age[30].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_authentication_invalid_keys.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_root_keys].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[has_signing_certs].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_iam/test_check_aws_iam_root_access[neither].yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml` & `geomancy-1.1.2/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/conftest.py` & `geomancy-1.1.2/tests/checks/aws/conftest.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/test_base.py` & `geomancy-1.1.2/tests/checks/aws/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/test_iam.py` & `geomancy-1.1.2/tests/checks/aws/test_iam.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/aws/test_s3.py` & `geomancy-1.1.2/tests/checks/aws/test_s3.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/test_base.py` & `geomancy-1.1.2/tests/checks/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/test_env.py` & `geomancy-1.1.2/tests/checks/test_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Test the environment variable check class
 """
 import os
 
+import pytest
 from pytest import MonkeyPatch
 
 from geomancy.checks import CheckEnv
 
 
 def test_check_env_missing():
     """Test CheckEnv for a missing environment variable"""
@@ -45,35 +46,41 @@
         assert check.name == "substitution"
         assert check.raw_value == f"${variable_name}"  # unprocessed value
         assert check.value == variable_value
 
         assert check.check().passed
 
 
-def test_check_env_regex(
-    variable_name="VARIABLE_NAME", variable_value="dev", regex="dev|prod|local"
-):
+@pytest.mark.parametrize("regex", ("dev|prod|local", "(dev|prod|local)"))
+def test_check_env_regex(regex):
+    variable_name = "VARIABLE_NAME"
+    variable_value = "dev"
+
     # Make sure the variable name isn't in the environment already
     assert variable_name not in os.environ
 
     # Place the variable in the environment and test the regex
     with MonkeyPatch.context() as mp:
         mp.setenv(variable_name, variable_value)
 
-        # The regex should match
+        # 1. The regex should match
         check1 = CheckEnv(name="regex1", value=f"${variable_name}", regex=regex)
-        assert check1.check().passed
+        result = check1.check()
+        assert result.passed
+        assert result.status == "passed"
 
         # Change the variable value to something else in which the regex will
         # fail
         mp.setenv(variable_name, f"!{variable_value}!")
 
-        # The regex should not match
+        # 2. The regex should not match
         check2 = CheckEnv(name="regex2", value=f"${variable_name}", regex=regex)
-        assert not check2.check().passed
+        result = check2.check()
+        assert not result.passed
+        assert result.status == f"failed (does not match regex '{regex}')"
 
 
 def test_check_base_types_dict():
     """Test the CheckBase.types_dict() method for the CheckEnv class."""
     types = CheckEnv.types()
 
     # Verify CheckEnv entries and aliases
```

### Comparing `geomancy-1.1.1/tests/checks/test_exec.py` & `geomancy-1.1.2/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/test_path.py` & `geomancy-1.1.2/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/test_platform.py` & `geomancy-1.1.2/tests/checks/test_platform.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/checks/test_python.py` & `geomancy-1.1.2/tests/checks/test_python.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/config/test_config.py` & `geomancy-1.1.2/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/conftest.py` & `geomancy-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/entrypoints/test_geo.py` & `geomancy-1.1.2/tests/entrypoints/test_geo.py`

 * *Files identical despite different names*

### Comparing `geomancy-1.1.1/tests/environment/test_dotenv.py` & `geomancy-1.1.2/tests/environment/test_dotenv.py`

 * *Files identical despite different names*

