# Comparing `tmp/dymoprint-2.0.0b0.tar.gz` & `tmp/dymoprint-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymoprint-2.0.0b0.tar", last modified: Sun Jun 11 11:49:04 2023, max compression
+gzip compressed data, was "dymoprint-2.1.0.tar", last modified: Sat Aug  5 17:09:30 2023, max compression
```

## Comparing `dymoprint-2.0.0b0.tar` & `dymoprint-2.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.989323 dymoprint-2.0.0b0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.989323 dymoprint-2.0.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.989323 dymoprint-2.0.0b0/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.993323 dymoprint-2.0.0b0/data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   690516 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   816716 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   623416 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   635996 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/barcode_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/gui_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/img_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/qr_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/txt_icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.993323 dymoprint-2.0.0b0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/doc/DymoPrint_example_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/doc/DymoPrint_example_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/doc/DymoPrint_example_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/dymoprint.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.993323 dymoprint-2.0.0b0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/src/dymoprint/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/barcode_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5743 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2217 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17404 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/dymo_print_engines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/font_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/q_dymo_label_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/q_dymo_labels_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/unicode_blocks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/src/dymoprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.136375 dymoprint-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.132375 dymoprint-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-05 17:09:10.000000 dymoprint-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.132375 dymoprint-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-05 17:09:10.000000 dymoprint-2.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-05 17:09:10.000000 dymoprint-2.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-05 17:09:10.000000 dymoprint-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-05 17:09:10.000000 dymoprint-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-08-05 17:09:10.000000 dymoprint-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-05 17:09:30.136375 dymoprint-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-08-05 17:09:10.000000 dymoprint-2.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-08-05 17:09:10.000000 dymoprint-2.1.0/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.128374 dymoprint-2.1.0/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.136375 dymoprint-2.1.0/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   690516 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   816716 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   623416 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   635996 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/barcode_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/gui_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/img_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/qr_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-05 17:09:10.000000 dymoprint-2.1.0/data/fonts/txt_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.136375 dymoprint-2.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-08-05 17:09:10.000000 dymoprint-2.1.0/doc/DymoPrint_example_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-08-05 17:09:10.000000 dymoprint-2.1.0/doc/DymoPrint_example_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-08-05 17:09:10.000000 dymoprint-2.1.0/doc/DymoPrint_example_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-05 17:09:10.000000 dymoprint-2.1.0/dymoprint.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-05 17:09:10.000000 dymoprint-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-05 17:09:30.140375 dymoprint-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-05 17:09:10.000000 dymoprint-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.136375 dymoprint-2.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.136375 dymoprint-2.1.0/src/dymoprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/barcode_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5768 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2247 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/dymo_print_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/font_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/q_dymo_label_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/q_dymo_labels_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/unicode_blocks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-08-05 17:09:10.000000 dymoprint-2.1.0/src/dymoprint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:09:30.136375 dymoprint-2.1.0/src/dymoprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-05 17:09:30.000000 dymoprint-2.1.0/src/dymoprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-05 17:09:30.000000 dymoprint-2.1.0/src/dymoprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:09:30.000000 dymoprint-2.1.0/src/dymoprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-05 17:09:30.000000 dymoprint-2.1.0/src/dymoprint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-05 17:09:30.000000 dymoprint-2.1.0/src/dymoprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-05 17:09:30.000000 dymoprint-2.1.0/src/dymoprint.egg-info/top_level.txt
```

### Comparing `dymoprint-2.0.0b0/.github/workflows/pypi-publish.yml` & `dymoprint-2.1.0/.github/workflows/pypi-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
       run: |
         python -m pip install --upgrade pip build twine
         python -m build
     - name: Test wheels
       run: |
         python -m twine check dist/*
     - name: Publish
-      uses: pypa/gh-action-pypi-publish@v1.8.6
+      uses: pypa/gh-action-pypi-publish@v1.8.8
       with:
         user: ${{ secrets.PYPI_USERNAME }}
         password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `dymoprint-2.0.0b0/.github/workflows/tests.yml` & `dymoprint-2.1.0/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
   pull_request:
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.7, 3.11]
 
     steps:
-    - uses: actions/checkout@v1
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
```

### Comparing `dymoprint-2.0.0b0/.gitignore` & `dymoprint-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/.pre-commit-config.yaml` & `dymoprint-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/LICENSE` & `dymoprint-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/PKG-INFO` & `dymoprint-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: dymoprint
-Version: 2.0.0b0
+Version: 2.1.0
 Summary: Linux Software to print with LabelManager PnP from Dymo
 Home-page: https://github.com/computerlyrik/dymoprint
 Author: Sebastian J. Bronner
 Author-email: waschtl@sbronner.com
 Maintainer: Ben Mares
 Maintainer-email: services-dymoprint@tensorial.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/computerlyrik/dymoprint
 Project-URL: Tracker, https://github.com/computerlyrik/dymoprint/issues
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Printing
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # dymoprint
 
@@ -29,25 +31,30 @@
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
 * Cloned to Github and formerly maintained by @computerlyrik: <https://github.com/computerlyrik/dymoprint>
 * Currently maintained by @maresb
 
 ## Features
 
-* Works on python 3.7 and up
-* Supports text printing
-* Supports qr code printing
-* Supports barcode printing
-* Supports image printing
-* Supports combined barcode / qrcode and text printing
-* GUI Application based on PyQt6 - expanded combinations
+* Text printing
+* QR code printing
+* Barcode printing
+* Image printing
+* Combinations of the above
+* GUI Application based on PyQt6
+
+### Experimental
+
+* LabelPoint 350
+* LabelManager 280
+* LabelManager 420P
+* LabelManager Wireless PnP
+* Windows support by setting the driver to WinUSB using [Zadig](https://zadig.akeo.ie/)
 
-## HELP WANTED
-
-Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
+For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -61,15 +68,28 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
-## Experimental features
+By default, users don't have permission to access generic USB devices, so you will
+need to add a rule. The first time you run `dymoprint`, it will give instructions
+about how to do this:
+
+```bash
+$ dymoprint "Hello world"
+...
+You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
+
+  echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-dymo-1001.rules
+...
+```
+
+## Testing experimental features
 
 To install a test branch, by user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/dymoprint@branchname
 ```
 
@@ -92,77 +112,14 @@
 This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
-## Configuration
-
-### For ubuntu based distributions
-
-Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
-**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
-
-```bash
-sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
-sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
-```
-
-and restart services with:
-
-```bash
-sudo systemctl restart udev.service
-```
-
-Finally, physically disconnect and reconnect the LabelManager PnP.
-
-([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
-
-### For arch based distributions
-
-(should also work for manjaro, but not tested yet)
-use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
-**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
-
-Install **usb_modeswitch** at first:
-
-```bash
-sudo pacman -S usb_modeswitch
-```
-
-if the **/etc/usb_modeswitch.d/** folder was not created at installation do:
-
-```bash
-sudo mkdir /etc/usb_modeswitch.d/
-````
-
-now copy the udev and usb_modswitch configs:
-
-```bash
-sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
-sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
-```
-
-and restart services with:
-
-```bash
-sudo udevadm control --reload
-```
-
-you might need to change the permissions of the hid device (dymoprint will tell if it is the case):
-
-```bash
-sudo chown your_user:users /dev/hidraw0
-```
-
-Finally, physically disconnect and reconnect the LabelManager PnP.
-
-([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
-
 ## Font management
 
 Fonts are managed via [dymoprint.ini](dymoprint.ini). This should be placed in your
 config folder (normally `~/.config`). An example file is provided here.
 
 You may choose any TTF Font you like
 
@@ -265,18 +222,21 @@
 dymoprint -c code128 Tst && \
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
-* (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
+* ~~(?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?~~
 * ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
 * ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
+* refactor code with better abstractions
+* pixel fonts
+* web interface
```

### Comparing `dymoprint-2.0.0b0/README.md` & `dymoprint-2.1.0/src/dymoprint.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,60 @@
+Metadata-Version: 2.1
+Name: dymoprint
+Version: 2.1.0
+Summary: Linux Software to print with LabelManager PnP from Dymo
+Home-page: https://github.com/computerlyrik/dymoprint
+Author: Sebastian J. Bronner
+Author-email: waschtl@sbronner.com
+Maintainer: Ben Mares
+Maintainer-email: services-dymoprint@tensorial.com
+License: Apache License 2.0
+Project-URL: Source, https://github.com/computerlyrik/dymoprint
+Project-URL: Tracker, https://github.com/computerlyrik/dymoprint/issues
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Printing
+Requires-Python: <4,>=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
 # dymoprint
 
 [![GitHub Actions (Tests)](https://github.com/computerlyrik/dymoprint/workflows/Tests/badge.svg)](https://github.com/computerlyrik/dymoprint)
 [![PyPI version](https://img.shields.io/pypi/v/dymoprint.svg)](https://pypi.org/project/dymoprint/)
 
 Linux Software to print with LabelManager PnP from Dymo
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
 * Cloned to Github and formerly maintained by @computerlyrik: <https://github.com/computerlyrik/dymoprint>
 * Currently maintained by @maresb
 
 ## Features
 
-* Works on python 3.7 and up
-* Supports text printing
-* Supports qr code printing
-* Supports barcode printing
-* Supports image printing
-* Supports combined barcode / qrcode and text printing
-* GUI Application based on PyQt6 - expanded combinations
-
-## HELP WANTED
+* Text printing
+* QR code printing
+* Barcode printing
+* Image printing
+* Combinations of the above
+* GUI Application based on PyQt6
+
+### Experimental
+
+* LabelPoint 350
+* LabelManager 280
+* LabelManager 420P
+* LabelManager Wireless PnP
+* Windows support by setting the driver to WinUSB using [Zadig](https://zadig.akeo.ie/)
 
-Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
+For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -39,15 +68,28 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
-## Experimental features
+By default, users don't have permission to access generic USB devices, so you will
+need to add a rule. The first time you run `dymoprint`, it will give instructions
+about how to do this:
+
+```bash
+$ dymoprint "Hello world"
+...
+You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
+
+  echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-dymo-1001.rules
+...
+```
+
+## Testing experimental features
 
 To install a test branch, by user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/dymoprint@branchname
 ```
 
@@ -70,77 +112,14 @@
 This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
-## Configuration
-
-### For ubuntu based distributions
-
-Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
-**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
-
-```bash
-sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
-sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
-```
-
-and restart services with:
-
-```bash
-sudo systemctl restart udev.service
-```
-
-Finally, physically disconnect and reconnect the LabelManager PnP.
-
-([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
-
-### For arch based distributions
-
-(should also work for manjaro, but not tested yet)
-use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
-**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
-
-Install **usb_modeswitch** at first:
-
-```bash
-sudo pacman -S usb_modeswitch
-```
-
-if the **/etc/usb_modeswitch.d/** folder was not created at installation do:
-
-```bash
-sudo mkdir /etc/usb_modeswitch.d/
-````
-
-now copy the udev and usb_modswitch configs:
-
-```bash
-sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
-sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
-```
-
-and restart services with:
-
-```bash
-sudo udevadm control --reload
-```
-
-you might need to change the permissions of the hid device (dymoprint will tell if it is the case):
-
-```bash
-sudo chown your_user:users /dev/hidraw0
-```
-
-Finally, physically disconnect and reconnect the LabelManager PnP.
-
-([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
-
 ## Font management
 
 Fonts are managed via [dymoprint.ini](dymoprint.ini). This should be placed in your
 config folder (normally `~/.config`). An example file is provided here.
 
 You may choose any TTF Font you like
 
@@ -243,18 +222,21 @@
 dymoprint -c code128 Tst && \
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
-* (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
+* ~~(?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?~~
 * ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
 * ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
+* refactor code with better abstractions
+* pixel fonts
+* web interface
```

### Comparing `dymoprint-2.0.0b0/TODO.md` & `dymoprint-2.1.0/TODO.md`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/Carlito-Bold.ttf` & `dymoprint-2.1.0/data/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/Carlito-BoldItalic.ttf` & `dymoprint-2.1.0/data/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/Carlito-Italic.ttf` & `dymoprint-2.1.0/data/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/Carlito-Regular.ttf` & `dymoprint-2.1.0/data/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/LICENSE` & `dymoprint-2.1.0/data/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/barcode_icon.png` & `dymoprint-2.1.0/data/fonts/barcode_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/gui_icon.png` & `dymoprint-2.1.0/data/fonts/gui_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/img_icon.png` & `dymoprint-2.1.0/data/fonts/img_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/data/fonts/txt_icon.png` & `dymoprint-2.1.0/data/fonts/txt_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/doc/DymoPrint_example_1.png` & `dymoprint-2.1.0/doc/DymoPrint_example_1.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/doc/DymoPrint_example_2.png` & `dymoprint-2.1.0/doc/DymoPrint_example_2.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/doc/DymoPrint_example_3.png` & `dymoprint-2.1.0/doc/DymoPrint_example_3.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/pyproject.toml` & `dymoprint-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 profile = "black"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
   py37
-  py38
-  py39
+  py311
 
 [gh-actions]
 python =
     3.7: py37
-    3.8: py38
-    3.9: py39
+    3.11: py311
 
 [testenv]
 commands =
   pip check
   pip freeze
   dymoprint --version
   dymoprint --help
```

### Comparing `dymoprint-2.0.0b0/setup.cfg` & `dymoprint-2.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 license_file = LICENSE
 classifiers = 
 	Operating System :: POSIX :: Linux
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Printing
 project_urls = 
 	Source = https://github.com/computerlyrik/dymoprint
 	Tracker = https://github.com/computerlyrik/dymoprint/issues
 
 [options]
 package_dir = 
@@ -28,15 +30,15 @@
 packages = 
 	dymoprint
 	dymoprint_fonts
 include_package_data = True
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	appdirs
-	Pillow>=8.1.2,<10
+	Pillow>=8.1.2,<11
 	PyQRCode>=1.2.1,<2
 	python-barcode>=0.13.1,<1
 	pyusb
 	PyQt6
 	PyQt6-tools
 python_requires = >=3.7,<4
 setup_requires =
```

### Comparing `dymoprint-2.0.0b0/setup.py` & `dymoprint-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/README.md` & `dymoprint-2.1.0/src/README.md`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint/barcode_writer.py` & `dymoprint-2.1.0/src/dymoprint/barcode_writer.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint/command_line.py` & `dymoprint-2.1.0/src/dymoprint/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,17 @@
     )
     parser.add_argument(
         "--scale", type=int, default=90, help="Scaling font factor, [0,10] [%%]"
     )
     parser.add_argument(
         "-t",
         type=int,
-        choices=[6, 9, 12],
+        choices=[6, 9, 12, 19],
         default=12,
-        help="Tape size: 6,9,12 mm, default=12mm",
+        help="Tape size: 6,9,12,19 mm, default=12mm",
     )
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     print_server = DymoPrinterServer()
@@ -188,8 +188,8 @@
         label_image.paste(label_bitmap, (margin, 0))
         if args.preview or args.preview_inverted:
             label_rotated = label_bitmap.transpose(Image.ROTATE_270)
             print(image_to_unicode(label_rotated, invert=args.preview_inverted))
         if args.imagemagick:
             ImageOps.invert(label_image).show()
     else:
-        print_server.print_label(label_bitmap, margin=args.m)
+        print_server.print_label(label_bitmap, margin=args.m, tape_size=args.t)
```

### Comparing `dymoprint-2.0.0b0/src/dymoprint/constants.py` & `dymoprint-2.1.0/src/dymoprint/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "Linux Software to print with LabelManager PnP from Dymo\nwritten in Python"
 )
 UNCONFIRMED_MESSAGE = (
     "WARNING: This device is not confirmed to work with this software. Please "
     "report your experiences in https://github.com/computerlyrik/dymoprint/issues/44"
 )
 SUPPORTED_PRODUCTS = {
+    0x0015: "LabelPoint 350",
     0x1001: "LabelManager PnP (no mode switch)",
     0x1002: "LabelManager PnP (mode switch)",
     0x1003: f"LabelManager 420P (no mode switch) {UNCONFIRMED_MESSAGE}",
     0x1004: f"LabelManager 420P (mode switch) {UNCONFIRMED_MESSAGE}",
     0x1005: "LabelManager 280 (no mode switch)",
     0x1006: "LabelManager 280 (no mode switch)",
     0x1007: f"LabelManager Wireless PnP (no mode switch) {UNCONFIRMED_MESSAGE}",
```

### Comparing `dymoprint-2.0.0b0/src/dymoprint/dymo_print_engines.py` & `dymoprint-2.1.0/src/dymoprint/dymo_print_engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,15 @@
     lines.append("")
     udev_rule = ", ".join(
         [
             'ACTION=="add"',
             'SUBSYSTEMS=="usb"',
             f'ATTRS{{idVendor}}=="{dev.idVendor:04x}"',
             f'ATTRS{{idProduct}}=="{dev.idProduct:04x}"',
-            'MODE="0660"',
-            'GROUP="plugdev"',
-            'TAG+="uaccess"',
+            'MODE="0666"',
         ]
     )
     lines.append(
         f"  echo '{udev_rule}' "
         f"| sudo tee /etc/udev/rules.d/91-dymo-{dev.idProduct:x}.rules"
     )
     lines.append("")
@@ -263,17 +261,17 @@
         font_offset = int((line_height - fontsize) / 2)
 
         if frame_width:
             frame_width = min(frame_width, font_offset)
             frame_width = min(frame_width, 3)
 
         font = ImageFont.truetype(font_file_name, fontsize)
-        label_width = max(font.getsize(line)[0] for line in labeltext) + (
-            font_offset * 2
-        )
+        boxes = (font.getbbox(line) for line in labeltext)
+        line_widths = (right - left for left, _, right, _ in boxes)
+        label_width = max(line_widths) + (font_offset * 2)
         text_bitmap = Image.new("1", (label_width, label_height))
         with draw_image(text_bitmap) as label_draw:
             # draw frame into empty image
             if frame_width:
                 label_draw.rectangle(
                     ((0, 4), (label_width - 1, label_height - 4)), fill=255
                 )
```

### Comparing `dymoprint-2.0.0b0/src/dymoprint/font_config.py` & `dymoprint-2.1.0/src/dymoprint/font_config.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint/gui.py` & `dymoprint-2.1.0/src/dymoprint/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,17 +65,19 @@
         shadow = QGraphicsDropShadowEffect()
         shadow.setBlurRadius(15)
         self.label_render.setGraphicsEffect(shadow)
 
         self.margin.setMinimum(20)
         self.margin.setMaximum(1000)
         self.margin.setValue(DEFAULT_MARGIN)
+        self.tape_size.addItem("19", 19)
         self.tape_size.addItem("12", 12)
         self.tape_size.addItem("9", 9)
         self.tape_size.addItem("6", 6)
+        self.tape_size.setCurrentIndex(1)
         self.min_label_len.setMinimum(0)
         self.min_label_len.setMaximum(1000)
         self.justify.addItems(["center", "left", "right"])
 
         self.foreground_color.addItems(
             ["black", "white", "yellow", "blue", "red", "green"]
         )
@@ -156,15 +158,17 @@
         p.end()
 
         self.label_render.setPixmap(q_image)
         self.label_render.adjustSize()
 
     def print_label(self):
         try:
-            self.print_server.print_label(self.label_bitmap, self.margin.value())
+            self.print_server.print_label(
+                self.label_bitmap, self.margin.value(), self.tape_size.currentData()
+            )
         except (RuntimeError, USBError) as err:
             print(traceback.format_exc())
             QMessageBox.warning(
                 self, "Printing Failed!", f"{err}\n\n{traceback.format_exc()}"
             )
```

### Comparing `dymoprint-2.0.0b0/src/dymoprint/labeler.py` & `dymoprint-2.1.0/src/dymoprint/labeler.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint/q_dymo_label_widgets.py` & `dymoprint-2.1.0/src/dymoprint/q_dymo_label_widgets.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint/q_dymo_labels_list.py` & `dymoprint-2.1.0/src/dymoprint/q_dymo_labels_list.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint/unicode_blocks.py` & `dymoprint-2.1.0/src/dymoprint/unicode_blocks.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint/utils.py` & `dymoprint-2.1.0/src/dymoprint/utils.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0b0/src/dymoprint.egg-info/PKG-INFO` & `dymoprint-2.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,36 @@
-Metadata-Version: 2.1
-Name: dymoprint
-Version: 2.0.0b0
-Summary: Linux Software to print with LabelManager PnP from Dymo
-Home-page: https://github.com/computerlyrik/dymoprint
-Author: Sebastian J. Bronner
-Author-email: waschtl@sbronner.com
-Maintainer: Ben Mares
-Maintainer-email: services-dymoprint@tensorial.com
-License: Apache License 2.0
-Project-URL: Source, https://github.com/computerlyrik/dymoprint
-Project-URL: Tracker, https://github.com/computerlyrik/dymoprint/issues
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Printing
-Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
-
 # dymoprint
 
 [![GitHub Actions (Tests)](https://github.com/computerlyrik/dymoprint/workflows/Tests/badge.svg)](https://github.com/computerlyrik/dymoprint)
 [![PyPI version](https://img.shields.io/pypi/v/dymoprint.svg)](https://pypi.org/project/dymoprint/)
 
 Linux Software to print with LabelManager PnP from Dymo
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
 * Cloned to Github and formerly maintained by @computerlyrik: <https://github.com/computerlyrik/dymoprint>
 * Currently maintained by @maresb
 
 ## Features
 
-* Works on python 3.7 and up
-* Supports text printing
-* Supports qr code printing
-* Supports barcode printing
-* Supports image printing
-* Supports combined barcode / qrcode and text printing
-* GUI Application based on PyQt6 - expanded combinations
-
-## HELP WANTED
+* Text printing
+* QR code printing
+* Barcode printing
+* Image printing
+* Combinations of the above
+* GUI Application based on PyQt6
+
+### Experimental
+
+* LabelPoint 350
+* LabelManager 280
+* LabelManager 420P
+* LabelManager Wireless PnP
+* Windows support by setting the driver to WinUSB using [Zadig](https://zadig.akeo.ie/)
 
-Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
+For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -61,15 +44,28 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
-## Experimental features
+By default, users don't have permission to access generic USB devices, so you will
+need to add a rule. The first time you run `dymoprint`, it will give instructions
+about how to do this:
+
+```bash
+$ dymoprint "Hello world"
+...
+You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
+
+  echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-dymo-1001.rules
+...
+```
+
+## Testing experimental features
 
 To install a test branch, by user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/dymoprint@branchname
 ```
 
@@ -92,77 +88,14 @@
 This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
-## Configuration
-
-### For ubuntu based distributions
-
-Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
-**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
-
-```bash
-sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
-sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
-```
-
-and restart services with:
-
-```bash
-sudo systemctl restart udev.service
-```
-
-Finally, physically disconnect and reconnect the LabelManager PnP.
-
-([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
-
-### For arch based distributions
-
-(should also work for manjaro, but not tested yet)
-use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
-**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
-
-Install **usb_modeswitch** at first:
-
-```bash
-sudo pacman -S usb_modeswitch
-```
-
-if the **/etc/usb_modeswitch.d/** folder was not created at installation do:
-
-```bash
-sudo mkdir /etc/usb_modeswitch.d/
-````
-
-now copy the udev and usb_modswitch configs:
-
-```bash
-sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
-sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
-```
-
-and restart services with:
-
-```bash
-sudo udevadm control --reload
-```
-
-you might need to change the permissions of the hid device (dymoprint will tell if it is the case):
-
-```bash
-sudo chown your_user:users /dev/hidraw0
-```
-
-Finally, physically disconnect and reconnect the LabelManager PnP.
-
-([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
-
 ## Font management
 
 Fonts are managed via [dymoprint.ini](dymoprint.ini). This should be placed in your
 config folder (normally `~/.config`). An example file is provided here.
 
 You may choose any TTF Font you like
 
@@ -265,18 +198,21 @@
 dymoprint -c code128 Tst && \
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
-* (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
+* ~~(?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?~~
 * ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
 * ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
+* refactor code with better abstractions
+* pixel fonts
+* web interface
```

### Comparing `dymoprint-2.0.0b0/src/dymoprint.egg-info/SOURCES.txt` & `dymoprint-2.1.0/src/dymoprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

