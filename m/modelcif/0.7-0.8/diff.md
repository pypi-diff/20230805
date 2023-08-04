# Comparing `tmp/modelcif-0.7.tar.gz` & `tmp/modelcif-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelcif-0.7.tar", last modified: Wed Jan 25 20:54:26 2023, max compression
+gzip compressed data, was "modelcif-0.8.tar", last modified: Fri Aug  4 23:29:58 2023, max compression
```

## Comparing `modelcif-0.7.tar` & `modelcif-0.8.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-25 20:54:26.871959 modelcif-0.7/
--rw-r--r--   0 ben        (501) staff       (20)     3797 2023-01-25 20:46:49.000000 modelcif-0.7/ChangeLog.rst
--rw-r--r--   0 ben        (501) staff       (20)     1079 2023-01-09 19:56:30.000000 modelcif-0.7/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)       60 2022-01-27 02:03:30.000000 modelcif-0.7/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     2846 2023-01-25 20:54:26.871547 modelcif-0.7/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     2279 2022-08-03 18:53:08.000000 modelcif-0.7/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-25 20:54:26.858948 modelcif-0.7/examples/
--rw-r--r--   0 ben        (501) staff       (20)      482 2023-01-12 20:02:50.000000 modelcif-0.7/examples/convert_bcif.py
--rw-r--r--   0 ben        (501) staff       (20)     3973 2022-07-07 22:24:51.000000 modelcif-0.7/examples/ligands.py
--rw-r--r--   0 ben        (501) staff       (20)     9161 2023-01-09 19:59:16.000000 modelcif-0.7/examples/mkmodbase.py
--rwxr-xr-x   0 ben        (501) staff       (20)      964 2023-01-24 20:27:38.000000 modelcif-0.7/examples/validate_mmcif.py
--rw-r--r--   0 ben        (501) staff       (20)     1720 2023-01-12 20:39:50.000000 modelcif-0.7/examples/validate_modbase.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-25 20:54:26.863461 modelcif-0.7/modelcif/
--rw-r--r--   0 ben        (501) staff       (20)    22572 2023-01-25 20:33:50.000000 modelcif-0.7/modelcif/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     5215 2022-07-22 20:11:22.000000 modelcif-0.7/modelcif/alignment.py
--rw-r--r--   0 ben        (501) staff       (20)     4374 2022-07-28 23:06:16.000000 modelcif-0.7/modelcif/associated.py
--rw-r--r--   0 ben        (501) staff       (20)     1504 2022-05-09 20:18:06.000000 modelcif-0.7/modelcif/data.py
--rw-r--r--   0 ben        (501) staff       (20)     2434 2022-07-08 07:21:20.000000 modelcif-0.7/modelcif/descriptor.py
--rw-r--r--   0 ben        (501) staff       (20)    38363 2023-01-25 20:32:47.000000 modelcif-0.7/modelcif/dumper.py
--rw-r--r--   0 ben        (501) staff       (20)     4228 2023-01-09 19:59:39.000000 modelcif-0.7/modelcif/model.py
--rw-r--r--   0 ben        (501) staff       (20)     2364 2022-05-09 20:17:50.000000 modelcif-0.7/modelcif/protocol.py
--rw-r--r--   0 ben        (501) staff       (20)     6367 2022-08-03 00:47:42.000000 modelcif-0.7/modelcif/qa_metric.py
--rw-r--r--   0 ben        (501) staff       (20)    38340 2023-01-24 20:34:49.000000 modelcif-0.7/modelcif/reader.py
--rw-r--r--   0 ben        (501) staff       (20)     5821 2022-09-16 22:15:34.000000 modelcif-0.7/modelcif/reference.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-25 20:54:26.865658 modelcif-0.7/modelcif.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2846 2023-01-25 20:54:26.000000 modelcif-0.7/modelcif.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      795 2023-01-25 20:54:26.000000 modelcif-0.7/modelcif.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-01-25 20:54:26.000000 modelcif-0.7/modelcif.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       10 2023-01-25 20:54:26.000000 modelcif-0.7/modelcif.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)        9 2023-01-25 20:54:26.000000 modelcif-0.7/modelcif.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-01-25 20:54:26.872076 modelcif-0.7/setup.cfg
--rwxr-xr-x   0 ben        (501) staff       (20)      997 2023-01-25 20:33:52.000000 modelcif-0.7/setup.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-25 20:54:26.870964 modelcif-0.7/test/
--rw-r--r--   0 ben        (501) staff       (20)     1109 2022-01-26 02:23:01.000000 modelcif-0.7/test/test_alignment.py
--rw-r--r--   0 ben        (501) staff       (20)      444 2022-07-08 07:13:40.000000 modelcif-0.7/test/test_descriptor.py
--rw-r--r--   0 ben        (501) staff       (20)    40637 2023-01-12 19:44:21.000000 modelcif-0.7/test/test_dumper.py
--rw-r--r--   0 ben        (501) staff       (20)     3427 2022-05-04 23:25:17.000000 modelcif-0.7/test/test_edit.py
--rw-r--r--   0 ben        (501) staff       (20)     3818 2023-01-12 20:43:02.000000 modelcif-0.7/test/test_examples.py
--rw-r--r--   0 ben        (501) staff       (20)     7123 2023-01-12 19:44:45.000000 modelcif-0.7/test/test_main.py
--rw-r--r--   0 ben        (501) staff       (20)     1417 2023-01-12 19:53:33.000000 modelcif-0.7/test/test_make_mmcif.py
--rw-r--r--   0 ben        (501) staff       (20)      857 2022-01-26 02:28:45.000000 modelcif-0.7/test/test_model.py
--rw-r--r--   0 ben        (501) staff       (20)     2522 2022-01-26 08:13:23.000000 modelcif-0.7/test/test_qa_metric.py
--rw-r--r--   0 ben        (501) staff       (20)    38395 2023-01-24 21:14:35.000000 modelcif-0.7/test/test_reader.py
--rw-r--r--   0 ben        (501) staff       (20)     1608 2022-01-26 02:30:38.000000 modelcif-0.7/test/test_reference.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-04 23:29:58.606939 modelcif-0.8/
+-rw-r--r--   0 ben        (501) staff       (20)     4063 2023-08-04 23:12:47.000000 modelcif-0.8/ChangeLog.rst
+-rw-r--r--   0 ben        (501) staff       (20)     1079 2023-01-09 19:56:30.000000 modelcif-0.8/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)       60 2022-01-27 02:03:30.000000 modelcif-0.8/MANIFEST.in
+-rw-r--r--   0 ben        (501) staff       (20)     2975 2023-08-04 23:29:58.606437 modelcif-0.8/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     2408 2023-08-04 15:42:30.000000 modelcif-0.8/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-04 23:29:58.591302 modelcif-0.8/examples/
+-rw-r--r--   0 ben        (501) staff       (20)      482 2023-01-12 20:02:50.000000 modelcif-0.8/examples/convert_bcif.py
+-rw-r--r--   0 ben        (501) staff       (20)     3973 2022-07-07 22:24:51.000000 modelcif-0.8/examples/ligands.py
+-rw-r--r--   0 ben        (501) staff       (20)     9161 2023-01-09 19:59:16.000000 modelcif-0.8/examples/mkmodbase.py
+-rwxr-xr-x   0 ben        (501) staff       (20)      964 2023-01-24 20:27:38.000000 modelcif-0.8/examples/validate_mmcif.py
+-rw-r--r--   0 ben        (501) staff       (20)     1720 2023-01-12 20:39:50.000000 modelcif-0.8/examples/validate_modbase.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-04 23:29:58.595682 modelcif-0.8/modelcif/
+-rw-r--r--   0 ben        (501) staff       (20)    22969 2023-08-04 23:16:13.000000 modelcif-0.8/modelcif/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     5215 2022-07-22 20:11:22.000000 modelcif-0.8/modelcif/alignment.py
+-rw-r--r--   0 ben        (501) staff       (20)     4780 2023-02-22 00:10:58.000000 modelcif-0.8/modelcif/associated.py
+-rw-r--r--   0 ben        (501) staff       (20)     1615 2023-02-22 00:11:01.000000 modelcif-0.8/modelcif/data.py
+-rw-r--r--   0 ben        (501) staff       (20)     2434 2022-07-08 07:21:20.000000 modelcif-0.8/modelcif/descriptor.py
+-rw-r--r--   0 ben        (501) staff       (20)    38539 2023-08-04 23:14:31.000000 modelcif-0.8/modelcif/dumper.py
+-rw-r--r--   0 ben        (501) staff       (20)     4228 2023-01-09 19:59:39.000000 modelcif-0.8/modelcif/model.py
+-rw-r--r--   0 ben        (501) staff       (20)     2364 2022-05-09 20:17:50.000000 modelcif-0.8/modelcif/protocol.py
+-rw-r--r--   0 ben        (501) staff       (20)     6367 2022-08-03 00:47:42.000000 modelcif-0.8/modelcif/qa_metric.py
+-rw-r--r--   0 ben        (501) staff       (20)    38726 2023-02-22 00:52:25.000000 modelcif-0.8/modelcif/reader.py
+-rw-r--r--   0 ben        (501) staff       (20)     5821 2022-09-16 22:15:34.000000 modelcif-0.8/modelcif/reference.py
+-rw-r--r--   0 ben        (501) staff       (20)      822 2023-07-31 19:58:48.000000 modelcif-0.8/modelcif/test.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-04 23:29:58.597787 modelcif-0.8/modelcif.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2975 2023-08-04 23:29:58.000000 modelcif-0.8/modelcif.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      812 2023-08-04 23:29:58.000000 modelcif-0.8/modelcif.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-08-04 23:29:58.000000 modelcif-0.8/modelcif.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       10 2023-08-04 23:29:58.000000 modelcif-0.8/modelcif.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)        9 2023-08-04 23:29:58.000000 modelcif-0.8/modelcif.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-08-04 23:29:58.607063 modelcif-0.8/setup.cfg
+-rwxr-xr-x   0 ben        (501) staff       (20)      997 2023-08-04 23:16:16.000000 modelcif-0.8/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-04 23:29:58.605583 modelcif-0.8/test/
+-rw-r--r--   0 ben        (501) staff       (20)     1109 2022-01-26 02:23:01.000000 modelcif-0.8/test/test_alignment.py
+-rw-r--r--   0 ben        (501) staff       (20)      444 2022-07-08 07:13:40.000000 modelcif-0.8/test/test_descriptor.py
+-rw-r--r--   0 ben        (501) staff       (20)    40960 2023-02-22 00:29:05.000000 modelcif-0.8/test/test_dumper.py
+-rw-r--r--   0 ben        (501) staff       (20)     3427 2022-05-04 23:25:17.000000 modelcif-0.8/test/test_edit.py
+-rw-r--r--   0 ben        (501) staff       (20)     3818 2023-01-12 20:43:02.000000 modelcif-0.8/test/test_examples.py
+-rw-r--r--   0 ben        (501) staff       (20)     7334 2023-02-22 00:24:41.000000 modelcif-0.8/test/test_main.py
+-rw-r--r--   0 ben        (501) staff       (20)     1417 2023-01-12 19:53:33.000000 modelcif-0.8/test/test_make_mmcif.py
+-rw-r--r--   0 ben        (501) staff       (20)      857 2022-01-26 02:28:45.000000 modelcif-0.8/test/test_model.py
+-rw-r--r--   0 ben        (501) staff       (20)     2522 2022-01-26 08:13:23.000000 modelcif-0.8/test/test_qa_metric.py
+-rw-r--r--   0 ben        (501) staff       (20)    38913 2023-02-22 00:51:25.000000 modelcif-0.8/test/test_reader.py
+-rw-r--r--   0 ben        (501) staff       (20)     1608 2022-01-26 02:30:38.000000 modelcif-0.8/test/test_reference.py
```

### Comparing `modelcif-0.7/ChangeLog.rst` & `modelcif-0.8/ChangeLog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.8 - 2023-08-04
+================
+ - :class:`modelcif.associated.File` now takes an optional ``data``
+   argument to allow describing any modeling input/output that is stored
+   in that file.
+ - RPM packages are now provided for Fedora and RedHat Enterprise Linux.
+
 0.7 - 2023-01-25
 ================
  - More examples have been added to demonstrate interconversion between
    mmCIF and BinaryCIF, and to validate mmCIF files.
  - A utility script ``util/make-mmcif.py`` has been added which can add
    minimal ModelCIF-related tables to an mmCIF file, to add in deposition.
  - The reader is now more robust when handling files that are not ModelCIF
```

### Comparing `modelcif-0.7/LICENSE` & `modelcif-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/PKG-INFO` & `modelcif-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelcif
-Version: 0.7
+Version: 0.8
 Summary: Package for handling ModelCIF mmCIF and BinaryCIF files
 Home-page: https://github.com/ihmwg/python-modelcif
 Author: Ben Webb
 Author-email: ben@salilab.org
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,20 @@
 
 If you are using [Anaconda Python](https://www.anaconda.com/), install with
 
 ```
 conda install -c conda-forge modelcif
 ```
 
+On a Fedora or RedHat Enterprise Linux box, install with
+
+```
+dnf copr enable salilab/salilab; dnf install python3-modelcif
+```
+
 Alternatively, install with pip:
 
 ```
 pip install modelcif
 ```
 
 # Installation from source code
```

### Comparing `modelcif-0.7/README.md` & `modelcif-0.8/modelcif.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: modelcif
+Version: 0.8
+Summary: Package for handling ModelCIF mmCIF and BinaryCIF files
+Home-page: https://github.com/ihmwg/python-modelcif
+Author: Ben Webb
+Author-email: ben@salilab.org
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5908678.svg)](https://doi.org/10.5281/zenodo.5908678)
 [![docs](https://readthedocs.org/projects/python-modelcif/badge/)](https://python-modelcif.readthedocs.org/)
 [![conda package](https://img.shields.io/conda/vn/conda-forge/modelcif.svg)](https://anaconda.org/conda-forge/modelcif)
 [![pypi package](https://badge.fury.io/py/modelcif.svg)](https://badge.fury.io/py/modelcif)
 [![Linux Build Status](https://github.com/ihmwg/python-modelcif/workflows/build/badge.svg)](https://github.com/ihmwg/python-modelcif/actions?query=workflow%3Abuild)
 [![Windows Build Status](https://ci.appveyor.com/api/projects/status/5o28oe477ii8ur4h?svg=true)](https://ci.appveyor.com/project/benmwebb/python-modelcif)
 [![codecov](https://codecov.io/gh/ihmwg/python-modelcif/branch/main/graph/badge.svg)](https://codecov.io/gh/ihmwg/python-modelcif)
@@ -19,14 +35,20 @@
 
 If you are using [Anaconda Python](https://www.anaconda.com/), install with
 
 ```
 conda install -c conda-forge modelcif
 ```
 
+On a Fedora or RedHat Enterprise Linux box, install with
+
+```
+dnf copr enable salilab/salilab; dnf install python3-modelcif
+```
+
 Alternatively, install with pip:
 
 ```
 pip install modelcif
 ```
 
 # Installation from source code
```

### Comparing `modelcif-0.7/examples/ligands.py` & `modelcif-0.8/examples/ligands.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/examples/mkmodbase.py` & `modelcif-0.8/examples/mkmodbase.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/examples/validate_mmcif.py` & `modelcif-0.8/examples/validate_mmcif.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/examples/validate_modbase.py` & `modelcif-0.8/examples/validate_modbase.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/modelcif/__init__.py` & `modelcif-0.8/modelcif/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 from ihm import Entity, AsymUnit, Software, Assembly, Residue  # noqa: F401
 from ihm import AsymUnitRange, _remove_identical  # noqa: F401
 import modelcif.data
 import sys
 
-__version__ = '0.7'
+__version__ = '0.8'
 
 
 class System(object):
     """Top-level class representing a complete modeled system.
 
        :param str title: Longer text description of the system.
        :param str id: Unique identifier for this system in the mmCIF file.
@@ -220,21 +220,32 @@
 
     def _all_data(self):
         def _all_data_in_groups():
             for dg in self.data_groups:
                 if isinstance(dg, list):
                     for data in dg:
                         yield data
+
+        def _all_data_in_files():
+            for repo in self.repositories:
+                for f in repo.files:
+                    if f.data:
+                        yield f.data
+                    if hasattr(f, 'files'):
+                        for subf in f.files:
+                            if subf.data:
+                                yield subf.data
         return itertools.chain(
             self.data,
             self.templates,
             self.target_entities,
             self.alignments,
             (model for group, model in self._all_models()),
-            _all_data_in_groups())
+            _all_data_in_groups(),
+            _all_data_in_files())
 
     def _all_data_groups(self):
         """Return all DataGroup (or singleton Data) objects"""
         return itertools.chain(
             self.data_groups,
             (step.input_data for p in self.protocols for step in p.steps
              if step.input_data),
@@ -285,15 +296,15 @@
 
 
 # Provide ma-specific docs for Software
 if sys.version_info[0] >= 3:
     Software.__doc__ = """Software used as part of the modeling protocol.
 
 :param str name: The name of the software.
-:param str classification: The major function of the sofware, for
+:param str classification: The major function of the software, for
        example 'model building', 'sample preparation', 'data collection'.
 :param str description: A longer text description of the software.
 :param str location: Place where the software can be found (e.g. URL).
 :param str type: Type of software (program/package/library/other).
 :param str version: The version used.
 :param citation: Publication describing the software.
 :type citation: :class:`ihm.Citation`
```

### Comparing `modelcif-0.7/modelcif/alignment.py` & `modelcif-0.8/modelcif/alignment.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/modelcif/associated.py` & `modelcif-0.8/modelcif/associated.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,30 +29,36 @@
 
 class File(object):
     """A single associated file. These objects can be added to a
        :class:`Repository` or a :class:`ZipFile`.
 
        :param str path: File name.
        :param str details: Any additional information about the file.
+       :param data: If available, the data (e.g. sequence, structure,
+              alignment) that are stored in the file.
+       :type data: :class:`~modelcif.data.Data`
     """
     file_type = 'file'
     file_content = 'other'
     file_format = 'other'
 
-    def __init__(self, path, details=None):
-        self.path, self.details = path, details
+    def __init__(self, path, details=None, data=None):
+        self.path, self.details, self.data = path, details, data
 
 
 class CIFFile(File):
     """An associated file in mmCIF or BinaryCIF format.
        See :class:`File` for more details.
 
        :param str path: File name that will be used to construct URLs in the
               main mmCIF file (see :class:`Repository` or :class:`ZipFile`).
        :param str details: Any additional information about the file.
+       :param data: If available, the data (e.g. sequence, structure,
+              alignment) that are stored in the file.
+       :type data: :class:`~modelcif.data.Data`
        :param list categories: If given, any mmCIF category names in this list
               are written out to ``local_path`` by
               :func:`modelcif.dumper.write` instead of to the primary file
               handle.
        :param list copy_categories: If given, any mmCIF category names in this
               list are written out to both ``local_path`` by
               :func:`modelcif.dumper.write` and the primary file handle.
@@ -70,16 +76,16 @@
 
     _binary_ff_map = {True: 'bcif', False: 'cif'}
 
     file_format = property(lambda self: self._binary_ff_map[self.binary])
 
     def __init__(self, path, details=None, categories=[], copy_categories=[],
                  entry_id='model', entry_details=None, local_path=None,
-                 binary=False):
-        super(CIFFile, self).__init__(path, details)
+                 binary=False, data=None):
+        super(CIFFile, self).__init__(path, details, data)
         self.categories = categories
         self.copy_categories = copy_categories
         self.id = entry_id
         self.entry_details = entry_details
         self.local_path = local_path or path
         self.binary = binary
 
@@ -99,10 +105,10 @@
               within this archive. Note that an archive cannot contain another
               archive.
     """
     file_type = 'archive'
     file_content = 'archive with multiple files'
     file_format = 'zip'
 
-    def __init__(self, path, details=None, files=[]):
-        super(ZipFile, self).__init__(path, details)
+    def __init__(self, path, details=None, files=[], data=None):
+        super(ZipFile, self).__init__(path, details, data)
         self.files = files
```

### Comparing `modelcif-0.7/modelcif/data.py` & `modelcif-0.8/modelcif/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
    See also :class:`modelcif.protocol.Step`.
 """
 
 
 class Data(object):
     """Some part of the system that is input or output by part of
-       the modeling protocol.
+       the modeling protocol, and/or stored in a file.
 
        Usually a subclass is passed to :class:`modelcif.protocol.Step`
-       to describe the input or output:
+       to describe the input or output, or to :class:`modelcif.associated.File`
+       to point to where the data are stored:
 
         - A database of possible template sequences/structures to construct
           or search (:class:`modelcif.ReferenceDatabase`)
         - A template structure (:class:`modelcif.Template`)
         - The sequence of the target (:class:`modelcif.Entity`)
         - A target-template alignment (:mod:`modelcif.alignment`)
         - Target structure coordinates (:class:`modelcif.model.Model`)
```

### Comparing `modelcif-0.7/modelcif/descriptor.py` & `modelcif-0.8/modelcif/descriptor.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/modelcif/dumper.py` & `modelcif-0.8/modelcif/dumper.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     URL = ("https://raw.githubusercontent.com/ihmwg/ModelCIF/%s/base/" +
            "mmcif_ma-core.dic")
 
     def dump(self, system, writer):
         with writer.category("_audit_conform") as lp:
             # Update to match the version of the ModelCIF dictionary
             # we support:
-            lp.write(dict_name="mmcif_ma.dic", dict_version="1.4.4",
-                     dict_location=self.URL % "330c8af")
+            lp.write(dict_name="mmcif_ma.dic", dict_version="1.4.5",
+                     dict_location=self.URL % "ba728c4")
 
 
 class _EntryLinkDumper(Dumper):
     def dump(self, system, writer):
         with writer.loop("_entry_link", ["id", "entry_id", "details"]) as lp:
             lp.write(id=1, entry_id=system.id, details=system.entry_details)
 
@@ -602,36 +602,38 @@
         self.dump_files(system, writer)
         self.dump_archive_files(system, writer)
 
     def dump_files(self, system, writer):
         with writer.loop(
                 "_ma_entry_associated_files",
                 ["id", "entry_id", "file_url", "file_type", "file_format",
-                 "file_content", "details"]) as lp:
+                 "file_content", "details", "data_id"]) as lp:
             for repo in system.repositories:
                 for f in repo.files:
                     lp.write(id=f._id, entry_id=system.id,
                              file_url=repo.get_url(f), file_type=f.file_type,
                              file_format=f.file_format,
-                             file_content=f.file_content, details=f.details)
+                             file_content=f.file_content, details=f.details,
+                             data_id=f.data._data_id if f.data else None)
 
     def dump_archive_files(self, system, writer):
         with writer.loop(
                 "_ma_associated_archive_file_details",
                 ["id", "archive_file_id", "file_path", "file_format",
-                 "file_content", "description"]) as lp:
+                 "file_content", "description", "data_id"]) as lp:
             for repo in system.repositories:
                 for f in repo.files:
                     if not hasattr(f, 'files'):
                         continue
                     for af in f.files:
                         lp.write(id=af._id, archive_file_id=f._id,
                                  file_path=af.path, file_format=af.file_format,
                                  file_content=af.file_content,
-                                 description=af.details)
+                                 description=af.details,
+                                 data_id=af.data._data_id if af.data else None)
 
 
 class _QAMetricDumper(Dumper):
     def finalize(self, system):
         # Get all metric classes used by all systems
         seen_metric_classes = set()
         self._metric_classes_by_id = []
```

### Comparing `modelcif-0.7/modelcif/model.py` & `modelcif-0.8/modelcif/model.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/modelcif/protocol.py` & `modelcif-0.8/modelcif/protocol.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/modelcif/qa_metric.py` & `modelcif-0.8/modelcif/qa_metric.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/modelcif/reader.py` & `modelcif-0.8/modelcif/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -737,51 +737,60 @@
 
     def __init__(self, *args):
         super(_AssociatedHandler, self).__init__(*args)
         self._repos_by_root = {}
         self._type_map, self._binary_type_map = _get_assoc_type_maps()
 
     def __call__(self, id, file_url, file_type, file_format, file_content,
-                 details):
+                 details, data_id):
         filecls = _get_assoc_class(
             file_content, file_format, self._type_map, self._binary_type_map)
         # Assume everything before last slash (if any) is URL root
         url_root, path = posixpath.split(file_url)
         url_root = url_root or None
         r = self._repos_by_root.get(url_root)
         if not r:
             r = modelcif.associated.Repository(url_root=url_root, files=[])
             self._repos_by_root[url_root] = r
             self.system.repositories.append(r)
-        c = filecls(path=path, details=details)
+        c = filecls(path=path, details=details, data=data_id)
         r.files.append(c)
         self.sysr.assoc_by_id[id] = c
 
+    def finalize(self):
+        # Map data_id to Data objects
+        for repo in self.system.repositories:
+            for f in repo.files:
+                f.data = self.sysr.data_by_id.get(f.data)
+
 
 class _AssociatedArchiveHandler(Handler):
     category = '_ma_associated_archive_file_details'
 
     def __init__(self, *args):
         super(_AssociatedArchiveHandler, self).__init__(*args)
         self._type_map, self._binary_type_map = _get_assoc_type_maps()
         self._archive_files = collections.defaultdict(list)
 
     def __call__(self, id, archive_file_id, file_path, file_format,
-                 file_content, description):
+                 file_content, description, data_id):
         filecls = _get_assoc_class(
             file_content, file_format, self._type_map, self._binary_type_map)
-        c = filecls(path=file_path, details=description)
+        c = filecls(path=file_path, details=description, data=data_id)
         # Top-level archive file might not exist yet
         self._archive_files[archive_file_id].append(c)
 
     def finalize(self):
         # Put files in archives
         for archive_file_id, files in self._archive_files.items():
             archive = self.sysr.assoc_by_id.get(archive_file_id)
             if archive:
+                # Map data_id to Data objects
+                for f in files:
+                    f.data = self.sysr.data_by_id.get(f.data)
                 archive.files = files
 
 
 def _make_qa_class(type_class, mode_class, p_name, p_description, p_software):
     """Create and return a new class to represent a QA metric"""
     class QA(type_class, mode_class):
         name = p_name
```

### Comparing `modelcif-0.7/modelcif/reference.py` & `modelcif-0.8/modelcif/reference.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/modelcif.egg-info/PKG-INFO` & `modelcif-0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: modelcif
-Version: 0.7
-Summary: Package for handling ModelCIF mmCIF and BinaryCIF files
-Home-page: https://github.com/ihmwg/python-modelcif
-Author: Ben Webb
-Author-email: ben@salilab.org
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5908678.svg)](https://doi.org/10.5281/zenodo.5908678)
 [![docs](https://readthedocs.org/projects/python-modelcif/badge/)](https://python-modelcif.readthedocs.org/)
 [![conda package](https://img.shields.io/conda/vn/conda-forge/modelcif.svg)](https://anaconda.org/conda-forge/modelcif)
 [![pypi package](https://badge.fury.io/py/modelcif.svg)](https://badge.fury.io/py/modelcif)
 [![Linux Build Status](https://github.com/ihmwg/python-modelcif/workflows/build/badge.svg)](https://github.com/ihmwg/python-modelcif/actions?query=workflow%3Abuild)
 [![Windows Build Status](https://ci.appveyor.com/api/projects/status/5o28oe477ii8ur4h?svg=true)](https://ci.appveyor.com/project/benmwebb/python-modelcif)
 [![codecov](https://codecov.io/gh/ihmwg/python-modelcif/branch/main/graph/badge.svg)](https://codecov.io/gh/ihmwg/python-modelcif)
@@ -35,14 +19,20 @@
 
 If you are using [Anaconda Python](https://www.anaconda.com/), install with
 
 ```
 conda install -c conda-forge modelcif
 ```
 
+On a Fedora or RedHat Enterprise Linux box, install with
+
+```
+dnf copr enable salilab/salilab; dnf install python3-modelcif
+```
+
 Alternatively, install with pip:
 
 ```
 pip install modelcif
 ```
 
 # Installation from source code
```

### Comparing `modelcif-0.7/modelcif.egg-info/SOURCES.txt` & `modelcif-0.8/modelcif.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 modelcif/descriptor.py
 modelcif/dumper.py
 modelcif/model.py
 modelcif/protocol.py
 modelcif/qa_metric.py
 modelcif/reader.py
 modelcif/reference.py
+modelcif/test.py
 modelcif.egg-info/PKG-INFO
 modelcif.egg-info/SOURCES.txt
 modelcif.egg-info/dependency_links.txt
 modelcif.egg-info/requires.txt
 modelcif.egg-info/top_level.txt
 test/test_alignment.py
 test/test_descriptor.py
```

### Comparing `modelcif-0.7/setup.py` & `modelcif-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 import sys
 
-VERSION = "0.7"
+VERSION = "0.8"
 
 copy_args = sys.argv[1:]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='modelcif',
```

### Comparing `modelcif-0.7/test/test_alignment.py` & `modelcif-0.8/test/test_alignment.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/test/test_dumper.py` & `modelcif-0.8/test/test_dumper.py`

 * *Files 0% similar despite different names*

```diff
@@ -839,51 +839,59 @@
 X 42 foo
 #
 """)
 
     def test_associated_dumper(self):
         """Test AssociatedDumper"""
         system = modelcif.System()
+        e = modelcif.Entity('M')
         # File in a repository
         f1 = modelcif.associated.File(path='foo.txt', details='test file')
         # File in an archive
         f2 = modelcif.associated.File(path='bar.txt', details='test file2')
         zf = modelcif.associated.ZipFile(path='t.zip', files=[f2])
-        # Local file
-        f3 = modelcif.associated.File(path='baz.txt', details='test file3')
+        # Local file with data
+        f3 = modelcif.associated.File(path='baz.txt', details='test file3',
+                                      data=e)
         r = modelcif.associated.Repository(url_root='https://example.com',
                                            files=[f1, zf])
         r2 = modelcif.associated.Repository(url_root=None, files=[f3])
         system.repositories.extend((r, r2))
 
+        system._before_write()  # populate data
+        dumper = modelcif.dumper._DataDumper()
+        dumper.finalize(system)  # Assign Data IDs
+
         dumper = modelcif.dumper._AssociatedDumper()
         dumper.finalize(system)
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
 _ma_entry_associated_files.id
 _ma_entry_associated_files.entry_id
 _ma_entry_associated_files.file_url
 _ma_entry_associated_files.file_type
 _ma_entry_associated_files.file_format
 _ma_entry_associated_files.file_content
 _ma_entry_associated_files.details
-1 model https://example.com/foo.txt file other other 'test file'
-2 model https://example.com/t.zip archive zip 'archive with multiple files' .
-3 model baz.txt file other other 'test file3'
+_ma_entry_associated_files.data_id
+1 model https://example.com/foo.txt file other other 'test file' .
+2 model https://example.com/t.zip archive zip 'archive with multiple files' . .
+3 model baz.txt file other other 'test file3' 1
 #
 #
 loop_
 _ma_associated_archive_file_details.id
 _ma_associated_archive_file_details.archive_file_id
 _ma_associated_archive_file_details.file_path
 _ma_associated_archive_file_details.file_format
 _ma_associated_archive_file_details.file_content
 _ma_associated_archive_file_details.description
-1 2 bar.txt other other 'test file2'
+_ma_associated_archive_file_details.data_id
+1 2 bar.txt other other 'test file2' .
 #
 """)
 
         # Should be an error to put a zip file inside another zip
         zf2 = modelcif.associated.ZipFile(path='test2.zip', files=[])
         zf.files.append(zf2)
         self.assertRaises(ValueError, dumper.finalize, system)
```

### Comparing `modelcif-0.7/test/test_edit.py` & `modelcif-0.8/test/test_edit.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/test/test_examples.py` & `modelcif-0.8/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/test/test_main.py` & `modelcif-0.8/test/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import utils
 
 TOPDIR = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 utils.set_search_paths(TOPDIR)
 import modelcif
 import modelcif.protocol
 import modelcif.descriptor
+import modelcif.associated
 import ihm
 
 
 class Tests(unittest.TestCase):
     def test_all_data(self):
         """Test _all_data() method"""
         s = modelcif.System()
@@ -21,17 +22,21 @@
         e3 = modelcif.Entity("A")
         s.data.extend((e1, e3))
 
         s.data_groups.append('something not a group')
         e4 = modelcif.Entity("M")
         s.data_groups.append(modelcif.data.DataGroup([e1, e4]))
 
+        e5 = modelcif.Entity("M")
+        f = modelcif.associated.File(path='foo', details='bar', data=e5)
+        s.repositories.append(modelcif.associated.Repository('/', [f]))
+
         d = s._all_data()
         # List may contain duplicates
-        self.assertEqual(list(d), [e1, e3, e1, e2, e1, e4])
+        self.assertEqual(list(d), [e1, e3, e1, e2, e1, e4, e5])
 
     def test_all_asym_units(self):
         """Test _all_asym_units() method"""
         s = modelcif.System()
         e1 = modelcif.Entity("DDDD")
         e2 = modelcif.Entity("MMMM")
         a1 = modelcif.AsymUnit(e1)
```

### Comparing `modelcif-0.7/test/test_make_mmcif.py` & `modelcif-0.8/test/test_make_mmcif.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/test/test_model.py` & `modelcif-0.8/test/test_model.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/test/test_qa_metric.py` & `modelcif-0.8/test/test_qa_metric.py`

 * *Files identical despite different names*

### Comparing `modelcif-0.7/test/test_reader.py` & `modelcif-0.8/test/test_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -927,39 +927,52 @@
         self.assertIsInstance(p.score, modelcif.alignment.HHblitsEValue)
         self.assertAlmostEqual(p.score.value, 2.0, delta=1e-6)
 
     def test_associated_files(self):
         """Test _AssociatedHandler and _AssociatedArchiveHandler"""
         cif = """
 loop_
+_ma_data.id
+_ma_data.name
+_ma_data.content_type
+_ma_data.content_type_other_details
+42 'Model subunit' target .
+loop_
+_ma_target_entity.entity_id
+_ma_target_entity.data_id
+_ma_target_entity.origin
+1 99 'reference database'
+loop_
 _ma_entry_associated_files.id
 _ma_entry_associated_files.entry_id
 _ma_entry_associated_files.file_url
 _ma_entry_associated_files.file_type
 _ma_entry_associated_files.file_format
 _ma_entry_associated_files.file_content
 _ma_entry_associated_files.details
-1 model https://example.com/foo.txt file other other 'test file'
-2 model https://example.com/t.zip archive zip 'archive with multiple files' .
-3 model baz.txt file other other 'test file3'
-4 model baz.cif file cif other 'test mmCIF'
-5 model baz.bcif file bcif other 'test BinaryCIF'
+_ma_entry_associated_files.data_id
+1 model https://example.com/foo.txt file other other 'test file' .
+2 model https://example.com/t.zip archive zip 'archive with multiple files' . .
+3 model baz.txt file other other 'test file3' .
+4 model baz.cif file cif other 'test mmCIF' .
+5 model baz.bcif file bcif other 'test BinaryCIF' 42
 #
 #
 loop_
 _ma_associated_archive_file_details.id
 _ma_associated_archive_file_details.archive_file_id
 _ma_associated_archive_file_details.file_path
 _ma_associated_archive_file_details.file_format
 _ma_associated_archive_file_details.file_content
 _ma_associated_archive_file_details.description
-1 2 bar.txt other other 'test file2'
-2 99 99.txt other other 'test file99'
-3 2 bar.cif cif other 'test mmCIF in zip'
-4 2 bar.bcif bcif 'local pairwise QA scores' 'test BinaryCIF in zip'
+_ma_associated_archive_file_details.data_id
+1 2 bar.txt other other 'test file2' .
+2 99 99.txt other other 'test file99' .
+3 2 bar.cif cif other 'test mmCIF in zip' .
+4 2 bar.bcif bcif 'local pairwise QA scores' 'test BinaryCIF in zip' 99
 """
         s, = modelcif.reader.read(StringIO(cif))
         r1, r2 = s.repositories
         self.assertEqual(r1.url_root, 'https://example.com')
         f1, zf = r1.files
         self.assertIsInstance(f1, modelcif.associated.File)
         self.assertEqual(f1.path, 'foo.txt')
@@ -968,28 +981,32 @@
         self.assertIsInstance(zf, modelcif.associated.ZipFile)
         self.assertEqual(zf.path, 't.zip')
         self.assertIsNone(zf.details)
 
         f2, f3, f4 = zf.files
         self.assertEqual(f2.path, 'bar.txt')
         self.assertEqual(f2.details, 'test file2')
+        self.assertIsNone(f2.data)
         self.assertIsInstance(f3, modelcif.associated.CIFFile)
         self.assertFalse(f3.binary)
         self.assertIsInstance(
             f4, modelcif.associated.LocalPairwiseQAScoresFile)
         self.assertTrue(f4.binary)
+        self.assertIsInstance(f4.data, modelcif.Entity)
 
         self.assertIsNone(r2.url_root)
         f3, f4, f5 = r2.files
         self.assertEqual(f3.path, 'baz.txt')
         self.assertEqual(f3.details, 'test file3')
         self.assertIsInstance(f4, modelcif.associated.CIFFile)
         self.assertFalse(f4.binary)
+        self.assertIsNone(f4.data)
         self.assertIsInstance(f5, modelcif.associated.CIFFile)
         self.assertTrue(f5.binary)
+        self.assertEqual(f5.data.__class__, modelcif.data.Data)
 
     def test_template_poly_handler(self):
         """Test _TemplatePolyHandler"""
         cif = """
 loop_
 _chem_comp.id
 _chem_comp.type
```

### Comparing `modelcif-0.7/test/test_reference.py` & `modelcif-0.8/test/test_reference.py`

 * *Files identical despite different names*

