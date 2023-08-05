# Comparing `tmp/rastermap-0.9.3.tar.gz` & `tmp/rastermap-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastermap-0.9.3.tar", last modified: Wed Aug  2 13:25:26 2023, max compression
+gzip compressed data, was "rastermap-0.9.4.tar", last modified: Sat Aug  5 17:21:59 2023, max compression
```

## Comparing `rastermap-0.9.3.tar` & `rastermap-0.9.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.774589 rastermap-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.778589 rastermap-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-02 13:25:16.000000 rastermap-0.9.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-02 13:25:16.000000 rastermap-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 13:25:16.000000 rastermap-0.9.3/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-02 13:25:16.000000 rastermap-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-08-02 13:25:26.782590 rastermap-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-08-02 13:25:16.000000 rastermap-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-02 13:25:16.000000 rastermap-0.9.3/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-02 13:25:16.000000 rastermap-0.9.3/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.778589 rastermap-0.9.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_largescale.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_singleneurons.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_widefield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_zebrafish.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.778589 rastermap-0.9.3/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig3.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig4.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig5.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig5.py
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/other_upsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/qrdqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/splitting.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/rastermap/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/rastermap/gui/
--rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28224 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/guiparts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17546 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/rastermap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:25:26.782590 rastermap-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-02 13:25:16.000000 rastermap-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 13:25:16.000000 rastermap-0.9.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-02 13:25:16.000000 rastermap-0.9.3/tests/test_rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-02 13:25:16.000000 rastermap-0.9.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.937479 rastermap-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.941479 rastermap-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-05 17:21:48.000000 rastermap-0.9.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-05 17:21:48.000000 rastermap-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-05 17:21:48.000000 rastermap-0.9.4/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-05 17:21:48.000000 rastermap-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-08-05 17:21:59.945479 rastermap-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-08-05 17:21:48.000000 rastermap-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-05 17:21:48.000000 rastermap-0.9.4/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-05 17:21:48.000000 rastermap-0.9.4/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.941479 rastermap-0.9.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_largescale.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_singleneurons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_widefield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_zebrafish.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.941479 rastermap-0.9.4/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/other_upsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/qrdqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/splitting.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/rastermap/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/guiparts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/rastermap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:21:59.945479 rastermap-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-05 17:21:48.000000 rastermap-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 17:21:48.000000 rastermap-0.9.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-05 17:21:48.000000 rastermap-0.9.4/tests/test_rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-05 17:21:48.000000 rastermap-0.9.4/tox.ini
```

### Comparing `rastermap-0.9.3/.github/workflows/test_and_deploy.yml` & `rastermap-0.9.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/.gitignore` & `rastermap-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/LICENSE` & `rastermap-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/PKG-INFO` & `rastermap-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastermap
-Version: 0.9.3
+Version: 0.9.4
 Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
 Home-page: https://github.com/MouseLand/rastermap
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: carsen.stringer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -99,15 +99,17 @@
 
 The quickest way to start is to open the GUI from a command line terminal. You might need to open an anaconda prompt if you did not add anaconda to the path. Then run:
 
 ~~~sh
 python -m rastermap
 ~~~
 
-To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
+To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). You can also try it out with our demo data available [here](https://osf.io/xn4cm/).
+
+Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
 GUI examples:
```

### Comparing `rastermap-0.9.3/README.md` & `rastermap-0.9.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,17 @@
 
 The quickest way to start is to open the GUI from a command line terminal. You might need to open an anaconda prompt if you did not add anaconda to the path. Then run:
 
 ~~~sh
 python -m rastermap
 ~~~
 
-To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
+To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). You can also try it out with our demo data available [here](https://osf.io/xn4cm/).
+
+Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
 GUI examples:
```

### Comparing `rastermap-0.9.3/conftest.py` & `rastermap-0.9.4/conftest.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/notebooks/rastermap_largescale.ipynb` & `rastermap-0.9.4/notebooks/rastermap_largescale.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/notebooks/rastermap_singleneurons.ipynb` & `rastermap-0.9.4/notebooks/rastermap_singleneurons.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/notebooks/rastermap_widefield.ipynb` & `rastermap-0.9.4/notebooks/rastermap_widefield.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/notebooks/rastermap_zebrafish.ipynb` & `rastermap-0.9.4/notebooks/rastermap_zebrafish.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/notebooks/tutorial.ipynb` & `rastermap-0.9.4/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig1.ipynb` & `rastermap-0.9.4/paper/fig1.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig1.py` & `rastermap-0.9.4/paper/fig1.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig2.ipynb` & `rastermap-0.9.4/paper/fig2.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig2.py` & `rastermap-0.9.4/paper/fig2.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig3.ipynb` & `rastermap-0.9.4/paper/fig3.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig3.py` & `rastermap-0.9.4/paper/fig3.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig4.ipynb` & `rastermap-0.9.4/paper/fig4.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig4.py` & `rastermap-0.9.4/paper/fig4.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig5.ipynb` & `rastermap-0.9.4/paper/fig5.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig5.py` & `rastermap-0.9.4/paper/fig5.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig_splitting.py` & `rastermap-0.9.4/paper/fig_splitting.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/fig_utils.py` & `rastermap-0.9.4/paper/fig_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,19 +77,21 @@
         xmin, xmax = 0, xmax - xmin
     im = ax.imshow(X[:, xmin0:xmax0], vmin=-vmax if symmetric else 0, vmax=vmax, 
               cmap="RdBu_r" if symmetric else "gray_r", aspect="auto")
     ax.axis("off")
     if label_pos=="left":
         if n_neurons is not None:
             ax.plot(-padding_x*xr * np.ones(2), nn - np.array([0, n_neurons/nper]), color="k")
-        ax.plot(xmin + np.array([0, fs*n_sec]), nn*(1+padding/2) + np.zeros(2), color="k")
+        if n_sec is not None:
+            ax.plot(xmin + np.array([0, fs*n_sec]), nn*(1+padding/2) + np.zeros(2), color="k")
     else:
         if n_neurons is not None:
             ax.plot((1+padding_x)*xr * np.ones(2), nn - np.array([0, n_neurons/nper]), color="k")
-        ax.plot(xmin + np.array([xr-fs*n_sec, xr]), nn*(1+padding/2) + np.zeros(2), color="k")
+        if n_sec is not None:
+            ax.plot(xmin + np.array([xr-fs*n_sec, xr]), nn*(1+padding/2) + np.zeros(2), color="k")
     ax.set_ylim([0, nn*(1+padding)])
     ax.invert_yaxis()
     if cax is not None:
         plt.colorbar(im, cax, orientation=cax_orientation)
         if cax_label=="x":
             cax.set_xlabel("z-scored\n ")
         else:
```

### Comparing `rastermap-0.9.3/paper/loaders.py` & `rastermap-0.9.4/paper/loaders.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/metrics.py` & `rastermap-0.9.4/paper/metrics.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/other_upsampling.py` & `rastermap-0.9.4/paper/other_upsampling.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/qrdqn.py` & `rastermap-0.9.4/paper/qrdqn.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/simulations.py` & `rastermap-0.9.4/paper/simulations.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/paper/splitting.ipynb` & `rastermap-0.9.4/paper/splitting.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/__main__.py` & `rastermap-0.9.4/rastermap/__main__.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/cluster.py` & `rastermap-0.9.4/rastermap/cluster.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/gui/colormaps.py` & `rastermap-0.9.4/rastermap/gui/colormaps.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/gui/gui.py` & `rastermap-0.9.4/rastermap/gui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         self.behav_data = None
         self.behav_binary_data = None
         self.behav_bin_plot_list = []
         self.behav_labels = []
         self.behav_binary_labels = []
         self.behav_corr_all = None
         self.zstack = None
-        self.xrange = None
+        self.xrange = slice(0, 100)
         self.file_iscell = None
         self.iscell = None
         self.neuron_pos = None
         self.save_path = None  # Set default to current folder
         self.embedding = None
         self.heatmap = None
         self.sat_slider.setValue([30., 70.])
@@ -465,21 +465,19 @@
         yr0 = min(4, self.nsmooth // 4)
         ym = self.nsmooth // 2
         self.selected = slice(ym - yr0, ym + yr0)
         if len(self.cluster_rois) > 0:
             for i in range(len(self.cluster_rois)):
                 self.p2.removeItem(self.cluster_rois[i])
         self.cluster_rois, self.cluster_slices = [], []
+        if self.neuron_pos is not None or self.behav_data is not None:
+            self.update_scatter(init=True)
         if self.user_clusters is None:
             self.add_cluster()
         self.get_behav_corr() if self.behav_data else None
-        if self.neuron_pos is not None or self.behav_data is not None:
-            self.update_scatter(init=True)
-        elif self.neuron_pos is None and self.scatter_comboBox.currentIndex()==0:
-            self.p5.clear()
         self.p2.show()
         self.p3.show()
 
     def add_cluster(self):
         roi_id = len(self.cluster_rois)
         self.cluster_rois.append(
             guiparts.ClusterROI(self, color=self.colors[roi_id],
@@ -586,37 +584,37 @@
                 self.p5.setLabel("bottom", "correlation")
         else:
             self.update_status_bar("ERROR: please upload behavioral data")
 
     def plot_neuron_pos(self, init=False, roi_id=None):
         if self.neuron_pos is not None:
             ypos, xpos = self.neuron_pos[:, 0], self.neuron_pos[:, 1]
-            self.plot_scatter(ypos, xpos, roi_id=roi_id)
+            self.plot_scatter(ypos, xpos, roi_id=roi_id, init=init)
             if init:
                 self.p5.setLabel("left", "y position")
                 self.p5.setLabel("bottom", "x position")
         else:
             self.update_status_bar("ERROR: please upload neuron position data")
 
-    def plot_scatter(self, x, y, roi_id=None, iplane=0):
+    def plot_scatter(self, x, y, roi_id=None, iplane=0, init=False):
         subsample = max(1, int(len(x)/5000))
         n_pts = len(x) // subsample
         marker_size = int(3 * max(1, 800 / n_pts))
         if self.all_neurons_checkBox.isChecked() and roi_id is None:
             colors = colormaps.gist_ncar[np.linspace(
                 0, 254, len(x)).astype("int")][self.sorting]
             brushes = [pg.mkBrush(color=c) for c in colors[::subsample]]
             self.scatter_plots[iplane][0].setData(x[::subsample], y[::subsample], 
                                                   symbol="o", size=marker_size,
                                                   brush=brushes,
                                                   hoverable=True)
             for i in range(1, nclust_max + 1):
                 self.scatter_plots[iplane][i].setData([], [])
         else:
-            if roi_id is None:
+            if roi_id is None or init:
                 self.scatter_plots[iplane][0].setData(
                     x, y, symbol="o", size=marker_size,
                     brush=pg.mkBrush(color=(180, 180, 180)),
                     hoverable=True)
                 for roi_id in range(nclust_max):
                     if roi_id < len(self.cluster_rois):
                         selected = self.neurons_selected(self.cluster_slices[roi_id])
```

### Comparing `rastermap-0.9.3/rastermap/gui/guiparts.py` & `rastermap-0.9.4/rastermap/gui/guiparts.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/gui/io.py` & `rastermap-0.9.4/rastermap/gui/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import pyqtgraph as pg
 from scipy.stats import zscore
 import scipy.io as sio
 from . import guiparts
 from ..io import _load_iscell, _load_stat, load_activity
 
 def _load_activity_gui(parent, X, Usv, Vsv, xy):
+    parent.reset_variables()
     igood = None
+    parent.neuron_pos = xy
     if X is not None:
         parent.update_status_bar(
             f"activity loaded: {X.shape[0]} samples by {X.shape[1]} timepoints")
         parent.update_status_bar(f"z-scoring activity matrix")
         parent.sp = zscore(X, axis=1)
         _load_iscell_stat(parent)
         del X
@@ -36,29 +38,26 @@
             parent.update_status_bar(
                 f"using voxel positions for xy")
         elif parent.Usv.ndim==2:
             parent.Usv = parent.Usv[igood]
             
         parent.update_status_bar(
             f"PCs of activity loaded: {Usv.shape[0]} samples by {Vsv.shape[0]} timepoints")
-        
+        parent.neuron_pos = xy if (igood is None or xy is None) else xy[igood] 
     else:
         raise ValueError("file missing keys / data")
 
-    parent.neuron_pos = xy if (igood is None or xy is None) else xy[igood]
-
     parent.n_samples = (parent.sp.shape[0] if parent.sp is not None 
                         else parent.Usv.shape[0])
     parent.n_time = (parent.sp.shape[1] if parent.sp is not None 
                         else parent.Vsv.shape[0])
     parent.embedding = np.arange(0, parent.n_samples).astype(np.int64)[:, np.newaxis]
     parent.sorting = np.arange(0, parent.n_samples).astype(np.int64)
     _load_sp(parent)
-
-
+    
 def load_mat(parent, name=None):
     """ load data matrix of neurons by time (*.npy or *.mat)
     
     Note: can only load mat files containing one key assigned to data matrix
     
     """
     if name is None:
@@ -107,15 +106,15 @@
         parent.smooth_limit = None
 
     print(f"setting bin size to {smooth} for visualization")
     parent.smooth.setText(str(smooth))
 
     parent.loaded = True
     parent.plot_activity(init=True)
-
+    
     parent.show()
     parent.loadNd.setEnabled(True)
     parent.loadXY.setEnabled(True)
     parent.runRmap.setEnabled(True)
 
 def get_behav_data(parent):
     dialog = QtWidgets.QDialog()
@@ -291,15 +290,14 @@
         elif len(data) != parent.sp.shape[0]:
             print("ERROR: npy array is not the same length as data ")
 
         if isinstance(data[0], np.ndarray):
             parent.neuron_pos = data
         elif isinstance(data[0], dict):
             parent.neuron_pos = np.array([s["med"] for s in data])
-
         parent.scatter_comboBox.setCurrentIndex(0)
         parent.plot_neuron_pos(init=True)
 
     except Exception as e:
         print("ERROR: this is not a *.npy array :( ")
```

### Comparing `rastermap-0.9.3/rastermap/gui/menus.py` & `rastermap-0.9.4/rastermap/gui/menus.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,11 +75,19 @@
     # Save processed data
     parent.saveProc = QAction("&Save processed data", parent)
     parent.saveProc.setShortcut("Ctrl+S")
     parent.saveProc.triggered.connect(lambda: io.save_proc(parent))
     parent.addAction(parent.saveProc)
     save_menu.addAction(parent.saveProc)
 
+    #help_menu = main_menu.addMenu("&Help")
+    ## Save processed data
+    #helpmenu = QAction("&Save processed data", parent)
+    #parent.saveProc.setShortcut("Ctrl+S")
+    #parent.saveProc.triggered.connect(lambda: io.save_proc(parent))
+    #parent.addAction(parent.saveProc)
+    #save_menu.addAction(parent.saveProc)
+
 
 def export_fig(parent):
     parent.win.scene().contextMenuItem = parent.p0
     parent.win.scene().showExportDialog()
```

### Comparing `rastermap-0.9.3/rastermap/gui/run.py` & `rastermap-0.9.4/rastermap/gui/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         self.error = False
         self.save_text()
         ops_path = os.path.join(os.getcwd(), "rmap_ops.npy")
         np.save(ops_path, self.ops)
         print("Running rastermap with command:")
         cmd = f"-u -W ignore -m rastermap --ops {ops_path} --S {parent.fname}"
         if parent.file_iscell is not None:
-            cmd += f"--iscell {parent.file_iscell}"
+            cmd += f" --iscell {parent.file_iscell}"
         print("python " + cmd)
         self.process.start(sys.executable, cmd.split(" "))
 
     def stop(self):
         self.finish = False
         self.process.kill()
```

### Comparing `rastermap-0.9.3/rastermap/gui/views.py` & `rastermap-0.9.4/rastermap/gui/views.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/io.py` & `rastermap-0.9.4/rastermap/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 print("cannot use xy from file: x and y positions of neurons are not same size as activity")
 
     return X, Usv, Vsv, xy
 
 def load_activity(filename):
     ext = os.path.splitext(filename)[-1]
     print("Loading " + filename)
-    Usv, Vsv = None, None
+    Usv, Vsv, xy = None, None, None
     if ext == ".mat":
         try:
             X = sio.loadmat(filename)
             if isinstance(X, dict):
                 for i, key in enumerate(X.keys()):
                     if key not in ["__header__", "__version__", "__globals__"]:
                         X = X[key]
@@ -104,18 +104,25 @@
                 keys = []
                 for i, key in enumerate(X.keys()):
                     if key not in ["__header__", "__version__", "__globals__"]:
                         keys.append(key)
                 X, Usv, Vsv, xy = _load_dict(X, keys)
     elif ext == ".npy":
         X = np.load(filename, allow_pickle=True)
-        if isinstance(X.item(), dict):
-            dat = X.item()
-            keys = dat.keys()
-            X, Usv, Vsv, xy = _load_dict(dat, keys)
+        try:
+            if isinstance(X.item(), dict):
+                dat = X.item()
+                keys = dat.keys()
+                X, Usv, Vsv, xy = _load_dict(dat, keys)
+        except:
+            print("data matrix:")
+            try:
+                print(X.shape)
+            except:
+                raise ValueError(".npy file does not contain an array or a dictionary")
     elif ext == ".npz":
         dat = np.load(filename, allow_pickle=True)
         keys = dat.files
         X, Usv, Vsv, xy = _load_dict(dat, keys)    
     elif ext == ".nwb":
         X, xy = _load_nwb(filename)
     else:
```

### Comparing `rastermap-0.9.3/rastermap/rastermap.py` & `rastermap-0.9.4/rastermap/rastermap.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/sort.py` & `rastermap-0.9.4/rastermap/sort.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/svd.py` & `rastermap-0.9.4/rastermap/svd.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/upsample.py` & `rastermap-0.9.4/rastermap/upsample.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap/utils.py` & `rastermap-0.9.4/rastermap/utils.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/rastermap.egg-info/PKG-INFO` & `rastermap-0.9.4/rastermap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastermap
-Version: 0.9.3
+Version: 0.9.4
 Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
 Home-page: https://github.com/MouseLand/rastermap
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: carsen.stringer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -99,15 +99,17 @@
 
 The quickest way to start is to open the GUI from a command line terminal. You might need to open an anaconda prompt if you did not add anaconda to the path. Then run:
 
 ~~~sh
 python -m rastermap
 ~~~
 
-To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
+To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). You can also try it out with our demo data available [here](https://osf.io/xn4cm/).
+
+Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
 GUI examples:
```

### Comparing `rastermap-0.9.3/rastermap.egg-info/SOURCES.txt` & `rastermap-0.9.4/rastermap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/setup.py` & `rastermap-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.3/tox.ini` & `rastermap-0.9.4/tox.ini`

 * *Files identical despite different names*

