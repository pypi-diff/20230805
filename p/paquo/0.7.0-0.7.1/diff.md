# Comparing `tmp/paquo-0.7.0.tar.gz` & `tmp/paquo-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paquo-0.7.0.tar", last modified: Sun Jul 16 19:25:50 2023, max compression
+gzip compressed data, was "paquo-0.7.1.tar", last modified: Sat Aug  5 15:55:06 2023, max compression
```

## Comparing `paquo-0.7.0.tar` & `paquo-0.7.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-16 19:25:43.000000 paquo-0.7.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-16 19:25:43.000000 paquo-0.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-16 19:25:43.000000 paquo-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-16 19:25:43.000000 paquo-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 19:25:43.000000 paquo-0.7.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-16 19:25:43.000000 paquo-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 19:25:43.000000 paquo-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-16 19:25:43.000000 paquo-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-16 19:25:50.647502 paquo-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-16 19:25:43.000000 paquo-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.639502 paquo-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   308228 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/_static/screenshot_example_05.png
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-16 19:25:43.000000 paquo-0.7.0/environment.devenv.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_01_read_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_02_add_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_03_project_with_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_04_project_with_image_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_05_draw_tiles_on_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/prepare_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-16 19:25:43.000000 paquo-0.7.0/extras/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/extras/osx_app_shim/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 19:25:43.000000 paquo-0.7.0/extras/osx_app_shim/PaquoOpenQpZip.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-16 19:25:43.000000 paquo-0.7.0/extras/osx_app_shim/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/paquo/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/.paquo.defaults.toml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/java.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/jpype_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/pathobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/paquo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_jpype_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_pathobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/paquo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-16 19:25:43.000000 paquo-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-16 19:25:50.651502 paquo-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.187695 paquo-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 15:54:54.000000 paquo-0.7.1/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-05 15:54:54.000000 paquo-0.7.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-05 15:54:54.000000 paquo-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-08-05 15:54:54.000000 paquo-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-05 15:54:54.000000 paquo-0.7.1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-05 15:54:54.000000 paquo-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 15:54:54.000000 paquo-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-05 15:54:54.000000 paquo-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-08-05 15:55:06.187695 paquo-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-05 15:54:54.000000 paquo-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.179695 paquo-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.179695 paquo-0.7.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.179695 paquo-0.7.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   308228 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/source/_static/screenshot_example_05.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-08-05 15:54:54.000000 paquo-0.7.1/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-05 15:54:54.000000 paquo-0.7.1/environment.devenv.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.179695 paquo-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-05 15:54:54.000000 paquo-0.7.1/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-05 15:54:54.000000 paquo-0.7.1/examples/example_01_read_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-05 15:54:54.000000 paquo-0.7.1/examples/example_02_add_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-05 15:54:54.000000 paquo-0.7.1/examples/example_03_project_with_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-05 15:54:54.000000 paquo-0.7.1/examples/example_04_project_with_image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-05 15:54:54.000000 paquo-0.7.1/examples/example_05_draw_tiles_on_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-05 15:54:54.000000 paquo-0.7.1/examples/prepare_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.179695 paquo-0.7.1/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-05 15:54:54.000000 paquo-0.7.1/extras/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.183695 paquo-0.7.1/extras/osx_app_shim/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-05 15:54:54.000000 paquo-0.7.1/extras/osx_app_shim/PaquoOpenQpZip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-05 15:54:54.000000 paquo-0.7.1/extras/osx_app_shim/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.183695 paquo-0.7.1/paquo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/.paquo.defaults.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-05 15:55:06.000000 paquo-0.7.1/paquo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27229 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/jpype_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/pathobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.187695 paquo-0.7.1/paquo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_jpype_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_pathobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-05 15:54:54.000000 paquo-0.7.1/paquo/tests/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:55:06.183695 paquo-0.7.1/paquo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-08-05 15:55:06.000000 paquo-0.7.1/paquo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-05 15:55:06.000000 paquo-0.7.1/paquo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 15:55:06.000000 paquo-0.7.1/paquo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 15:55:06.000000 paquo-0.7.1/paquo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-05 15:55:06.000000 paquo-0.7.1/paquo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 15:55:06.000000 paquo-0.7.1/paquo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-05 15:54:54.000000 paquo-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-05 15:55:06.187695 paquo-0.7.1/setup.cfg
```

### Comparing `paquo-0.7.0/.pre-commit-config.yaml` & `paquo-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/CHANGELOG.md` & `paquo-0.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-...
+
+## [0.7.1] - 2023-08-05
+### Fixed
+- prevent warning in ome conversion with pydantic>=2
+- speedup hierarchy loading in readonly mode
+- fix import of geojson tile objects
 
 ## [0.7.0] - 2023-06-16
 ### Changed
 - drop Python=3.7 support
 
 ### Added
 - paquo: support for newer ome-types
@@ -137,15 +142,16 @@
 - `QuPathProject.add_image` is now calling `QuPathProject.save`
 
 ## [0.1.0] - 2020-08-12
 ### Added
 - initial release of paquo
 
 
-[Unreleased]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.0...HEAD
+[Unreleased]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.1...HEAD
+[0.7.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.6.1...v0.7.0
 [0.6.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.6.0...v0.6.1
 [0.6.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.5.0...v0.5.1
 [0.5.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.4.2...v0.5.0
 [0.4.2]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.4.1...v0.4.2
 [0.4.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.4.0...v0.4.1
```

### Comparing `paquo-0.7.0/CONTRIBUTING.md` & `paquo-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/LICENSE` & `paquo-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/PKG-INFO` & `paquo-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paquo
-Version: 0.7.0
+Version: 0.7.1
 Summary: library for interacting with QuPath
 Home-page: https://github.com/bayer-science-for-a-better-life/paquo
 Download-URL: https://github.com/bayer-science-for-a-better-life/paquo
 Author: Santiago Villalba, Andreas Poehlmann
 Author-email: santiago.villalba@bayer.com, andreas.poehlmann@bayer.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paquo-0.7.0/README.md` & `paquo-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/Makefile` & `paquo-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/source/_static/screenshot_example_05.png` & `paquo-0.7.1/docs/source/_static/screenshot_example_05.png`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/source/api.rst` & `paquo-0.7.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/source/conf.py` & `paquo-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/source/configuration.rst` & `paquo-0.7.1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/source/index.rst` & `paquo-0.7.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/source/installation.rst` & `paquo-0.7.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/docs/source/quickstart.rst` & `paquo-0.7.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/environment.devenv.yml` & `paquo-0.7.1/environment.devenv.yml`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/examples/README.md` & `paquo-0.7.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/examples/example_01_read_annotations.py` & `paquo-0.7.1/examples/example_01_read_annotations.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/examples/example_02_add_annotations.py` & `paquo-0.7.1/examples/example_02_add_annotations.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/examples/example_03_project_with_classes.py` & `paquo-0.7.1/examples/example_03_project_with_classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/examples/example_04_project_with_image_metadata.py` & `paquo-0.7.1/examples/example_04_project_with_image_metadata.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/examples/example_05_draw_tiles_on_image.py` & `paquo-0.7.1/examples/example_05_draw_tiles_on_image.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/examples/prepare_resources.py` & `paquo-0.7.1/examples/prepare_resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,22 +24,17 @@
 def download_image(copies=1):
     """download the smallest aperio test image svs"""
     # openslide aperio test image
     images_base_url = "http://openslide.cs.cmu.edu/download/openslide-testdata/Aperio/"
     small_image = "CMU-1-Small-Region.svs"
     # download svs from openslide test images
     url = images_base_url + small_image
-    with urllib.request.urlopen(url) as response:  # nosec B310
-        buffer = io.BytesIO(response.read())
-        for idx in range(copies):
-            img_fn = IMAGES_DIR / f"image_{idx}.svs"
-            with open(img_fn, 'wb') as out_file:
-                shutil.copyfileobj(buffer, out_file)
-                yield img_fn
-            buffer.seek(0)
+    for idx in range(copies):
+        img_fn = IMAGES_DIR / f"image_{idx}.svs"
+        yield img_fn
 
 
 def prepare_example_resources():
     """build an example project"""
     from paquo.projects import QuPathProject
     from paquo.images import QuPathImageType
     from paquo.classes import QuPathPathClass
```

### Comparing `paquo-0.7.0/extras/README.md` & `paquo-0.7.1/extras/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/.paquo.defaults.toml` & `paquo-0.7.1/paquo/.paquo.defaults.toml`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/__main__.py` & `paquo-0.7.1/paquo/__main__.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/_cli.py` & `paquo-0.7.1/paquo/_cli.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/_config.py` & `paquo-0.7.1/paquo/_config.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/_logging.py` & `paquo-0.7.1/paquo/_logging.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/_repr.py` & `paquo-0.7.1/paquo/_repr.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/_utils.py` & `paquo-0.7.1/paquo/_utils.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/classes.py` & `paquo-0.7.1/paquo/classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/colors.py` & `paquo-0.7.1/paquo/colors.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/hierarchy.py` & `paquo-0.7.1/paquo/hierarchy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import collections
 import json
 import math
 import reprlib
 import struct
+import warnings
 from contextlib import contextmanager
 from contextlib import suppress
 from typing import Any
 from typing import Counter as CounterType
 from typing import Iterable
 from typing import Iterator
 from typing import MutableSet
@@ -17,15 +18,19 @@
 from typing import overload
 
 from paquo._logging import get_logger
 from paquo._utils import cached_property
 from paquo.classes import QuPathPathClass
 from paquo.java import GsonTools
 from paquo.java import IllegalArgumentException
+from paquo.java import PathAnnotationObject
+from paquo.java import PathDetectionObject
 from paquo.java import PathObjectHierarchy
+from paquo.java import PathTileObject
+from paquo.java import String
 from paquo.java import compatibility
 from paquo.pathobjects import BaseGeometry
 from paquo.pathobjects import PathROIObjectType
 from paquo.pathobjects import QuPathPathAnnotationObject
 from paquo.pathobjects import QuPathPathDetectionObject
 from paquo.pathobjects import QuPathPathTileObject
 from paquo.pathobjects import fix_geojson_geometry
@@ -394,54 +399,77 @@
         """
         # todo: use geojson module for type checking?
         if self._readonly:
             raise OSError("project in readonly mode")
         if not isinstance(geojson, list):
             raise TypeError("requires a geojson list")
 
+        requires_annotation_json_fix = compatibility.requires_annotation_json_fix()
+
         aos = []
         skipped: "CounterType[str]" = collections.Counter()
         for annotation in geojson:
             try:
                 if fix_invalid:
                     annotation["geometry"] = fix_geojson_geometry(annotation["geometry"])
 
+                properties = annotation["properties"]
+                if "objectType" in properties:
+                    # https://github.com/qupath/qupath/pull/1099
+                    object_type = properties["objectType"]
+                elif "object_type" in properties:
+                    object_type = properties["object_type"]
+                else:
+                    object_type = "unknown"
+
                 # compatibility layer
-                # todo: should maybe test at the beginning of this method
-                #   if the version supports id or not, instead of checking
-                #   the version number...
                 if (
-                    compatibility.requires_annotation_json_fix()
+                    requires_annotation_json_fix
                     and 'id' not in annotation
                 ):
-                    object_type = annotation['properties'].get("object_type", "unknown")
                     object_id = {
                         'annotation': "PathAnnotationObject",
                         'detection': "PathDetectionObject",
                         'tile': "PathTileObject",
                         'cell': "PathCellObject",
                         'tma_core': "TMACoreObject",
+                        'tmaCore': "TMACoreObject",  # https://github.com/qupath/qupath/pull/1099
                         'root': "PathRootObject",
                         'unknown': "PathAnnotationObject",
                     }.get(object_type, None)
                     if object_id is None:
                         _logger.warn(f"annotation has incompatible object_type: '{object_type}'")
                         object_id = "PathAnnotationObject"
                     annotation['id'] = object_id
 
-                ao = QuPathPathAnnotationObject.from_geojson(annotation)
+                gson = GsonTools.getInstance()
+                if object_type == "annotation":
+                    java_obj = gson.fromJson(String(json.dumps(annotation)), PathAnnotationObject)
+                elif object_type == "detection":
+                    java_obj = gson.fromJson(String(json.dumps(annotation)), PathDetectionObject)
+                elif object_type == "tile":
+                    java_obj = gson.fromJson(String(json.dumps(annotation)), PathTileObject)
+                else:
+                    if object_type != "unknown":
+                        warnings.warn(
+                            f"Trying to load annotation object_type={object_type!r}. "
+                            "Please report this on the paquo issue tracker on github and provide a geojson example. "
+                            "https://github.com/Bayer-Group/paquo/issues",
+                            stacklevel=2,
+                        )
+                    java_obj = gson.fromJson(String(json.dumps(annotation)), PathAnnotationObject)
 
             except (IllegalArgumentException, ValueError) as err:
                 _logger.warn(f"Annotation skipped: {err}")
                 class_ = annotation["properties"].get("classification", {}).get("name", "UNDEFINED")
                 skipped[class_] += 1
                 continue
 
             else:
-                aos.append(ao.java_object)
+                aos.append(java_obj)
 
         if skipped:
             n_skipped = sum(skipped.values())
             if raise_on_skip:
                 raise ValueError(f"could not convert {n_skipped} annotations")
             _logger.error(
                 f"skipped {n_skipped} annotation objects: {skipped.most_common()}"
@@ -506,15 +534,15 @@
             if class_name:
                 _m[f"{prefix}:path_class"] = class_name
             if ao.name:
                 _m[f"{prefix}:name"] = ao.name
             for k, v in ao.measurements.items():
                 _m[f"{prefix}:measurement:{k}"] = v
 
-            if "ms" in Map.__fields__:
+            if "ms" in Map.__annotations__:
                 map_annotation = MapAnnotation(  # type: ignore
                     value=Map(
                         ms=[
                             M(k=_key, value=str(_value))
                             for _key, _value in _m.items()
                         ]
                     )
```

### Comparing `paquo-0.7.0/paquo/images.py` & `paquo-0.7.1/paquo/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,19 +582,22 @@
             raise AttributeError("project in readonly mode")
         self._properties.clear()
         self._properties.update(value)
 
     @cached_property
     def hierarchy(self) -> QuPathPathObjectHierarchy:
         """the image entry hierarchy. it contains all annotations"""
-        try:
-            h = self._image_data.getHierarchy()
-        except OSError:
-            _log.warning("could not open image data. loading annotation hierarchy from project.")
+        if self._readonly:
             h = self.java_object.readHierarchy()
+        else:
+            try:
+                h = self._image_data.getHierarchy()
+            except OSError:
+                _log.warning("could not open image data. loading annotation hierarchy from project.")
+                h = self.java_object.readHierarchy()
 
         return QuPathPathObjectHierarchy(h, readonly=self._readonly, image_name=self.image_name)
 
     def __repr__(self):
         return f"ImageEntry(image_name='{self.image_name}')"
 
     def _repr_html_(self, compact=False, index=0):
```

### Comparing `paquo-0.7.0/paquo/java.py` & `paquo-0.7.1/paquo/java.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/jpype_backend.py` & `paquo-0.7.1/paquo/jpype_backend.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/pathobjects.py` & `paquo-0.7.1/paquo/pathobjects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/projects.py` & `paquo-0.7.1/paquo/projects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/conftest.py` & `paquo-0.7.1/paquo/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_classes.py` & `paquo-0.7.1/paquo/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_colors.py` & `paquo-0.7.1/paquo/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_config.py` & `paquo-0.7.1/paquo/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_hierarchy.py` & `paquo-0.7.1/paquo/tests/test_hierarchy.py`

 * *Files 9% similar despite different names*

```diff
@@ -392,7 +392,42 @@
 
 def test_serialize_to_ome(project_with_annotations):
     pytest.importorskip("ome_types")
     xml = project_with_annotations.images[0].hierarchy.to_ome_xml()
 
     assert xml.startswith("<OME")
     assert xml.strip().endswith("</OME>")
+
+
+TEST_ANNOTATION_OBJECT_TYPE_TILE = {
+    "features": [
+        {
+            "geometry": {
+                "coordinates": [
+                    [
+                        [0, 23904],
+                        [350, 23904],
+                        [350, 24254],
+                        [0, 24254],
+                        [0, 23904],
+                    ]
+                ],
+                "type": "Polygon"
+            },
+            "properties": {
+                "isLocked": True,
+                "measurements": {
+                    "prob_notumor": 0.9998319149017334,
+                    "prob_tumor": 0.00016804548795334995
+                },
+                "objectType": "tile"
+            },
+            "type": "Feature"
+        }
+    ],
+    "type": "FeatureCollection"
+}
+
+
+def test_load_object_type_tile_geojson(empty_hierarchy):
+    geojson = deepcopy(TEST_ANNOTATION_OBJECT_TYPE_TILE)["features"]
+    empty_hierarchy.load_geojson(geojson)
```

### Comparing `paquo-0.7.0/paquo/tests/test_images.py` & `paquo-0.7.1/paquo/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_jpype_backend.py` & `paquo-0.7.1/paquo/tests/test_jpype_backend.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_main.py` & `paquo-0.7.1/paquo/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_pathobjects.py` & `paquo-0.7.1/paquo/tests/test_pathobjects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_projects.py` & `paquo-0.7.1/paquo/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_readonly.py` & `paquo-0.7.1/paquo/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo/tests/test_repr.py` & `paquo-0.7.1/paquo/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/paquo.egg-info/PKG-INFO` & `paquo-0.7.1/paquo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paquo
-Version: 0.7.0
+Version: 0.7.1
 Summary: library for interacting with QuPath
 Home-page: https://github.com/bayer-science-for-a-better-life/paquo
 Download-URL: https://github.com/bayer-science-for-a-better-life/paquo
 Author: Santiago Villalba, Andreas Poehlmann
 Author-email: santiago.villalba@bayer.com, andreas.poehlmann@bayer.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paquo-0.7.0/paquo.egg-info/SOURCES.txt` & `paquo-0.7.1/paquo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/pyproject.toml` & `paquo-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `paquo-0.7.0/setup.cfg` & `paquo-0.7.1/setup.cfg`

 * *Files identical despite different names*

