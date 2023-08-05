# Comparing `tmp/utz-0.4.1.tar.gz` & `tmp/utz-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utz-0.4.1.tar", last modified: Thu Aug  3 15:59:17 2023, max compression
+gzip compressed data, was "utz-0.4.2.tar", last modified: Sat Aug  5 03:23:56 2023, max compression
```

## Comparing `utz-0.4.1.tar` & `utz-0.4.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.878284 utz-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 15:57:40.000000 utz-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-03 15:59:17.878284 utz-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 15:57:40.000000 utz-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:59:17.878284 utz-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-03 15:57:40.000000 utz-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.874284 utz-0.4.1/utz/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-03 15:57:40.000000 utz-0.4.1/utz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 15:57:40.000000 utz-0.4.1/utz/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 15:57:40.000000 utz-0.4.1/utz/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-03 15:57:40.000000 utz-0.4.1/utz/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 15:57:40.000000 utz-0.4.1/utz/case.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 15:57:40.000000 utz-0.4.1/utz/cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 15:57:40.000000 utz-0.4.1/utz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-03 15:57:40.000000 utz-0.4.1/utz/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 15:57:40.000000 utz-0.4.1/utz/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-03 15:57:40.000000 utz-0.4.1/utz/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 15:57:40.000000 utz-0.4.1/utz/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-03 15:57:40.000000 utz-0.4.1/utz/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-03 15:57:40.000000 utz-0.4.1/utz/df_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-08-03 15:57:40.000000 utz-0.4.1/utz/diff_dfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.874284 utz-0.4.1/utz/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 15:57:40.000000 utz-0.4.1/utz/docker/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-03 15:57:40.000000 utz-0.4.1/utz/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 15:57:40.000000 utz-0.4.1/utz/fn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.878284 utz-0.4.1/utz/git/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/head.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-03 15:57:40.000000 utz-0.4.1/utz/git/submodule.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 15:57:40.000000 utz-0.4.1/utz/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 15:57:40.000000 utz-0.4.1/utz/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-03 15:57:40.000000 utz-0.4.1/utz/o.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 15:57:40.000000 utz-0.4.1/utz/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 15:57:40.000000 utz-0.4.1/utz/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-03 15:57:40.000000 utz-0.4.1/utz/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-03 15:57:40.000000 utz-0.4.1/utz/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-03 15:57:40.000000 utz-0.4.1/utz/pnds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.878284 utz-0.4.1/utz/process/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-03 15:57:40.000000 utz-0.4.1/utz/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-03 15:57:40.000000 utz-0.4.1/utz/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-03 15:57:40.000000 utz-0.4.1/utz/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 15:57:40.000000 utz-0.4.1/utz/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 15:57:40.000000 utz-0.4.1/utz/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-03 15:57:40.000000 utz-0.4.1/utz/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-03 15:57:40.000000 utz-0.4.1/utz/tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-03 15:57:40.000000 utz-0.4.1/utz/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-03 15:57:40.000000 utz-0.4.1/utz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-03 15:57:40.000000 utz-0.4.1/utz/ym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-08-03 15:57:40.000000 utz-0.4.1/utz/ymd.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 15:57:40.000000 utz-0.4.1/utz/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:59:17.874284 utz-0.4.1/utz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 15:59:17.000000 utz-0.4.1/utz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:23:56.643897 utz-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-05 03:22:05.000000 utz-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-05 03:23:56.643897 utz-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-05 03:22:05.000000 utz-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 03:23:56.643897 utz-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-05 03:22:05.000000 utz-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:23:56.639897 utz-0.4.2/utz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-05 03:22:05.000000 utz-0.4.2/utz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-05 03:22:05.000000 utz-0.4.2/utz/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-05 03:22:05.000000 utz-0.4.2/utz/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-05 03:22:05.000000 utz-0.4.2/utz/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-05 03:22:05.000000 utz-0.4.2/utz/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-05 03:22:05.000000 utz-0.4.2/utz/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-05 03:22:05.000000 utz-0.4.2/utz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-05 03:22:05.000000 utz-0.4.2/utz/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-05 03:22:05.000000 utz-0.4.2/utz/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-08-05 03:22:05.000000 utz-0.4.2/utz/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-05 03:22:05.000000 utz-0.4.2/utz/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-05 03:22:05.000000 utz-0.4.2/utz/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-05 03:22:05.000000 utz-0.4.2/utz/df_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-08-05 03:22:05.000000 utz-0.4.2/utz/diff_dfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:23:56.643897 utz-0.4.2/utz/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-05 03:22:05.000000 utz-0.4.2/utz/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-05 03:22:05.000000 utz-0.4.2/utz/docker/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-08-05 03:22:05.000000 utz-0.4.2/utz/docker/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-05 03:22:05.000000 utz-0.4.2/utz/docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-05 03:22:05.000000 utz-0.4.2/utz/docker/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-05 03:22:05.000000 utz-0.4.2/utz/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-05 03:22:05.000000 utz-0.4.2/utz/fn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:23:56.643897 utz-0.4.2/utz/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-05 03:22:05.000000 utz-0.4.2/utz/git/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-05 03:22:05.000000 utz-0.4.2/utz/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-05 03:22:05.000000 utz-0.4.2/utz/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-05 03:22:05.000000 utz-0.4.2/utz/o.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-05 03:22:05.000000 utz-0.4.2/utz/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-05 03:22:05.000000 utz-0.4.2/utz/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-05 03:22:05.000000 utz-0.4.2/utz/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-08-05 03:22:05.000000 utz-0.4.2/utz/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-05 03:22:05.000000 utz-0.4.2/utz/pnds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:23:56.643897 utz-0.4.2/utz/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-05 03:22:05.000000 utz-0.4.2/utz/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-05 03:22:05.000000 utz-0.4.2/utz/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-05 03:22:05.000000 utz-0.4.2/utz/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-05 03:22:05.000000 utz-0.4.2/utz/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-05 03:22:05.000000 utz-0.4.2/utz/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-05 03:22:05.000000 utz-0.4.2/utz/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-05 03:22:05.000000 utz-0.4.2/utz/tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-05 03:22:05.000000 utz-0.4.2/utz/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-05 03:22:05.000000 utz-0.4.2/utz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-05 03:22:05.000000 utz-0.4.2/utz/ym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-08-05 03:22:05.000000 utz-0.4.2/utz/ymd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-05 03:22:05.000000 utz-0.4.2/utz/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:23:56.639897 utz-0.4.2/utz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-05 03:23:56.000000 utz-0.4.2/utz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-05 03:23:56.000000 utz-0.4.2/utz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:23:56.000000 utz-0.4.2/utz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-05 03:23:56.000000 utz-0.4.2/utz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-05 03:23:56.000000 utz-0.4.2/utz.egg-info/top_level.txt
```

### Comparing `utz-0.4.1/LICENSE` & `utz-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/PKG-INFO` & `utz-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.4.1
+Version: 0.4.2
 Summary: ("oots"): imports and utilities for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `utz-0.4.1/README.md` & `utz-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/setup.py` & `utz-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,12 +27,12 @@
         'pytest-mock',
     ],
 }
 extras_require['all'] = sum(extras_require.values(), [ 'pyyaml', ])
 
 setup(
     name="utz",
-    version="0.4.1",
+    version="0.4.2",
     install_requires=open('requirements.txt', 'r').read(),
     extras_require=extras_require,
     url="https://github.com/runsascoded/utz",
 )
```

### Comparing `utz-0.4.1/utz/__init__.py` & `utz-0.4.2/utz/__init__.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/argparse.py` & `utz-0.4.2/utz/argparse.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/backoff.py` & `utz-0.4.2/utz/backoff.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/bases.py` & `utz-0.4.2/utz/bases.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/cli.py` & `utz-0.4.2/utz/cli.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/collections.py` & `utz-0.4.2/utz/collections.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/colors.py` & `utz-0.4.2/utz/colors.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/context.py` & `utz-0.4.2/utz/context.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/dataclasses.py` & `utz-0.4.2/utz/dataclasses.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/defaultdict.py` & `utz-0.4.2/utz/defaultdict.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/df_counts.py` & `utz-0.4.2/utz/df_counts.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/diff_dfs.py` & `utz-0.4.2/utz/diff_dfs.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/docker/dsl.py` & `utz-0.4.2/utz/docker/dsl.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/docker/file.py` & `utz-0.4.2/utz/docker/file.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/escape.py` & `utz-0.4.2/utz/escape.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/git/__init__.py` & `utz-0.4.2/utz/git/__init__.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/git/_checkout.py` & `utz-0.4.2/utz/git/_checkout.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/git/branch.py` & `utz-0.4.2/utz/git/branch.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/git/clone.py` & `utz-0.4.2/utz/git/clone.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/git/ctx.py` & `utz-0.4.2/utz/git/ctx.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/git/github.py` & `utz-0.4.2/utz/git/github.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 GITHUB_REPOSITORY = 'GITHUB_REPOSITORY'
 
 
 def repository_option(
         *flag_args,
         env=GITHUB_REPOSITORY,
-        help='Repository name with owner, e.g. "owner/repo"', **flag_kwargs,
+        help='Repository name (with owner, e.g. "owner/repo"), defaults to $GITHUB_REPOSITORY then `gh repo view --json nameWithOwner`', **flag_kwargs,
 ):
     if not flag_args:
         flag_args = ('-R', '--repository')
 
     def option(fn):
         import click
         @click.option(*flag_args, help=help, **flag_kwargs)
```

### Comparing `utz-0.4.1/utz/git/remote.py` & `utz-0.4.2/utz/git/remote.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/git/submodule.py` & `utz-0.4.2/utz/git/submodule.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/methods.py` & `utz-0.4.2/utz/methods.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/o.py` & `utz-0.4.2/utz/o.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/pdf.py` & `utz-0.4.2/utz/pdf.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/plots.py` & `utz-0.4.2/utz/plots.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/pnds.py` & `utz-0.4.2/utz/pnds.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/process/__init__.py` & `utz-0.4.2/utz/process/__init__.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/setup.py` & `utz-0.4.2/utz/setup.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/sql.py` & `utz-0.4.2/utz/sql.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/ssh.py` & `utz-0.4.2/utz/ssh.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/time.py` & `utz-0.4.2/utz/time.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/use.py` & `utz-0.4.2/utz/use.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/version.py` & `utz-0.4.2/utz/version.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/ym.py` & `utz-0.4.2/utz/ym.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/ymd.py` & `utz-0.4.2/utz/ymd.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz/zip.py` & `utz-0.4.2/utz/zip.py`

 * *Files identical despite different names*

### Comparing `utz-0.4.1/utz.egg-info/PKG-INFO` & `utz-0.4.2/utz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utz
-Version: 0.4.1
+Version: 0.4.2
 Summary: ("oots"): imports and utilities for easy wildcard-importing + boilerplate-reduction
 Home-page: https://github.com/runsascoded/utz
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `utz-0.4.1/utz.egg-info/SOURCES.txt` & `utz-0.4.2/utz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

