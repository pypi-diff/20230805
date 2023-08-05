# Comparing `tmp/swcgeom-0.8.0.tar.gz` & `tmp/swcgeom-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swcgeom-0.8.0.tar", last modified: Tue Apr 18 15:00:56 2023, max compression
+gzip compressed data, was "swcgeom-0.9.0.tar", last modified: Thu May  4 03:36:14 2023, max compression
```

## Comparing `swcgeom-0.8.0.tar` & `swcgeom-0.9.0.tar`

### file list

```diff
@@ -1,96 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.474729 swcgeom-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.458728 swcgeom-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.462728 swcgeom-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-18 15:00:43.000000 swcgeom-0.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-18 15:00:43.000000 swcgeom-0.8.0/.github/workflows/github-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-18 15:00:43.000000 swcgeom-0.8.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-18 15:00:43.000000 swcgeom-0.8.0/.github/workflows/test-pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-18 15:00:43.000000 swcgeom-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-04-18 15:00:43.000000 swcgeom-0.8.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.462728 swcgeom-0.8.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-18 15:00:43.000000 swcgeom-0.8.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-04-18 15:00:43.000000 swcgeom-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-18 15:00:43.000000 swcgeom-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-18 15:00:56.474729 swcgeom-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-18 15:00:43.000000 swcgeom-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.462728 swcgeom-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    56312 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/Branch.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59312 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/BranchTree.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/CollectTips.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   166229 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/CutTree.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   154485 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/Features.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/ImageStack.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   149381 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/MST.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   305302 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/SpectralClustering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   403664 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/Tree.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.466729 swcgeom-0.8.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/data/101711-10_4p5-of-16_initial.CNG.swc
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/data/101711-11_16-of-16_initial.CNG.swc
--rw-r--r--   0 runner    (1001) docker     (123)   370235 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/data/1059283677_15257_2226-X16029-Y23953.swc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.466729 swcgeom-0.8.0/examples/dgl/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/dgl/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.466729 swcgeom-0.8.0/examples/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/pytorch/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/pytorch/branch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-18 15:00:43.000000 swcgeom-0.8.0/examples/pytorch/tree_folder_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-18 15:00:43.000000 swcgeom-0.8.0/git-conventional-commits.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-18 15:00:43.000000 swcgeom-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:00:56.474729 swcgeom-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.466729 swcgeom-0.8.0/swcgeom/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 15:00:56.000000 swcgeom-0.8.0/swcgeom/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.466729 swcgeom-0.8.0/swcgeom/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/analysis/branch_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/analysis/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/analysis/node_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/analysis/path_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/analysis/sholl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/analysis/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.470729 swcgeom-0.8.0/swcgeom/core/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/branch_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.470729 swcgeom-0.8.0/swcgeom/core/swc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc_utils/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc_utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc_utils/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc_utils/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/swc_utils/subtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/core/tree_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.470729 swcgeom-0.8.0/swcgeom/images/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/images/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/images/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.470729 swcgeom-0.8.0/swcgeom/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/image_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/mst.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/transforms/tree_assembler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.474729 swcgeom-0.8.0/swcgeom/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/utils/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/utils/sdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-18 15:00:43.000000 swcgeom-0.8.0/swcgeom/utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:00:56.466729 swcgeom-0.8.0/swcgeom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-18 15:00:56.000000 swcgeom-0.8.0/swcgeom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-18 15:00:56.000000 swcgeom-0.8.0/swcgeom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:00:56.000000 swcgeom-0.8.0/swcgeom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:00:56.000000 swcgeom-0.8.0/swcgeom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 15:00:56.000000 swcgeom-0.8.0/swcgeom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.852933 swcgeom-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.840933 swcgeom-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.844933 swcgeom-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-04 03:36:02.000000 swcgeom-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 03:36:02.000000 swcgeom-0.9.0/.github/workflows/github-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-04 03:36:02.000000 swcgeom-0.9.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 03:36:02.000000 swcgeom-0.9.0/.github/workflows/test-pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-04 03:36:02.000000 swcgeom-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-05-04 03:36:02.000000 swcgeom-0.9.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.844933 swcgeom-0.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 03:36:02.000000 swcgeom-0.9.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-05-04 03:36:02.000000 swcgeom-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-04 03:36:02.000000 swcgeom-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 03:36:14.852933 swcgeom-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-04 03:36:02.000000 swcgeom-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.844933 swcgeom-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    56312 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/Branch.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59312 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/BranchTree.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/CollectTips.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   166229 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/CutTree.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   154485 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/Features.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/GeometryTransform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/ImageStack.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   149381 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/MST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   305302 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/SpectralClustering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   403664 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/Tree.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.844933 swcgeom-0.9.0/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/data/101711-10_4p5-of-16_initial.CNG.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/data/101711-11_16-of-16_initial.CNG.swc
+-rw-r--r--   0 runner    (1001) docker     (123)   370235 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/data/1059283677_15257_2226-X16029-Y23953.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/data/toydata.swc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.844933 swcgeom-0.9.0/examples/dgl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/dgl/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.848933 swcgeom-0.9.0/examples/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/pytorch/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/pytorch/branch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-04 03:36:02.000000 swcgeom-0.9.0/examples/pytorch/tree_folder_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-04 03:36:02.000000 swcgeom-0.9.0/git-conventional-commits.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-04 03:36:02.000000 swcgeom-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 03:36:14.852933 swcgeom-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.848933 swcgeom-0.9.0/swcgeom/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 03:36:14.000000 swcgeom-0.9.0/swcgeom/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.848933 swcgeom-0.9.0/swcgeom/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/analysis/branch_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/analysis/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/analysis/node_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/analysis/path_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/analysis/sholl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/analysis/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.848933 swcgeom-0.9.0/swcgeom/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/branch_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.852933 swcgeom-0.9.0/swcgeom/core/swc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc_utils/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc_utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc_utils/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc_utils/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/swc_utils/subtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/core/tree_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.852933 swcgeom-0.9.0/swcgeom/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/images/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/images/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.852933 swcgeom-0.9.0/swcgeom/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/image_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/mst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/transforms/tree_assembler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.852933 swcgeom-0.9.0/swcgeom/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/utils/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/utils/sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-04 03:36:02.000000 swcgeom-0.9.0/swcgeom/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:36:14.848933 swcgeom-0.9.0/swcgeom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 03:36:14.000000 swcgeom-0.9.0/swcgeom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-04 03:36:14.000000 swcgeom-0.9.0/swcgeom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:36:14.000000 swcgeom-0.9.0/swcgeom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 03:36:14.000000 swcgeom-0.9.0/swcgeom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 03:36:14.000000 swcgeom-0.9.0/swcgeom.egg-info/top_level.txt
```

### Comparing `swcgeom-0.8.0/.github/workflows/build.yml` & `swcgeom-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/.github/workflows/github-publish.yml` & `swcgeom-0.9.0/.github/workflows/github-publish.yml`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/.github/workflows/pypi-publish.yml` & `swcgeom-0.9.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/.github/workflows/test-pypi-publish.yml` & `swcgeom-0.9.0/.github/workflows/test-pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/.gitignore` & `swcgeom-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/.pylintrc` & `swcgeom-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/CHANGELOG.md` & `swcgeom-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+# Changelog
+
+## **0.9.0**&emsp;<sub><sup>2023-05-04 ([1a3e9d4...797934f](https://github.com/yzx9/swcgeom/compare/1a3e9d4f7a0d1442fbb62f4693f5b5ec6d787af4...797934f120c0de266fc7d21038b5d17a1e2fbabc?diff=split))</sup></sub>
+
+### Features
+
+##### `analysis`
+
+- plot sholl circles by default ([797934f](https://github.com/yzx9/swcgeom/commit/797934f120c0de266fc7d21038b5d17a1e2fbabc))
+
+##### `images`
+
+- add transform support to folder ([167f67c](https://github.com/yzx9/swcgeom/commit/167f67c6f6ba58e80280d66df27caf47cf3dd3e6))
+- support disable compression ([9db01e9](https://github.com/yzx9/swcgeom/commit/9db01e94b063c1ec9efcf8fb906f2c732805e45f))
+- check if is a valid fname ([4d98abc](https://github.com/yzx9/swcgeom/commit/4d98abc66955d62760047c4fcfb1007f1dc9d64a))
+
+##### `transform`
+
+- add image stack center transform ([0fd1441](https://github.com/yzx9/swcgeom/commit/0fd14411e7b552f7b6d66a1f9c77f69adb0c379a))
+- expose static method ([c65c0cb](https://github.com/yzx9/swcgeom/commit/c65c0cba316797bedda5070b2db2a1a622931c20))
+
+### Bug Fixes
+
+##### `core`
+- change \`w\` to ones ([325ff1e](https://github.com/yzx9/swcgeom/commit/325ff1efe5cc662f7731003919f313cdd219caad))
+
+### BREAKING CHANGES
+
+- `analysis` plot sholl circles by default ([797934f](https://github.com/yzx9/swcgeom/commit/797934f120c0de266fc7d21038b5d17a1e2fbabc))
+- `images` folder do not move channel to first ([fd3a3cb](https://github.com/yzx9/swcgeom/commit/fd3a3cbea59f910ab31682c9272957cfea56eaa4))
+
+<br>
+
 ## **0.8.0**&emsp;<sub><sup>2023-04-18 ([3d2d660...bfee570](https://github.com/yzx9/swcgeom/compare/3d2d66034b269b1acf9a62cfeb8a8d3b85d1791a...bfee570d9989f10e5784323a60d2f06d5cf0877d?diff=split))</sup></sub>
 
 ### Features
 
 ##### `analysis`
 
 - add node count ([149ecec](https://github.com/yzx9/swcgeom/commit/149ecec3543d9f5f63b5a140deb7975328f08589))
```

### Comparing `swcgeom-0.8.0/PKG-INFO` & `swcgeom-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swcgeom
-Version: 0.8.0
+Version: 0.9.0
 Summary: A neuron geometry library for swc format
 Author-email: yzx9 <yuan.zx@outlook.com>
 License: CC4.0 BY-NC-SA
 Project-URL: repository, https://github.com/yzx9/swcgeom
 Keywords: neuron,swc,geom
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swcgeom-0.8.0/README.md` & `swcgeom-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/Branch.ipynb` & `swcgeom-0.9.0/examples/Branch.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/BranchTree.ipynb` & `swcgeom-0.9.0/examples/BranchTree.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/CollectTips.ipynb` & `swcgeom-0.9.0/examples/CollectTips.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/CutTree.ipynb` & `swcgeom-0.9.0/examples/CutTree.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/Features.ipynb` & `swcgeom-0.9.0/examples/Features.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/ImageStack.ipynb` & `swcgeom-0.9.0/examples/ImageStack.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/MST.ipynb` & `swcgeom-0.9.0/examples/MST.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/SpectralClustering.ipynb` & `swcgeom-0.9.0/examples/SpectralClustering.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/Tree.ipynb` & `swcgeom-0.9.0/examples/Tree.ipynb`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/data/101711-10_4p5-of-16_initial.CNG.swc` & `swcgeom-0.9.0/examples/data/101711-10_4p5-of-16_initial.CNG.swc`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/data/101711-11_16-of-16_initial.CNG.swc` & `swcgeom-0.9.0/examples/data/101711-11_16-of-16_initial.CNG.swc`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/data/1059283677_15257_2226-X16029-Y23953.swc` & `swcgeom-0.9.0/examples/data/1059283677_15257_2226-X16029-Y23953.swc`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/dgl/graph.py` & `swcgeom-0.9.0/examples/dgl/graph.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/pytorch/branch.py` & `swcgeom-0.9.0/examples/pytorch/branch.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/pytorch/branch_dataset.py` & `swcgeom-0.9.0/examples/pytorch/branch_dataset.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/examples/pytorch/tree_folder_dataset.py` & `swcgeom-0.9.0/examples/pytorch/tree_folder_dataset.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/git-conventional-commits.yaml` & `swcgeom-0.9.0/git-conventional-commits.yaml`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/pyproject.toml` & `swcgeom-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/analysis/branch_features.py` & `swcgeom-0.9.0/swcgeom/analysis/branch_features.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/analysis/feature_extractor.py` & `swcgeom-0.9.0/swcgeom/analysis/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/analysis/node_features.py` & `swcgeom-0.9.0/swcgeom/analysis/node_features.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/analysis/path_features.py` & `swcgeom-0.9.0/swcgeom/analysis/path_features.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/analysis/sholl.py` & `swcgeom-0.9.0/swcgeom/analysis/sholl.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,80 +6,98 @@
 import numpy as np
 import numpy.typing as npt
 import seaborn as sns
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
 from ..core import Tree
+from ..transforms import TranslateOrigin
 from ..utils import draw_circles, get_fig_ax
+from .visualization import draw
 
 __all__ = ["Sholl"]
 
+XLABEL = "Radial Distance"
+YLABLE = "Count of Intersections"
+
 
 class Sholl:
     """Sholl analysis.
 
     References
     ----------
     [1] Dendritic organization in the neurons of the visual and motor
     cortices of the cat J. Anat., 87 (1953), pp. 387-406
     """
 
+    tree: Tree
     rs: npt.NDArray[np.float32]
     rmax: float
 
     # compat
     step: float | None = None
 
     def __init__(
         self,
         tree: Tree,
         step: Optional[float] = None,
     ) -> None:
-        xyz = tree.get_segments().xyz() - tree.soma().xyz()  # shift
-        self.rs = np.linalg.norm(xyz, axis=2)
+        self.tree = TranslateOrigin.transform(tree)  # shift
+        self.rs = np.linalg.norm(self.tree.get_segments().xyz(), axis=2)
         self.rmax = self.rs.max()
 
         if step is not None:
             warnings.warn(
                 "`Sholl(x, step=...)` has been replaced by "
                 "`Sholl(x).get(steps=...)` since v0.6.0 because it has "
                 "been change to dynamic calculate, and will be removed "
                 "in next version",
                 DeprecationWarning,
             )
             self.step = step
 
     def get(self, steps: int | npt.ArrayLike = 20) -> npt.NDArray[np.int64]:
-        xs, rs = self._get_rs(steps=steps), self.rs
-        intersections = [np.logical_and(rs[:, 0] <= i, rs[:, 1] > i) for i in xs]
+        intersections = [
+            np.logical_or(
+                np.logical_and(self.rs[:, 0] <= r, self.rs[:, 1] > r),
+                np.logical_and(self.rs[:, 1] <= r, self.rs[:, 0] > r),
+            )
+            for r in self._get_rs(steps=steps)
+        ]
         return np.count_nonzero(intersections, axis=1)
 
     def intersect(self, r: float) -> int:
-        return np.count_nonzero(np.logical_and(self.rs[:, 0] <= r, self.rs[:, 1] > r))
+        return np.count_nonzero(
+            np.logical_or(
+                np.logical_and(self.rs[:, 0] <= r, self.rs[:, 1] > r),
+                np.logical_and(self.rs[:, 1] <= r, self.rs[:, 0] > r),
+            )
+        )
 
     def plot(  # pylint: disable=too-many-arguments
         self,
         steps: List[float] | int = 20,
         plot_type: str | None = None,
-        kind: Literal["bar", "linechart", "circles"] = "bar",
+        kind: Literal["bar", "linechart", "circles"] = "circles",
         fig: Figure | None = None,
         ax: Axes | None = None,
         **kwargs,
     ) -> Tuple[Figure, Axes]:
         """Plot Sholl analysis.
 
         Parameters
         ----------
         steps : int or List[float], default to 20
             Steps of raius of circle. If steps is int, then it will be
             evenly divided into n radii.
-        kind : "bar" | "linechart" | "circles", default `bar`
+        kind : "bar" | "linechart" | "circles", default `circles`
         fig : ~matplotlib.figure.Figure
         ax : ~matplotlib.axes.Axes
+        **kwargs :
+            Forwarding to plot method.
         """
         if plot_type is not None:
             warnings.warn(
                 "`plot_type` has been renamed to `kind` since v0.5.0, "
                 "and will be removed in next version",
                 DeprecationWarning,
             )
@@ -87,26 +105,37 @@
 
         xs = self._get_rs(steps=steps)
         ys = self.get(steps=xs)
         fig, ax = get_fig_ax(fig, ax)
         match kind:
             case "bar":
                 sns.barplot(x=xs, y=ys, ax=ax, **kwargs)
-                ax.set_ylabel("Count of Intersections")
+                ax.set_ylabel(YLABLE)
             case "linechart":
                 sns.lineplot(x=xs, y=ys, ax=ax, **kwargs)
-                ax.set_ylabel("Count of Intersections")
+                ax.set_ylabel(YLABLE)
             case "circles":
                 kwargs.setdefault("y_min", 0)
+                drawtree = kwargs.pop("drawtree", True)
+                colorbar = kwargs.pop("colorbar", True)
                 patches = draw_circles(ax, xs, ys, **kwargs)
-                fig.colorbar(patches, ax=ax)
+
+                if drawtree is True:
+                    draw(self.tree, ax=ax, direction_indicator=False)
+                elif isinstance(drawtree, str):
+                    draw(self.tree, ax=ax, color=drawtree, direction_indicator=False)
+
+                if colorbar is True:
+                    fig.colorbar(patches, ax=ax, label=YLABLE)
+                elif isinstance(colorbar, (Axes, np.ndarray, list)):
+                    fig.colorbar(patches, ax=colorbar, label=YLABLE)
             case _:
                 raise ValueError(f"unsupported kind: {kind}")
 
-        ax.set_xlabel("Radial Distance")
+        ax.set_xlabel(XLABEL)
         return fig, ax
 
     @staticmethod
     def get_rs(rmax: float, steps: int | npt.ArrayLike) -> npt.NDArray[np.float32]:
         """Function to calculate the list of radius used by the sholl."""
         if isinstance(steps, int):
             s = rmax / (steps + 1)
```

### Comparing `swcgeom-0.8.0/swcgeom/analysis/visualization.py` & `swcgeom-0.9.0/swcgeom/analysis/visualization.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/branch.py` & `swcgeom-0.9.0/swcgeom/core/branch.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/branch_tree.py` & `swcgeom-0.9.0/swcgeom/core/branch_tree.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/node.py` & `swcgeom-0.9.0/swcgeom/core/node.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/path.py` & `swcgeom-0.9.0/swcgeom/core/path.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/population.py` & `swcgeom-0.9.0/swcgeom/core/population.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/segment.py` & `swcgeom-0.9.0/swcgeom/core/segment.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/swc.py` & `swcgeom-0.9.0/swcgeom/core/swc.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def xyz(self) -> npt.NDArray[np.float32]:
         """Get the coordinates of shape(n_sample, 3)."""
         return np.stack([self.x(), self.y(), self.z()], axis=1)
 
     def xyzw(self) -> npt.NDArray[np.float32]:
         """Get the homogeneous coordinates of shape(n_sample, 4)."""
-        w = np.zeros_like(self.x())
+        w = np.ones_like(self.x())
         return np.stack([self.x(), self.y(), self.z(), w], axis=1)
 
     def xyzr(self) -> npt.NDArray[np.float32]:
         """Get the coordinates and radius array of shape(n_sample, 4)."""
         return np.stack([self.x(), self.y(), self.z(), self.r()], axis=1)
 
     @abstractmethod
```

### Comparing `swcgeom-0.8.0/swcgeom/core/swc_utils/assembler.py` & `swcgeom-0.9.0/swcgeom/core/swc_utils/assembler.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/swc_utils/base.py` & `swcgeom-0.9.0/swcgeom/core/swc_utils/base.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/swc_utils/checker.py` & `swcgeom-0.9.0/swcgeom/core/swc_utils/checker.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/swc_utils/io.py` & `swcgeom-0.9.0/swcgeom/core/swc_utils/io.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/swc_utils/normalizer.py` & `swcgeom-0.9.0/swcgeom/core/swc_utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/swc_utils/subtree.py` & `swcgeom-0.9.0/swcgeom/core/swc_utils/subtree.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/tree.py` & `swcgeom-0.9.0/swcgeom/core/tree.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/core/tree_utils.py` & `swcgeom-0.9.0/swcgeom/core/tree_utils.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/images/folder.py` & `swcgeom-0.9.0/swcgeom/images/folder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,146 @@
 """Image stack folder."""
 
 import os
 import re
 from abc import ABC, abstractmethod
-from typing import Callable, Iterable, List, Literal, Optional, Tuple, TypeVar
+from typing import Callable, Generic, Iterable, List, Literal, Optional, Tuple, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 from typing_extensions import Self
 
+from ..transforms import Identity, Transform
 from .io import read_imgs
 
 __all__ = [
     "ImageStackFolder",
     "LabeledImageStackFolder",
     "PathImageStackFolder",
 ]
 
 T = TypeVar("T")
 
 
-class ImageStackFolderBase(ABC):
+class ImageStackFolderBase(Generic[T], ABC):
     """Image stack folder base."""
 
     files: List[str]
+    transform: Transform[npt.NDArray[np.float32], T]
 
-    def __init__(self, files: Iterable[str]) -> None:
+    def __init__(
+        self,
+        files: Iterable[str],
+        *,
+        transform: Optional[Transform[npt.NDArray[np.float32], T]] = None,
+    ) -> None:
         super().__init__()
         self.files = list(files)
+        self.transform = transform or Identity()  # type: ignore
 
     @abstractmethod
-    def __getitem__(self, key: str, /) -> npt.NDArray[np.float32]:
+    def __getitem__(self, key: str, /) -> T:
         raise NotImplementedError()
 
     def __len__(self) -> int:
         return len(self.files)
 
-    def _get(self, fname: str) -> npt.NDArray[np.float32]:
+    def _get(self, fname: str) -> T:
         imgs = self.read_imgs(fname)
-        # TODO: support transforms
+        imgs = self.transform(imgs)
         return imgs
 
     @staticmethod
     def read_imgs(fname: str) -> npt.NDArray[np.float32]:
-        imgs = read_imgs(fname).get_full()
-        imgs = np.moveaxis(imgs, -1, 0)  # (X, Y, Z, C) -> (C, X, Y, Z)
-        return imgs
+        return read_imgs(fname).get_full()
 
     @staticmethod
     def scan(root: str, *, pattern: Optional[str] = None) -> List[str]:
         is_valid = re.compile(pattern).match if pattern is not None else truthly
 
         fs = []
         for d, _, files in os.walk(root):
             fs.extend(os.path.join(d, f) for f in files if is_valid(f))
 
         return fs
 
 
-class ImageStackFolder(ImageStackFolderBase):
+class ImageStackFolder(Generic[T], ImageStackFolderBase[T]):
     """Image stack folder."""
 
-    def __getitem__(self, idx: int, /) -> npt.NDArray[np.float32]:
+    def __getitem__(self, idx: int, /) -> T:
         return self._get(self.files[idx])
 
     @classmethod
-    def from_dir(cls, root: str, *, pattern: Optional[str] = None) -> Self:
-        return cls(cls.scan(root, pattern=pattern))
+    def from_dir(cls, root: str, *, pattern: Optional[str] = None, **kwargs) -> Self:
+        """
+        Parameters
+        ----------
+        root : str
+        pattern : str, optional
+            Filter files by pattern.
+        **kwargs
+            Pass to `cls.__init__`
+        """
+        return cls(cls.scan(root, pattern=pattern), **kwargs)
 
 
-class LabeledImageStackFolder(ImageStackFolderBase):
+class LabeledImageStackFolder(Generic[T], ImageStackFolderBase[T]):
     """Image stack folder with label."""
 
     labels: List[int]
 
-    def __init__(self, files: Iterable[str], labels: Iterable[int]):
-        super().__init__(files)
+    def __init__(self, files: Iterable[str], labels: Iterable[int], **kwargs):
+        super().__init__(files, **kwargs)
         self.labels = list(labels)
 
     def __getitem__(self, idx: int) -> Tuple[npt.NDArray[np.float32], int]:
         return self.read_imgs(self.files[idx]), self.labels[idx]
 
     @classmethod
     def from_dir(
         cls,
         root: str,
         label: int | Callable[[str], int],
         *,
         pattern: Optional[str] = None,
+        **kwargs,
     ) -> Self:
         files = cls.scan(root, pattern=pattern)
         if callable(label):
             labels = [label(f) for f in files]
         elif isinstance(label, int):
             labels = [label for _ in files]
         else:
-            raise ValueError("")
-        return cls(files, labels)
+            raise ValueError("invalid label")
+        return cls(files, labels, **kwargs)
 
 
-class PathImageStackFolder(ImageStackFolder):
+class PathImageStackFolder(Generic[T], ImageStackFolder[T]):
     """Image stack folder with relpath."""
 
     root: str
 
-    def __getitem__(self, idx: int) -> Tuple[npt.NDArray[np.float32], str]:
+    def __init__(self, files: Iterable[str], *, root: str, **kwargs):
+        super().__init__(files, **kwargs)
+        self.root = root
+
+    def __getitem__(self, idx: int) -> Tuple[T, str]:
         relpath = os.path.relpath(self.files[idx], self.root)
-        return self.read_imgs(self.files[idx]), relpath
+        return self._get(self.files[idx]), relpath
 
     @classmethod
-    def from_dir(cls, root: str, *, pattern: Optional[str] = None) -> Self:
-        return cls(cls.scan(root, pattern=pattern))
+    def from_dir(cls, root: str, *, pattern: Optional[str] = None, **kwargs) -> Self:
+        """
+        Parameters
+        ----------
+        root : str
+        pattern : str, optional
+            Filter files by pattern.
+        **kwargs
+            Pass to `cls.__init__`
+        """
+        return cls(cls.scan(root, pattern=pattern), root=root, **kwargs)
 
 
 def truthly(*args, **kwargs) -> Literal[True]:  # pylint: disable=unused-argument
     return True
```

### Comparing `swcgeom-0.8.0/swcgeom/images/io.py` & `swcgeom-0.9.0/swcgeom/images/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 import os
 import re
 import warnings
 from abc import ABC, abstractmethod
 from functools import cache, lru_cache
-from typing import Any, Callable, Iterable, List, Optional, Tuple, overload
+from typing import Any, Callable, Iterable, List, Literal, Optional, Tuple, overload
 
 import nrrd
 import numpy as np
 import numpy.typing as npt
 import tifffile
 
 __all__ = ["read_imgs", "save_tiff", "read_images"]
@@ -84,48 +84,52 @@
         return TiffImageStack(fname, **kwargs)
     if ext in [".nrrd"]:
         return NrrdImageStack(fname, **kwargs)
     if ext in [".npy", ".npz"]:
         return NDArrayImageStack(np.load(fname), **kwargs)
     if TeraflyImageStack.is_root(fname):
         return TeraflyImageStack(fname, **kwargs)
+    if not os.path.exists(fname):
+        raise ValueError("image stack not exists")
     raise ValueError("unsupported image stack")
 
 
 def save_tiff(
     data: npt.NDArray | ImageStack,
     fname: str,
+    *,
     dtype: Optional[np.unsignedinteger | np.floating] = None,
-    c_first: bool = False,
     swap_xy: bool = False,
+    compression: str | Literal[False] = "zlib",
     **kwargs,
 ) -> None:
     """Save image stack as tiff.
 
     Parameters
     ----------
     data : array
         The image stack.
     fname : str
     dtype : np.dtype, optional
         Casting data to specified dtype. If integer and float
         conversions occur, they will be scaled (assuming floats are
         between 0 and 1).
-    c_first : bool, default False
-        If true, data should be an array of shape (C, X, Y, Z), or
-        (X, Y, Z, C) or (X, Y, Z) otherwise.
     swap_xy : bool, default False
         Swap axes `x` and `y`.
+    compression : str | False, default `zlib`
+        Compression algorithm, forwarding to `tifffile.imwrite`. If no
+        algorithnm is specify specified, we will use the zlib algorithm
+        with compression level 6 by default.
+    **kwargs : Dict[str, Any], optional
+        Forwarding to `tifffile.imwrite`
     """
     if isinstance(data, ImageStack):
         data = data.get_full()  # TODO: avoid load full imgs to memory
 
-    if c_first:
-        data = data.swapaxes(0, 1)  # (C, _, _, _) -> (_, _, _, C)
-    elif data.ndim == 3:
+    if data.ndim == 3:
         data = np.expand_dims(data, -1)  # (_, _, _)  -> (_, _, _, C), C === 1
 
     if swap_xy:
         data = data.swapaxes(0, 1)  # (X, Y, _, _) -> (Y, X, _, _)
 
     assert data.ndim == 4, "should be an array of shape (X, Y, Z, C)"
     assert data.shape[-1] in [1, 3], "support 'miniblack' or 'rgb'"
@@ -140,21 +144,24 @@
         ):
             scaler_factor = 1 / UINT_MAX[np.dtype(data.dtype)]  # type: ignore
         else:
             scaler_factor = 1
 
         data = (data * scaler_factor).astype(dtype)
 
+    if compression is not False:
+        kwargs.setdefault("compression", compression)
+        if compression == "zlib":
+            kwargs.setdefault("compressionargs", {"level": 6})
+
     tifffile.imwrite(
         fname,
         np.moveaxis(data, 2, 0),  # (_, _, Z, _) -> (Z, _, _, _)
         photometric="rgb" if data.shape[-1] == 3 else "minisblack",
         metadata={"axes": "ZXYC" if not swap_xy else "ZYXC"},
-        compression="zlib",
-        compressionargs={"level": 6},
         **kwargs,
     )
 
 
 class NDArrayImageStack(ImageStack):
     """NDArray image stack."""
```

### Comparing `swcgeom-0.8.0/swcgeom/transforms/base.py` & `swcgeom-0.9.0/swcgeom/transforms/base.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/transforms/branch.py` & `swcgeom-0.9.0/swcgeom/transforms/branch.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/transforms/geometry.py` & `swcgeom-0.9.0/swcgeom/transforms/geometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """SWC geometry operations."""
 
+import warnings
 from typing import Generic, Literal, Optional, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
 from ..core import DictSWC
-from ..core.swc_utils import SWCNames, get_names
+from ..core.swc_utils import SWCNames
 from ..utils import rotate3d, rotate3d_x, rotate3d_y, rotate3d_z, scale3d, translate3d
 from .base import Transform
 
 __all__ = [
     "Normalizer",
     "AffineTransform",
     "Translate",
@@ -26,24 +27,27 @@
 Center = Literal["root", "soma", "origin"]
 
 
 # pylint: disable=too-few-public-methods
 class Normalizer(Generic[T], Transform[T, T]):
     """Noramlize coordinates and radius to 0-1."""
 
-    names: SWCNames
-
     def __init__(self, *, names: Optional[SWCNames] = None) -> None:
         super().__init__()
-        self.names = get_names(names)
+        if names is not None:
+            warnings.warn(
+                "`name` parameter is no longer needed, now use the "
+                "built-in names table, you can directly remove it.",
+                DeprecationWarning,
+            )
 
     def __call__(self, x: T) -> T:
         """Scale the `x`, `y`, `z`, `r` of nodes to 0-1."""
         new_tree = x.copy()
-        xyzr = [self.names.x, self.names.y, self.names.z, self.names.r]
+        xyzr = [x.names.x, x.names.y, x.names.z, x.names.r]
         for key in xyzr:  # TODO: does r is the same?
             vs = new_tree.ndata[key]
             new_tree.ndata[key] = (vs - np.min(vs)) / np.max(vs)
 
         return new_tree
 
 
@@ -59,127 +63,148 @@
         tm: npt.NDArray[np.float32],
         center: Center = "origin",
         *,
         fmt: str,
         names: Optional[SWCNames] = None,
     ) -> None:
         self.tm, self.center, self.fmt = tm, center, fmt
-        self.names = get_names(names)
+        if names is not None:
+            warnings.warn(
+                "`name` parameter is no longer needed, now use the "
+                "built-in names table, you can directly remove it.",
+                DeprecationWarning,
+            )
 
     def __call__(self, x: T) -> T:
         match self.center:
             case "root" | "soma":
-                idx = np.nonzero(x.ndata[self.names.pid] == -1)[0].item()
+                idx = np.nonzero(x.ndata[x.names.pid] == -1)[0].item()
                 xyz = x.xyz()[idx]
                 tm = (
                     translate3d(-xyz[0], -xyz[1], -xyz[2])
                     .dot(self.tm)
                     .dot(translate3d(xyz[0], xyz[1], xyz[2]))
                 )
             case _:
                 tm = self.tm
 
-        xyzw = x.xyzw().dot(tm).T
-        y = x.copy()
-        y.ndata[self.names.x] = xyzw[0]
-        y.ndata[self.names.y] = xyzw[1]
-        y.ndata[self.names.z] = xyzw[2]
-        return y
+        return self.apply(x, tm)
 
     def __repr__(self) -> str:
         return self.fmt
 
+    @staticmethod
+    def apply(x: T, tm: npt.NDArray[np.float32]) -> T:
+        xyzw = x.xyzw().dot(tm.T).T
+        xyzw /= xyzw[3]
+
+        y = x.copy()
+        y.ndata[x.names.x] = xyzw[0]
+        y.ndata[x.names.y] = xyzw[1]
+        y.ndata[x.names.z] = xyzw[2]
+        return y
+
 
-class Translate(AffineTransform[T]):
+class Translate(Generic[T], AffineTransform[T]):
     """Translate SWC."""
 
-    def __init__(self, tx: float, ty: float, tz: float) -> None:
+    def __init__(self, tx: float, ty: float, tz: float, **kwargs) -> None:
         fmt = f"Translate-{tx}-{ty}-{tz}"
-        super().__init__(translate3d(tx, ty, tz), fmt=fmt)
+        super().__init__(translate3d(tx, ty, tz), fmt=fmt, **kwargs)
 
     @classmethod
-    def transform(cls, x: T, tx: float, ty: float, tz: float) -> T:
-        return cls(tx, ty, tz)(x)
+    def transform(cls, x: T, tx: float, ty: float, tz: float, **kwargs) -> T:
+        return cls(tx, ty, tz, **kwargs)(x)
 
 
-class TranslateOrigin:
+class TranslateOrigin(Generic[T], Transform[T, T]):
     """Translate root of SWC to origin point."""
 
-    def __init__(self, names: Optional[SWCNames] = None) -> None:
-        self.names = get_names(names)
-
     def __call__(self, x: T) -> T:
-        idx = np.nonzero(x.ndata[self.names.pid] == -1)[0].item()
-        xyz = x.xyz()[idx]
-        tm = translate3d(-xyz[0], -xyz[1], -xyz[2])
+        return self.transform(x)
 
-        xyzw = x.xyzw().dot(tm).T
-        y = x.copy()
-        y.ndata[self.names.x] = xyzw[0]
-        y.ndata[self.names.y] = xyzw[1]
-        y.ndata[self.names.z] = xyzw[2]
-        return y
+    @classmethod
+    def transform(cls, x: T) -> T:
+        pid = np.nonzero(x.ndata[x.names.pid] == -1)[0].item()
+        xyzw = x.xyzw()
+        tm = translate3d(-xyzw[pid, 0], -xyzw[pid, 1], -xyzw[pid, 2])
+        return AffineTransform.apply(x, tm)
 
 
-class Scale(AffineTransform[T]):
+class Scale(Generic[T], AffineTransform[T]):
     """Scale SWC."""
 
     def __init__(
-        self, sx: float, sy: float, sz: float, center: Center = "root"
+        self, sx: float, sy: float, sz: float, center: Center = "root", **kwargs
     ) -> None:
         fmt = f"Scale-{sx}-{sy}-{sz}"
-        super().__init__(scale3d(sx, sy, sz), center=center, fmt=fmt)
+        super().__init__(scale3d(sx, sy, sz), center=center, fmt=fmt, **kwargs)
 
     @classmethod
     def transform(  # pylint: disable=too-many-arguments
-        cls, x: T, sx: float, sy: float, sz: float, center: Center = "root"
+        cls, x: T, sx: float, sy: float, sz: float, center: Center = "root", **kwargs
     ) -> T:
-        return cls(sx, sy, sz, center=center)(x)
+        return cls(sx, sy, sz, center=center, **kwargs)(x)
 
 
-class Rotate(AffineTransform[T]):
+class Rotate(Generic[T], AffineTransform[T]):
     """Rotate SWC."""
 
     def __init__(
-        self, n: npt.NDArray[np.float32], theta: float, center: Center = "root"
+        self,
+        n: npt.NDArray[np.float32],
+        theta: float,
+        center: Center = "root",
+        **kwargs,
     ) -> None:
         fmt = f"Rotate-{n[0]}-{n[1]}-{n[2]}-{theta:.4f}"
-        super().__init__(rotate3d(n, theta), center=center, fmt=fmt)
+        super().__init__(rotate3d(n, theta), center=center, fmt=fmt, **kwargs)
 
     @classmethod
     def transform(
-        cls, x: T, n: npt.NDArray[np.float32], theta: float, center: Center = "root"
+        cls,
+        x: T,
+        n: npt.NDArray[np.float32],
+        theta: float,
+        center: Center = "root",
+        **kwargs,
     ) -> T:
-        return cls(n, theta, center=center)(x)
+        return cls(n, theta, center=center, **kwargs)(x)
 
 
-class RotateX(AffineTransform[T]):
+class RotateX(Generic[T], AffineTransform[T]):
     """Rotate SWC with x-axis."""
 
-    def __init__(self, theta: float, center: Center = "root") -> None:
-        super().__init__(rotate3d_x(theta), center=center, fmt=f"RotateX-{theta}")
+    def __init__(self, theta: float, center: Center = "root", **kwargs) -> None:
+        super().__init__(
+            rotate3d_x(theta), center=center, fmt=f"RotateX-{theta}", **kwargs
+        )
 
     @classmethod
-    def transform(cls, x: T, theta: float, center: Center = "root") -> T:
-        return cls(theta, center=center)(x)
+    def transform(cls, x: T, theta: float, center: Center = "root", **kwargs) -> T:
+        return cls(theta, center=center, **kwargs)(x)
 
 
-class RotateY(AffineTransform[T]):
+class RotateY(Generic[T], AffineTransform[T]):
     """Rotate SWC with y-axis."""
 
-    def __init__(self, theta: float, center: Center = "root") -> None:
-        super().__init__(rotate3d_y(theta), center=center, fmt=f"RotateX-{theta}")
+    def __init__(self, theta: float, center: Center = "root", **kwargs) -> None:
+        super().__init__(
+            rotate3d_y(theta), center=center, fmt=f"RotateX-{theta}", **kwargs
+        )
 
     @classmethod
-    def transform(cls, x: T, theta: float, center: Center = "root") -> T:
-        return cls(theta, center=center)(x)
+    def transform(cls, x: T, theta: float, center: Center = "root", **kwargs) -> T:
+        return cls(theta, center=center, **kwargs)(x)
 
 
-class RotateZ(AffineTransform[T]):
+class RotateZ(Generic[T], AffineTransform[T]):
     """Rotate SWC with z-axis."""
 
-    def __init__(self, theta: float, center: Center = "root") -> None:
-        super().__init__(rotate3d_z(theta), center=center, fmt=f"RotateX-{theta}")
+    def __init__(self, theta: float, center: Center = "root", **kwargs) -> None:
+        super().__init__(
+            rotate3d_z(theta), center=center, fmt=f"RotateX-{theta}", **kwargs
+        )
 
     @classmethod
-    def transform(cls, x: T, theta: float, center: Center = "root") -> T:
-        return cls(theta, center=center)(x)
+    def transform(cls, x: T, theta: float, center: Center = "root", **kwargs) -> T:
+        return cls(theta, center=center, **kwargs)(x)
```

### Comparing `swcgeom-0.8.0/swcgeom/transforms/image_stack.py` & `swcgeom-0.9.0/swcgeom/transforms/image_stack.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/transforms/mst.py` & `swcgeom-0.9.0/swcgeom/transforms/mst.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/transforms/population.py` & `swcgeom-0.9.0/swcgeom/transforms/population.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/transforms/tree.py` & `swcgeom-0.9.0/swcgeom/transforms/tree.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/transforms/tree_assembler.py` & `swcgeom-0.9.0/swcgeom/transforms/tree_assembler.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/utils/download.py` & `swcgeom-0.9.0/swcgeom/utils/download.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/utils/numpy.py` & `swcgeom-0.9.0/swcgeom/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/utils/renderer.py` & `swcgeom-0.9.0/swcgeom/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/utils/sdf.py` & `swcgeom-0.9.0/swcgeom/utils/sdf.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom/utils/transforms.py` & `swcgeom-0.9.0/swcgeom/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swcgeom-0.8.0/swcgeom.egg-info/PKG-INFO` & `swcgeom-0.9.0/swcgeom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swcgeom
-Version: 0.8.0
+Version: 0.9.0
 Summary: A neuron geometry library for swc format
 Author-email: yzx9 <yuan.zx@outlook.com>
 License: CC4.0 BY-NC-SA
 Project-URL: repository, https://github.com/yzx9/swcgeom
 Keywords: neuron,swc,geom
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swcgeom-0.8.0/swcgeom.egg-info/SOURCES.txt` & `swcgeom-0.9.0/swcgeom.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 .github/workflows/test-pypi-publish.yml
 .vscode/settings.json
 examples/Branch.ipynb
 examples/BranchTree.ipynb
 examples/CollectTips.ipynb
 examples/CutTree.ipynb
 examples/Features.ipynb
+examples/GeometryTransform.ipynb
 examples/ImageStack.ipynb
 examples/MST.ipynb
 examples/SpectralClustering.ipynb
 examples/Tree.ipynb
 examples/data/101711-10_4p5-of-16_initial.CNG.swc
 examples/data/101711-11_16-of-16_initial.CNG.swc
 examples/data/1059283677_15257_2226-X16029-Y23953.swc
+examples/data/toydata.swc
 examples/dgl/graph.py
 examples/pytorch/branch.py
 examples/pytorch/branch_dataset.py
 examples/pytorch/tree_folder_dataset.py
 swcgeom/__init__.py
 swcgeom/_version.py
 swcgeom.egg-info/PKG-INFO
@@ -61,14 +63,15 @@
 swcgeom/images/folder.py
 swcgeom/images/io.py
 swcgeom/transforms/__init__.py
 swcgeom/transforms/base.py
 swcgeom/transforms/branch.py
 swcgeom/transforms/geometry.py
 swcgeom/transforms/image_stack.py
+swcgeom/transforms/images.py
 swcgeom/transforms/mst.py
 swcgeom/transforms/population.py
 swcgeom/transforms/tree.py
 swcgeom/transforms/tree_assembler.py
 swcgeom/utils/__init__.py
 swcgeom/utils/debug.py
 swcgeom/utils/download.py
```

