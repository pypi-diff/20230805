# Comparing `tmp/msplotter-0.1.32.tar.gz` & `tmp/msplotter-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msplotter-0.1.32.tar", last modified: Thu Jul 27 15:52:58 2023, max compression
+gzip compressed data, was "msplotter-0.1.34.tar", last modified: Fri Aug  4 20:20:31 2023, max compression
```

## Comparing `msplotter-0.1.32.tar` & `msplotter-0.1.34.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.242394 msplotter-0.1.32/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.32/LICENSE
--rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-27 15:52:58.241084 msplotter-0.1.32/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)     4123 2023-07-22 19:56:11.000000 msplotter-0.1.32/README.md
--rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-27 15:24:07.000000 msplotter-0.1.32/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-27 15:52:58.242534 msplotter-0.1.32/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.205446 msplotter-0.1.32/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.217405 msplotter-0.1.32/src/msp/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.32/src/msp/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.32/src/msp/__main__.py
--rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.32/src/msp/arrows.py
--rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.32/src/msp/colormap_picker.py
--rw-r--r--   0 msp        (501) staff       (20)    20747 2023-07-27 15:24:07.000000 msplotter-0.1.32/src/msp/gui.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.235094 msplotter-0.1.32/src/msp/images/
--rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.32/src/msp/images/Blues.png
--rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/BuGn.png
--rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/BuPu.png
--rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/GnBu.png
--rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Greens.png
--rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Greys.png
--rw-r--r--   0 msp        (501) staff       (20)   353491 2023-07-22 04:33:21.000000 msplotter-0.1.32/src/msp/images/MSPlotter_gui.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/OrRd.png
--rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Oranges.png
--rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/PuBu.png
--rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/PuBuGn.png
--rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/PuRd.png
--rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Purples.png
--rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/RdPu.png
--rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Reds.png
--rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlGn.png
--rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlGnBu.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlOrBr.png
--rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlOrRd.png
--rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/logo.png
--rw-r--r--   0 msp        (501) staff       (20)    36197 2023-07-24 05:39:10.000000 msplotter-0.1.32/src/msp/msplotter.py
--rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.32/src/msp/plot.py
--rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.32/src/msp/slider_widget.py
--rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.32/src/msp/spinbox.py
--rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.32/src/msp/user_input.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.239799 msplotter-0.1.32/src/msplotter.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      966 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 20:20:31.442243 msplotter-0.1.34/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.34/LICENSE
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-08-04 20:20:31.441617 msplotter-0.1.34/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)     4123 2023-07-22 19:56:11.000000 msplotter-0.1.34/README.md
+-rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-30 03:33:05.000000 msplotter-0.1.34/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-08-04 20:20:31.442389 msplotter-0.1.34/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 20:20:31.403257 msplotter-0.1.34/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 20:20:31.415289 msplotter-0.1.34/src/msp/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.34/src/msp/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.34/src/msp/__main__.py
+-rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.34/src/msp/arrows.py
+-rw-r--r--   0 msp        (501) staff       (20)     5110 2023-07-30 03:41:21.000000 msplotter-0.1.34/src/msp/colormap_picker.py
+-rw-r--r--   0 msp        (501) staff       (20)    21092 2023-07-30 05:31:09.000000 msplotter-0.1.34/src/msp/gui.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 20:20:31.435743 msplotter-0.1.34/src/msp/images/
+-rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.34/src/msp/images/Blues.png
+-rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/BuGn.png
+-rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/BuPu.png
+-rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/GnBu.png
+-rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/Greens.png
+-rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/Greys.png
+-rw-r--r--   0 msp        (501) staff       (20)   353491 2023-07-22 04:33:21.000000 msplotter-0.1.34/src/msp/images/MSPlotter_gui.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/OrRd.png
+-rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/Oranges.png
+-rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/PuBu.png
+-rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/PuBuGn.png
+-rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/PuRd.png
+-rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/Purples.png
+-rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/RdPu.png
+-rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/Reds.png
+-rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/YlGn.png
+-rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/YlGnBu.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/YlOrBr.png
+-rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/YlOrRd.png
+-rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.34/src/msp/images/logo.png
+-rw-r--r--   0 msp        (501) staff       (20)    37471 2023-07-30 05:27:32.000000 msplotter-0.1.34/src/msp/msplotter.py
+-rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.34/src/msp/plot.py
+-rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.34/src/msp/slider_widget.py
+-rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.34/src/msp/spinbox.py
+-rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.34/src/msp/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 20:20:31.440690 msplotter-0.1.34/src/msplotter.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-08-04 20:20:31.000000 msplotter-0.1.34/src/msplotter.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      966 2023-08-04 20:20:31.000000 msplotter-0.1.34/src/msplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-08-04 20:20:31.000000 msplotter-0.1.34/src/msplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       48 2023-08-04 20:20:31.000000 msplotter-0.1.34/src/msplotter.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)       55 2023-08-04 20:20:31.000000 msplotter-0.1.34/src/msplotter.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        4 2023-08-04 20:20:31.000000 msplotter-0.1.34/src/msplotter.egg-info/top_level.txt
```

### Comparing `msplotter-0.1.32/LICENSE` & `msplotter-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/PKG-INFO` & `msplotter-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.32
+Version: 0.1.34
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.32/README.md` & `msplotter-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/pyproject.toml` & `msplotter-0.1.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msplotter"
-version = "0.1.32"
+version = "0.1.34"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Make a graphical representation of a blastn alignment"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
```

### Comparing `msplotter-0.1.32/src/msp/arrows.py` & `msplotter-0.1.34/src/msp/arrows.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/colormap_picker.py` & `msplotter-0.1.34/src/msp/colormap_picker.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 
 import os
 from pathlib import Path
 from PIL import Image
+from importlib import resources
 
 import customtkinter
 
 from msp.slider_widget import Slider
+import msp
 
 
 class ColormapPicker(customtkinter.CTkToplevel):
 
     cmaps = [
         'Greys', 'Purples', 'Blues', 'Greens', 'Oranges', 'Reds', 'YlOrBr',
         'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu', 'GnBu', 'PuBu', 'YlGnBu',
@@ -89,15 +91,15 @@
         # ############# #
         # Make colormap #
         # ############# #
         # Initialized selected colormap and range_colormap.
         self.selected_colormap = None
         self.range_colormap = None
         # Get path to current directory
-        self.current_dir = Path(os.path.dirname(os.path.realpath(__file__)))
+        self.current_dir = resources.files(msp)
         # Show selected colormap.
         self.update_colormap()
 
         # ################# #
         # show range slider #
         # ################# #
         self.range_slider = Slider(
```

### Comparing `msplotter-0.1.32/src/msp/gui.py` & `msplotter-0.1.34/src/msp/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 License
 -------
 This file is part of MSPloter
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 from pathlib import Path
+from importlib import resources
 
 from tkinter import filedialog
 import customtkinter
 
 import msp.msplotter as msp
 from msp.colormap_picker import ColormapPicker
 from msp.plot import Plot
 from msp.spinbox import FloatSpinbox
+import msp as current_module
 
 class App(customtkinter.CTk):
     """msplotter GUI."""
     def __init__(self):
         super().__init__()
         # -- Variables for BLASTing and plotting ------------------------------
         self.figure_plt = None                 # matplotlib object.
@@ -460,24 +462,29 @@
         self.width_entry.configure(state='disabled')
         self.height_entry.configure(state='normal')
         self.height_entry.delete(0, 'end')
         self.height_entry.configure(state='disabled')
 
     def plot_figure(self):
         """Plot alignments using msplotter."""
+        # Make output path for temporary files.
+        module_path = resources.files(current_module)
+        path_tmp_files = module_path / "tmp_files"
         # Create fasta files for BLASTing.
-        faa_files = msp.make_fasta_file(self.gb_files)
+        faa_files = msp.make_fasta_files(self.gb_files, path_tmp_files)
         # Run blastn locally.
-        xml_results = msp.run_blastn(faa_files)
+        xml_results = msp.run_blastn(faa_files, path_tmp_files)
         # Delete fasta files used for BLASTing.
         msp.delete_files(faa_files)
         # Make a list of `BlastnAlignment` classes from the xml blastn results.
         alignments = msp.get_alignment_records(xml_results)
         # Delete xml documents.
         msp.delete_files(xml_results)
+        # Make sure that tmp_files directory is clean
+        msp.clean_directory(path_tmp_files)
         # Make a list of `GenBankRecord` classes from the gb files.
         gb_records = msp.get_gb_records(self.gb_files)
         # Get figure size
         width, height = self.get_figure_size()
         # Make figure.
         self.figure_msp = msp.MakeFigure(
             alignments,
```

### Comparing `msplotter-0.1.32/src/msp/images/Blues.png` & `msplotter-0.1.34/src/msp/images/Blues.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/BuGn.png` & `msplotter-0.1.34/src/msp/images/BuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/BuPu.png` & `msplotter-0.1.34/src/msp/images/BuPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/GnBu.png` & `msplotter-0.1.34/src/msp/images/GnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/Greens.png` & `msplotter-0.1.34/src/msp/images/Greens.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/MSPlotter_gui.png` & `msplotter-0.1.34/src/msp/images/MSPlotter_gui.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/OrRd.png` & `msplotter-0.1.34/src/msp/images/OrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/Oranges.png` & `msplotter-0.1.34/src/msp/images/Oranges.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/PuBu.png` & `msplotter-0.1.34/src/msp/images/PuBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/PuBuGn.png` & `msplotter-0.1.34/src/msp/images/PuBuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/PuRd.png` & `msplotter-0.1.34/src/msp/images/PuRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/Purples.png` & `msplotter-0.1.34/src/msp/images/Purples.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/RdPu.png` & `msplotter-0.1.34/src/msp/images/RdPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/Reds.png` & `msplotter-0.1.34/src/msp/images/Reds.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/YlGn.png` & `msplotter-0.1.34/src/msp/images/YlGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/YlGnBu.png` & `msplotter-0.1.34/src/msp/images/YlGnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/YlOrBr.png` & `msplotter-0.1.34/src/msp/images/YlOrBr.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/YlOrRd.png` & `msplotter-0.1.34/src/msp/images/YlOrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/images/logo.png` & `msplotter-0.1.34/src/msp/images/logo.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/msplotter.py` & `msplotter-0.1.34/src/msp/msplotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 import os
 import sys
 from pathlib import Path
 from typing import Union
+from importlib import resources
 
 import matplotlib as mpl
 from matplotlib.axes import Axes
 import matplotlib.colors as colors
 from matplotlib.colors import Colormap
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
@@ -33,14 +34,15 @@
 import numpy as np
 from Bio import SeqIO
 from Bio.Blast import NCBIXML
 from Bio.Blast.Applications import NcbiblastnCommandline
 from Bio.SeqRecord import SeqRecord
 
 from msp.arrows import Arrow
+import msp
 
 
 class GenBankRecord:
     """Store relevant info from a GenBank file.
 
     Attributes
     ----------
@@ -204,80 +206,111 @@
         self.hit_to = hit_to
         self.identity = identity
         self.positive = positive
         self.align_len = align_len
         self.homology = identity / align_len
 
 
-def make_fasta_file(gb_files):
-    """Make fasta files from GenBank files and save them in local directory.
+def make_fasta_files(gb_files: list[Path], output_path: Path) -> list[Path]:
+    """Make fasta files from GenBank files.
 
     Parameters
     ----------
-    gb_files : list
-        List of GenBank files.
+    gb_files : list[Path]
+        Paths' list of GenBank files.
+    output_path : Path
+        Path to folder that will store the fasta files.
 
     Returns
     -------
-    faa_files : list
-        List of fasta files names.
+    faa_files : list[Path]
+        Paths' list of fasta files names.
     """
+    # Initiate list to store paths to fasta files.
     faa_files = []
+    # Iterate over paths of gb files.
     for gb_file in gb_files:
+        # Read gb files and make a new record
         record = SeqIO.read(gb_file, "genbank")
-        faa_name = record.name + '.faa'
         new_record = SeqRecord(
             record.seq,
             id=record.id,
             description=record.description
         )
-        SeqIO.write(new_record, faa_name, 'fasta')
-        faa_files.append(faa_name)
+        # Get name of gb file without extension
+        name = gb_file.name.split('.')[0]
+        faa_name = name + '.faa'
+        # Make otuput path
+        output_file = output_path / faa_name
+        # Create fata file
+        SeqIO.write(new_record, output_file, 'fasta')
+        # Append path of fasta file to faa_files list.
+        faa_files.append(output_file)
     return faa_files
 
 
-def run_blastn(faa_files):
+def run_blastn(faa_files: list[Path], output_path: Path) -> list[Path]:
     """Run blastn locally and create xml result file(s).
 
     Parameters
     ----------
-    faa_files : list
-        List of fasta files.
+    faa_files : list[Path]
+        Paths' list of fasta files.
+    output_path : Path
+        Path to save files produced by blastn
 
     Returns
     -------
-    results : list
-        List of xml files' names with blastn results.
+    results : list[Path]
+        Paths' list of xml files with blastn results.
     """
+    # Initiate list to store paths to xml results.
     results = []
+    # Iterate over paths of fasta files.
     for i in range(len(faa_files) - 1):
-        output_file = 'result' + str(i) + '.xml'
+        # Make path to outpu file
+        output_file_name = 'result' + str(i) + '.xml'
+        output_file = output_path / output_file_name
+        # Run blastn
         blastn_cline = NcbiblastnCommandline(
             query=faa_files[i],
             subject=faa_files[i+1],
             outfmt=5,
             out=output_file)
         stdout, stderr = blastn_cline()
+        # Append path to xlm results to the result list
         results.append(output_file)
         print(
             f'BLASTing {faa_files[i]} (query) and {faa_files[i+1]} (subject)\n'
         )
-        # print(stdout + '\n' + stderr)
+        print(stdout + '\n' + stderr)
     return results
 
 
 def delete_files(documents: list) -> None:
     """Delete the files from `documents` list."""
     for document in documents:
         if os.path.exists(document):
             os.remove(document)
         else:
             print(f"File {document} does not exist")
 
 
+def clean_directory(directory_path: Path) -> None:
+    """If directory is not empty, delete all files"""
+    if not any(directory_path.iterdir()):
+        return
+    else:
+        for item in directory_path.glob("*"):
+            if item.is_file():
+                item.unlink()
+            elif item.is_dir():
+                item.rmdir()
+
+
 def get_alignment_records(alignment_files: list) -> list:
     """Parse xml alignment files and make list of `BlastnAlignment` classes."""
     alignments = [BlastnAlignment(alignment) for alignment in alignment_files]
     return alignments
 
 
 def get_gb_records(gb_files: list) -> list:
@@ -906,15 +939,15 @@
     Parameters
     ----------
     user_input : UserInput class object.
     """
     # Get list of input files' paths.
     gb_files = user_input.input_files
     # Create fasta files for BLASTing.
-    faa_files = make_fasta_file(gb_files)
+    faa_files = make_fasta_files(gb_files)
     # Run blastn locally.
     xml_results = run_blastn(faa_files)
     # Delete fasta files used for BLASTing.
     delete_files(faa_files)
     # Make a list of `BlastnAlignment` classes from the xml blastn results.
     alignments = get_alignment_records(xml_results)
     # Delete xml documents.
```

### Comparing `msplotter-0.1.32/src/msp/plot.py` & `msplotter-0.1.34/src/msp/plot.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/slider_widget.py` & `msplotter-0.1.34/src/msp/slider_widget.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/spinbox.py` & `msplotter-0.1.34/src/msp/spinbox.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msp/user_input.py` & `msplotter-0.1.34/src/msp/user_input.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.32/src/msplotter.egg-info/PKG-INFO` & `msplotter-0.1.34/src/msplotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.32
+Version: 0.1.34
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.32/src/msplotter.egg-info/SOURCES.txt` & `msplotter-0.1.34/src/msplotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

