# Comparing `tmp/maroon-0.1.44.tar.gz` & `tmp/maroon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maroon-0.1.44.tar", max compression
+gzip compressed data, was "maroon-0.2.0.tar", max compression
```

## Comparing `maroon-0.1.44.tar` & `maroon-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-07-01 14:35:28.852594 maroon-0.1.44/LICENSE
--rw-r--r--   0        0        0     1037 2023-07-01 14:35:28.852594 maroon-0.1.44/README.md
--rw-r--r--   0        0        0        0 2023-07-01 14:35:28.852594 maroon-0.1.44/maroon/__init__.py
--rw-r--r--   0        0        0     1021 2023-07-01 14:35:28.852594 maroon-0.1.44/maroon/cli.py
--rw-r--r--   0        0        0     1334 2023-07-01 14:35:28.852594 maroon-0.1.44/maroon/cue.py
--rw-r--r--   0        0        0      889 2023-07-01 14:35:28.852594 maroon-0.1.44/maroon/rename.py
--rw-r--r--   0        0        0     5183 2023-07-01 14:35:28.852594 maroon-0.1.44/maroon/transform.py
--rw-r--r--   0        0        0      464 2023-07-01 14:35:28.852594 maroon-0.1.44/pyproject.toml
--rw-r--r--   0        0        0     1703 1970-01-01 00:00:00.000000 maroon-0.1.44/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 22:46:33.666072 maroon-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1295 2023-08-04 22:46:33.666072 maroon-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 22:46:33.666072 maroon-0.2.0/maroon/__init__.py
+-rw-r--r--   0        0        0     1021 2023-08-04 22:46:33.670072 maroon-0.2.0/maroon/cli.py
+-rw-r--r--   0        0        0     1941 2023-08-04 22:46:33.670072 maroon-0.2.0/maroon/cue.py
+-rw-r--r--   0        0        0      889 2023-08-04 22:46:33.670072 maroon-0.2.0/maroon/rename.py
+-rw-r--r--   0        0        0     5193 2023-08-04 22:46:33.670072 maroon-0.2.0/maroon/transform.py
+-rw-r--r--   0        0        0      482 2023-08-04 22:46:33.670072 maroon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 maroon-0.2.0/PKG-INFO
```

### Comparing `maroon-0.1.44/LICENSE` & `maroon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maroon-0.1.44/README.md` & `maroon-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,38 @@
 
 [![Upload Python Package](https://github.com/trojblue/maroon/actions/workflows/python-publish.yml/badge.svg)](https://github.com/trojblue/maroon/actions/workflows/python-publish.yml)
 [![PyPI version](https://badge.fury.io/py/maroon.svg)](https://badge.fury.io/py/maroon)
 [![PyPI - License](https://img.shields.io/pypi/l/maroon)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 ![Python](https://img.shields.io/badge/python-3.10-blue.svg) 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+
+## Features
+convert `wav` and `cue` files into flac tracks, 
+- split tracks into folders according to disc number
+- adding genre info into metadata
+```bash
+maroon format <something.cue>
+```
+sample run:
+```bash
+Name of the album (default: i): 菊花夜行军
+Genre of the album (split by ; sign):Chinese; Folk; Acoustic; Chinese Folk; Avant Folk; Folk Rock
+Splitting CDImage: 100%|██████████| 10/10 [00:07<00:00,  1.37it/s]
+Split 10 tracks.
+```
+
+
 ## Installation
 install from PyPI:
 ```bash
 pip install maroon
 ```
 
 build from source:
 ```bash
 git clone https://github.com/trojblue/maroon
 cd maroon
 poetry install
 poetry build
 pip install dist/<build_version>.whl
 ```
-
-## Usage
-maroon rearranges your subfolders in an album dir into roon-friendly `DISC*/`format, and splits `.cue` files into individual`.flac` files, containing metadata: 
-```bash
-maroon format <album dir>
-```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `maroon-0.1.44/maroon/cli.py` & `maroon-0.2.0/maroon/cli.py`

 * *Files identical despite different names*

### Comparing `maroon-0.1.44/maroon/rename.py` & `maroon-0.2.0/maroon/rename.py`

 * *Files identical despite different names*

### Comparing `maroon-0.1.44/maroon/transform.py` & `maroon-0.2.0/maroon/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,13 +136,13 @@
     transform = Transform(meta)
     transform.process()
     post_process = PostProcess(meta, transform)
     post_process.done()
 
 
 if __name__ == "__main__":
-    cue_path = r"D:\Andrew\Downloads\tmp\存流 - ARU\存流 - ARU.cue"
+    cue_path = r"X:\0音乐\Chinese\交工乐队 - 菊花夜行军\i\CDImage.cue"
     meta = Meta(cue_path)
     transform = Transform(meta)
     transform.process()
     post_process = PostProcess(meta, transform)
     post_process.done()
```

### Comparing `maroon-0.1.44/PKG-INFO` & `maroon-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: maroon
-Version: 0.1.44
+Version: 0.2.0
 Summary: Maroon is a package that manages music for Roon
 License: GPL-3.0
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: mutagen (>=1.46.0,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: tinytag (>=1.9.0,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
@@ -22,14 +23,31 @@
 
 [![Upload Python Package](https://github.com/trojblue/maroon/actions/workflows/python-publish.yml/badge.svg)](https://github.com/trojblue/maroon/actions/workflows/python-publish.yml)
 [![PyPI version](https://badge.fury.io/py/maroon.svg)](https://badge.fury.io/py/maroon)
 [![PyPI - License](https://img.shields.io/pypi/l/maroon)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 ![Python](https://img.shields.io/badge/python-3.10-blue.svg) 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+
+## Features
+convert `wav` and `cue` files into flac tracks, 
+- split tracks into folders according to disc number
+- adding genre info into metadata
+```bash
+maroon format <something.cue>
+```
+sample run:
+```bash
+Name of the album (default: i): 菊花夜行军
+Genre of the album (split by ; sign):Chinese; Folk; Acoustic; Chinese Folk; Avant Folk; Folk Rock
+Splitting CDImage: 100%|██████████| 10/10 [00:07<00:00,  1.37it/s]
+Split 10 tracks.
+```
+
+
 ## Installation
 install from PyPI:
 ```bash
 pip install maroon
 ```
 
 build from source:
@@ -37,13 +55,7 @@
 git clone https://github.com/trojblue/maroon
 cd maroon
 poetry install
 poetry build
 pip install dist/<build_version>.whl
 ```
 
-## Usage
-maroon rearranges your subfolders in an album dir into roon-friendly `DISC*/`format, and splits `.cue` files into individual`.flac` files, containing metadata: 
-```bash
-maroon format <album dir>
-```
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

