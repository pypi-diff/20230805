# Comparing `tmp/mosec-0.7.2.tar.gz` & `tmp/mosec-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosec-0.7.2.tar", last modified: Wed Jun 21 03:43:27 2023, max compression
+gzip compressed data, was "mosec-0.8.0.tar", last modified: Sat Aug  5 01:37:24 2023, max compression
```

## Comparing `mosec-0.7.2.tar` & `mosec-0.8.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.460288 mosec-0.7.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-21 03:41:04.000000 mosec-0.7.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-21 03:41:04.000000 mosec-0.7.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-21 03:41:04.000000 mosec-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 03:41:04.000000 mosec-0.7.2/.lycheeignore
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-21 03:41:04.000000 mosec-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 03:41:04.000000 mosec-0.7.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-21 03:41:04.000000 mosec-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    29267 2023-06-21 03:41:04.000000 mosec-0.7.2/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 03:41:04.000000 mosec-0.7.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-21 03:41:04.000000 mosec-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 03:41:04.000000 mosec-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-21 03:41:04.000000 mosec-0.7.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-06-21 03:43:27.464288 mosec-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-21 03:41:04.000000 mosec-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-21 03:41:04.000000 mosec-0.7.2/build.envd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.460288 mosec-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.460288 mosec-0.7.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.460288 mosec-0.7.2/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/development/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/development/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.460288 mosec-0.7.2/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/echo.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/env.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/ipc.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/jax.md
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/metric.md
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/pytorch.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/stable_diffusion.md
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/examples/validate.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.460288 mosec-0.7.2/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/reference/arguments.md
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-21 03:41:04.000000 mosec-0.7.2/docs/source/reference/interface.md
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-21 03:41:04.000000 mosec-0.7.2/license.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/mosec/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 03:43:27.000000 mosec-0.7.2/mosec/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/dry_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/mosec/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/mixin/msgpack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/mixin/numbin_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/mixin/plasma_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/mixin/redis_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/mixin/typed_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/mosec/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/plugins/plasma_shm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/mosec/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-21 03:41:04.000000 mosec-0.7.2/mosec/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/mosec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-06-21 03:43:27.000000 mosec-0.7.2/mosec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-21 03:43:27.000000 mosec-0.7.2/mosec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:43:27.000000 mosec-0.7.2/mosec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:43:27.000000 mosec-0.7.2/mosec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-21 03:43:27.000000 mosec-0.7.2/mosec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 03:43:27.000000 mosec-0.7.2/mosec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-21 03:41:04.000000 mosec-0.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 03:41:04.000000 mosec-0.7.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-21 03:41:04.000000 mosec-0.7.2/requirements/doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 03:41:04.000000 mosec-0.7.2/requirements/mixin.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 03:41:04.000000 mosec-0.7.2/rustfmt.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:43:27.464288 mosec-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-21 03:41:04.000000 mosec-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:27.464288 mosec-0.7.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-21 03:41:04.000000 mosec-0.7.2/src/apidoc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-21 03:41:04.000000 mosec-0.7.2/src/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-21 03:41:04.000000 mosec-0.7.2/src/coordinator.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-21 03:41:04.000000 mosec-0.7.2/src/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-21 03:41:04.000000 mosec-0.7.2/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-21 03:41:04.000000 mosec-0.7.2/src/metrics.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-06-21 03:41:04.000000 mosec-0.7.2/src/protocol.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-21 03:41:04.000000 mosec-0.7.2/src/routes.rs
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-21 03:41:04.000000 mosec-0.7.2/src/tasks.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.603366 mosec-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.595366 mosec-0.8.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-05 01:35:41.000000 mosec-0.8.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-05 01:35:41.000000 mosec-0.8.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-05 01:35:41.000000 mosec-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-05 01:35:41.000000 mosec-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-05 01:35:41.000000 mosec-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-05 01:35:41.000000 mosec-0.8.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-05 01:35:41.000000 mosec-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35692 2023-08-05 01:35:41.000000 mosec-0.8.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-05 01:35:41.000000 mosec-0.8.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-08-05 01:35:41.000000 mosec-0.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-05 01:35:41.000000 mosec-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-05 01:35:41.000000 mosec-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-05 01:35:41.000000 mosec-0.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-08-05 01:37:24.603366 mosec-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-08-05 01:35:41.000000 mosec-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-05 01:35:41.000000 mosec-0.8.0/build.envd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.595366 mosec-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.595366 mosec-0.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.595366 mosec-0.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.595366 mosec-0.8.0/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/development/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/development/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.595366 mosec-0.8.0/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/echo.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/env.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/ipc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/jax.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/metric.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/multi_route.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/pytorch.md
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/stable_diffusion.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/examples/validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.595366 mosec-0.8.0/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/reference/arguments.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/reference/concept.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/reference/interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-05 01:35:41.000000 mosec-0.8.0/docs/source/reference/migration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-05 01:35:41.000000 mosec-0.8.0/license.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-05 01:35:41.000000 mosec-0.8.0/lychee.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.599367 mosec-0.8.0/mosec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-05 01:37:24.000000 mosec-0.8.0/mosec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.599367 mosec-0.8.0/mosec/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/mixin/msgpack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/mixin/numbin_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/mixin/plasma_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/mixin/redis_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/mixin/typed_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.603366 mosec-0.8.0/mosec/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-05 01:35:41.000000 mosec-0.8.0/mosec/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.599367 mosec-0.8.0/mosec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-08-05 01:37:24.000000 mosec-0.8.0/mosec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-05 01:37:24.000000 mosec-0.8.0/mosec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:37:24.000000 mosec-0.8.0/mosec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:37:24.000000 mosec-0.8.0/mosec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-05 01:37:24.000000 mosec-0.8.0/mosec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 01:37:24.000000 mosec-0.8.0/mosec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-08-05 01:35:41.000000 mosec-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.603366 mosec-0.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 01:35:41.000000 mosec-0.8.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-05 01:35:41.000000 mosec-0.8.0/requirements/doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-05 01:35:41.000000 mosec-0.8.0/requirements/mixin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-05 01:35:41.000000 mosec-0.8.0/rustfmt.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:37:24.603366 mosec-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-08-05 01:35:41.000000 mosec-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:37:24.603366 mosec-0.8.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-05 01:35:41.000000 mosec-0.8.0/src/apidoc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-08-05 01:35:41.000000 mosec-0.8.0/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-05 01:35:41.000000 mosec-0.8.0/src/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-05 01:35:41.000000 mosec-0.8.0/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-05 01:35:41.000000 mosec-0.8.0/src/metrics.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-08-05 01:35:41.000000 mosec-0.8.0/src/protocol.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-05 01:35:41.000000 mosec-0.8.0/src/routes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-08-05 01:35:41.000000 mosec-0.8.0/src/tasks.rs
```

### Comparing `mosec-0.7.2/.gitignore` & `mosec-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/CONTRIBUTING.md` & `mosec-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/Cargo.lock` & `mosec-0.8.0/Cargo.lock`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "argh"
-version = "0.1.10"
+name = "addr2line"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab257697eb9496bf75526f0217b5ed64636a9cfafa78b8365c71bd283fcef93e"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
 dependencies = [
- "argh_derive",
- "argh_shared",
+ "gimli",
 ]
 
 [[package]]
-name = "argh_derive"
-version = "0.1.10"
+name = "adler"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b382dbd3288e053331f03399e1db106c9fb0d8562ad62cb04859ae926f324fa6"
-dependencies = [
- "argh_shared",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "argh_shared"
-version = "0.1.10"
+name = "aho-corasick"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64cb94155d965e3d37ffbbe7cc5b82c3dd79dd33bd48e536f73d2cfb8d85506f"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+dependencies = [
+ "memchr",
+]
 
 [[package]]
 name = "async-channel"
-version = "1.8.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf46fee83e5ccffc220104713af3292ff9bc7c64c7de289f66dae8e38d826833"
+checksum = "81953c529336010edd6d8e358f886d9581267795c61b19475b71314bffa46d35"
 dependencies = [
  "concurrent-queue",
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
@@ -56,26 +52,26 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -126,91 +122,201 @@
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "block-buffer"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
+name = "byteorder"
+version = "1.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+
+[[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "concurrent-queue"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c278839b831783b70278b14df4d45e1beb1aad306c07bb796637de9a0e323e8e"
+checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
+name = "cpufeatures"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "crc32fast"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "crypto-common"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
+dependencies = [
+ "generic-array",
+ "typenum",
+]
+
+[[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "convert_case",
  "proc-macro2",
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "digest"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+dependencies = [
+ "block-buffer",
+ "crypto-common",
+]
+
+[[package]]
+name = "dirs"
+version = "4.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
+dependencies = [
+ "dirs-sys",
+]
+
+[[package]]
+name = "dirs-sys"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi",
+]
+
+[[package]]
 name = "dtoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "65d09067bfacaa79114679b279d7f5885b53295b1e2cfb4e79c8e4bd3d633169"
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
+name = "flate2"
+version = "1.0.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
+dependencies = [
+ "crc32fast",
+ "miniz_oxide",
+]
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures-channel"
 version = "0.3.28"
@@ -241,29 +347,53 @@
  "futures-core",
  "futures-task",
  "pin-project-lite",
  "pin-utils",
 ]
 
 [[package]]
-name = "hashbrown"
-version = "0.12.3"
+name = "generic-array"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+dependencies = [
+ "typenum",
+ "version_check",
+]
 
 [[package]]
-name = "hermit-abi"
-version = "0.2.6"
+name = "getrandom"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
+ "cfg-if",
  "libc",
+ "wasi",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+
+[[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "http"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
@@ -291,17 +421,17 @@
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
 [[package]]
 name = "hyper"
-version = "0.14.26"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "http",
  "http-body",
@@ -314,19 +444,19 @@
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.3"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
 dependencies = [
- "autocfg",
+ "equivalent",
  "hashbrown",
  "serde",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.6"
@@ -337,36 +467,33 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "matchit"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b87248edafb776e59e6ee64a79086f65890d3510f2c656c000bf2a7e8a0aea40"
 
@@ -379,61 +506,79 @@
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
+name = "mime_guess"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
+dependencies = [
+ "mime",
+ "unicase",
+]
+
+[[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "log",
  "wasi",
- "windows-sys 0.45.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "mosec"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
- "argh",
  "async-channel",
  "async-stream",
  "axum",
  "bytes",
  "derive_more",
  "hyper",
  "once_cell",
  "prometheus-client",
  "serde",
  "serde_json",
  "tokio",
  "tracing",
  "tracing-subscriber",
  "utoipa",
+ "utoipa-swagger-ui",
 ]
 
 [[package]]
 name = "nu-ansi-term"
 version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "num_threads"
@@ -441,14 +586,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "overload"
@@ -464,56 +618,56 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -539,17 +693,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.55"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0dd4be24fcdcfeaa12a432d588dc59bbad6cad3510c67e74a2b6b2fc950564"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prometheus-client"
 version = "0.21.1"
@@ -571,31 +725,109 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
+name = "redox_users"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+dependencies = [
+ "getrandom",
+ "redox_syscall 0.2.16",
+ "thiserror",
+]
+
+[[package]]
+name = "regex"
+version = "1.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+
+[[package]]
+name = "rust-embed"
+version = "6.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a36224c3276f8c4ebc8c20f158eca7ca4359c8db89991c4925132aaaf6702661"
+dependencies = [
+ "rust-embed-impl",
+ "rust-embed-utils",
+ "walkdir",
+]
+
+[[package]]
+name = "rust-embed-impl"
+version = "6.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49b94b81e5b2c284684141a2fb9e2a31be90638caf040bf9afbc5a0416afe1ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "rust-embed-utils",
+ "shellexpand",
+ "syn 2.0.22",
+ "walkdir",
+]
+
+[[package]]
+name = "rust-embed-utils"
+version = "7.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d38ff6bf570dc3bb7100fce9f7b60c33fa71d80e88da3f2580df4ff2bdded74"
+dependencies = [
+ "sha2",
+ "walkdir",
+]
+
+[[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
@@ -609,50 +841,59 @@
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
+name = "same-file"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
+dependencies = [
+ "winapi-util",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -673,23 +914,43 @@
  "form_urlencoded",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "sha2"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
+dependencies = [
+ "cfg-if",
+ "cpufeatures",
+ "digest",
+]
+
+[[package]]
 name = "sharded-slab"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
+name = "shellexpand"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7ccc8076840c4da029af4f87e4e8daeb0fca6b87bbb02e10cb60b791450e11e4"
+dependencies = [
+ "dirs",
+]
+
+[[package]]
 name = "signal-hook-registry"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
@@ -719,95 +980,116 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
+name = "thiserror"
+version = "1.0.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.22",
+]
+
+[[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "libc",
  "num_threads",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
@@ -845,28 +1127,28 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-log"
@@ -910,41 +1192,72 @@
 [[package]]
 name = "try-lock"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
 
 [[package]]
+name = "typenum"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+
+[[package]]
+name = "unicase"
+version = "2.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50f37be617794602aabbeee0be4f259dc1778fabe05e2d67ee8f79326d5cb4f6"
+dependencies = [
+ "version_check",
+]
+
+[[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "utoipa"
-version = "3.3.0"
+version = "3.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68ae74ef183fae36d650f063ae7bde1cacbe1cd7e72b617cbe1e985551878b98"
+checksum = "8c624186f22e625eb8faa777cb33d34cd595aa16d1742aa1d8b6cf35d3e4dda9"
 dependencies = [
  "indexmap",
  "serde",
  "serde_json",
  "utoipa-gen",
 ]
 
 [[package]]
 name = "utoipa-gen"
-version = "3.3.0"
+version = "3.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ea8ac818da7e746a63285594cce8a96f5e00ee31994e655bd827569cb8b137b"
+checksum = "b9ce5f21ca77e010f5283fa791c6ab892c68b3668a1bdc6b7ac6cf978f5d5b30"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.22",
+]
+
+[[package]]
+name = "utoipa-swagger-ui"
+version = "3.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "062bba5a3568e126ac72049a63254f4cb1da2eb713db0c1ab2a4c76be191db8c"
+dependencies = [
+ "axum",
+ "mime_guess",
+ "regex",
+ "rust-embed",
+ "serde",
+ "serde_json",
+ "utoipa",
+ "zip",
 ]
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
@@ -952,20 +1265,29 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "walkdir"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
+dependencies = [
+ "same-file",
+ "winapi-util",
+]
+
+[[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -984,143 +1306,98 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
+name = "winapi-util"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+dependencies = [
+ "winapi",
+]
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
-name = "windows_x86_64_msvc"
-version = "0.48.0"
+name = "zip"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
+dependencies = [
+ "byteorder",
+ "crc32fast",
+ "crossbeam-utils",
+ "flate2",
+]
```

### Comparing `mosec-0.7.2/Cargo.toml` & `mosec-0.8.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "mosec"
-version = "0.7.2"
+version = "0.8.0"
 authors = ["Keming <kemingy94@gmail.com>", "Zichen <lkevinzc@gmail.com>"]
 edition = "2021"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/mosecorg/mosec"
 description = "Model Serving made Efficient in the Cloud."
 documentation = "https://docs.rs/mosec"
@@ -15,16 +15,16 @@
 hyper = { version = "0.14", features = ["http1", "server", "runtime"] }
 bytes = "1"
 tracing = "0.1"
 tracing-subscriber = { version = "0.3", features = ["local-time", "json"] }
 tokio = { version = "1", features = ["rt", "rt-multi-thread", "time", "macros", "sync", "signal", "io-util"] }
 derive_more = { version = "0.99", features = ["display", "error", "from"] }
 # MPMS that only one consumer sees each message & async
-async-channel = { version = "1" }
+async-channel = "1.9"
 once_cell = "1.18"
-prometheus-client = "0.21.1"
-argh = "0.1"
-axum = "0.6.18"
+prometheus-client = "0.21"
+axum = "0.6"
 async-stream = "0.3.5"
-utoipa = "3.3.0"
-serde_json = "1.0.96"
-serde = "1.0.163"
+utoipa = "3.4"
+serde_json = "1.0"
+serde = "1.0"
+utoipa-swagger-ui = { version = "3", features = ["axum"] }
```

### Comparing `mosec-0.7.2/LICENSE` & `mosec-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/Makefile` & `mosec-0.8.0/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	rustup toolchain install nightly
 	rustup component add rustfmt --toolchain nightly
 
 dev:
 	cargo build
 	@mkdir -p mosec/bin
 	@cp ./target/debug/mosec mosec/bin/
-	pip install -e .
+	pip install -e .[dev,doc,mixin]
 
 test: dev
 	echo "Running tests for the main logic"
 	pytest tests -vv -s -m "not shm"
 	RUST_BACKTRACE=1 cargo test -vv
 
 test_shm: dev
@@ -28,17 +28,20 @@
 
 test_all: dev
 	@pip install -q -r requirements/mixin.txt
 	echo "Running tests for the all features"
 	pytest tests -vv -s
 	RUST_BACKTRACE=1 cargo test -vv
 
+test_chaos: dev
+	@python -m tests.bad_req
+
 doc:
 	@cd docs && make html && cd ../
-	@python -m http.server -d docs/build/html
+	@python -m http.server -d docs/build/html 7291 -b 127.0.0.1
 
 clean:
 	@cargo clean
 	@-rm -rf build/ dist/ .eggs/ site/ *.egg-info .pytest_cache .mypy_cache
 	@-find . -name '*.pyc' -type f -exec rm -rf {} +
 	@-find . -name '__pycache__' -exec rm -rf {} +
 
@@ -57,16 +60,17 @@
 	@black ${PY_SOURCE_FILES}
 	@cargo +nightly fmt --all
 
 lint:
 	@pip install -q -e .
 	isort --check --diff --project=mosec ${PY_SOURCE_FILES}
 	black --check --diff ${PY_SOURCE_FILES}
-	pylint -j 8 --recursive=y mosec
+	pylint -j 8 --recursive=y mosec setup.py
 	pylint -j 8 --recursive=y --disable=import-error examples --generated-members=numpy.*,torch.*,cv2.*,cv.*
+	pylint -j 8 --recursive=y tests --disable=unused-argument,missing-function-docstring,missing-class-docstring,redefined-outer-name,too-few-public-methods,consider-using-with
 	pydocstyle mosec
 	@-rm mosec/_version.py
 	pyright --stats
 	mypy --non-interactive --install-types ${PY_SOURCE_FILES}
 	cargo +nightly fmt -- --check
 
 semantic_lint:
```

### Comparing `mosec-0.7.2/PKG-INFO` & `mosec-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosec
-Version: 0.7.2
+Version: 0.8.0
 Summary: Model Serving made Efficient in the Cloud.
 Home-page: https://github.com/mosecorg/mosec
 Author: Keming Yang
 Author-email: kemingy94@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -21,14 +21,17 @@
 <p align="center">
   <a href="https://discord.gg/Jq5vxuH69W">
     <img alt="discord invitation link" src="https://dcbadge.vercel.app/api/server/Jq5vxuH69W?style=flat">
   </a>
   <a href="https://pypi.org/project/mosec/">
     <img src="https://badge.fury.io/py/mosec.svg" alt="PyPI version" height="20">
   </a>
+  <a href="https://anaconda.org/conda-forge/mosec">
+    <img src="https://anaconda.org/conda-forge/mosec/badges/version.svg" alt="conda-forge">
+  </a>
   <a href="https://pypi.org/project/mosec">
     <img src="https://img.shields.io/pypi/pyversions/mosec" alt="Python Version" />
   </a>
   <a href="https://pepy.tech/project/mosec">
     <img src="https://pepy.tech/badge/mosec/month" alt="PyPi Downloads" height="20">
   </a>
   <a href="https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)">
@@ -72,14 +75,17 @@
 
 ```shell
 pip install --upgrade diffusers[torch] transformers
 ```
 
 ### Write the server
 
+<details>
+<summary>Click me for server codes with explanations.</summary>
+
 Firstly, we import the libraries and set up a basic logger to better observe what happens.
 
 ```python
 from io import BytesIO
 from typing import List
 
 import torch  # type: ignore
@@ -104,15 +110,15 @@
 class StableDiffusion(MsgpackMixin, Worker):
     def __init__(self):
         self.pipe = StableDiffusionPipeline.from_pretrained(
             "runwayml/stable-diffusion-v1-5", torch_dtype=torch.float16
         )
         device = "cuda" if torch.cuda.is_available() else "cpu"
         self.pipe = self.pipe.to(device)
-        self.example = ["useless example prompt"] * 4  # warmup (bs=4)
+        self.example = ["useless example prompt"] * 4  # warmup (batch_size=4)
 
     def forward(self, data: List[str]) -> List[memoryview]:
         logger.debug("generate images for %s", data)
         res = self.pipe(data)
         logger.debug("NSFW: %s", res[1])
         images = []
         for img in res[0]:
@@ -120,48 +126,54 @@
             img.save(dummy_file, format="JPEG")
             images.append(dummy_file.getbuffer())
         return images
 ```
 
 > **Note**
 >
-> (a) In this example we return an image in the binary format, which JSON does not support (unless encoded with base64 that makes it longer). Hence, msgpack suits our need better. If we do not inherit `MsgpackMixin`, JSON will be used by default. In other words, the protocol of the service request/response can either be msgpack or JSON.
+> (a) In this example we return an image in the binary format, which JSON does not support (unless encoded with base64 that makes the payload larger). Hence, msgpack suits our need better. If we do not inherit `MsgpackMixin`, JSON will be used by default. In other words, the protocol of the service request/response can be either msgpack, JSON, or any other format (check our [mixins](https://mosecorg.github.io/mosec/reference/interface.html#module-mosec.mixin)).
 >
 > (b) Warm-up usually helps to allocate GPU memory in advance. If the warm-up example is specified, the service will only be ready after the example is forwarded through the handler. However, if no example is given, the first request's latency is expected to be longer. The `example` should be set as a single item or a tuple depending on what `forward` expects to receive. Moreover, in the case where you want to warm up with multiple different examples, you may set `multi_examples` (demo [here](https://mosecorg.github.io/mosec/examples/jax.html)).
 >
-> (c) This example shows a single-stage service, where the `StableDiffusion` worker directly takes in client's prompt request and responds the image. Thus the `forward` can be considered as a complete service handler. However, we can also design a multi-stage service with workers doing different jobs (e.g., downloading images, forward model, post-processing) in a pipeline. In this case, the whole pipeline is considered as the service handler, with the first worker taking in the request and the last worker sending out the response. The data flow between workers is done by inter-process communication.
+> (c) This example shows a single-stage service, where the `StableDiffusion` worker directly takes in client's prompt request and responds the image. Thus the `forward` can be considered as a complete service handler. However, we can also design a multi-stage service with workers doing different jobs (e.g., downloading images, model inference, post-processing) in a pipeline. In this case, the whole pipeline is considered as the service handler, with the first worker taking in the request and the last worker sending out the response. The data flow between workers is done by inter-process communication.
 >
 > (d) Since dynamic batching is enabled in this example, the `forward` method will wishfully receive a _list_ of string, e.g., `['a cute cat playing with a red ball', 'a man sitting in front of a computer', ...]`, aggregated from different clients for _batch inference_, improving the system throughput.
 
-Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the flag `--wait` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
+Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the `max_wait_time=10` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
 
 ```python
 if __name__ == "__main__":
     server = Server()
     # 1) `num` specifies the number of processes that will be spawned to run in parallel.
     # 2) By configuring the `max_batch_size` with the value > 1, the input data in your
     # `forward` function will be a list (batch); otherwise, it's a single item.
     server.append_worker(StableDiffusion, num=1, max_batch_size=4, max_wait_time=10)
     server.run()
 ```
+</details>
 
 ### Run the server
 
+<details>
+<summary>Click me to see how to run and query the server.</summary>
+
 The above snippets are merged in our example file. You may directly run at the project root level. We first have a look at the _command line arguments_ (explanations [here](https://mosecorg.github.io/mosec/reference/arguments.html)):
 
 ```shell
 python examples/stable_diffusion/server.py --help
 ```
 
 Then let's start the server with debug logs:
 
 ```shell
-python examples/stable_diffusion/server.py --debug
+python examples/stable_diffusion/server.py --log-level debug --timeout 30000
 ```
 
+Open `http://127.0.0.1:8000/openapi/swagger/` in your browser to get the OpenAPI doc.
+
 And in another terminal, test it:
 
 ```shell
 python examples/stable_diffusion/client.py --prompt "a cute cat playing with a red ball" --output cat.jpg --port 8000
 ```
 
 You will get an image named "cat.jpg" in the current directory.
@@ -169,49 +181,62 @@
 You can check the metrics:
 
 ```shell
 curl http://127.0.0.1:8000/metrics
 ```
 
 That's it! You have just hosted your **_stable-diffusion model_** as a service! 😉
+</details>
 
 ## Examples
 
 More ready-to-use examples can be found in the [Example](https://mosecorg.github.io/mosec/examples/index.html) section. It includes:
 
-- [Multi-stage workflow demo](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
+- [Pipeline](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
 - [Request validation](https://mosecorg.github.io/mosec/examples/validate.html): validate the request with type annotation.
+- [Multiple route](https://mosecorg.github.io/mosec/examples/multi_route.html): serve multiple models in one service
 - [Shared memory IPC](https://mosecorg.github.io/mosec/examples/ipc.html): inter-process communication with shared memory.
 - [Customized GPU allocation](https://mosecorg.github.io/mosec/examples/env.html): deploy multiple replicas, each using different GPUs.
 - [Customized metrics](https://mosecorg.github.io/mosec/examples/metric.html): record your own metrics for monitoring.
 - [Jax jitted inference](https://mosecorg.github.io/mosec/examples/jax.html): just-in-time compilation speeds up the inference.
 - PyTorch deep learning models:
   - [sentiment analysis](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing): infer the sentiment of a sentence.
   - [image recognition](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision): categorize a given image.
   - [stable diffusion](https://mosecorg.github.io/mosec/examples/stable_diffusion.html): generate images based on texts, with msgpack serialization.
 
 ## Configuration
 
 - Dynamic batching
-  - `max_batch_size` is configured when you `append_worker` (make sure inference with the max value won't cause the out-of-memory in GPU).
-  - `--wait (default=10ms)` is configured through CLI arguments (this usually should <= one batch inference duration).
-  - If enabled, it will collect a batch either when it reaches the `max_batch_size` or the `wait` time.
-- Check the [arguments doc](https://mosecorg.github.io/mosec/reference/arguments.html).
+  - `max_batch_size` and `max_wait_time (millisecond)` are configured when you call `append_worker`.
+  - Make sure inference with the `max_batch_size` value won't cause the out-of-memory in GPU.
+  - Normally, `max_wait_time` should be less than the batch inference time.
+  - If enabled, it will collect a batch either when the number of accumulated requests reaches `max_batch_size` or when `max_wait_time` has elapsed. The service will benefit from this feature when the traffic is high.
+- Check the [arguments doc](https://mosecorg.github.io/mosec/reference/arguments.html) for other configurations.
 
 ## Deployment
 
-- This may require some shared memory, remember to set the `--shm-size` flag if you are using docker.
-- This service doesn't require Gunicorn or NGINX, but you can certainly use the ingress controller. BTW, it should be the PID 1 process in the container since it controls multiple processes.
+- If you're looking for a GPU base image with `mosec` installed, you can check the official image [`mosecorg/mosec`](https://hub.docker.com/r/mosecorg/mosec). For the complex use case, check out [envd](https://github.com/tensorchord/envd).
+- This service doesn't need Gunicorn or NGINX, but you can certainly use the ingress controller when necessary.
+- This service should be the PID 1 process in the container since it controls multiple processes. If you need to run multiple processes in one container, you will need a supervisor. You may choose [Supervisor](https://github.com/Supervisor/supervisor) or [Horust](https://github.com/FedericoPonzi/Horust).
 - Remember to collect the **metrics**.
   - `mosec_service_batch_size_bucket` shows the batch size distribution.
   - `mosec_service_batch_duration_second_bucket` shows the duration of dynamic batching for each connection in each stage (starts from receiving the first task).
   - `mosec_service_process_duration_second_bucket` shows the duration of processing for each connection in each stage (including the IPC time but excluding the `mosec_service_batch_duration_second_bucket`).
   - `mosec_service_remaining_task` shows the number of currently processing tasks.
   - `mosec_service_throughput` shows the service throughput.
-- Stop the service with `SIGINT` or `SIGTERM` since it has the graceful shutdown logic.
+- Stop the service with `SIGINT` (`CTRL+C`) or `SIGTERM` (`kill {PID}`) since it has the graceful shutdown logic.
+
+## Performance tuning
+
+- Find out the best `max_batch_size` and `max_wait_time` for your inference service. The metrics will show the histograms of the real batch size and batch duration. Those are the key information to adjust these two parameters.
+- Try to split the whole inference process into separate CPU and GPU stages (ref [DistilBERT](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing)). Different stages will be run in a [data pipeline](https://en.wikipedia.org/wiki/Pipeline_(software)), which will keep the GPU busy.
+- You can also adjust the number of workers in each stage. For example, if your pipeline consists of a CPU stage for preprocessing and a GPU stage for model inference, increasing the number of CPU-stage workers can help to produce more data to be batched for model inference at the GPU stage; increasing the GPU-stage workers can fully utilize the GPU memory and computation power. Both ways may contribute to higher GPU utilization, which consequently results in higher service throughput.
+- For multi-stage services, note that the data passing through different stages will be serialized/deserialized by the `serialize_ipc/deserialize_ipc` methods, so extremely large data might make the whole pipeline slow. The serialized data is passed to the next stage through rust by default, you could enable shared memory to potentially reduce the latency (ref [RedisShmIPCMixin](https://mosecorg.github.io/mosec/examples/ipc.html#redis-shm-ipc-py)).
+- You should choose appropriate `serialize/deserialize` methods, which are used to decode the user request and encode the response. By default, both are using JSON. However, images and embeddings are not well supported by JSON. You can choose msgpack which is faster and binary compatible (ref [Stable Diffusion](https://mosecorg.github.io/mosec/examples/stable_diffusion.html)).
+- Configure the threads for OpenBLAS or MKL. It might not be able to choose the most suitable CPUs used by the current Python process. You can configure it for each worker by using the [env](https://mosecorg.github.io/mosec/reference/interface.html#mosec.server.Server.append_worker) (ref [custom GPU allocation](https://mosecorg.github.io/mosec/examples/env.html)).
 
 ## Adopters
 
 Here are some of the companies and individual users that are using Mosec:
 
 - [Modelz](https://modelz.ai): Serverless platform for ML inference.
 - [MOSS](https://github.com/OpenLMLab/MOSS/blob/main/README_en.md): An open sourced conversational language model like ChatGPT.
```

### Comparing `mosec-0.7.2/README.md` & `mosec-0.8.0/mosec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,37 @@
+Metadata-Version: 2.1
+Name: mosec
+Version: 0.8.0
+Summary: Model Serving made Efficient in the Cloud.
+Home-page: https://github.com/mosecorg/mosec
+Author: Keming Yang
+Author-email: kemingy94@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: mixin
+Provides-Extra: doc
+License-File: LICENSE
+
 <p align="center">
   <img src="https://user-images.githubusercontent.com/38581401/240117836-f06199ba-c80d-413a-9cb4-5adc76316bda.png" height="230" alt="MOSEC" />
 </p>
 
 <p align="center">
   <a href="https://discord.gg/Jq5vxuH69W">
     <img alt="discord invitation link" src="https://dcbadge.vercel.app/api/server/Jq5vxuH69W?style=flat">
   </a>
   <a href="https://pypi.org/project/mosec/">
     <img src="https://badge.fury.io/py/mosec.svg" alt="PyPI version" height="20">
   </a>
+  <a href="https://anaconda.org/conda-forge/mosec">
+    <img src="https://anaconda.org/conda-forge/mosec/badges/version.svg" alt="conda-forge">
+  </a>
   <a href="https://pypi.org/project/mosec">
     <img src="https://img.shields.io/pypi/pyversions/mosec" alt="Python Version" />
   </a>
   <a href="https://pepy.tech/project/mosec">
     <img src="https://pepy.tech/badge/mosec/month" alt="PyPi Downloads" height="20">
   </a>
   <a href="https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)">
@@ -56,14 +75,17 @@
 
 ```shell
 pip install --upgrade diffusers[torch] transformers
 ```
 
 ### Write the server
 
+<details>
+<summary>Click me for server codes with explanations.</summary>
+
 Firstly, we import the libraries and set up a basic logger to better observe what happens.
 
 ```python
 from io import BytesIO
 from typing import List
 
 import torch  # type: ignore
@@ -88,15 +110,15 @@
 class StableDiffusion(MsgpackMixin, Worker):
     def __init__(self):
         self.pipe = StableDiffusionPipeline.from_pretrained(
             "runwayml/stable-diffusion-v1-5", torch_dtype=torch.float16
         )
         device = "cuda" if torch.cuda.is_available() else "cpu"
         self.pipe = self.pipe.to(device)
-        self.example = ["useless example prompt"] * 4  # warmup (bs=4)
+        self.example = ["useless example prompt"] * 4  # warmup (batch_size=4)
 
     def forward(self, data: List[str]) -> List[memoryview]:
         logger.debug("generate images for %s", data)
         res = self.pipe(data)
         logger.debug("NSFW: %s", res[1])
         images = []
         for img in res[0]:
@@ -104,48 +126,54 @@
             img.save(dummy_file, format="JPEG")
             images.append(dummy_file.getbuffer())
         return images
 ```
 
 > **Note**
 >
-> (a) In this example we return an image in the binary format, which JSON does not support (unless encoded with base64 that makes it longer). Hence, msgpack suits our need better. If we do not inherit `MsgpackMixin`, JSON will be used by default. In other words, the protocol of the service request/response can either be msgpack or JSON.
+> (a) In this example we return an image in the binary format, which JSON does not support (unless encoded with base64 that makes the payload larger). Hence, msgpack suits our need better. If we do not inherit `MsgpackMixin`, JSON will be used by default. In other words, the protocol of the service request/response can be either msgpack, JSON, or any other format (check our [mixins](https://mosecorg.github.io/mosec/reference/interface.html#module-mosec.mixin)).
 >
 > (b) Warm-up usually helps to allocate GPU memory in advance. If the warm-up example is specified, the service will only be ready after the example is forwarded through the handler. However, if no example is given, the first request's latency is expected to be longer. The `example` should be set as a single item or a tuple depending on what `forward` expects to receive. Moreover, in the case where you want to warm up with multiple different examples, you may set `multi_examples` (demo [here](https://mosecorg.github.io/mosec/examples/jax.html)).
 >
-> (c) This example shows a single-stage service, where the `StableDiffusion` worker directly takes in client's prompt request and responds the image. Thus the `forward` can be considered as a complete service handler. However, we can also design a multi-stage service with workers doing different jobs (e.g., downloading images, forward model, post-processing) in a pipeline. In this case, the whole pipeline is considered as the service handler, with the first worker taking in the request and the last worker sending out the response. The data flow between workers is done by inter-process communication.
+> (c) This example shows a single-stage service, where the `StableDiffusion` worker directly takes in client's prompt request and responds the image. Thus the `forward` can be considered as a complete service handler. However, we can also design a multi-stage service with workers doing different jobs (e.g., downloading images, model inference, post-processing) in a pipeline. In this case, the whole pipeline is considered as the service handler, with the first worker taking in the request and the last worker sending out the response. The data flow between workers is done by inter-process communication.
 >
 > (d) Since dynamic batching is enabled in this example, the `forward` method will wishfully receive a _list_ of string, e.g., `['a cute cat playing with a red ball', 'a man sitting in front of a computer', ...]`, aggregated from different clients for _batch inference_, improving the system throughput.
 
-Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the flag `--wait` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
+Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the `max_wait_time=10` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
 
 ```python
 if __name__ == "__main__":
     server = Server()
     # 1) `num` specifies the number of processes that will be spawned to run in parallel.
     # 2) By configuring the `max_batch_size` with the value > 1, the input data in your
     # `forward` function will be a list (batch); otherwise, it's a single item.
     server.append_worker(StableDiffusion, num=1, max_batch_size=4, max_wait_time=10)
     server.run()
 ```
+</details>
 
 ### Run the server
 
+<details>
+<summary>Click me to see how to run and query the server.</summary>
+
 The above snippets are merged in our example file. You may directly run at the project root level. We first have a look at the _command line arguments_ (explanations [here](https://mosecorg.github.io/mosec/reference/arguments.html)):
 
 ```shell
 python examples/stable_diffusion/server.py --help
 ```
 
 Then let's start the server with debug logs:
 
 ```shell
-python examples/stable_diffusion/server.py --debug
+python examples/stable_diffusion/server.py --log-level debug --timeout 30000
 ```
 
+Open `http://127.0.0.1:8000/openapi/swagger/` in your browser to get the OpenAPI doc.
+
 And in another terminal, test it:
 
 ```shell
 python examples/stable_diffusion/client.py --prompt "a cute cat playing with a red ball" --output cat.jpg --port 8000
 ```
 
 You will get an image named "cat.jpg" in the current directory.
@@ -153,49 +181,62 @@
 You can check the metrics:
 
 ```shell
 curl http://127.0.0.1:8000/metrics
 ```
 
 That's it! You have just hosted your **_stable-diffusion model_** as a service! 😉
+</details>
 
 ## Examples
 
 More ready-to-use examples can be found in the [Example](https://mosecorg.github.io/mosec/examples/index.html) section. It includes:
 
-- [Multi-stage workflow demo](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
+- [Pipeline](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
 - [Request validation](https://mosecorg.github.io/mosec/examples/validate.html): validate the request with type annotation.
+- [Multiple route](https://mosecorg.github.io/mosec/examples/multi_route.html): serve multiple models in one service
 - [Shared memory IPC](https://mosecorg.github.io/mosec/examples/ipc.html): inter-process communication with shared memory.
 - [Customized GPU allocation](https://mosecorg.github.io/mosec/examples/env.html): deploy multiple replicas, each using different GPUs.
 - [Customized metrics](https://mosecorg.github.io/mosec/examples/metric.html): record your own metrics for monitoring.
 - [Jax jitted inference](https://mosecorg.github.io/mosec/examples/jax.html): just-in-time compilation speeds up the inference.
 - PyTorch deep learning models:
   - [sentiment analysis](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing): infer the sentiment of a sentence.
   - [image recognition](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision): categorize a given image.
   - [stable diffusion](https://mosecorg.github.io/mosec/examples/stable_diffusion.html): generate images based on texts, with msgpack serialization.
 
 ## Configuration
 
 - Dynamic batching
-  - `max_batch_size` is configured when you `append_worker` (make sure inference with the max value won't cause the out-of-memory in GPU).
-  - `--wait (default=10ms)` is configured through CLI arguments (this usually should <= one batch inference duration).
-  - If enabled, it will collect a batch either when it reaches the `max_batch_size` or the `wait` time.
-- Check the [arguments doc](https://mosecorg.github.io/mosec/reference/arguments.html).
+  - `max_batch_size` and `max_wait_time (millisecond)` are configured when you call `append_worker`.
+  - Make sure inference with the `max_batch_size` value won't cause the out-of-memory in GPU.
+  - Normally, `max_wait_time` should be less than the batch inference time.
+  - If enabled, it will collect a batch either when the number of accumulated requests reaches `max_batch_size` or when `max_wait_time` has elapsed. The service will benefit from this feature when the traffic is high.
+- Check the [arguments doc](https://mosecorg.github.io/mosec/reference/arguments.html) for other configurations.
 
 ## Deployment
 
-- This may require some shared memory, remember to set the `--shm-size` flag if you are using docker.
-- This service doesn't require Gunicorn or NGINX, but you can certainly use the ingress controller. BTW, it should be the PID 1 process in the container since it controls multiple processes.
+- If you're looking for a GPU base image with `mosec` installed, you can check the official image [`mosecorg/mosec`](https://hub.docker.com/r/mosecorg/mosec). For the complex use case, check out [envd](https://github.com/tensorchord/envd).
+- This service doesn't need Gunicorn or NGINX, but you can certainly use the ingress controller when necessary.
+- This service should be the PID 1 process in the container since it controls multiple processes. If you need to run multiple processes in one container, you will need a supervisor. You may choose [Supervisor](https://github.com/Supervisor/supervisor) or [Horust](https://github.com/FedericoPonzi/Horust).
 - Remember to collect the **metrics**.
   - `mosec_service_batch_size_bucket` shows the batch size distribution.
   - `mosec_service_batch_duration_second_bucket` shows the duration of dynamic batching for each connection in each stage (starts from receiving the first task).
   - `mosec_service_process_duration_second_bucket` shows the duration of processing for each connection in each stage (including the IPC time but excluding the `mosec_service_batch_duration_second_bucket`).
   - `mosec_service_remaining_task` shows the number of currently processing tasks.
   - `mosec_service_throughput` shows the service throughput.
-- Stop the service with `SIGINT` or `SIGTERM` since it has the graceful shutdown logic.
+- Stop the service with `SIGINT` (`CTRL+C`) or `SIGTERM` (`kill {PID}`) since it has the graceful shutdown logic.
+
+## Performance tuning
+
+- Find out the best `max_batch_size` and `max_wait_time` for your inference service. The metrics will show the histograms of the real batch size and batch duration. Those are the key information to adjust these two parameters.
+- Try to split the whole inference process into separate CPU and GPU stages (ref [DistilBERT](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing)). Different stages will be run in a [data pipeline](https://en.wikipedia.org/wiki/Pipeline_(software)), which will keep the GPU busy.
+- You can also adjust the number of workers in each stage. For example, if your pipeline consists of a CPU stage for preprocessing and a GPU stage for model inference, increasing the number of CPU-stage workers can help to produce more data to be batched for model inference at the GPU stage; increasing the GPU-stage workers can fully utilize the GPU memory and computation power. Both ways may contribute to higher GPU utilization, which consequently results in higher service throughput.
+- For multi-stage services, note that the data passing through different stages will be serialized/deserialized by the `serialize_ipc/deserialize_ipc` methods, so extremely large data might make the whole pipeline slow. The serialized data is passed to the next stage through rust by default, you could enable shared memory to potentially reduce the latency (ref [RedisShmIPCMixin](https://mosecorg.github.io/mosec/examples/ipc.html#redis-shm-ipc-py)).
+- You should choose appropriate `serialize/deserialize` methods, which are used to decode the user request and encode the response. By default, both are using JSON. However, images and embeddings are not well supported by JSON. You can choose msgpack which is faster and binary compatible (ref [Stable Diffusion](https://mosecorg.github.io/mosec/examples/stable_diffusion.html)).
+- Configure the threads for OpenBLAS or MKL. It might not be able to choose the most suitable CPUs used by the current Python process. You can configure it for each worker by using the [env](https://mosecorg.github.io/mosec/reference/interface.html#mosec.server.Server.append_worker) (ref [custom GPU allocation](https://mosecorg.github.io/mosec/examples/env.html)).
 
 ## Adopters
 
 Here are some of the companies and individual users that are using Mosec:
 
 - [Modelz](https://modelz.ai): Serverless platform for ML inference.
 - [MOSS](https://github.com/OpenLMLab/MOSS/blob/main/README_en.md): An open sourced conversational language model like ChatGPT.
@@ -216,7 +257,9 @@
 ```
 
 ## Contributing
 
 We welcome any kind of contribution. Please give us feedback by [raising issues](https://github.com/mosecorg/mosec/issues/new/choose) or discussing on [Discord](https://discord.gg/Jq5vxuH69W). You could also directly [contribute](https://mosecorg.github.io/mosec/development/contributing.html) your code and pull request!
 
 To start develop, you can use [envd](https://github.com/tensorchord/envd) to create an isolated and clean Python & Rust environment. Check the [envd-docs](https://envd.tensorchord.ai/) or [build.envd](https://github.com/mosecorg/mosec/blob/main/build.envd) for more information.
+
+
```

### Comparing `mosec-0.7.2/build.envd` & `mosec-0.8.0/build.envd`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/make.bat` & `mosec-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/conf.py` & `mosec-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/examples/echo.md` & `mosec-0.8.0/docs/source/examples/echo.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/examples/env.md` & `mosec-0.8.0/docs/source/examples/env.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/examples/index.md` & `mosec-0.8.0/docs/source/examples/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 env
 ipc
 jax
 metric
 pytorch
 stable_diffusion
 validate
+multi_route
 ```
 
 We provide examples across different ML frameworks and for various tasks in this section.
 
 ## Requirements
 
 All the examples in this section are self-contained and tested. Feel free to grab one and run:
```

### Comparing `mosec-0.7.2/docs/source/examples/ipc.md` & `mosec-0.8.0/docs/source/examples/ipc.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/examples/jax.md` & `mosec-0.8.0/docs/source/examples/jax.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/examples/metric.md` & `mosec-0.8.0/docs/source/examples/metric.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/examples/pytorch.md` & `mosec-0.8.0/docs/source/examples/pytorch.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/docs/source/examples/stable_diffusion.md` & `mosec-0.8.0/docs/source/examples/stable_diffusion.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 docker run --rm --gpus all -p 8000:8000 sd:serving
 ```
 
 ```{include} ../../../examples/stable_diffusion/server.py
 :code: python
 ```
 
+```shell
+python server.py --timeout 30000
+```
+
 ## Client
 
 ```shell
 python client.py --prompt "a cute cat site on the basketball"
 ```
 
 ```{include} ../../../examples/stable_diffusion/client.py
```

### Comparing `mosec-0.7.2/docs/source/examples/validate.md` & `mosec-0.8.0/docs/source/examples/validate.md`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/license.json` & `mosec-0.8.0/license.json`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/__init__.py` & `mosec-0.8.0/mosec/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,30 @@
     ClientError,
     DecodingError,
     EncodingError,
     ServerError,
     ValidationError,
 )
 from mosec.log import get_logger
+from mosec.runtime import Runtime
 from mosec.server import Server
 from mosec.worker import SSEWorker, Worker
 
 try:
     from mosec._version import __version__  # type: ignore
 except ImportError:
     from setuptools_scm import get_version  # type: ignore
 
     __version__ = get_version(root="..", relative_to=__file__)
 
 __all__ = [
     "Server",
     "Worker",
     "SSEWorker",
+    "Runtime",
     "ServerError",
     "ClientError",
     "ValidationError",
     "EncodingError",
     "DecodingError",
     "get_logger",
 ]
```

### Comparing `mosec-0.7.2/mosec/args.py` & `mosec-0.8.0/mosec/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,44 +27,49 @@
 import random
 import socket
 import tempfile
 import warnings
 
 from mosec.env import get_env_namespace
 
+DEFAULT_WAIT_MS = 10
+
 
 def is_port_available(addr: str, port: int) -> bool:
     """Check if the port is available to use."""
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     err = sock.connect_ex((addr, port))
     sock.close()
     # https://docs.python.org/3/library/errno.html
-    if 0 == err:
+    if err == 0:
         return False
-    if errno.ECONNREFUSED == err:
+    if err == errno.ECONNREFUSED:
         return True
     raise RuntimeError(
         f"Check {addr}:{port} socket connection err: {err}{errno.errorcode[err]}"
     )
 
 
 def build_arguments_parser() -> argparse.ArgumentParser:
     """Build CLI arguments."""
     parser = argparse.ArgumentParser(
         description="Mosec Server Configurations",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        epilog="The following arguments can be set through environment variables: "
-        "(path, capacity, timeout, address, port, namespace, debug, dry_run). "
-        "Note that the environment variable should start with `MOSEC_` with upper "
+        epilog="The following arguments can be set through environment variables: ("
+        "path, capacity, timeout, address, port, namespace, debug, log_level, dry_run"
+        "). Note that the environment variable should start with `MOSEC_` with upper "
         "case. For example: `MOSEC_PORT=8080 MOSEC_TIMEOUT=5000 python main.py`.",
     )
 
     parser.add_argument(
         "--path",
-        help="Unix Domain Socket address for internal Inter-Process Communication",
+        help=(
+            "Unix Domain Socket address for internal Inter-Process Communication."
+            "If not set, a random path will be created under the temporary dir."
+        ),
         type=str,
         default=os.path.join(
             tempfile.gettempdir(), f"mosec_{random.randrange(2**32):x}"
         ),
     )
 
     parser.add_argument(
@@ -82,15 +87,15 @@
         default=3000,
     )
 
     parser.add_argument(
         "--wait",
         help="[deprecated] Wait time for the batcher to batch (milliseconds)",
         type=int,
-        default=10,
+        default=DEFAULT_WAIT_MS,
     )
 
     parser.add_argument(
         "--address",
         help="Address of the HTTP service",
         type=str,
         default="0.0.0.0",
@@ -133,21 +138,29 @@
 
 
 def parse_arguments() -> argparse.Namespace:
     """Parse user configurations."""
     parser = build_arguments_parser()
     args, _ = parser.parse_known_args(namespace=get_env_namespace())
 
-    if args.wait != 10:
+    if args.wait != DEFAULT_WAIT_MS:
         warnings.warn(
             "`--wait` is deprecated and will be removed in v1, please configure"
             "the `max_wait_time` on `Server.append_worker`",
             DeprecationWarning,
         )
 
+    if args.debug:
+        args.log_level = "debug"
+        warnings.warn(
+            "`--debug` is deprecated and will be removed in v1, please configure"
+            "`--log_level=debug`",
+            DeprecationWarning,
+        )
+
     if not is_port_available(args.address, args.port):
         raise RuntimeError(
             f"{args.address}:{args.port} is in use. "
             "Please change to a free one (use `--port`)."
         )
 
     return args
```

### Comparing `mosec-0.7.2/mosec/coordinator.py` & `mosec-0.8.0/mosec/coordinator.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,40 +10,45 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """The Coordinator is used to control the data flow between `Worker` and `Server`."""
 
+import enum
 import os
 import queue
 import signal
 import socket
 import struct
 import threading
 import time
 import traceback
 from contextlib import contextmanager
 from multiprocessing.synchronize import Event
-from typing import Any, Callable, Optional, Sequence, Tuple, Type
+from typing import Any, Optional, Sequence, Type
 
 from mosec.errors import MosecError, MosecTimeoutError
-from mosec.ipc import IPCWrapper
 from mosec.log import get_internal_logger
 from mosec.protocol import HTTPStautsCode, Protocol
 from mosec.worker import SSEWorker, Worker
 
 logger = get_internal_logger()
 
 
 CONN_MAX_RETRY = 10
 CONN_CHECK_INTERVAL = 1
 
-STAGE_INGRESS = "ingress"
-STAGE_EGRESS = "egress"
+
+class State(enum.IntFlag):
+    """Task state."""
+
+    INGRESS = 0b1
+    EGRESS = 0b10
+
 
 PROTOCOL_TIMEOUT = 2.0
 
 
 @contextmanager
 def set_mosec_timeout(duration: int):
     """Context manager to set a timeout for a code block.
@@ -93,65 +98,50 @@
     """
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         worker: Type[Worker],
         max_batch_size: int,
-        stage: str,
         shutdown: Event,
         shutdown_notify: Event,
         socket_prefix: str,
-        stage_id: int,
+        stage_name: str,
         worker_id: int,
-        ipc_wrapper: Optional[Callable[..., IPCWrapper]],
         timeout: int,
     ):
         """Initialize the mosec coordinator.
 
         Args:
-            worker (Worker): subclass of `mosec.Worker` implemented by users.
-            max_batch_size (int): maximum batch size for this worker.
-            stage (str): identifier to distinguish the first and last stages.
-            shutdown (Event): `multiprocessing.synchronize.Event` object for shutdown
+            worker: subclass of `mosec.Worker` implemented by users.
+            max_batch_size: maximum batch size for this worker.
+            shutdown: `multiprocessing.synchronize.Event` object for shutdown
                 IPC.
-            socket_prefix (str): prefix for the socket addresses.
-            stage_id (int): identification number for worker stages.
-            worker_id (int): identification number for worker processes at the same
+            socket_prefix: prefix for the socket addresses.
+            stage_name: identification name for this worker stage.
+            worker_id: identification number for worker processes at the same
                 stage.
-            ipc_wrapper (IPCWrapper): IPC wrapper class to be initialized.
-            timeout (int): timeout for the `forward` function.
-
-        Raises:
-            TypeError: ipc_wrapper should inherit from `IPCWrapper`
+            timeout: timeout for the `forward` function.
         """
-        self.worker = worker()
-        self.worker.worker_id = worker_id
-        self.worker.max_batch_size = max_batch_size
-        self.worker.stage = stage
+        self.name = f"<{stage_name}|{worker_id}>"
         self.timeout = timeout
-        self.name = f"<{stage_id}|{worker.__name__}|{worker_id}>"
         self.current_ids: Sequence[bytes] = []
         self.semaphore = FakeSemaphore()  # type: ignore
 
+        self.worker = worker()
+        self.worker.worker_id = worker_id
+        self.worker.max_batch_size = max_batch_size
+        self.worker.stage = stage_name
+
         self.protocol = Protocol(
             name=self.name,
-            addr=os.path.join(socket_prefix, f"ipc_{stage_id}.socket"),
+            addr=os.path.join(socket_prefix, f"ipc_{stage_name}.socket"),
             timeout=PROTOCOL_TIMEOUT,
         )
 
-        # optional plugin features - ipc wrapper
-        self.ipc_wrapper: Optional[IPCWrapper] = None
-        if ipc_wrapper is not None:
-            self.ipc_wrapper = ipc_wrapper()
-            if not issubclass(type(self.ipc_wrapper), IPCWrapper):
-                raise TypeError(
-                    "ipc_wrapper must be the subclass of mosec.plugins.IPCWrapper"
-                )
-
         # ignore termination & interruption signal
         signal.signal(signal.SIGTERM, signal.SIG_IGN)
         signal.signal(signal.SIGINT, signal.SIG_IGN)
         self.shutdown = shutdown
         self.shutdown_notify = shutdown_notify
 
         # SSE support
@@ -193,15 +183,17 @@
         """Send stream data from the worker to the server through the socket."""
         while not self.shutdown.is_set():
             try:
                 text, index = self.stream.get(timeout=self.timeout)
                 # encode the text with UTF-8
                 payloads = (text.encode(),)
                 ids = (self.current_ids[index],)
-                self.protocol.send(HTTPStautsCode.STREAM_EVENT, ids, payloads)
+                self.protocol.send(
+                    HTTPStautsCode.STREAM_EVENT, ids, (0,) * len(ids), payloads
+                )
                 self.semaphore.release()
             except queue.Empty:
                 continue
 
     def warmup(self):
         """Warmup to allocate resources (useful for GPU workload)[Optional]."""
         need_warmup = self.worker.example or self.worker.multi_examples
@@ -239,120 +231,82 @@
             except OSError as err:
                 if not self.shutdown_notify.is_set():
                     logger.error("%s socket connection error: %s", self.name, err)
                 break
 
             self.coordinate()
 
-    def get_decoder(self) -> Callable[[bytes], Any]:
-        """Get the decoder function for this stage.
-
-        The first stage will use the worker's deserialize function.
-        """
-        if STAGE_INGRESS in self.worker.stage:
-            return self.worker.deserialize
-        return self.worker.deserialize_ipc
-
-    def get_encoder(self) -> Callable[[Any], bytes]:
-        """Get the encoder function for this stage.
-
-        The last stage will use the worker's serialize function.
-        """
-        if STAGE_EGRESS in self.worker.stage:
-            return self.worker.serialize
-        return self.worker.serialize_ipc
-
-    def get_protocol_recv(
-        self,
-    ) -> Callable[[], Tuple[bytes, Sequence[bytes], Sequence[bytes]]]:
-        """Get the protocol receive function for this stage.
-
-        IPC wrapper will be used if it's provided and the stage is not the first one.
-        """
-        if STAGE_INGRESS in self.worker.stage or self.ipc_wrapper is None:
-            return self.protocol.receive
-
-        # TODO(kemingy) find a better way
-        def wrapped_recv() -> Tuple[bytes, Sequence[bytes], Sequence[bytes]]:
-            flag, ids, payloads = self.protocol.receive()
-            payloads = self.ipc_wrapper.get(  # type: ignore
-                [bytes(x) for x in payloads]
-            )
-            return flag, ids, payloads
-
-        return wrapped_recv
-
-    def get_protocol_send(
-        self,
-    ) -> Callable[[int, Sequence[bytes], Sequence[bytes]], None]:
-        """Get the protocol send function for this stage.
-
-        IPC wrapper will be used if it's provided and the stage is not the last one.
-        """
-        if STAGE_EGRESS in self.worker.stage or self.ipc_wrapper is None:
-            return self.protocol.send
-
-        # TODO(kemingy) find a better way
-        def wrapped_send(flag: int, ids: Sequence[bytes], payloads: Sequence[bytes]):
-            if flag == HTTPStautsCode.OK:
-                payloads = self.ipc_wrapper.put(payloads)  # type: ignore
-            return self.protocol.send(flag, ids, payloads)
+    def decode(self, payload: bytes, state: int) -> Any:
+        """Decode the payload with the state."""
+        return (
+            self.worker.deserialize(payload)
+            if state & State.INGRESS
+            else self.worker.deserialize_ipc(payload)
+        )
 
-        return wrapped_send
+    def encode(self, data: Any, state: int) -> bytes:
+        """Encode the data with the state."""
+        return (
+            self.worker.serialize(data)
+            if state & State.EGRESS
+            else self.worker.serialize_ipc(data)
+        )
 
     def coordinate(self):
         """Start coordinating the protocol's communication and worker's forward pass."""
-        decoder = self.get_decoder()
-        encoder = self.get_encoder()
-        protocol_recv = self.get_protocol_recv()
-        protocol_send = self.get_protocol_send()
         while not self.shutdown.is_set():
             try:
-                _, ids, payloads = protocol_recv()
+                # flag received from the server is not used
+                _, ids, states, payloads = self.protocol.receive()
                 # expose here to be used by stream event
                 self.current_ids = ids
             except socket.timeout:
                 continue
             except (struct.error, OSError) as err:
                 if not self.shutdown_notify.is_set():
                     logger.error("%s failed to read from socket: %s", self.name, err)
                 break
 
             # pylint: disable=broad-except
             length = len(payloads)
             try:
-                data = [decoder(item) for item in payloads]
+                data = [
+                    self.decode(payload, state)
+                    for (payload, state) in zip(payloads, states)
+                ]
                 with set_mosec_timeout(self.timeout):
                     data = (
                         self.worker.forward(data)
                         if self.worker.max_batch_size > 1
                         else (self.worker.forward(data[0]),)
                     )
                 if len(data) != length:
                     raise ValueError(
                         "returned data size doesn't match the input data size:"
                         f"input({length})!=output({len(data)})"
                     )
                 status = HTTPStautsCode.OK
-                payloads = [encoder(item) for item in data]
+                payloads = [
+                    self.encode(datum, state) for (datum, state) in zip(data, states)
+                ]
             except (MosecError, MosecTimeoutError) as err:
                 err_msg = str(err).replace("\n", " - ")
                 err_msg = err_msg if err_msg else err.msg
                 logger.info("%s %s: %s", self.name, err.msg, err_msg)
                 status = err.code
                 payloads = [f"{err.msg}: {err_msg}".encode()] * length
             except Exception:
                 logger.warning(traceback.format_exc().replace("\n", " "))
                 status = HTTPStautsCode.INTERNAL_ERROR
                 payloads = ["inference internal error".encode()] * length
 
             try:
                 # pylint: disable=consider-using-with
                 self.semaphore.acquire(timeout=self.timeout)
-                protocol_send(status, ids, payloads)
+                self.protocol.send(status, ids, states, payloads)
             except OSError as err:
                 logger.error("%s failed to send to socket: %s", self.name, err)
                 break
             finally:
                 self.semaphore.release()
 
         self.protocol.close()
```

### Comparing `mosec-0.7.2/mosec/dry_run.py` & `mosec-0.8.0/mosec/dry_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 from __future__ import annotations
 
 import json
 import signal
 import sys
 import time
 from multiprocessing.context import SpawnContext, SpawnProcess
-from typing import TYPE_CHECKING, List, Tuple, Union
+from typing import TYPE_CHECKING, Dict, List, Tuple, Union
 
 from mosec.env import env_var_context
 from mosec.log import get_internal_logger
-from mosec.runtime import PyRuntimeManager, Runtime
+from mosec.runtime import Runtime
 from mosec.worker import Worker
 
 if TYPE_CHECKING:
     from multiprocessing.connection import PipeConnection  # type: ignore
     from multiprocessing.synchronize import Event
 
 logger = get_internal_logger()
@@ -51,18 +51,15 @@
 
     if shutdown_notify.is_set():
         return
 
     try:
         data = receiver.recv() if ingress else worker.deserialize(receiver.recv_bytes())
         logger.info("%s received %s", worker, data)
-        if batch > 1:
-            data = worker.forward([data])[0]
-        else:
-            data = worker.forward(data)
+        data = worker.forward([data])[0] if batch > 1 else worker.forward(data)
         logger.info("%s inference result: %s", worker, data)
         data = worker.serialize(data)
         sender.send_bytes(data)
     # pylint: disable=broad-except
     except Exception as err:
         logger.error("get error in %s: %s", worker, err)
         shutdown_notify.set()
@@ -74,176 +71,183 @@
     def __init__(self, process_context: SpawnContext, shutdown_notify: Event):
         """Initialize a process pool.
 
         Args:
             process_context: server context of spawn process
             shutdown_notify: event of server will shutdown
         """
-        self._process_context = process_context
-        self._shutdown_notify = shutdown_notify
+        self.process_context = process_context
+        self.shutdown_notify = shutdown_notify
 
-        self._pool: List[SpawnProcess] = []
-        self._sender_pipes: List[PipeConnection] = []
-        self._receiver_pipes: List[PipeConnection] = []
+        self.processes: List[SpawnProcess] = []
+        self.sender_pipes: List[PipeConnection] = []
+        self.receiver_pipes: List[PipeConnection] = []
 
     def new_pipe(self):
         """Create new pipe for dry run workers to communicate."""
-        receiver, sender = self._process_context.Pipe(duplex=False)
-        self._sender_pipes.append(sender)
-        self._receiver_pipes.append(receiver)
+        receiver, sender = self.process_context.Pipe(duplex=False)
+        self.sender_pipes.append(sender)
+        self.receiver_pipes.append(receiver)
 
-    def start_worker(self, worker_runtime: Runtime, first: bool):
+    def start_worker(self, worker_runtime: Runtime, init: bool):
         """Start the worker process for dry run.
 
         Args:
             worker_runtime: worker runtime to start
-            first: whether the worker is tried to start at first time
+            init: whether the worker is tried to start at the first time
 
         """
         self.new_pipe()
-        coordinator = self._process_context.Process(
+        coordinator = self.process_context.Process(
             target=dry_run_func,
             args=(
                 worker_runtime.worker,
                 worker_runtime.max_batch_size,
-                self._receiver_pipes[-2],
-                self._sender_pipes[-1],
-                first,
-                self._shutdown_notify,
+                self.receiver_pipes[-2],
+                self.sender_pipes[-1],
+                init,
+                self.shutdown_notify,
             ),
             daemon=True,
         )
 
         with env_var_context(worker_runtime.env, 0):
             coordinator.start()
 
-        self._pool.append(coordinator)
+        self.processes.append(coordinator)
 
     def probe_worker_liveness(self) -> Tuple[Union[int, None], Union[int, None]]:
         """Check every worker is running/alive.
 
         Returns:
             index: index of the first failed worker
             exitcode: exitcode of the first failed worker
 
         """
-        for i, process in enumerate(self._pool):
+        for i, process in enumerate(self.processes):
             if process.exitcode is not None:
                 return i, process.exitcode
         return None, None
 
     def wait_all(self) -> Tuple[Union[int, None], Union[int, None]]:
         """Blocking until all worker to end or one failed.
 
         Returns:
             index: index of the first failed worker
             exitcode: exitcode of the first failed worker
 
         """
-        for i, process in enumerate(self._pool):
+        for i, process in enumerate(self.processes):
             process.join()
             if process.exitcode != 0:
                 return i, process.exitcode
         return None, None
 
     def first_last_pipe(self):
         """Get first sender and last receiver pipes."""
-        return self._sender_pipes[0], self._receiver_pipes[-1]
+        return self.sender_pipes[0], self.receiver_pipes[-1]
 
 
 class DryRunner:
     """Dry run the full stage.
 
     If examples are provided in the ingress :py:class:`Worker <mosec.worker.Worker>`,
     they will be used to pass through all the stages.
 
     For each stage, there will be only 1 worker. If `env` is provided during
     :py:meth:`append_worker <mosec.server.Server.append_worker>`, the 1st one
     will be used.
     """
 
-    def __init__(self, manager: PyRuntimeManager):
+    def __init__(self, router: Dict[str, List[Runtime]]):
         """Init dry runner."""
-        logger.info("init dry runner for %s", manager.workers)
-
-        self._manager = manager
-        self._process_context: SpawnContext = SpawnContext()
-        self._shutdown_notify: Event = self._process_context.Event()
-        self._pool = Pool(self._process_context, self._shutdown_notify)
+        self.router = router
+        self.process_context: SpawnContext = SpawnContext()
+        self.shutdown_notify: Event = self.process_context.Event()
 
         signal.signal(signal.SIGTERM, self.terminate)
         signal.signal(signal.SIGINT, self.terminate)
 
     def terminate(self, signum, framestack):
         """Terminate the dry run."""
         logger.info("received terminate signal [%s] %s", signum, framestack)
-        self._shutdown_notify.set()
+        self.shutdown_notify.set()
 
     def run(self):
         """Execute thr dry run process."""
-        self._pool.new_pipe()
-        for i, worker_runtime in enumerate(self._manager):
-            self._pool.start_worker(worker_runtime, i == 0)
-
-        logger.info("dry run init successful")
-        self.warmup()
-
-        logger.info("wait for worker init done")
-        if not self._shutdown_notify.is_set():
-            self._shutdown_notify.set()
-
-        failed, exitcode = self._pool.wait_all()
-        if failed is not None:
-            logger.warning(
-                "detect %s with abnormal exit code %d",
-                self._manager.workers[failed],
-                exitcode,
+        for endpoint, runtimes in self.router.items():
+            logger.info(
+                "init dry run for endpoint %s with %s",
+                endpoint,
+                [runtime.name for runtime in runtimes],
             )
-            sys.exit(exitcode)
+
+            pool = Pool(self.process_context, self.shutdown_notify)
+            pool.new_pipe()
+            for i, worker_runtime in enumerate(runtimes):
+                pool.start_worker(worker_runtime, i == 0)
+
+            logger.info("dry run init successful")
+            self.warmup(runtimes, pool)
+
+            logger.info("wait for worker init done")
+            if not self.shutdown_notify.is_set():
+                self.shutdown_notify.set()
+
+            failed, exitcode = pool.wait_all()
+            if failed is not None:
+                logger.warning(
+                    "detect %s with abnormal exit code %d",
+                    runtimes[failed].name,
+                    exitcode,
+                )
+                sys.exit(exitcode)
+
+            self.shutdown_notify.clear()
         logger.info("dry run exit")
 
-    def warmup(self):
+    def warmup(self, runtimes: List[Runtime], pool: Pool):
         """Warmup the service.
 
         If neither `example` nor `multi_examples` is provided, it will only
         init the worker class.
         """
-        ingress = self._manager.workers[0]
+        ingress = runtimes[0].worker
         example = None
         if ingress.example:
             example = ingress.example
         elif ingress.multi_examples:
             assert isinstance(ingress.multi_examples, list), (
                 "`multi_examples` " "should be a list of data"
             )
             example = ingress.multi_examples[0]
 
         if not example:
             logger.info("cannot find the example in the 1st stage worker, skip warmup")
             return
 
-        sender, receiver = self._pool.first_last_pipe()
+        sender, receiver = pool.first_last_pipe()
         start_time = time.perf_counter()
         sender.send(example)
 
-        while not self._shutdown_notify.is_set():
+        while not self.shutdown_notify.is_set():
             if receiver.poll(0.1):
                 break
             # liveness probe
-            failed, exitcode = self._pool.probe_worker_liveness()
+            failed, exitcode = pool.probe_worker_liveness()
             if failed is not None:
                 logger.warning(
                     "worker %s exit with code %d",
-                    self._manager.workers[failed],
+                    runtimes[failed].name,
                     exitcode,
                 )
-                self._shutdown_notify.set()
+                self.shutdown_notify.set()
                 break
 
-        if self._shutdown_notify.is_set():
+        if self.shutdown_notify.is_set():
             sys.exit(1)
 
         res = receiver.recv_bytes()
         duration = time.perf_counter() - start_time
         logger.info(
             "dry run result: %s",
             json.dumps(
```

### Comparing `mosec-0.7.2/mosec/env.py` & `mosec-0.8.0/mosec/env.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/errors.py` & `mosec-0.8.0/mosec/errors.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/log.py` & `mosec-0.8.0/mosec/log.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/mixin/__init__.py` & `mosec-0.8.0/mosec/mixin/__init__.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/mixin/msgpack_worker.py` & `mosec-0.8.0/mosec/mixin/msgpack_worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/mixin/numbin_worker.py` & `mosec-0.8.0/mosec/mixin/numbin_worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/mixin/plasma_worker.py` & `mosec-0.8.0/mosec/mixin/plasma_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,25 @@
 ```{warning}
 The plasma is deprecated in `pyarrow`. Please use Redis instead.
 ```
 """
 
 import warnings
 from os import environ
-from typing import TYPE_CHECKING, Any
+from typing import Any
 
 from mosec.worker import Worker
 
 try:
     from pyarrow import plasma  # type: ignore
 except ImportError:
     warnings.warn(
         "pyarrow is not installed. PlasmaShmMixin is not available.", ImportWarning
     )
 
-if TYPE_CHECKING:
-    from pyarrow import plasma
-
 
 _PLASMA_PATH_ENV = "MOSEC_INTERNAL_PLASMA_PATH"
 
 
 class PlasmaShmIPCMixin(Worker):
     """Plasma shared memory worker mixin interface."""
```

### Comparing `mosec-0.7.2/mosec/mixin/redis_worker.py` & `mosec-0.8.0/mosec/mixin/redis_worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/mixin/typed_worker.py` & `mosec-0.8.0/mosec/mixin/typed_worker.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/plugins/__init__.py` & `mosec-0.8.0/mosec/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-# Copyright 2022 MOSEC Authors
+# Copyright 2023 MOSEC Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Provide useful tools to extend MOSEC."""
+"""Provide common useful utils to develop MOSEC."""
 
-from mosec.plugins.plasma_shm import PlasmaShmWrapper
+from mosec.utils.types import ParseTarget, parse_func_type
 
-__all__ = ["PlasmaShmWrapper"]
+__all__ = [
+    "parse_func_type",
+    "ParseTarget",
+]
```

### Comparing `mosec-0.7.2/mosec/protocol.py` & `mosec-0.8.0/mosec/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,19 +50,21 @@
     """
 
     # byte formats (https://docs.python.org/3/library/struct.html#format-characters)
     FORMAT_FLAG = "!H"
     FORMAT_BATCH = "!H"
     FORMAT_ID = "!I"
     FORMAT_LENGTH = "!I"
+    FORMAT_STATE = "!H"
 
     # lengths
     LENGTH_TASK_FLAG = 2
     LENGTH_TASK_BATCH = 2
     LENGTH_TASK_ID = 4
+    LENGTH_TASK_STATE = 2
     LENGTH_TASK_BODY_LEN = 4
 
     def __init__(
         self,
         name: str,
         addr: str,
         timeout: float = 2.0,
@@ -78,29 +80,31 @@
             socket.AF_UNIX,
             socket.SOCK_STREAM,
         )
         self.socket.settimeout(timeout)
         self.name = name
         self.addr = addr
 
-    def receive(self) -> Tuple[bytes, Sequence[bytes], Sequence[bytes]]:
+    def receive(self) -> Tuple[bytes, Sequence[bytes], Sequence[int], Sequence[bytes]]:
         """Receive tasks from the server."""
         flag = self.socket.recv(self.LENGTH_TASK_FLAG)
         batch_size_bytes = self.socket.recv(self.LENGTH_TASK_BATCH)
         batch_size = struct.unpack(self.FORMAT_BATCH, batch_size_bytes)[0]
-        ids, payloads = [], []
+        ids, states, payloads = [], [], []
         total_bytes = 0
 
         while batch_size > 0:
             batch_size -= 1
             id_bytes = self.socket.recv(self.LENGTH_TASK_ID)
+            state_bytes = self.socket.recv(self.LENGTH_TASK_STATE)
             length_bytes = self.socket.recv(self.LENGTH_TASK_BODY_LEN)
             length = struct.unpack(self.FORMAT_LENGTH, length_bytes)[0]
             payload = _recv_all(self.socket, length)
             ids.append(id_bytes)
+            states.append(struct.unpack(self.FORMAT_STATE, state_bytes)[0])
             payloads.append(payload)
             total_bytes += length
 
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(
                 "%s received %d tasks with ids: %s",
                 self.name,
@@ -110,29 +114,35 @@
 
         if total_bytes > IPC_LARGE_DATA_SIZE:
             warnings.warn(
                 f"IPC data ({total_bytes} bytes) is large, "
                 "which may affect performance",
                 RuntimeWarning,
             )
-        return flag, ids, payloads
+        return flag, ids, states, payloads
 
-    def send(self, flag: int, ids: Sequence[bytes], payloads: Sequence[bytes]):
+    def send(
+        self,
+        flag: int,
+        ids: Sequence[bytes],
+        states: Sequence[int],
+        payloads: Sequence[bytes],
+    ):
         """Send results to the server."""
         data = BytesIO()
         data.write(struct.pack(self.FORMAT_FLAG, flag))
         if len(ids) != len(payloads):
             raise ValueError("`ids` have different length with `payloads`")
         batch_size = len(ids)
         data.write(struct.pack(self.FORMAT_BATCH, batch_size))
         if batch_size > 0:
-            for task_id, payload in zip(ids, payloads):
-                length = struct.pack(self.FORMAT_LENGTH, len(payload))
+            for task_id, state, payload in zip(ids, states, payloads):
                 data.write(task_id)
-                data.write(length)
+                data.write(struct.pack(self.FORMAT_STATE, state))
+                data.write(struct.pack(self.FORMAT_LENGTH, len(payload)))
                 data.write(payload)
         self.socket.sendall(data.getbuffer())
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(
                 "%s sent %d(%d) tasks with ids: %s",
                 self.name,
                 len(ids),
```

### Comparing `mosec-0.7.2/mosec/runtime.py` & `mosec-0.8.0/mosec/runtime.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,170 +12,162 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Managers to control Coordinator and Mosec process."""
 
 import multiprocessing as mp
 import subprocess
-from functools import partial
 from multiprocessing.context import ForkContext, SpawnContext
 from multiprocessing.process import BaseProcess
 from multiprocessing.synchronize import Event
 from pathlib import Path
 from time import monotonic, sleep
-from typing import Any, Callable, Dict, Iterable, List, Optional, Type, Union, cast
+from typing import Callable, Dict, Iterable, List, Optional, Type, Union, cast
 
 import pkg_resources
 
-from mosec.coordinator import STAGE_EGRESS, STAGE_INGRESS, Coordinator
+from mosec.coordinator import Coordinator
 from mosec.env import env_var_context, validate_env, validate_int_ge
-from mosec.ipc import IPCWrapper
 from mosec.log import get_internal_logger
 from mosec.worker import Worker
 
 logger = get_internal_logger()
 
 NEW_PROCESS_METHOD = {"spawn", "fork"}
 
 
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-arguments
+# pylint: disable=too-few-public-methods
 class Runtime:
     """The wrapper with one worker and its arguments."""
 
+    # count how many runtime instances have been created
+    _stage_id: int = 0
+
     def __init__(
         self,
         worker: Type[Worker],
-        num: int,
-        max_batch_size: int,
-        max_wait_time: int,
-        stage_id: int,
-        timeout: int,
-        start_method: str,
-        env: Union[None, List[Dict[str, str]]],
-        ipc_wrapper: Optional[Union[Type[IPCWrapper], partial]],
+        num: int = 1,
+        max_batch_size: int = 1,
+        max_wait_time: int = 10,
+        timeout: int = 3,
+        start_method: str = "spawn",
+        env: Union[None, List[Dict[str, str]]] = None,
     ):
         """Initialize the mosec coordinator.
 
         Args:
             worker (Worker): subclass of `mosec.Worker` implemented by users.
             num (int): number of workers
             max_batch_size: the maximum batch size allowed (>=1), will enable the
                 dynamic batching if it > 1
             max_wait_time (int): the maximum wait time (millisecond)
                 for dynamic batching, needs to be used with `max_batch_size`
                 to enable the feature. If not configure, will use the CLI
                 argument `--wait` (default=10ms)
-            stage_id (int): identification number for worker stages.
-            timeout (int): timeout for the `forward` function.
+            timeout (int): timeout (second) for the `forward` function.
             start_method: the process starting method ("spawn" or "fork")
             env: the environment variables to set before starting the process
-            ipc_wrapper (IPCWrapper): IPC wrapper class to be initialized.
-
-
-        Raises:
-            TypeError: ipc_wrapper should inherit from `IPCWrapper`
         """
         self.worker = worker
         self.num = num
         self.max_batch_size = max_batch_size
         self.max_wait_time = max_wait_time
-        self.stage_id = stage_id
         self.timeout = timeout
         self.start_method = start_method
         self.env = env
-        self.ipc_wrapper = ipc_wrapper
 
+        Runtime._stage_id += 1
+        # adding the stage id in case the worker class is added to multiple stages
+        self.name = f"{self.worker.__name__}_{self._stage_id}"
         self._pool: List[Union[BaseProcess, None]] = [None for _ in range(self.num)]
 
+        self._validate()
+
     @staticmethod
     def _process_healthy(process: Union[BaseProcess, None]) -> bool:
         """Check if the child process is healthy.
 
         ref: https://docs.python.org/3/library/multiprocessing.html
 
             The exit code will be None if the process has not yet terminated.
         """
         return process is not None and process.exitcode is None
 
     def _healthy(self, method: Callable[[Iterable[object]], bool]) -> bool:
+        """Check if all/any of the child processes are healthy."""
         return method(self._pool)
 
     def _start_process(
         self,
         worker_id: int,
-        stage_label: str,
         work_path: str,
         shutdown: Event,
         shutdown_notify: Event,
     ):
+        """Start a worker process in the context."""
         context = mp.get_context(self.start_method)
         context = cast(Union[SpawnContext, ForkContext], context)
         coordinator_process = context.Process(
             target=Coordinator,
             args=(
                 self.worker,
                 self.max_batch_size,
-                stage_label,
                 shutdown,
                 shutdown_notify,
                 work_path,
-                self.stage_id,
+                self.name,
                 worker_id + 1,
-                self.ipc_wrapper,
                 self.timeout,
             ),
             daemon=True,
         )
 
         with env_var_context(self.env, worker_id):
             coordinator_process.start()
 
         self._pool[worker_id] = coordinator_process
 
-    def check(
+    def _check(
         self,
-        first: bool,
-        stage_label: str,
         work_path: str,
         shutdown: Event,
         shutdown_notify: Event,
+        init: bool,
     ) -> bool:
         """Check and start the worker process if it has not started yet.
 
         Args:
-            first: whether the worker is tried to start at first time
-            stage_label: label of worker ingress and egress
             work_path: path of working directory
             shutdown: Event of server shutdown
             shutdown_notify: Event of server will shutdown
+            init: whether the worker is tried to start at the first time
 
         Returns:
             Whether the worker is started successfully
         """
         # for every sequential stage
         self._pool = [p if self._process_healthy(p) else None for p in self._pool]
         if self._healthy(all):
             # this stage is healthy
             return True
-        if not first and not self._healthy(any):
+        if not init and not self._healthy(any):
             # this stage might contain bugs
             return False
 
         need_start_id = [
             worker_id for worker_id in range(self.num) if self._pool[worker_id] is None
         ]
         for worker_id in need_start_id:
             # for every worker in each stage
-            self._start_process(
-                worker_id, stage_label, work_path, shutdown, shutdown_notify
-            )
+            self._start_process(worker_id, work_path, shutdown, shutdown_notify)
         return True
 
-    def validate(self):
+    def _validate(self):
         """Validate arguments of worker runtime."""
         validate_env(self.env, self.num)
         assert issubclass(
             self.worker, Worker
         ), "worker must be inherited from mosec.Worker"
         validate_int_ge(self.num, "worker number")
         validate_int_ge(self.max_batch_size, "maximum batch size")
@@ -193,123 +185,89 @@
         """Initialize a coordinator manager.
 
         Args:
             work_path: path of working directory
             shutdown: Event of server shutdown
             shutdown_notify: Event of server will shutdown
         """
-        self._runtimes: List[Runtime] = []
+        self.runtimes: List[Runtime] = []
 
         self._work_path = work_path
-        self._shutdown = shutdown
-        self._shutdown_notify = shutdown_notify
-
-    def __iter__(self):
-        """Iterate workers of manager."""
-        return self._runtimes.__iter__()
+        self.shutdown = shutdown
+        self.shutdown_notify = shutdown_notify
 
     @property
     def worker_count(self) -> int:
         """Get number of workers."""
-        return len(self._runtimes)
+        return len(self.runtimes)
 
     @property
     def workers(self) -> List[Type[Worker]]:
         """Get List of workers."""
-        return [r.worker for r in self._runtimes]
-
-    def egress_mime(self) -> str:
-        """Return mime of egress worker."""
-        return self._runtimes[-1].worker.resp_mime_type
+        return [r.worker for r in self.runtimes]
 
     def append(self, runtime: Runtime):
         """Sequentially appends workers to the workflow pipeline."""
-        self._runtimes.append(runtime)
-
-    def _label_stage(self, stage_id: int) -> str:
-        stage = ""
-        if stage_id == 0:
-            stage += STAGE_INGRESS
-        if stage_id == self.worker_count - 1:
-            stage += STAGE_EGRESS
-        return stage
+        self.runtimes.append(runtime)
 
-    def check_and_start(self, first: bool) -> Union[Runtime, None]:
+    def check_and_start(self, init: bool) -> Union[Runtime, None]:
         """Check all worker processes and try to start failed ones.
 
         Args:
-            first: whether the worker is tried to start at first time
+            init: whether the worker is tried to start at the first time
         """
-        for stage_id, worker_runtime in enumerate(self._runtimes):
-            label = self._label_stage(stage_id)
-            success = worker_runtime.check(
-                first, label, self._work_path, self._shutdown, self._shutdown_notify
-            )
-            if not success:
+        for worker_runtime in self.runtimes:
+            if not worker_runtime._check(  # pylint: disable=protected-access
+                self._work_path, self.shutdown, self.shutdown_notify, init
+            ):
                 return worker_runtime
         return None
 
 
 class RsRuntimeManager:
     """The manager to control Mosec process."""
 
-    def __init__(
-        self, py_manager: PyRuntimeManager, endpoint: str, configs: Dict[str, Any]
-    ):
+    def __init__(self, timeout: int):
         """Initialize a Mosec manager.
 
         Args:
-            manager: manager of python coordinator
-            endpoint: event of server shutdown
-            configs: config
+            timeout: service timeout in milliseconds
         """
-        self._process: Optional[subprocess.Popen] = None
+        self.process: Optional[subprocess.Popen] = None
 
-        self._py_manager: PyRuntimeManager = py_manager
-        self._endpoint = endpoint
-        self._server_path = Path(
+        self.server_path = Path(
             pkg_resources.resource_filename("mosec", "bin"), "mosec"
         )
-        self._configs: Dict[str, Any] = configs
+        self.timeout = timeout
 
     def halt(self):
         """Graceful shutdown."""
         # terminate controller first and wait for a graceful period
-        if self._process is None:
+        if self.process is None:
             return
-        self._process.terminate()
-        graceful_period = monotonic() + self._configs["timeout"] / 1000
+        self.process.terminate()
+        graceful_period = monotonic() + self.timeout / 1000
         while monotonic() < graceful_period:
-            ctr_exitcode = self._process.poll()
+            ctr_exitcode = self.process.poll()
             if ctr_exitcode is None:
                 sleep(0.1)
                 continue
             # exited
             if ctr_exitcode:  # on error
                 logger.error("mosec service halted on error [%d]", ctr_exitcode)
             else:
                 logger.info("mosec service halted normally [%d]", ctr_exitcode)
             break
 
         if monotonic() > graceful_period:
             logger.error("failed to terminate mosec service, will try to kill it")
-            self._process.kill()
+            self.process.kill()
 
-    def start(self) -> subprocess.Popen:
-        """Start the Mosec process."""
-        # pylint: disable=consider-using-with
-        self._process = subprocess.Popen([self._server_path] + self._controller_args())
-        return self._process
+    def start(self, config_path: Path) -> subprocess.Popen:
+        """Start the Mosec process.
 
-    def _controller_args(self):
-        args = []
-        self._configs.pop("dry_run")
-        for key, value in self._configs.items():
-            args.extend([f"--{key.replace('_', '-')}", str(value).lower()])
-        for worker_runtime in self._py_manager:
-            args.extend(["--batches", str(worker_runtime.max_batch_size)])
-            args.extend(["--waits", str(worker_runtime.max_wait_time)])
-        mime_type = self._py_manager.egress_mime()
-        args.extend(["--mime", mime_type])
-        args.extend(["--endpoint", self._endpoint])
-        logger.info("mosec received arguments: %s", args)
-        return args
+        Args:
+            config_path: configuration path of mosec
+        """
+        # pylint: disable=consider-using-with
+        self.process = subprocess.Popen([self.server_path, config_path])
+        return self.process
```

### Comparing `mosec-0.7.2/mosec/server.py` & `mosec-0.8.0/mosec/server.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,93 +20,78 @@
 Dynamic Batching
 ----------------
 
     The user may enable the dynamic batching feature for any stage when the
     corresponding worker is appended, by setting the
     :py:meth:`append_worker(max_batch_size) <Server.append_worker>`.
 
-Multiprocess
-------------
+Multiprocessing
+---------------
 
     The user may spawn multiple processes for any stage when the
     corresponding worker is appended, by setting the
     :py:meth:`append_worker(num) <Server.append_worker>`.
 """
 
 import json
 import multiprocessing as mp
-import os
 import pathlib
 import shutil
 import signal
 import subprocess
 import traceback
-from functools import partial
+from collections import defaultdict
 from multiprocessing.synchronize import Event
 from time import sleep
-from typing import Dict, List, Optional, Type, Union
+from typing import Dict, List, Type, Union
 
 from mosec.args import parse_arguments
 from mosec.dry_run import DryRunner
-from mosec.ipc import IPCWrapper
 from mosec.log import get_internal_logger
 from mosec.runtime import PyRuntimeManager, RsRuntimeManager, Runtime
 from mosec.utils import ParseTarget
-from mosec.worker import MOSEC_REF_TEMPLATE, Worker
+from mosec.worker import MOSEC_REF_TEMPLATE, SSEWorker, Worker
 
 logger = get_internal_logger()
 
 
 GUARD_CHECK_INTERVAL = 1
-MOSEC_OPENAPI_PATH = "mosec_openapi.json"
+MOSEC_RESERVED_ENDPOINTS = {"/", "/metrics", "/openapi"}
 
 
 class Server:
     """MOSEC server interface.
 
     It allows users to sequentially append workers they implemented, builds
     the workflow pipeline automatically and starts up the server.
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(
-        self,
-        ipc_wrapper: Optional[Union[IPCWrapper, partial]] = None,
-        endpoint: str = "/inference",
-    ):
-        """Initialize a MOSEC Server.
-
-        Args:
-            ipc_wrapper: (deprecated) wrapper function (before and after) IPC
-            endpoint: path to route inference
-        """
-        self.ipc_wrapper = ipc_wrapper
-        self.endpoint = endpoint
-
+    def __init__(self):
+        """Initialize a MOSEC Server."""
         self._shutdown: Event = mp.get_context("spawn").Event()
         self._shutdown_notify: Event = mp.get_context("spawn").Event()
         self._configs: dict = vars(parse_arguments())
 
-        self.coordinator_manager: PyRuntimeManager = PyRuntimeManager(
+        self._py_runtime_manager: PyRuntimeManager = PyRuntimeManager(
             self._configs["path"], self._shutdown, self._shutdown_notify
         )
-        self.controller = RsRuntimeManager(
-            self.coordinator_manager, endpoint, self._configs
-        )
+        self._rs_runtime_manager = RsRuntimeManager(self._configs["timeout"])
+        self._router: Dict[str, List[Runtime]] = defaultdict(list)
 
         self._daemon: Dict[str, Union[subprocess.Popen, mp.Process]] = {}
 
         self._server_shutdown: bool = False
 
     def _handle_signal(self):
         signal.signal(signal.SIGTERM, self._terminate)
         signal.signal(signal.SIGINT, self._terminate)
 
     def _validate_server(self):
-        assert self.coordinator_manager.worker_count > 0, (
+        assert self._py_runtime_manager.worker_count > 0, (
             "no worker registered\n"
             "help: use `.append_worker(...)` to register at least one worker"
         )
 
     def _check_daemon(self):
         for name, proc in self._daemon.items():
             if proc is None:
@@ -119,46 +104,74 @@
 
             if code is not None:
                 self._terminate(
                     code,
                     f"mosec daemon [{name}] exited on error code: {code}",
                 )
 
-    def _start_controller(self):
-        """Subprocess to start controller program."""
+    def _start_rs_runtime(self):
+        """Subprocess to start the rust runtime manager program."""
         if self._server_shutdown:
             return
-        process = self.controller.start()
-        self.register_daemon("controller", process)
+
+        # dump the config to a JSON file
+        config_path = pathlib.Path(self._configs["path"]) / "config.json"
+        configs = {"runtimes": [], "routes": []}
+        for key, value in self._configs.items():
+            if key in ("dry_run", "debug", "wait"):
+                continue
+            configs[key] = value
+        for runtime in self._py_runtime_manager.runtimes:
+            configs["runtimes"].append(
+                {
+                    "worker": runtime.name,
+                    "max_batch_size": runtime.max_batch_size,
+                    "max_wait_time": runtime.max_wait_time,
+                }
+            )
+        for endpoint, pipeline in self._router.items():
+            configs["routes"].append(
+                {
+                    "endpoint": endpoint,
+                    "workers": [runtime.name for runtime in pipeline],
+                    "is_sse": issubclass(pipeline[-1].worker, SSEWorker),
+                    **generate_openapi([runtime.worker for runtime in pipeline]),
+                }
+            )
+        config_path.parent.mkdir(parents=True, exist_ok=True)
+        with open(config_path, "w", encoding="utf-8") as file:
+            json.dump(configs, file, indent=2)
+
+        process = self._rs_runtime_manager.start(config_path)
+        self.register_daemon("rs_runtime", process)
 
     def _terminate(self, signum, framestack):
         logger.info("received signum[%s], terminating server [%s]", signum, framestack)
         self._server_shutdown = True
 
-    def _manage_coordinators(self):
-        first = True
+    def _manage_py_runtime(self):
+        init = True
         while not self._server_shutdown:
-            failed_worker = self.coordinator_manager.check_and_start(first)
-            if failed_worker is not None:
+            failed_runtime = self._py_runtime_manager.check_and_start(init)
+            if failed_runtime is not None:
                 self._terminate(
                     1,
-                    f"all the {failed_worker.worker.__name__} workers"
-                    f" at stage {failed_worker.stage_id} exited;"
+                    f"all the {failed_runtime.name} workers exited;"
                     " please check for bugs or socket connection issues",
                 )
-            first = False
+            init = False
             self._check_daemon()
             sleep(GUARD_CHECK_INTERVAL)
 
     def _halt(self):
         """Graceful shutdown."""
-        # notify coordinators for the shutdown
+        # notify the rs runtime to shutdown
         self._shutdown_notify.set()
-        self.controller.halt()
-        # shutdown coordinators
+        self._rs_runtime_manager.halt()
+        # shutdown py runtime manager
         self._shutdown.set()
         shutil.rmtree(self._configs["path"], ignore_errors=True)
         logger.info("mosec exited normally")
 
     def register_daemon(self, name: str, proc: subprocess.Popen):
         """Register a daemon to be monitored.
 
@@ -178,96 +191,120 @@
         worker: Type[Worker],
         num: int = 1,
         max_batch_size: int = 1,
         max_wait_time: int = 0,
         start_method: str = "spawn",
         env: Union[None, List[Dict[str, str]]] = None,
         timeout: int = 0,
+        route: Union[str, List[str]] = "/inference",
     ):
         """Sequentially appends workers to the workflow pipeline.
 
         Args:
             worker: the class you inherit from :class:`Worker<mosec.worker.Worker>`
                 which implements the :py:meth:`forward<mosec.worker.Worker.forward>`
             num: the number of processes for parallel computing (>=1)
             max_batch_size: the maximum batch size allowed (>=1), will enable the
                 dynamic batching if it > 1
             max_wait_time: the maximum wait time (millisecond) for dynamic batching,
                 needs to be used with `max_batch_size` to enable the feature. If not
                 configure, will use the CLI argument `--wait` (default=10ms)
-            start_method: the process starting method ("spawn" or "fork")
+            start_method: the process starting method ("spawn" or "fork"). (DO NOT
+                change this unless you understand the difference between them)
             env: the environment variables to set before starting the process
             timeout: the timeout (second) for each worker forward processing (>=1)
+            route: the route path for this worker. If not configured, will use the
+                default route path `/inference`. If a list is provided, different
+                route paths will share the same worker.
         """
         timeout = timeout if timeout >= 1 else self._configs["timeout"] // 1000
         max_wait_time = max_wait_time if max_wait_time >= 1 else self._configs["wait"]
-        stage_id = self.coordinator_manager.worker_count
         runtime = Runtime(
             worker,
             num,
             max_batch_size,
             max_wait_time,
-            stage_id + 1,
             timeout,
             start_method,
             env,
-            None,
-        )
-        runtime.validate()
-        self.coordinator_manager.append(runtime)
-
-    def _generate_openapi(self):
-        """Generate the OpenAPI specification."""
-        if self.coordinator_manager.worker_count <= 0:
-            return
-        workers = self.coordinator_manager.workers
-        request_worker_cls, response_worker_cls = workers[0], workers[-1]
-        input_schema, input_components = request_worker_cls.get_forward_json_schema(
-            ParseTarget.INPUT, MOSEC_REF_TEMPLATE
-        )
-        return_schema, return_components = response_worker_cls.get_forward_json_schema(
-            ParseTarget.RETURN, MOSEC_REF_TEMPLATE
         )
+        self._register_route(runtime, route)
+        self._py_runtime_manager.append(runtime)
 
-        def make_body(description, mime, schema):
-            if not schema:
-                return None
-            return {"description": description, "content": {mime: {"schema": schema}}}
-
-        schema = {
-            "request_body": make_body(
-                "Mosec Inference Request Body",
-                request_worker_cls.resp_mime_type,
-                input_schema,
-            ),
-            "responses": None
-            if not return_schema
-            else {
-                200: make_body(
-                    "Mosec Inference Result",
-                    response_worker_cls.resp_mime_type,
-                    return_schema,
-                )
-            },
-            "schemas": {**input_components, **return_components},
-        }
-        tmp_path = pathlib.Path(os.path.join(self._configs["path"], MOSEC_OPENAPI_PATH))
-        tmp_path.parent.mkdir(parents=True, exist_ok=True)
-        with open(tmp_path, "w", encoding="utf-8") as file:
-            json.dump(schema, file)
+    def register_runtime(self, routes: Dict[str, List[Runtime]]):
+        """Register the runtime to the routes."""
+        if self._py_runtime_manager.worker_count > 0:
+            raise RuntimeError(
+                "`register_runtime` can only be registered to an empty mosec server"
+            )
+        unique_runtimes = set()
+        for endpoint, runtimes in routes.items():
+            for runtime in runtimes:
+                self._register_route(runtime, endpoint)
+                unique_runtimes.add(runtime)
+        for runtime in unique_runtimes:
+            self._py_runtime_manager.append(runtime)
+
+    def _register_route(self, runtime: Runtime, route: Union[str, List[str]]):
+        """Register the route path for the worker."""
+        if isinstance(route, str):
+            if route in MOSEC_RESERVED_ENDPOINTS:
+                raise ValueError(f"'{route}' is reserved, try another one")
+            self._router[route].append(runtime)
+        elif isinstance(route, list):
+            for endpoint in route:
+                if endpoint in MOSEC_RESERVED_ENDPOINTS:
+                    raise ValueError(f"'{endpoint}' is reserved, try another one")
+                self._router[endpoint].append(runtime)
 
     def run(self):
         """Start the mosec model server."""
         self._validate_server()
         if self._configs["dry_run"]:
-            DryRunner(self.coordinator_manager).run()
+            DryRunner(self._router).run()
             return
 
         self._handle_signal()
-        self._generate_openapi()
-        self._start_controller()
+        self._start_rs_runtime()
         try:
-            self._manage_coordinators()
+            self._manage_py_runtime()
         # pylint: disable=broad-except
         except Exception:
             logger.error(traceback.format_exc().replace("\n", " "))
         self._halt()
+
+
+def generate_openapi(workers: List[Type[Worker]]):
+    """Generate the OpenAPI specification for one pipeline."""
+    if not workers:
+        return {}
+    request_worker_cls, response_worker_cls = workers[0], workers[-1]
+    input_schema, input_components = request_worker_cls.get_forward_json_schema(
+        ParseTarget.INPUT, MOSEC_REF_TEMPLATE
+    )
+    return_schema, return_components = response_worker_cls.get_forward_json_schema(
+        ParseTarget.RETURN, MOSEC_REF_TEMPLATE
+    )
+
+    def make_body(description, mime, schema):
+        if not schema:
+            return None
+        return {"description": description, "content": {mime: {"schema": schema}}}
+
+    return {
+        "request_body": make_body(
+            "Mosec Inference Request Body",
+            request_worker_cls.resp_mime_type,
+            input_schema,
+        ),
+        "responses": None
+        if not return_schema
+        else {
+            "200": make_body(
+                "Mosec Inference Result",
+                response_worker_cls.resp_mime_type,
+                return_schema,
+            )
+        },
+        "schemas": {**input_components, **return_components},
+        "mime": response_worker_cls.resp_mime_type,
+    }
```

### Comparing `mosec-0.7.2/mosec/utils/types.py` & `mosec-0.8.0/mosec/utils/types.py`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/mosec/worker.py` & `mosec-0.8.0/mosec/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,14 +230,15 @@
 
 
 class SSEWorker(Worker):
     """MOSEC worker with Server-Sent Events (SSE) support."""
 
     _stream_queue: SimpleQueue
     _stream_semaphore: Semaphore
+    resp_mime_type = "text/event-stream"
 
     def send_stream_event(self, text: str, index: int = 0):
         """Send a stream event to the client.
 
         Args:
             text: the text to be sent, needs to be UTF-8 compatible
             index: the index of the stream event. For the single request, this will
```

### Comparing `mosec-0.7.2/mosec.egg-info/PKG-INFO` & `mosec-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-Metadata-Version: 2.1
-Name: mosec
-Version: 0.7.2
-Summary: Model Serving made Efficient in the Cloud.
-Home-page: https://github.com/mosecorg/mosec
-Author: Keming Yang
-Author-email: kemingy94@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: mixin
-Provides-Extra: doc
-License-File: LICENSE
-
 <p align="center">
   <img src="https://user-images.githubusercontent.com/38581401/240117836-f06199ba-c80d-413a-9cb4-5adc76316bda.png" height="230" alt="MOSEC" />
 </p>
 
 <p align="center">
   <a href="https://discord.gg/Jq5vxuH69W">
     <img alt="discord invitation link" src="https://dcbadge.vercel.app/api/server/Jq5vxuH69W?style=flat">
   </a>
   <a href="https://pypi.org/project/mosec/">
     <img src="https://badge.fury.io/py/mosec.svg" alt="PyPI version" height="20">
   </a>
+  <a href="https://anaconda.org/conda-forge/mosec">
+    <img src="https://anaconda.org/conda-forge/mosec/badges/version.svg" alt="conda-forge">
+  </a>
   <a href="https://pypi.org/project/mosec">
     <img src="https://img.shields.io/pypi/pyversions/mosec" alt="Python Version" />
   </a>
   <a href="https://pepy.tech/project/mosec">
     <img src="https://pepy.tech/badge/mosec/month" alt="PyPi Downloads" height="20">
   </a>
   <a href="https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)">
@@ -72,14 +59,17 @@
 
 ```shell
 pip install --upgrade diffusers[torch] transformers
 ```
 
 ### Write the server
 
+<details>
+<summary>Click me for server codes with explanations.</summary>
+
 Firstly, we import the libraries and set up a basic logger to better observe what happens.
 
 ```python
 from io import BytesIO
 from typing import List
 
 import torch  # type: ignore
@@ -104,15 +94,15 @@
 class StableDiffusion(MsgpackMixin, Worker):
     def __init__(self):
         self.pipe = StableDiffusionPipeline.from_pretrained(
             "runwayml/stable-diffusion-v1-5", torch_dtype=torch.float16
         )
         device = "cuda" if torch.cuda.is_available() else "cpu"
         self.pipe = self.pipe.to(device)
-        self.example = ["useless example prompt"] * 4  # warmup (bs=4)
+        self.example = ["useless example prompt"] * 4  # warmup (batch_size=4)
 
     def forward(self, data: List[str]) -> List[memoryview]:
         logger.debug("generate images for %s", data)
         res = self.pipe(data)
         logger.debug("NSFW: %s", res[1])
         images = []
         for img in res[0]:
@@ -120,48 +110,54 @@
             img.save(dummy_file, format="JPEG")
             images.append(dummy_file.getbuffer())
         return images
 ```
 
 > **Note**
 >
-> (a) In this example we return an image in the binary format, which JSON does not support (unless encoded with base64 that makes it longer). Hence, msgpack suits our need better. If we do not inherit `MsgpackMixin`, JSON will be used by default. In other words, the protocol of the service request/response can either be msgpack or JSON.
+> (a) In this example we return an image in the binary format, which JSON does not support (unless encoded with base64 that makes the payload larger). Hence, msgpack suits our need better. If we do not inherit `MsgpackMixin`, JSON will be used by default. In other words, the protocol of the service request/response can be either msgpack, JSON, or any other format (check our [mixins](https://mosecorg.github.io/mosec/reference/interface.html#module-mosec.mixin)).
 >
 > (b) Warm-up usually helps to allocate GPU memory in advance. If the warm-up example is specified, the service will only be ready after the example is forwarded through the handler. However, if no example is given, the first request's latency is expected to be longer. The `example` should be set as a single item or a tuple depending on what `forward` expects to receive. Moreover, in the case where you want to warm up with multiple different examples, you may set `multi_examples` (demo [here](https://mosecorg.github.io/mosec/examples/jax.html)).
 >
-> (c) This example shows a single-stage service, where the `StableDiffusion` worker directly takes in client's prompt request and responds the image. Thus the `forward` can be considered as a complete service handler. However, we can also design a multi-stage service with workers doing different jobs (e.g., downloading images, forward model, post-processing) in a pipeline. In this case, the whole pipeline is considered as the service handler, with the first worker taking in the request and the last worker sending out the response. The data flow between workers is done by inter-process communication.
+> (c) This example shows a single-stage service, where the `StableDiffusion` worker directly takes in client's prompt request and responds the image. Thus the `forward` can be considered as a complete service handler. However, we can also design a multi-stage service with workers doing different jobs (e.g., downloading images, model inference, post-processing) in a pipeline. In this case, the whole pipeline is considered as the service handler, with the first worker taking in the request and the last worker sending out the response. The data flow between workers is done by inter-process communication.
 >
 > (d) Since dynamic batching is enabled in this example, the `forward` method will wishfully receive a _list_ of string, e.g., `['a cute cat playing with a red ball', 'a man sitting in front of a computer', ...]`, aggregated from different clients for _batch inference_, improving the system throughput.
 
-Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the flag `--wait` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
+Finally, we append the worker to the server to construct a *single-stage* workflow (multiple stages can be [pipelined](https://en.wikipedia.org/wiki/Pipeline_(computing)) to further boost the throughput, see [this example](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision)), and specify the number of processes we want it to run in parallel (`num=1`), and the maximum batch size (`max_batch_size=4`, the maximum number of requests dynamic batching will accumulate before timeout; timeout is defined with the `max_wait_time=10` in milliseconds, meaning the longest time Mosec waits until sending the batch to the Worker).
 
 ```python
 if __name__ == "__main__":
     server = Server()
     # 1) `num` specifies the number of processes that will be spawned to run in parallel.
     # 2) By configuring the `max_batch_size` with the value > 1, the input data in your
     # `forward` function will be a list (batch); otherwise, it's a single item.
     server.append_worker(StableDiffusion, num=1, max_batch_size=4, max_wait_time=10)
     server.run()
 ```
+</details>
 
 ### Run the server
 
+<details>
+<summary>Click me to see how to run and query the server.</summary>
+
 The above snippets are merged in our example file. You may directly run at the project root level. We first have a look at the _command line arguments_ (explanations [here](https://mosecorg.github.io/mosec/reference/arguments.html)):
 
 ```shell
 python examples/stable_diffusion/server.py --help
 ```
 
 Then let's start the server with debug logs:
 
 ```shell
-python examples/stable_diffusion/server.py --debug
+python examples/stable_diffusion/server.py --log-level debug --timeout 30000
 ```
 
+Open `http://127.0.0.1:8000/openapi/swagger/` in your browser to get the OpenAPI doc.
+
 And in another terminal, test it:
 
 ```shell
 python examples/stable_diffusion/client.py --prompt "a cute cat playing with a red ball" --output cat.jpg --port 8000
 ```
 
 You will get an image named "cat.jpg" in the current directory.
@@ -169,49 +165,62 @@
 You can check the metrics:
 
 ```shell
 curl http://127.0.0.1:8000/metrics
 ```
 
 That's it! You have just hosted your **_stable-diffusion model_** as a service! 😉
+</details>
 
 ## Examples
 
 More ready-to-use examples can be found in the [Example](https://mosecorg.github.io/mosec/examples/index.html) section. It includes:
 
-- [Multi-stage workflow demo](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
+- [Pipeline](https://mosecorg.github.io/mosec/examples/echo.html): a simple echo demo even without any ML model.
 - [Request validation](https://mosecorg.github.io/mosec/examples/validate.html): validate the request with type annotation.
+- [Multiple route](https://mosecorg.github.io/mosec/examples/multi_route.html): serve multiple models in one service
 - [Shared memory IPC](https://mosecorg.github.io/mosec/examples/ipc.html): inter-process communication with shared memory.
 - [Customized GPU allocation](https://mosecorg.github.io/mosec/examples/env.html): deploy multiple replicas, each using different GPUs.
 - [Customized metrics](https://mosecorg.github.io/mosec/examples/metric.html): record your own metrics for monitoring.
 - [Jax jitted inference](https://mosecorg.github.io/mosec/examples/jax.html): just-in-time compilation speeds up the inference.
 - PyTorch deep learning models:
   - [sentiment analysis](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing): infer the sentiment of a sentence.
   - [image recognition](https://mosecorg.github.io/mosec/examples/pytorch.html#computer-vision): categorize a given image.
   - [stable diffusion](https://mosecorg.github.io/mosec/examples/stable_diffusion.html): generate images based on texts, with msgpack serialization.
 
 ## Configuration
 
 - Dynamic batching
-  - `max_batch_size` is configured when you `append_worker` (make sure inference with the max value won't cause the out-of-memory in GPU).
-  - `--wait (default=10ms)` is configured through CLI arguments (this usually should <= one batch inference duration).
-  - If enabled, it will collect a batch either when it reaches the `max_batch_size` or the `wait` time.
-- Check the [arguments doc](https://mosecorg.github.io/mosec/reference/arguments.html).
+  - `max_batch_size` and `max_wait_time (millisecond)` are configured when you call `append_worker`.
+  - Make sure inference with the `max_batch_size` value won't cause the out-of-memory in GPU.
+  - Normally, `max_wait_time` should be less than the batch inference time.
+  - If enabled, it will collect a batch either when the number of accumulated requests reaches `max_batch_size` or when `max_wait_time` has elapsed. The service will benefit from this feature when the traffic is high.
+- Check the [arguments doc](https://mosecorg.github.io/mosec/reference/arguments.html) for other configurations.
 
 ## Deployment
 
-- This may require some shared memory, remember to set the `--shm-size` flag if you are using docker.
-- This service doesn't require Gunicorn or NGINX, but you can certainly use the ingress controller. BTW, it should be the PID 1 process in the container since it controls multiple processes.
+- If you're looking for a GPU base image with `mosec` installed, you can check the official image [`mosecorg/mosec`](https://hub.docker.com/r/mosecorg/mosec). For the complex use case, check out [envd](https://github.com/tensorchord/envd).
+- This service doesn't need Gunicorn or NGINX, but you can certainly use the ingress controller when necessary.
+- This service should be the PID 1 process in the container since it controls multiple processes. If you need to run multiple processes in one container, you will need a supervisor. You may choose [Supervisor](https://github.com/Supervisor/supervisor) or [Horust](https://github.com/FedericoPonzi/Horust).
 - Remember to collect the **metrics**.
   - `mosec_service_batch_size_bucket` shows the batch size distribution.
   - `mosec_service_batch_duration_second_bucket` shows the duration of dynamic batching for each connection in each stage (starts from receiving the first task).
   - `mosec_service_process_duration_second_bucket` shows the duration of processing for each connection in each stage (including the IPC time but excluding the `mosec_service_batch_duration_second_bucket`).
   - `mosec_service_remaining_task` shows the number of currently processing tasks.
   - `mosec_service_throughput` shows the service throughput.
-- Stop the service with `SIGINT` or `SIGTERM` since it has the graceful shutdown logic.
+- Stop the service with `SIGINT` (`CTRL+C`) or `SIGTERM` (`kill {PID}`) since it has the graceful shutdown logic.
+
+## Performance tuning
+
+- Find out the best `max_batch_size` and `max_wait_time` for your inference service. The metrics will show the histograms of the real batch size and batch duration. Those are the key information to adjust these two parameters.
+- Try to split the whole inference process into separate CPU and GPU stages (ref [DistilBERT](https://mosecorg.github.io/mosec/examples/pytorch.html#natural-language-processing)). Different stages will be run in a [data pipeline](https://en.wikipedia.org/wiki/Pipeline_(software)), which will keep the GPU busy.
+- You can also adjust the number of workers in each stage. For example, if your pipeline consists of a CPU stage for preprocessing and a GPU stage for model inference, increasing the number of CPU-stage workers can help to produce more data to be batched for model inference at the GPU stage; increasing the GPU-stage workers can fully utilize the GPU memory and computation power. Both ways may contribute to higher GPU utilization, which consequently results in higher service throughput.
+- For multi-stage services, note that the data passing through different stages will be serialized/deserialized by the `serialize_ipc/deserialize_ipc` methods, so extremely large data might make the whole pipeline slow. The serialized data is passed to the next stage through rust by default, you could enable shared memory to potentially reduce the latency (ref [RedisShmIPCMixin](https://mosecorg.github.io/mosec/examples/ipc.html#redis-shm-ipc-py)).
+- You should choose appropriate `serialize/deserialize` methods, which are used to decode the user request and encode the response. By default, both are using JSON. However, images and embeddings are not well supported by JSON. You can choose msgpack which is faster and binary compatible (ref [Stable Diffusion](https://mosecorg.github.io/mosec/examples/stable_diffusion.html)).
+- Configure the threads for OpenBLAS or MKL. It might not be able to choose the most suitable CPUs used by the current Python process. You can configure it for each worker by using the [env](https://mosecorg.github.io/mosec/reference/interface.html#mosec.server.Server.append_worker) (ref [custom GPU allocation](https://mosecorg.github.io/mosec/examples/env.html)).
 
 ## Adopters
 
 Here are some of the companies and individual users that are using Mosec:
 
 - [Modelz](https://modelz.ai): Serverless platform for ML inference.
 - [MOSS](https://github.com/OpenLMLab/MOSS/blob/main/README_en.md): An open sourced conversational language model like ChatGPT.
@@ -232,9 +241,7 @@
 ```
 
 ## Contributing
 
 We welcome any kind of contribution. Please give us feedback by [raising issues](https://github.com/mosecorg/mosec/issues/new/choose) or discussing on [Discord](https://discord.gg/Jq5vxuH69W). You could also directly [contribute](https://mosecorg.github.io/mosec/development/contributing.html) your code and pull request!
 
 To start develop, you can use [envd](https://github.com/tensorchord/envd) to create an isolated and clean Python & Rust environment. Check the [envd-docs](https://envd.tensorchord.ai/) or [build.envd](https://github.com/mosecorg/mosec/blob/main/build.envd) for more information.
-
-
```

### Comparing `mosec-0.7.2/mosec.egg-info/SOURCES.txt` & `mosec-0.8.0/mosec.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 .gitignore
-.lycheeignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 CITATION.cff
 CONTRIBUTING.md
 Cargo.lock
 Cargo.toml
+Dockerfile
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 build.envd
 license.json
+lychee.toml
 pyproject.toml
 rustfmt.toml
 setup.py
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.md
 docs/source/license.md
+docs/source/_static/.gitkeep
 docs/source/development/contributing.md
 docs/source/development/index.md
 docs/source/examples/echo.md
 docs/source/examples/env.md
 docs/source/examples/index.md
 docs/source/examples/ipc.md
 docs/source/examples/jax.md
 docs/source/examples/metric.md
+docs/source/examples/multi_route.md
 docs/source/examples/pytorch.md
 docs/source/examples/stable_diffusion.md
 docs/source/examples/validate.md
 docs/source/reference/arguments.md
+docs/source/reference/concept.md
 docs/source/reference/index.md
 docs/source/reference/interface.md
+docs/source/reference/migration.md
 mosec/__init__.py
 mosec/_version.py
 mosec/args.py
 mosec/coordinator.py
 mosec/dry_run.py
 mosec/env.py
 mosec/errors.py
-mosec/ipc.py
 mosec/log.py
 mosec/protocol.py
 mosec/py.typed
 mosec/runtime.py
 mosec/server.py
 mosec/worker.py
 mosec.egg-info/PKG-INFO
@@ -57,23 +62,20 @@
 mosec.egg-info/top_level.txt
 mosec/mixin/__init__.py
 mosec/mixin/msgpack_worker.py
 mosec/mixin/numbin_worker.py
 mosec/mixin/plasma_worker.py
 mosec/mixin/redis_worker.py
 mosec/mixin/typed_worker.py
-mosec/plugins/__init__.py
-mosec/plugins/plasma_shm.py
 mosec/utils/__init__.py
 mosec/utils/types.py
 requirements/dev.txt
 requirements/doc.txt
 requirements/mixin.txt
 src/apidoc.rs
-src/args.rs
-src/coordinator.rs
+src/config.rs
 src/errors.rs
 src/main.rs
 src/metrics.rs
 src/protocol.rs
 src/routes.rs
 src/tasks.rs
```

### Comparing `mosec-0.7.2/pyproject.toml` & `mosec-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -86,7 +86,14 @@
 [pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 markers = [
     "shm: mark a test is related to shared memory",
 ]
+
+[tool.ruff]
+target-version = "py38"
+line-length = 88
+select = ["E", "F", "B", "I", "SIM", "TID", "PL"]
+[tool.ruff.pylint]
+max-args = 11
```

### Comparing `mosec-0.7.2/setup.py` & `mosec-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Build the package with Rust binary."""
+
 import os
 import shutil
 import subprocess
 from io import open
 
 from setuptools import Extension, find_packages, setup
 from setuptools.command.build_ext import build_ext as _build_ext
@@ -19,14 +21,15 @@
     doc_requirements = f.read().splitlines()
 
 with open(os.path.join(here, "requirements/mixin.txt"), encoding="utf-8") as f:
     mixin_requirements = f.read().splitlines()
 
 
 class RustExtension(Extension):
+    # pylint: disable=too-few-public-methods
     """Custom Extension class for rust"""
 
 
 ext_modules = []
 
 if os.getenv("PRODUCTION_MODE"):
     ext_modules.append(RustExtension(name="mosec.bin", sources=["src/*"]))
@@ -62,14 +65,15 @@
             target_dir = os.path.join("target", "release", PACKAGE_NAME)
         os.makedirs(build_libpath, exist_ok=True)
         shutil.copy(target_dir, build_libpath)
 
         if self.inplace:
             os.makedirs(os.path.dirname(libpath), exist_ok=True)
             shutil.copy(build_libpath, libpath)
+        return None
 
 
 setup(
     name=PACKAGE_NAME,
     author="Keming Yang",
     author_email="kemingy94@gmail.com",
     description="Model Serving made Efficient in the Cloud.",
@@ -85,9 +89,9 @@
     extras_require={
         "dev": dev_requirements,
         "mixin": mixin_requirements,
         "doc": doc_requirements,
     },
     zip_safe=False,
     ext_modules=ext_modules,  # type: ignore
-    cmdclass=dict(build_ext=RustBuildExt),  # type: ignore
+    cmdclass={"build_ext": RustBuildExt},  # type: ignore
 )
```

### Comparing `mosec-0.7.2/src/errors.rs` & `mosec-0.8.0/src/errors.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/src/main.rs` & `mosec-0.8.0/src/main.rs`

 * *Files 22% similar despite different names*

```diff
@@ -9,42 +9,40 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 mod apidoc;
-mod args;
-mod coordinator;
+mod config;
 mod errors;
 mod metrics;
 mod protocol;
 mod routes;
 mod tasks;
 
+use std::env;
 use std::fs::read_to_string;
 use std::net::SocketAddr;
-use std::path::Path;
 
 use axum::routing::{get, post};
 use axum::Router;
 use tokio::signal::unix::{signal, SignalKind};
-use tracing::info;
+use tracing::{debug, info};
 use tracing_subscriber::fmt::time::OffsetTime;
 use tracing_subscriber::prelude::*;
 use tracing_subscriber::{filter, Layer};
 use utoipa::OpenApi;
+use utoipa_swagger_ui::SwaggerUi;
 
 use crate::apidoc::MosecOpenAPI;
-use crate::args::Opts;
-use crate::coordinator::Coordinator;
-use crate::routes::{index, inference, metrics, openapi_json, sse_inference, AppState, RustAPIDoc};
-use crate::tasks::TaskManager;
-
-const MOSEC_OPENAPI_PATH: &str = "mosec_openapi.json";
+use crate::config::Config;
+use crate::metrics::{Metrics, METRICS};
+use crate::routes::{index, inference, metrics, sse_inference, RustAPIDoc};
+use crate::tasks::{TaskManager, TASK_MANAGER};
 
 async fn shutdown_signal() {
     let mut interrupt = signal(SignalKind::interrupt()).unwrap();
     let mut terminate = signal(SignalKind::terminate()).unwrap();
     loop {
         tokio::select! {
             _ = interrupt.recv() => {
@@ -60,74 +58,90 @@
                 break;
             },
         };
     }
 }
 
 #[tokio::main]
-async fn run(opts: &Opts) {
-    let python_api =
-        read_to_string(Path::new(&opts.path).join(MOSEC_OPENAPI_PATH)).unwrap_or_default();
-    let mut api = MosecOpenAPI {
+async fn run(conf: &Config) {
+    let mut doc = MosecOpenAPI {
         api: RustAPIDoc::openapi(),
     };
-    api.merge("/inference", python_api.parse().unwrap_or_default());
-    api.replace_path_item("/inference", &opts.endpoint);
+    for route in &conf.routes {
+        doc.merge_route(route);
+    }
+    doc.clean();
 
-    let state = AppState {
-        mime: opts.mime.clone(),
-        openapi: api,
-    };
-    let coordinator = Coordinator::init_from_opts(opts);
-    let barrier = coordinator.run();
-    barrier.wait().await;
-    let app = Router::new()
+    let metrics_instance = Metrics::init_with_namespace(&conf.namespace, conf.timeout);
+    METRICS.set(metrics_instance).unwrap();
+    let mut task_manager = TaskManager::new(conf.timeout);
+    let barrier = task_manager.init_from_config(conf);
+    TASK_MANAGER.set(task_manager).unwrap();
+
+    let mut router = Router::new()
+        .merge(SwaggerUi::new("/openapi/swagger").url("/openapi/metadata.json", doc.api))
         .route("/", get(index))
-        .route("/openapi", get(openapi_json))
-        .route("/metrics", get(metrics))
-        .route(&opts.endpoint, post(inference))
-        .route("/sse_inference", post(sse_inference))
-        .with_state(state);
+        .route("/metrics", get(metrics));
 
-    let addr: SocketAddr = format!("{}:{}", opts.address, opts.port).parse().unwrap();
+    for route in &conf.routes {
+        if route.is_sse {
+            router = router.route(&route.endpoint, post(sse_inference));
+        } else {
+            router = router.route(&route.endpoint, post(inference));
+        }
+    }
+
+    // wait until each stage has at least one worker alive
+    barrier.wait().await;
+    let addr: SocketAddr = format!("{}:{}", conf.address, conf.port).parse().unwrap();
     info!(?addr, "http service is running");
     axum::Server::bind(&addr)
-        .serve(app.into_make_service())
+        .serve(router.into_make_service())
         .with_graceful_shutdown(shutdown_signal())
         .await
         .unwrap();
 }
 
 fn main() {
-    let opts: Opts = argh::from_env();
+    // let opts: Opts = argh::from_env();
+    let cmd_args: Vec<String> = env::args().collect();
+    if cmd_args.len() != 2 {
+        println!(
+            "expect one argument as the config path but got {:?}",
+            cmd_args
+        );
+        return;
+    }
+    let config_str = read_to_string(&cmd_args[1]).expect("read config file failure");
+    let conf: Config = serde_json::from_str(&config_str).expect("parse config failure");
 
     // this has to be defined before tokio multi-threads
     let timer = OffsetTime::local_rfc_3339().expect("local time offset");
-    if opts.debug || opts.log_level == "debug" {
+    if conf.log_level == "debug" {
         // use colorful log for debug
         let output = tracing_subscriber::fmt::layer().compact().with_timer(timer);
         tracing_subscriber::registry()
             .with(
                 output
                     .with_filter(filter::filter_fn(|metadata| {
                         !metadata.target().starts_with("hyper")
                     }))
                     .with_filter(filter::LevelFilter::DEBUG),
             )
             .init();
     } else {
         // use JSON format for production
-        let level = match opts.log_level.as_str() {
+        let level = match conf.log_level.as_str() {
             "error" => tracing::Level::ERROR,
             "warning" => tracing::Level::WARN,
             _ => tracing::Level::INFO,
         };
         tracing_subscriber::fmt()
             .with_max_level(level)
             .json()
             .with_timer(timer)
             .init();
     }
 
-    info!(?opts, "parse service arguments");
-    run(&opts);
+    debug!(?conf, "parse service arguments");
+    run(&conf);
 }
```

### Comparing `mosec-0.7.2/src/metrics.rs` & `mosec-0.8.0/src/metrics.rs`

 * *Files identical despite different names*

### Comparing `mosec-0.7.2/src/protocol.rs` & `mosec-0.8.0/src/protocol.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use std::path::PathBuf;
 use std::sync::Arc;
 use std::time::{Duration, Instant};
 
-use async_channel::{Receiver, Sender};
+use async_channel::Receiver;
 use bytes::{BufMut, Bytes, BytesMut};
 use tokio::io::{self, AsyncReadExt, AsyncWriteExt};
 use tokio::net::{UnixListener, UnixStream};
 use tokio::sync::Barrier;
 use tracing::{debug, error, info, warn};
 
 use crate::metrics::{Metrics, StageConnectionLabel};
 use crate::tasks::{TaskCode, TaskManager};
 
 const FLAG_U8_SIZE: usize = 2;
 const NUM_U8_SIZE: usize = 2;
+const STATE_U8_SIZE: usize = 2;
 const TASK_ID_U8_SIZE: usize = 4;
 const LENGTH_U8_SIZE: usize = 4;
 
 const BIT_STATUS_OK: u16 = 0b1;
 const BIT_STATUS_BAD_REQ: u16 = 0b10;
 const BIT_STATUS_VALIDATION_ERR: u16 = 0b100;
 const BIT_STATUS_TIMEOUT_ERR: u16 = 0b10000;
@@ -39,136 +40,140 @@
 // Others are treated as Internal Error
 
 #[allow(clippy::too_many_arguments)]
 pub(crate) async fn communicate(
     path: PathBuf,
     batch_size: usize,
     wait_time: Duration,
-    stage_id: String,
+    stage_name: String,
     receiver: Receiver<u32>,
-    sender: Sender<u32>,
-    last_sender: Sender<u32>,
     barrier: Arc<Barrier>,
 ) {
     let listener = UnixListener::bind(&path).expect("failed to bind to the socket");
     let mut connection_id: u32 = 0;
     loop {
         connection_id += 1;
-        let sender_clone = sender.clone();
-        let last_sender_clone = last_sender.clone();
         let receiver_clone = receiver.clone();
-        let stage_id_label = stage_id.clone();
+        let stage_name_label = stage_name.clone();
         let connection_id_label = connection_id.to_string();
         info!(?path, "begin listening to socket");
         match listener.accept().await {
             Ok((mut stream, addr)) => {
                 info!(?addr, "socket accepted connection from");
                 tokio::spawn(async move {
                     let mut code: TaskCode = TaskCode::InternalError;
                     let mut ids: Vec<u32> = Vec::with_capacity(batch_size);
                     let mut data: Vec<Bytes> = Vec::with_capacity(batch_size);
+                    let mut states: Vec<u16> = Vec::with_capacity(batch_size);
                     let task_manager = TaskManager::global();
                     let metrics = Metrics::global();
                     let metric_label = StageConnectionLabel {
-                        stage: stage_id_label.clone(),
+                        stage: stage_name_label.clone(),
                         connection: connection_id_label,
                     };
                     loop {
                         ids.clear();
                         data.clear();
+                        states.clear();
                         let batch_timer =
                             get_batch(&receiver_clone, batch_size, &mut ids, wait_time).await;
                         if let Some(timer) = batch_timer {
                             metrics
                                 .batch_duration
                                 .get_or_create(&metric_label)
                                 .observe(timer.elapsed().as_secs_f64())
                         }
                         // start record the duration metrics here because receiving the first task
                         // depends on when the request comes in.
                         let start_timer = Instant::now();
-                        task_manager.get_multi_tasks_data(&mut ids, &mut data);
+                        task_manager.get_multi_tasks_data(&mut ids, &mut data, &mut states);
                         if data.is_empty() {
                             continue;
                         }
                         if batch_size > 1 {
                             // only record the batch size when it's set to a number > 1
                             metrics
                                 .batch_size
                                 .get_or_create(&metric_label)
                                 .observe(data.len() as f64);
                         }
-                        if let Err(err) = send_message(&mut stream, &ids, &data).await {
-                            error!(%err, %stage_id_label, %connection_id, "socket send message error");
+                        if let Err(err) = send_message(&mut stream, &ids, &data, &states).await {
+                            error!(%err, %stage_name_label, %connection_id, "socket send message error");
                             info!(
                                 "service failed to write data to stream, will try to send task \
                                  back to see if other thread can handle it"
                             );
                             for id in &ids {
-                                last_sender_clone.send(*id).await.expect("sender is closed");
+                                task_manager.send_task(id).await;
                             }
                             break;
                         }
-                        debug!(%stage_id_label, %connection_id, "socket finished to send message");
+                        debug!(%stage_name_label, %connection_id, "socket finished to send message");
 
                         ids.clear();
                         data.clear();
+                        states.clear();
                         if let Err(err) =
-                            read_message(&mut stream, &mut code, &mut ids, &mut data).await
+                            read_message(&mut stream, &mut code, &mut ids, &mut data, &mut states)
+                                .await
                         {
-                            error!(%err, %stage_id_label, %connection_id, "socket receive message error");
+                            error!(%err, %stage_name_label, %connection_id, "socket receive message error");
                             break;
                         }
-                        debug!(%stage_id_label, %connection_id, "socket finished to read message");
+                        debug!(%stage_name_label, %connection_id, "socket finished to read message");
                         while code == TaskCode::StreamEvent {
                             send_stream_event(&ids, &data).await;
                             ids.clear();
                             data.clear();
-                            if let Err(err) =
-                                read_message(&mut stream, &mut code, &mut ids, &mut data).await
+                            states.clear();
+                            if let Err(err) = read_message(
+                                &mut stream,
+                                &mut code,
+                                &mut ids,
+                                &mut data,
+                                &mut states,
+                            )
+                            .await
                             {
-                                error!(%err, %stage_id_label, %connection_id, "socket receive message error");
+                                error!(%err, %stage_name_label, %connection_id, "socket receive message error");
                                 break;
                             }
-                            debug!(%stage_id_label, %connection_id, "socket finished to read message");
+                            debug!(%stage_name_label, %connection_id, "socket finished to read message");
                         }
                         task_manager.update_multi_tasks(code, &ids, &data).await;
                         match code {
                             TaskCode::Normal => {
                                 for id in &ids {
-                                    sender_clone
-                                        .send(*id)
-                                        .await
-                                        .expect("next channel is closed");
+                                    task_manager.send_task(id).await;
                                 }
                                 // only the normal tasks will be recorded
                                 metrics
                                     .duration
                                     .get_or_create(&metric_label)
                                     .observe(start_timer.elapsed().as_secs_f64());
                             }
                             _ => {
                                 warn!(
                                     ?ids,
                                     ?code,
-                                    ?stage_id_label,
+                                    ?stage_name_label,
                                     ?connection_id,
                                     "abnormal tasks, check Python log for more details"
                                 );
                             }
                         }
                     }
                 });
                 // ensure every stage is properly initialized (including warmup)
                 if connection_id == 1 {
                     barrier.wait().await;
                 }
             }
             Err(err) => {
-                error!(%err, %stage_id, %connection_id, "socket failed to accept the connection");
+                error!(%err, %stage_name, %connection_id, "socket failed to accept the connection");
                 break;
             }
         }
     }
 }
 
 async fn send_stream_event(ids: &[u32], data: &[Bytes]) {
@@ -189,14 +194,15 @@
 }
 
 async fn read_message(
     stream: &mut UnixStream,
     code: &mut TaskCode,
     ids: &mut Vec<u32>,
     data: &mut Vec<Bytes>,
+    states: &mut Vec<u16>,
 ) -> Result<(), io::Error> {
     stream.readable().await?;
     let mut flag_buf = [0u8; FLAG_U8_SIZE];
     let mut num_buf = [0u8; NUM_U8_SIZE];
     stream.read_exact(&mut flag_buf).await?;
     stream.read_exact(&mut num_buf).await?;
     let flag = u16::from_be_bytes(flag_buf);
@@ -215,22 +221,26 @@
     } else {
         TaskCode::InternalError
     };
     debug!(?flag, ?flag_buf, "read message");
 
     let mut id_buf = [0u8; TASK_ID_U8_SIZE];
     let mut length_buf = [0u8; LENGTH_U8_SIZE];
+    let mut state_buf = [0u8; STATE_U8_SIZE];
     for _ in 0..num {
         stream.read_exact(&mut id_buf).await?;
+        stream.read_exact(&mut state_buf).await?;
         stream.read_exact(&mut length_buf).await?;
         let id = u32::from_be_bytes(id_buf);
+        let state = u16::from_be_bytes(state_buf);
         let length = u32::from_be_bytes(length_buf);
         let mut data_buf = vec![0u8; length as usize];
         stream.read_exact(&mut data_buf).await?;
         ids.push(id);
+        states.push(state);
         data.push(data_buf.into());
     }
     let byte_size = data.iter().fold(0, |acc, x| acc + x.len());
     debug!(
         ?ids,
         ?code,
         ?num,
@@ -275,21 +285,23 @@
     Some(start_time)
 }
 
 async fn send_message(
     stream: &mut UnixStream,
     ids: &[u32],
     data: &[Bytes],
+    states: &[u16],
 ) -> Result<(), io::Error> {
     stream.writable().await?;
     let mut buffer = BytesMut::new();
     buffer.put_u16(0); // flag
     buffer.put_u16(ids.len() as u16);
     for i in 0..ids.len() {
         buffer.put_u32(ids[i]);
+        buffer.put_u16(states[i]);
         buffer.put_u32(data[i].len() as u32);
         buffer.put(data[i].clone());
     }
     stream.write_all(&buffer).await?;
     debug!(?ids, batch_size=%ids.len(), byte_size=%buffer.len(), "send data to the socket");
 
     Ok(())
@@ -341,31 +353,42 @@
         let path = env::temp_dir().join("mosec_test.ipc");
         if path.exists() {
             std::fs::remove_file(&path).expect("remove file error");
         }
         let listener = UnixListener::bind(&path).expect("bind error");
         let ids = vec![0u32, 1];
         let data = vec![Bytes::from_static(b"hello"), Bytes::from_static(b"world")];
+        let states = vec![1u16, 2];
 
         // setup the server in another tokio thread
         let ids_clone = ids.clone();
         let data_clone = data.clone();
+        let states_clone = states.clone();
         tokio::spawn(async move {
             let (mut stream, _addr) = listener.accept().await.unwrap();
-            send_message(&mut stream, &ids_clone, &data_clone)
+            send_message(&mut stream, &ids_clone, &data_clone, &states_clone)
                 .await
                 .expect("send message error");
             tokio::time::sleep(Duration::from_millis(1)).await;
         });
 
         let mut stream = UnixStream::connect(&path).await.unwrap();
         let mut recv_ids = Vec::new();
+        let mut recv_states = Vec::new();
         let mut recv_data = Vec::new();
         let mut code = TaskCode::InternalError;
-        read_message(&mut stream, &mut code, &mut recv_ids, &mut recv_data)
-            .await
-            .expect("read message error");
+        read_message(
+            &mut stream,
+            &mut code,
+            &mut recv_ids,
+            &mut recv_data,
+            &mut recv_states,
+        )
+        .await
+        .expect("read message error");
 
         assert_eq!(recv_ids, ids);
         assert_eq!(recv_data, data);
+        assert_eq!(recv_states, states);
+        std::fs::remove_file(&path).expect("failed to remove the test socket file");
     }
 }
```

### Comparing `mosec-0.7.2/src/routes.rs` & `mosec-0.8.0/src/routes.rs`

 * *Files 16% similar despite different names*

```diff
@@ -11,40 +11,34 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use std::time::Duration;
 
 use axum::body::BoxBody;
-use axum::extract::State;
+use axum::http::Uri;
 use axum::response::sse::{Event, KeepAlive, Sse};
 use axum::response::IntoResponse;
 use bytes::Bytes;
 use hyper::body::to_bytes;
 use hyper::header::{HeaderValue, CONTENT_TYPE};
 use hyper::{Body, Request, Response, StatusCode};
 use prometheus_client::encoding::text::encode;
 use tracing::warn;
 use utoipa::OpenApi;
 
-use crate::apidoc::MosecOpenAPI;
 use crate::errors::ServiceError;
 use crate::metrics::{CodeLabel, Metrics, DURATION_LABEL, REGISTRY};
 use crate::tasks::{TaskCode, TaskManager};
 
 const SERVER_INFO: &str = concat!(env!("CARGO_PKG_NAME"), "/", env!("CARGO_PKG_VERSION"));
 const RESPONSE_DEFAULT: &[u8] = b"MOSEC service";
 const RESPONSE_EMPTY: &[u8] = b"no data provided";
 const RESPONSE_SHUTDOWN: &[u8] = b"gracefully shutting down";
-
-#[derive(Clone)]
-pub(crate) struct AppState {
-    pub mime: String,
-    pub openapi: MosecOpenAPI,
-}
+const DEFAULT_RESPONSE_MIME: &str = "application/json";
 
 fn build_response(status: StatusCode, content: Bytes) -> Response<Body> {
     Response::builder()
         .status(status)
         .header("server", HeaderValue::from_static(SERVER_INFO))
         .body(Body::from(content))
         .unwrap()
@@ -89,47 +83,33 @@
     let mut encoded = String::new();
     let registry = REGISTRY.get().unwrap();
     encode(&mut encoded, registry).unwrap();
     build_response(StatusCode::OK, Bytes::from(encoded))
 }
 
 #[utoipa::path(
-    get,
-    path = "/openapi",
-    responses(
-        (status = StatusCode::OK, description = "Get OpenAPI doc", body = String)
-    )
-)]
-pub(crate) async fn openapi_json(
-    State(state): State<AppState>,
-    _: Request<Body>,
-) -> Response<Body> {
-    let s = state
-        .openapi
-        .api
-        .to_json()
-        .unwrap_or("OpenAPI generation failed".to_string());
-    build_response(StatusCode::OK, Bytes::from(s))
-}
-
-#[utoipa::path(
     post,
-    path = "/inference",
+    path = "/openapi/reserved/inference",
     responses(
         (status = StatusCode::OK, description = "Inference"),
         (status = StatusCode::BAD_REQUEST, description = "BAD_REQUEST"),
         (status = StatusCode::SERVICE_UNAVAILABLE, description = "SERVICE_UNAVAILABLE"),
         (status = StatusCode::UNPROCESSABLE_ENTITY, description = "UNPROCESSABLE_ENTITY"),
         (status = StatusCode::REQUEST_TIMEOUT, description = "REQUEST_TIMEOUT"),
         (status = StatusCode::INTERNAL_SERVER_ERROR, description = "INTERNAL_SERVER_ERROR"),
         (status = StatusCode::TOO_MANY_REQUESTS, description = "TOO_MANY_REQUESTS"),
     ),
 )]
-pub(crate) async fn inference(State(state): State<AppState>, req: Request<Body>) -> Response<Body> {
+pub(crate) async fn inference(uri: Uri, req: Request<Body>) -> Response<Body> {
     let task_manager = TaskManager::global();
+    let endpoint = uri.path();
+    let mime = match task_manager.get_mime_type(endpoint) {
+        Some(mime) => mime.as_str(),
+        None => DEFAULT_RESPONSE_MIME,
+    };
     let data = to_bytes(req.into_body()).await.unwrap();
 
     if task_manager.is_shutdown() {
         return build_response(
             StatusCode::SERVICE_UNAVAILABLE,
             Bytes::from_static(RESPONSE_SHUTDOWN),
         );
@@ -138,15 +118,15 @@
     if data.is_empty() {
         return build_response(StatusCode::OK, Bytes::from_static(RESPONSE_EMPTY));
     }
 
     let (status, content);
     let metrics = Metrics::global();
     metrics.remaining_task.inc();
-    match task_manager.submit_task(data).await {
+    match task_manager.submit_task(data, endpoint).await {
         Ok(task) => {
             content = task.data;
             status = match task.code {
                 TaskCode::Normal => {
                     // Record latency only for successful tasks
                     metrics
                         .duration
@@ -181,34 +161,35 @@
             code: status.as_u16(),
         })
         .inc();
 
     let mut resp = build_response(status, content);
     if status == StatusCode::OK {
         resp.headers_mut()
-            .insert(CONTENT_TYPE, HeaderValue::from_str(&state.mime).unwrap());
+            .insert(CONTENT_TYPE, HeaderValue::from_str(mime).unwrap());
     }
     resp
 }
 
 #[utoipa::path(
     post,
-    path = "/sse_inference",
+    path = "/openapi/reserved/inference_sse",
     responses(
         (status = StatusCode::OK, description = "Inference"),
         (status = StatusCode::BAD_REQUEST, description = "BAD_REQUEST"),
         (status = StatusCode::SERVICE_UNAVAILABLE, description = "SERVICE_UNAVAILABLE"),
         (status = StatusCode::UNPROCESSABLE_ENTITY, description = "UNPROCESSABLE_ENTITY"),
         (status = StatusCode::REQUEST_TIMEOUT, description = "REQUEST_TIMEOUT"),
         (status = StatusCode::INTERNAL_SERVER_ERROR, description = "INTERNAL_SERVER_ERROR"),
         (status = StatusCode::TOO_MANY_REQUESTS, description = "TOO_MANY_REQUESTS"),
     ),
 )]
-pub(crate) async fn sse_inference(req: Request<Body>) -> Response<BoxBody> {
+pub(crate) async fn sse_inference(uri: Uri, req: Request<Body>) -> Response<BoxBody> {
     let task_manager = TaskManager::global();
+    let endpoint = uri.path();
     let data = to_bytes(req.into_body()).await.unwrap();
 
     if task_manager.is_shutdown() {
         return (
             StatusCode::SERVICE_UNAVAILABLE,
             Bytes::from_static(RESPONSE_SHUTDOWN),
         )
@@ -216,15 +197,15 @@
     }
 
     if data.is_empty() {
         return (StatusCode::OK, Bytes::from_static(RESPONSE_EMPTY)).into_response();
     }
 
     let metrics = Metrics::global();
-    match task_manager.submit_sse_task(data).await {
+    match task_manager.submit_sse_task(data, endpoint).await {
         Ok(mut rx) => {
             let stream = async_stream::stream! {
                 while let Some((msg, code)) = rx.recv().await {
                     yield match code {
                         TaskCode::Normal => {
                             Ok(Event::default().data(String::from_utf8_lossy(&msg)))
                         },
@@ -260,9 +241,9 @@
                 .inc();
             (status, content).into_response()
         }
     }
 }
 
 #[derive(OpenApi)]
-#[openapi(paths(index, metrics, openapi_json, inference, sse_inference))]
+#[openapi(paths(index, metrics, inference, sse_inference))]
 pub(crate) struct RustAPIDoc;
```

### Comparing `mosec-0.7.2/src/tasks.rs` & `mosec-0.8.0/src/tasks.rs`

 * *Files 16% similar despite different names*

```diff
@@ -9,141 +9,229 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 use std::collections::HashMap;
+use std::path::Path;
 use std::sync::atomic::{AtomicBool, Ordering};
-use std::sync::{Mutex, RwLock};
+use std::sync::{Arc, Mutex};
 use std::time::{Duration, Instant};
 
 use bytes::Bytes;
 use hyper::StatusCode;
 use once_cell::sync::OnceCell;
-use tokio::sync::{mpsc, oneshot};
+use tokio::sync::{mpsc, oneshot, Barrier};
 use tokio::time;
 use tracing::{debug, error, info, warn};
 
+use crate::config::Config;
 use crate::errors::ServiceError;
 use crate::metrics::{CodeLabel, Metrics, DURATION_LABEL};
+use crate::protocol::communicate;
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq, derive_more::Display, derive_more::Error)]
 pub(crate) enum TaskCode {
     #[display(fmt = "200: OK")]
     Normal,
     #[display(fmt = "400: Bad Request")]
     BadRequestError,
     #[display(fmt = "422: Unprocessable Content")]
     ValidationError,
     #[display(fmt = "408: Request Timeout")]
     TimeoutError,
     #[display(fmt = "500: Internal Server Error")]
     InternalError,
     // special case
-    #[display(fmt = "500: Internal Server Error")]
+    #[display(fmt = "200: Server Sent Event")]
     StreamEvent,
 }
 
 #[derive(Debug, Clone)]
 pub(crate) struct Task {
     pub(crate) code: TaskCode,
     pub(crate) data: Bytes,
+    pub(crate) stage: usize,
+    pub(crate) route: String,
     pub(crate) create_at: Instant,
 }
 
 impl Task {
-    fn new(data: Bytes) -> Self {
+    fn new(data: Bytes, route: String) -> Self {
         Self {
             code: TaskCode::InternalError,
             data,
+            stage: 0,
+            route,
             create_at: Instant::now(),
         }
     }
 
     fn update(&mut self, code: TaskCode, data: &Bytes) {
         self.code = code;
         self.data = data.clone();
+        self.stage += 1;
+    }
+
+    /// Encode the current state of the task into a 16-bit integer.
+    /// 0000 0000 0000 00yx
+    /// x: is ingress
+    /// y: is egress
+    fn encode_state(&self, total: usize) -> u16 {
+        let mut state = 0;
+        state |= (self.stage == 0) as u16;
+        state |= ((total - 1 == self.stage) as u16) << 1;
+        state
     }
 }
 
 #[derive(Debug)]
 pub(crate) struct TaskManager {
-    table: RwLock<HashMap<u32, Task>>,
+    table: Mutex<HashMap<u32, Task>>,
     notifiers: Mutex<HashMap<u32, oneshot::Sender<()>>>,
     stream_senders: Mutex<HashMap<u32, mpsc::Sender<(Bytes, TaskCode)>>>,
     timeout: Duration,
     current_id: Mutex<u32>,
-    channel: async_channel::Sender<u32>,
+    senders: HashMap<String, Vec<async_channel::Sender<u32>>>,
+    mime_types: HashMap<String, String>,
     shutdown: AtomicBool,
 }
 
 pub(crate) static TASK_MANAGER: OnceCell<TaskManager> = OnceCell::new();
 
 impl TaskManager {
     pub(crate) fn global() -> &'static TaskManager {
         TASK_MANAGER.get().expect("task manager is not initialized")
     }
 
-    pub(crate) fn new(timeout: Duration, channel: async_channel::Sender<u32>) -> Self {
+    pub(crate) fn new(timeout: u64) -> Self {
         Self {
-            table: RwLock::new(HashMap::new()),
+            table: Mutex::new(HashMap::new()),
             notifiers: Mutex::new(HashMap::new()),
             stream_senders: Mutex::new(HashMap::new()),
-            timeout,
+            timeout: Duration::from_millis(timeout),
             current_id: Mutex::new(0),
-            channel,
+            senders: HashMap::new(),
+            mime_types: HashMap::new(),
             shutdown: AtomicBool::new(false),
         }
     }
 
+    pub(crate) fn init_from_config(&mut self, conf: &Config) -> Arc<Barrier> {
+        let barrier = Arc::new(Barrier::new(conf.runtimes.len() + 1));
+
+        let mut worker_channel =
+            HashMap::<String, (async_channel::Receiver<u32>, async_channel::Sender<u32>)>::new();
+        let dir = Path::new(&conf.path);
+
+        // run the coordinator in different threads
+        for runtime in &conf.runtimes {
+            let (tx, rx) = async_channel::bounded::<u32>(conf.capacity);
+            worker_channel.insert(runtime.worker.clone(), (rx.clone(), tx));
+            let path = dir.join(format!("ipc_{}.socket", runtime.worker));
+            tokio::spawn(communicate(
+                path,
+                runtime.max_batch_size,
+                Duration::from_millis(runtime.max_wait_time),
+                runtime.worker.clone(),
+                rx,
+                barrier.clone(),
+            ));
+        }
+
+        for route in &conf.routes {
+            self.mime_types
+                .insert(route.endpoint.clone(), route.mime.clone());
+            let worker_senders = route
+                .workers
+                .iter()
+                .map(|w| worker_channel[w].1.clone())
+                .collect();
+            self.senders.insert(route.endpoint.clone(), worker_senders);
+        }
+
+        barrier
+    }
+
+    pub(crate) fn get_mime_type(&self, endpoint: &str) -> Option<&String> {
+        self.mime_types.get(endpoint)
+    }
+
+    pub(crate) async fn send_task(&self, id: &u32) {
+        let stage: usize;
+        let route: &Vec<async_channel::Sender<u32>>;
+        {
+            let table = self.table.lock().unwrap();
+            match table.get(id) {
+                Some(task) => {
+                    stage = task.stage;
+                    route = &self.senders[&task.route];
+                }
+                None => {
+                    warn!(%id, "failed to get the task when trying to send it");
+                    return;
+                }
+            };
+        }
+        if stage >= route.len() {
+            self.notify_task_done(id);
+            return;
+        }
+        if route[stage].send(*id).await.is_err() {
+            warn!(%id, "failed to send this task, the sender might be closed");
+        }
+    }
+
     pub(crate) async fn shutdown(&self) {
         self.shutdown.store(true, Ordering::Release);
         let fut = time::timeout(self.timeout, async {
             let mut interval = time::interval(Duration::from_millis(100));
             let mut retry = 0;
             loop {
                 interval.tick().await;
-                let remaining_task_num = self.table.read().unwrap().len();
+                let remaining_task_num = self.table.lock().unwrap().len();
                 if remaining_task_num == 0 {
                     break;
                 }
                 retry += 1;
                 if (retry % 10) == 0 {
                     info!(%remaining_task_num, "waiting for remaining tasks to complete");
                 }
             }
         });
         if fut.await.is_err() {
             error!("service task manager shutdown timeout");
         }
     }
 
-    pub(crate) async fn submit_task(&self, data: Bytes) -> Result<Task, ServiceError> {
-        let (id, rx) = self.add_new_task(data)?;
+    pub(crate) async fn submit_task(&self, data: Bytes, key: &str) -> Result<Task, ServiceError> {
+        let (id, rx) = self.add_new_task(data, key)?;
         if let Err(err) = time::timeout(self.timeout, rx).await {
-            warn!(%id, %err, "task was not completed in the expected time");
+            warn!(%id, %err, "task was not completed in the expected time, if this happens a lot, \
+                you might want to increase the service timeout");
             self.delete_task(id, false);
             return Err(ServiceError::Timeout);
         }
-        let mut table = self.table.write().unwrap();
+        let mut table = self.table.lock().unwrap();
         match table.remove(&id) {
             Some(task) => Ok(task),
             None => {
                 error!(%id, "cannot find the task when trying to remove it");
                 Err(ServiceError::UnknownError)
             }
         }
     }
 
     pub(crate) async fn submit_sse_task(
         &self,
         data: Bytes,
+        key: &str,
     ) -> Result<mpsc::Receiver<(Bytes, TaskCode)>, ServiceError> {
-        let (id, rx) = self.add_new_task(data)?;
+        let (id, rx) = self.add_new_task(data, key)?;
         let (sender, receiver) = mpsc::channel(16);
 
         {
             let mut stream_senders = self.stream_senders.lock().unwrap();
             stream_senders.insert(id, sender);
         }
         let metrics = Metrics::global();
@@ -161,107 +249,114 @@
     pub(crate) fn delete_task(&self, id: u32, has_stream: bool) -> Option<Task> {
         let task;
         {
             let mut notifiers = self.notifiers.lock().unwrap();
             notifiers.remove(&id);
         }
         {
-            let mut table = self.table.write().unwrap();
+            let mut table = self.table.lock().unwrap();
             task = table.remove(&id);
         }
         if has_stream {
             let mut stream_senders = self.stream_senders.lock().unwrap();
             stream_senders.remove(&id);
         }
         task
     }
 
     pub(crate) fn is_shutdown(&self) -> bool {
         self.shutdown.load(Ordering::Acquire)
     }
 
-    fn add_new_task(&self, data: Bytes) -> Result<(u32, oneshot::Receiver<()>), ServiceError> {
+    fn add_new_task(
+        &self,
+        data: Bytes,
+        key: &str,
+    ) -> Result<(u32, oneshot::Receiver<()>), ServiceError> {
         let (tx, rx) = oneshot::channel();
         let id: u32;
         {
             let mut current_id = self.current_id.lock().unwrap();
             id = *current_id;
             *current_id = id.wrapping_add(1);
         }
         {
             let mut notifiers = self.notifiers.lock().unwrap();
             notifiers.insert(id, tx);
         }
         {
-            let mut table = self.table.write().unwrap();
-            table.insert(id, Task::new(data));
+            let mut table = self.table.lock().unwrap();
+            table.insert(id, Task::new(data, key.to_string()));
         }
         debug!(%id, "add a new task");
 
-        if self.channel.try_send(id).is_err() {
+        if self.senders[key][0].try_send(id).is_err() {
             warn!(%id, "reach the capacity limit, will delete this task");
             self.delete_task(id, false);
             return Err(ServiceError::TooManyRequests);
         }
         Ok((id, rx))
     }
 
-    pub(crate) fn notify_task_done(&self, id: u32) {
+    pub(crate) fn notify_task_done(&self, id: &u32) {
         let res;
         {
             let mut notifiers = self.notifiers.lock().unwrap();
-            res = notifiers.remove(&id);
+            res = notifiers.remove(id);
         }
         if let Some(sender) = res {
             if !sender.is_closed() {
                 sender.send(()).unwrap();
             } else {
                 warn!(%id, "the task notifier is already closed, will delete it \
                     (this is usually because the client side has closed the connection)");
                 {
-                    let mut table = self.table.write().unwrap();
-                    table.remove(&id);
+                    let mut table = self.table.lock().unwrap();
+                    table.remove(id);
                 }
                 let metrics = Metrics::global();
                 metrics.remaining_task.dec();
             }
         } else {
             // if the task is already timeout, the notifier may be removed by another thread
             info!(%id, "cannot find the task notifier, maybe this task has expired");
         }
     }
 
-    pub(crate) fn get_multi_tasks_data(&self, ids: &mut Vec<u32>, data: &mut Vec<Bytes>) {
-        let table = self.table.read().unwrap();
+    pub(crate) fn get_multi_tasks_data(
+        &self,
+        ids: &mut Vec<u32>,
+        data: &mut Vec<Bytes>,
+        states: &mut Vec<u16>,
+    ) {
+        let table = self.table.lock().unwrap();
         // delete the task_id if the task_id doesn't exist in the table
         ids.retain(|&id| match table.get(&id) {
             Some(task) => {
                 data.push(task.data.clone());
+                states.push(task.encode_state(self.senders[&task.route].len()));
                 true
             }
             None => false,
         });
     }
 
     pub(crate) async fn update_multi_tasks(&self, code: TaskCode, ids: &[u32], data: &[Bytes]) {
         let mut abnormal_tasks = Vec::new();
         {
             // make sure the table lock is released since the next func call may need to acquire
             // the notifiers lock, we'd better only hold one lock at a time
-            let mut table = self.table.write().unwrap();
+            let mut table = self.table.lock().unwrap();
             for i in 0..ids.len() {
                 let task = table.get_mut(&ids[i]);
                 match task {
                     Some(task) => {
                         task.update(code, &data[i]);
-                        match code {
-                            TaskCode::Normal => {}
-                            _ => {
-                                abnormal_tasks.push(ids[i]);
-                            }
+                        if code != TaskCode::Normal {
+                            abnormal_tasks.push(ids[i]);
                         }
                     }
                     None => {
                         // if the task is already timeout, it may be removed by another thread
                         info!(id=%ids[i], "cannot find this task, maybe it has expired");
                     }
                 }
@@ -274,15 +369,15 @@
                     if let Err(err) = sender.send((data[i].clone(), code)).await {
                         info!(%err, task_id=abnormal_tasks[i], "failed to send stream event");
                     }
                     debug!(%code, task_id=abnormal_tasks[i], "sent abnormal task event to the channel");
                 }
             }
         }
-        for task_id in abnormal_tasks {
+        for task_id in &abnormal_tasks {
             self.notify_task_done(task_id);
         }
     }
 }
 
 async fn wait_sse_finish(id: u32, timeout: Duration, notifier: oneshot::Receiver<()>) {
     let task_manager = TaskManager::global();
@@ -307,131 +402,153 @@
         .inc();
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
+    const DEFAULT_ENDPOINT: &str = "/inference";
+
     #[test]
     fn create_and_update_task() {
         let now = Instant::now();
-        let mut task = Task::new(Bytes::from_static(b"hello"));
+        let mut task = Task::new(Bytes::from_static(b"hello"), "".to_string());
         assert!(task.create_at > now);
         assert!(task.create_at < Instant::now());
         assert!(matches!(task.code, TaskCode::InternalError));
         assert_eq!(task.data, Bytes::from_static(b"hello"));
 
         task.update(TaskCode::Normal, &Bytes::from_static(b"world"));
         assert!(matches!(task.code, TaskCode::Normal));
         assert_eq!(task.data, Bytes::from_static(b"world"));
     }
 
     #[tokio::test]
     async fn task_manager_add_new_task() {
-        let (tx, rx) = async_channel::bounded(1);
-        let task_manager = TaskManager::new(Duration::from_secs(1), tx);
+        let mut task_manager = TaskManager::new(1000);
+        task_manager.init_from_config(&Config::default());
         let (id, _rx) = task_manager
-            .add_new_task(Bytes::from_static(b"hello"))
+            .add_new_task(Bytes::from_static(b"hello"), DEFAULT_ENDPOINT)
             .unwrap();
         assert_eq!(id, 0);
         {
-            let table = task_manager.table.read().unwrap();
+            let table = task_manager.table.lock().unwrap();
             let task = table.get(&id).unwrap();
             assert_eq!(task.data, Bytes::from_static(b"hello"));
         }
-        let recv_id = rx.recv().await.unwrap();
-        assert_eq!(recv_id, id);
 
         // add a new task
         let (id, _rx) = task_manager
-            .add_new_task(Bytes::from_static(b"world"))
+            .add_new_task(Bytes::from_static(b"world"), DEFAULT_ENDPOINT)
             .unwrap();
         assert_eq!(id, 1);
         {
-            let table = task_manager.table.read().unwrap();
+            let table = task_manager.table.lock().unwrap();
             let task = table.get(&id).unwrap();
             assert_eq!(task.data, Bytes::from_static(b"world"));
         }
-        let recv_id = rx.recv().await.unwrap();
-        assert_eq!(recv_id, id);
     }
 
     #[tokio::test]
     async fn task_manager_timeout() {
-        let (tx, _rx) = async_channel::bounded(1);
-        let task_manager = TaskManager::new(Duration::from_millis(1), tx);
+        let mut task_manager = TaskManager::new(1);
+        task_manager.init_from_config(&Config::default());
 
         // wait until this task timeout
-        let res = task_manager.submit_task(Bytes::from_static(b"hello")).await;
+        let res = task_manager
+            .submit_task(Bytes::from_static(b"hello"), DEFAULT_ENDPOINT)
+            .await;
         assert!(matches!(res.unwrap_err(), ServiceError::Timeout));
     }
 
     #[tokio::test]
     async fn task_manager_too_many_request() {
-        let (tx, _rx) = async_channel::bounded(1);
-        // push one task into the channel to make the channel full
-        let _ = tx.send(0u32).await;
-        let task_manager = TaskManager::new(Duration::from_millis(1), tx);
+        let mut task_manager = TaskManager::new(1);
+        let mut config = Config::default();
+        // capacity > 0
+        config.capacity = 1;
+        task_manager.init_from_config(&config);
+        // send one task id to block the channel
+        task_manager.senders[DEFAULT_ENDPOINT][0]
+            .send(0)
+            .await
+            .unwrap();
 
-        // trigger too many request since the capacity is 0
-        let res = task_manager.submit_task(Bytes::from_static(b"hello")).await;
+        // trigger too many request since the capacity is 1
+        let res = task_manager
+            .submit_task(Bytes::from_static(b"hello"), DEFAULT_ENDPOINT)
+            .await;
         assert!(matches!(res.unwrap_err(), ServiceError::TooManyRequests));
     }
 
     #[tokio::test]
     async fn task_manager_graceful_shutdown() {
-        let (tx, _rx) = async_channel::bounded(1);
-        let task_manager = TaskManager::new(Duration::from_millis(1), tx);
+        let mut task_manager = TaskManager::new(1);
+        task_manager.init_from_config(&Config::default());
         assert!(!task_manager.is_shutdown());
         task_manager.shutdown().await;
         assert!(task_manager.is_shutdown());
+    }
 
-        let (tx, _rx) = async_channel::bounded(1);
-        let task_manager = TaskManager::new(Duration::from_millis(10), tx);
+    #[tokio::test]
+    async fn task_manager_graceful_shutdown_after_timeout() {
+        let mut task_manager = TaskManager::new(10);
+        task_manager.init_from_config(&Config::default());
         {
             // block with one task in the channel
-            let mut table = task_manager.table.write().unwrap();
-            table.insert(0u32, Task::new(Bytes::from_static(b"hello")));
+            let mut table = task_manager.table.lock().unwrap();
+            table.insert(
+                0u32,
+                Task::new(Bytes::from_static(b"hello"), DEFAULT_ENDPOINT.to_string()),
+            );
         }
         assert!(!task_manager.is_shutdown());
         let now = Instant::now();
         task_manager.shutdown().await;
         assert!(task_manager.is_shutdown());
         // force shutdown after a timeout duration
         assert!(now.elapsed() >= Duration::from_millis(10));
     }
 
     #[tokio::test]
     async fn task_manager_get_and_update_task() {
-        let (tx, _rx) = async_channel::bounded(1);
-        let task_manager = TaskManager::new(Duration::from_millis(1), tx);
+        let mut task_manager = TaskManager::new(1);
+        task_manager.init_from_config(&Config::default());
 
         // add some tasks to the table
         {
-            let mut table = task_manager.table.write().unwrap();
-            table.insert(0, Task::new(Bytes::from_static(b"hello")));
-            table.insert(1, Task::new(Bytes::from_static(b"world")));
+            let mut table = task_manager.table.lock().unwrap();
+            table.insert(
+                0,
+                Task::new(Bytes::from_static(b"hello"), DEFAULT_ENDPOINT.to_string()),
+            );
+            table.insert(
+                1,
+                Task::new(Bytes::from_static(b"world"), DEFAULT_ENDPOINT.to_string()),
+            );
         }
 
         let mut task_ids = vec![0, 1, 2];
         let mut data = Vec::new();
-        task_manager.get_multi_tasks_data(&mut task_ids, &mut data);
+        let mut states = Vec::new();
+        task_manager.get_multi_tasks_data(&mut task_ids, &mut data, &mut states);
         assert_eq!(task_ids, vec![0, 1]);
         assert_eq!(
             data,
             vec![Bytes::from_static(b"hello"), Bytes::from_static(b"world")]
         );
+        assert_eq!(states, vec![3 as u16, 3 as u16]);
 
         // update tasks
         data = vec![Bytes::from_static(b"rust"), Bytes::from_static(b"tokio")];
         task_manager
             .update_multi_tasks(TaskCode::Normal, &task_ids, &data)
             .await;
         let mut new_data = Vec::new();
-        task_manager.get_multi_tasks_data(&mut task_ids, &mut new_data);
+        task_manager.get_multi_tasks_data(&mut task_ids, &mut new_data, &mut states);
         assert_eq!(task_ids, vec![0, 1]);
         assert_eq!(
             new_data,
             vec![Bytes::from_static(b"rust"), Bytes::from_static(b"tokio")]
         );
     }
 }
```

