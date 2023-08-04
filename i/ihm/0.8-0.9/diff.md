# Comparing `tmp/ihm-0.8.tar.gz` & `tmp/ihm-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ihm-0.8.tar", last modified: Tue May 28 23:25:17 2019, max compression
+gzip compressed data, was "dist/ihm-0.9.tar", last modified: Fri May 31 23:10:41 2019, max compression
```

## Comparing `ihm-0.8.tar` & `ihm-0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2019-05-28 23:25:17.000000 ihm-0.8/
--rw-r--r--   0 ben        (501) staff       (20)       84 2019-05-28 23:21:35.000000 ihm-0.8/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     3568 2019-05-28 23:25:17.000000 ihm-0.8/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     2500 2019-05-08 19:45:22.000000 ihm-0.8/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2019-05-28 23:25:17.000000 ihm-0.8/ihm/
--rw-r--r--   0 ben        (501) staff       (20)    49126 2019-05-28 23:21:32.000000 ihm-0.8/ihm/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     8836 2018-03-03 00:58:40.000000 ihm-0.8/ihm/_compat_collections.py
--rw-r--r--   0 ben        (501) staff       (20)     3096 2018-06-05 20:29:33.000000 ihm-0.8/ihm/analysis.py
--rw-r--r--   0 ben        (501) staff       (20)     1365 2019-03-20 03:11:38.000000 ihm-0.8/ihm/cross_linkers.py
--rw-r--r--   0 ben        (501) staff       (20)     3932 2019-05-08 19:45:22.000000 ihm-0.8/ihm/dataset.py
--rw-r--r--   0 ben        (501) staff       (20)    14170 2019-05-08 19:45:22.000000 ihm-0.8/ihm/dictionary.py
--rw-r--r--   0 ben        (501) staff       (20)   122598 2019-05-28 22:37:04.000000 ihm-0.8/ihm/dumper.py
--rw-r--r--   0 ben        (501) staff       (20)    38951 2019-05-28 22:46:16.000000 ihm-0.8/ihm/flr.py
--rw-r--r--   0 ben        (501) staff       (20)    24732 2019-05-08 19:45:22.000000 ihm-0.8/ihm/format.py
--rw-r--r--   0 ben        (501) staff       (20)    19946 2019-05-08 19:45:22.000000 ihm-0.8/ihm/format_bcif.py
--rw-r--r--   0 ben        (501) staff       (20)     7489 2019-04-10 17:29:55.000000 ihm-0.8/ihm/geometry.py
--rw-r--r--   0 ben        (501) staff       (20)    13166 2019-05-08 05:21:23.000000 ihm-0.8/ihm/location.py
--rw-r--r--   0 ben        (501) staff       (20)    22557 2019-03-21 23:08:12.000000 ihm-0.8/ihm/metadata.py
--rw-r--r--   0 ben        (501) staff       (20)    14548 2019-05-08 19:45:22.000000 ihm-0.8/ihm/model.py
--rw-r--r--   0 ben        (501) staff       (20)     2526 2018-06-05 20:29:33.000000 ihm-0.8/ihm/protocol.py
--rw-r--r--   0 ben        (501) staff       (20)   118422 2019-05-28 23:09:38.000000 ihm-0.8/ihm/reader.py
--rw-r--r--   0 ben        (501) staff       (20)     4681 2019-05-08 19:45:22.000000 ihm-0.8/ihm/representation.py
--rw-r--r--   0 ben        (501) staff       (20)    26553 2019-05-08 18:26:06.000000 ihm-0.8/ihm/restraint.py
--rw-r--r--   0 ben        (501) staff       (20)     1710 2019-03-21 23:08:12.000000 ihm-0.8/ihm/source.py
--rw-r--r--   0 ben        (501) staff       (20)     9427 2019-05-08 19:45:22.000000 ihm-0.8/ihm/startmodel.py
--rw-r--r--   0 ben        (501) staff       (20)     1248 2019-05-08 19:45:22.000000 ihm-0.8/ihm/util.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2019-05-28 23:25:17.000000 ihm-0.8/ihm.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     3568 2019-05-28 23:25:17.000000 ihm-0.8/ihm.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1040 2019-05-28 23:25:17.000000 ihm-0.8/ihm.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2019-05-28 23:25:17.000000 ihm-0.8/ihm.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)        8 2019-05-28 23:25:17.000000 ihm-0.8/ihm.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)        4 2019-05-28 23:25:17.000000 ihm-0.8/ihm.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       38 2019-05-28 23:25:17.000000 ihm-0.8/setup.cfg
--rwxr-xr-x   0 ben        (501) staff       (20)     2056 2019-05-28 23:21:38.000000 ihm-0.8/setup.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2019-05-28 23:25:17.000000 ihm-0.8/src/
--rw-r--r--   0 ben        (501) staff       (20)    40956 2019-05-08 19:45:22.000000 ihm-0.8/src/ihm_format.c
--rw-r--r--   0 ben        (501) staff       (20)     6791 2019-05-08 19:45:22.000000 ihm-0.8/src/ihm_format.h
--rw-r--r--   0 ben        (501) staff       (20)    14666 2019-05-08 19:45:22.000000 ihm-0.8/src/ihm_format.i
--rw-r--r--   0 ben        (501) staff       (20)   178065 2019-05-28 23:25:15.000000 ihm-0.8/src/ihm_format_wrap_0.8.c
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2019-05-28 23:25:17.000000 ihm-0.8/test/
--rw-r--r--   0 ben        (501) staff       (20)     2214 2019-05-23 17:07:01.000000 ihm-0.8/test/test_analysis.py
--rw-r--r--   0 ben        (501) staff       (20)      525 2019-01-04 22:53:29.000000 ihm-0.8/test/test_cross_linkers.py
--rw-r--r--   0 ben        (501) staff       (20)     7439 2019-05-23 17:07:12.000000 ihm-0.8/test/test_dataset.py
--rw-r--r--   0 ben        (501) staff       (20)    13216 2019-05-23 17:07:45.000000 ihm-0.8/test/test_dictionary.py
--rw-r--r--   0 ben        (501) staff       (20)   136578 2019-05-28 22:46:18.000000 ihm-0.8/test/test_dumper.py
--rw-r--r--   0 ben        (501) staff       (20)      731 2019-05-08 19:45:22.000000 ihm-0.8/test/test_edit.py
--rw-r--r--   0 ben        (501) staff       (20)     3053 2019-05-08 19:45:22.000000 ihm-0.8/test/test_examples.py
--rw-r--r--   0 ben        (501) staff       (20)    61054 2019-05-28 22:51:26.000000 ihm-0.8/test/test_flr.py
--rw-r--r--   0 ben        (501) staff       (20)    29543 2019-05-09 02:52:05.000000 ihm-0.8/test/test_format.py
--rw-r--r--   0 ben        (501) staff       (20)    26271 2019-05-23 17:09:30.000000 ihm-0.8/test/test_format_bcif.py
--rw-r--r--   0 ben        (501) staff       (20)     5013 2019-05-23 17:10:56.000000 ihm-0.8/test/test_geometry.py
--rw-r--r--   0 ben        (501) staff       (20)     9967 2019-05-23 17:11:23.000000 ihm-0.8/test/test_location.py
--rw-r--r--   0 ben        (501) staff       (20)    31322 2019-05-24 21:58:07.000000 ihm-0.8/test/test_main.py
--rw-r--r--   0 ben        (501) staff       (20)    16390 2019-05-23 17:14:26.000000 ihm-0.8/test/test_metadata.py
--rw-r--r--   0 ben        (501) staff       (20)     5656 2019-05-23 17:14:46.000000 ihm-0.8/test/test_model.py
--rw-r--r--   0 ben        (501) staff       (20)      707 2019-05-23 17:14:56.000000 ihm-0.8/test/test_protocol.py
--rw-r--r--   0 ben        (501) staff       (20)   122067 2019-05-28 22:50:08.000000 ihm-0.8/test/test_reader.py
--rw-r--r--   0 ben        (501) staff       (20)     2478 2019-05-23 17:23:02.000000 ihm-0.8/test/test_representation.py
--rw-r--r--   0 ben        (501) staff       (20)     8325 2019-05-23 17:24:15.000000 ihm-0.8/test/test_restraint.py
--rw-r--r--   0 ben        (501) staff       (20)     3761 2019-05-08 19:45:22.000000 ihm-0.8/test/test_startmodel.py
--rw-r--r--   0 ben        (501) staff       (20)     2340 2018-09-25 15:39:21.000000 ihm-0.8/test/test_util.py
+drwxr-xr-x   0 ben      (11000) sali       (455)        0 2019-05-31 23:10:41.000000 ihm-0.9/
+-rw-r--r--   0 ben      (11000) sali       (455)       84 2019-05-31 23:08:02.000000 ihm-0.9/MANIFEST.in
+-rw-r--r--   0 ben      (11000) sali       (455)     3568 2019-05-31 23:10:41.000000 ihm-0.9/PKG-INFO
+-rw-r--r--   0 ben      (11000) sali       (455)     2500 2019-05-09 00:38:13.000000 ihm-0.9/README.md
+drwxr-xr-x   0 ben      (11000) sali       (455)        0 2019-05-31 23:10:41.000000 ihm-0.9/ihm/
+-rw-r--r--   0 ben      (11000) sali       (455)    49882 2019-05-31 23:07:59.000000 ihm-0.9/ihm/__init__.py
+-rw-r--r--   0 ben      (11000) sali       (455)     8836 2019-05-03 20:53:28.000000 ihm-0.9/ihm/_compat_collections.py
+-rw-r--r--   0 ben      (11000) sali       (455)     3096 2019-05-03 20:53:28.000000 ihm-0.9/ihm/analysis.py
+-rw-r--r--   0 ben      (11000) sali       (455)     1712 2019-05-31 22:14:34.000000 ihm-0.9/ihm/cross_linkers.py
+-rw-r--r--   0 ben      (11000) sali       (455)     4558 2019-05-31 20:30:22.000000 ihm-0.9/ihm/dataset.py
+-rw-r--r--   0 ben      (11000) sali       (455)    14170 2019-05-09 00:38:13.000000 ihm-0.9/ihm/dictionary.py
+-rw-r--r--   0 ben      (11000) sali       (455)   125952 2019-05-31 21:32:39.000000 ihm-0.9/ihm/dumper.py
+-rw-r--r--   0 ben      (11000) sali       (455)    38951 2019-05-28 23:10:10.000000 ihm-0.9/ihm/flr.py
+-rw-r--r--   0 ben      (11000) sali       (455)    24732 2019-05-09 00:38:13.000000 ihm-0.9/ihm/format.py
+-rw-r--r--   0 ben      (11000) sali       (455)    19946 2019-05-09 00:38:13.000000 ihm-0.9/ihm/format_bcif.py
+-rw-r--r--   0 ben      (11000) sali       (455)     7489 2019-05-03 20:53:28.000000 ihm-0.9/ihm/geometry.py
+-rw-r--r--   0 ben      (11000) sali       (455)    13166 2019-05-08 21:20:22.000000 ihm-0.9/ihm/location.py
+-rw-r--r--   0 ben      (11000) sali       (455)    22557 2019-05-03 20:53:28.000000 ihm-0.9/ihm/metadata.py
+-rw-r--r--   0 ben      (11000) sali       (455)    14548 2019-05-09 00:38:13.000000 ihm-0.9/ihm/model.py
+-rw-r--r--   0 ben      (11000) sali       (455)     2526 2019-05-03 20:53:28.000000 ihm-0.9/ihm/protocol.py
+-rw-r--r--   0 ben      (11000) sali       (455)   121025 2019-05-31 22:50:41.000000 ihm-0.9/ihm/reader.py
+-rw-r--r--   0 ben      (11000) sali       (455)     5154 2019-05-31 20:30:22.000000 ihm-0.9/ihm/representation.py
+-rw-r--r--   0 ben      (11000) sali       (455)    26553 2019-05-08 21:20:22.000000 ihm-0.9/ihm/restraint.py
+-rw-r--r--   0 ben      (11000) sali       (455)     1710 2019-05-03 20:53:28.000000 ihm-0.9/ihm/source.py
+-rw-r--r--   0 ben      (11000) sali       (455)     9514 2019-05-31 20:30:16.000000 ihm-0.9/ihm/startmodel.py
+-rw-r--r--   0 ben      (11000) sali       (455)     1386 2019-05-31 20:30:16.000000 ihm-0.9/ihm/util.py
+drwxr-xr-x   0 ben      (11000) sali       (455)        0 2019-05-31 23:10:41.000000 ihm-0.9/ihm.egg-info/
+-rw-r--r--   0 ben      (11000) sali       (455)     3568 2019-05-31 23:10:40.000000 ihm-0.9/ihm.egg-info/PKG-INFO
+-rw-r--r--   0 ben      (11000) sali       (455)     1040 2019-05-31 23:10:40.000000 ihm-0.9/ihm.egg-info/SOURCES.txt
+-rw-r--r--   0 ben      (11000) sali       (455)        1 2019-05-31 23:10:40.000000 ihm-0.9/ihm.egg-info/dependency_links.txt
+-rw-r--r--   0 ben      (11000) sali       (455)        8 2019-05-31 23:10:40.000000 ihm-0.9/ihm.egg-info/requires.txt
+-rw-r--r--   0 ben      (11000) sali       (455)        4 2019-05-31 23:10:40.000000 ihm-0.9/ihm.egg-info/top_level.txt
+-rw-r--r--   0 ben      (11000) sali       (455)       38 2019-05-31 23:10:41.000000 ihm-0.9/setup.cfg
+-rwxr-xr-x   0 ben      (11000) sali       (455)     2056 2019-05-31 23:08:05.000000 ihm-0.9/setup.py
+drwxr-xr-x   0 ben      (11000) sali       (455)        0 2019-05-31 23:10:41.000000 ihm-0.9/src/
+-rw-r--r--   0 ben      (11000) sali       (455)    40956 2019-05-09 00:38:13.000000 ihm-0.9/src/ihm_format.c
+-rw-r--r--   0 ben      (11000) sali       (455)     6791 2019-05-09 00:38:13.000000 ihm-0.9/src/ihm_format.h
+-rw-r--r--   0 ben      (11000) sali       (455)    14666 2019-05-09 00:38:13.000000 ihm-0.9/src/ihm_format.i
+-rw-r--r--   0 ben      (11000) sali       (455)   185508 2019-05-31 23:10:37.000000 ihm-0.9/src/ihm_format_wrap_0.9.c
+drwxr-xr-x   0 ben      (11000) sali       (455)        0 2019-05-31 23:10:41.000000 ihm-0.9/test/
+-rw-r--r--   0 ben      (11000) sali       (455)     2214 2019-05-28 23:10:11.000000 ihm-0.9/test/test_analysis.py
+-rw-r--r--   0 ben      (11000) sali       (455)      525 2019-05-03 20:53:28.000000 ihm-0.9/test/test_cross_linkers.py
+-rw-r--r--   0 ben      (11000) sali       (455)     7439 2019-05-31 20:03:06.000000 ihm-0.9/test/test_dataset.py
+-rw-r--r--   0 ben      (11000) sali       (455)    13216 2019-05-28 23:10:11.000000 ihm-0.9/test/test_dictionary.py
+-rw-r--r--   0 ben      (11000) sali       (455)   140226 2019-05-31 20:59:56.000000 ihm-0.9/test/test_dumper.py
+-rw-r--r--   0 ben      (11000) sali       (455)      855 2019-05-31 20:30:16.000000 ihm-0.9/test/test_edit.py
+-rw-r--r--   0 ben      (11000) sali       (455)     3053 2019-05-31 20:30:22.000000 ihm-0.9/test/test_examples.py
+-rw-r--r--   0 ben      (11000) sali       (455)    61054 2019-05-28 23:10:11.000000 ihm-0.9/test/test_flr.py
+-rw-r--r--   0 ben      (11000) sali       (455)    29543 2019-05-22 22:13:53.000000 ihm-0.9/test/test_format.py
+-rw-r--r--   0 ben      (11000) sali       (455)    26271 2019-05-28 23:10:11.000000 ihm-0.9/test/test_format_bcif.py
+-rw-r--r--   0 ben      (11000) sali       (455)     5013 2019-05-28 23:10:11.000000 ihm-0.9/test/test_geometry.py
+-rw-r--r--   0 ben      (11000) sali       (455)     9967 2019-05-28 23:10:11.000000 ihm-0.9/test/test_location.py
+-rw-r--r--   0 ben      (11000) sali       (455)    32416 2019-05-31 20:30:16.000000 ihm-0.9/test/test_main.py
+-rw-r--r--   0 ben      (11000) sali       (455)    16390 2019-05-28 23:10:11.000000 ihm-0.9/test/test_metadata.py
+-rw-r--r--   0 ben      (11000) sali       (455)     5656 2019-05-28 23:10:11.000000 ihm-0.9/test/test_model.py
+-rw-r--r--   0 ben      (11000) sali       (455)      707 2019-05-28 23:10:11.000000 ihm-0.9/test/test_protocol.py
+-rw-r--r--   0 ben      (11000) sali       (455)   124454 2019-05-31 22:49:50.000000 ihm-0.9/test/test_reader.py
+-rw-r--r--   0 ben      (11000) sali       (455)     2478 2019-05-28 23:10:11.000000 ihm-0.9/test/test_representation.py
+-rw-r--r--   0 ben      (11000) sali       (455)     8325 2019-05-28 23:10:11.000000 ihm-0.9/test/test_restraint.py
+-rw-r--r--   0 ben      (11000) sali       (455)     3826 2019-05-31 20:30:22.000000 ihm-0.9/test/test_startmodel.py
+-rw-r--r--   0 ben      (11000) sali       (455)     2340 2019-05-03 20:53:28.000000 ihm-0.9/test/test_util.py
```

### Comparing `ihm-0.8/PKG-INFO` & `ihm-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihm
-Version: 0.8
+Version: 0.9
 Summary: Package for handling IHM mmCIF and BinaryCIF files
 Home-page: https://github.com/ihmwg/python-ihm
 Author: Ben Webb
 Author-email: ben@salilab.org
 License: UNKNOWN
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2603378.svg)](https://doi.org/10.5281/zenodo.2603378)
         [![docs](https://readthedocs.org/projects/python-ihm/badge/)](https://python-ihm.readthedocs.org/)
```

### Comparing `ihm-0.8/README.md` & `ihm-0.9/README.md`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/__init__.py` & `ihm-0.9/ihm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Handle different naming of urllib in Python 2/3
 try:
     import urllib.request as urllib2
 except ImportError:
     import urllib2
 import json
 
-__version__ = '0.8'
+__version__ = '0.9'
 
 class __UnknownValue(object):
     # Represent the mmCIF 'unknown' special value
 
     def __str__(self):
         return '?'
     __repr__ = __str__
@@ -373,29 +373,31 @@
                 for alld in _all_datasets_and_parents(p):
                     yield alld
             yield d
         for d in self._all_datasets_except_parents():
             for alld in _all_datasets_and_parents(d):
                 yield alld
 
+    def _all_densities(self):
+        for ensemble in self.ensembles:
+            for density in ensemble.densities:
+                yield density
+
     def _all_locations(self):
         """Iterate over all Locations in the system.
            This includes all Locations referenced from other objects, plus
            any referenced from the top-level system.
            Duplicates may be present."""
-        def all_densities():
-            for ensemble in self.ensembles:
-                for density in ensemble.densities:
-                    yield density
         return itertools.chain(
                 self.locations,
                 (dataset.location for dataset in self._all_datasets()
                           if hasattr(dataset, 'location') and dataset.location),
                 (ensemble.file for ensemble in self.ensembles if ensemble.file),
-                (density.file for density in all_densities() if density.file),
+                (density.file for density in self._all_densities()
+                              if density.file),
                 (sm.script_file for sm in self._all_starting_models()
                                          if sm.script_file),
                 (template.alignment_file for template in self._all_templates()
                                          if template.alignment_file),
                 (step.script_file for step in self._all_protocol_steps()
                                            if step.script_file),
                 (step.script_file for step in self._all_analysis_steps()
@@ -447,14 +449,27 @@
         return _remove_identical(itertools.chain(
                         self.citations,
                         (restraint.fitting_method_citation_id
                             for restraint in self.restraints
                             if hasattr(restraint, 'fitting_method_citation_id')
                             and restraint.fitting_method_citation_id)))
 
+    def _all_entity_ranges(self):
+        """Iterate over all Entity ranges in the system (these may be
+           :class:`Entity`, :class:`AsymUnit`, :class:`EntityRange` or
+           :class:`AsymUnitRange` objects).
+           Note that we don't include self.entities or self.asym_units here,
+           as we only want ranges that were actually used.
+           Duplicates may be present."""
+        return (itertools.chain(
+                        (sm.asym_unit for sm in self._all_starting_models()),
+                        (seg.asym_unit for seg in self._all_segments()),
+                        (comp for a in self._all_assemblies() for comp in a),
+                        (d.asym_unit for d in self._all_densities())))
+
     def _make_complete_assembly(self):
         """Fill in the complete assembly with all entities/asym units"""
         # Clear out any existing components
         self.complete_assembly[:] = []
 
         # Include all asym units
         seen_entities = {}
```

### Comparing `ihm-0.8/ihm/_compat_collections.py` & `ihm-0.9/ihm/_compat_collections.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/analysis.py` & `ihm-0.9/ihm/analysis.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/cross_linkers.py` & `ihm-0.9/ihm/cross_linkers.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,12 +17,18 @@
               smiles='C1C(C(=O)N(C1=O)OC(=O)CCCCCCC(=O)ON2C(=O)CC(C2=O)S(=O)'
                      '(=O)O)S(=O)(=O)O',
               inchi='1S/C16H20N2O14S2/c19-11-7-9(33(25,26)27)15(23)17(11)31'
                     '-13(21)5-3-1-2-4-6-14(22)32-18-12(20)8-10(16(18)24)'
                     '34(28,29)30/h9-10H,1-8H2,(H,25,26,27)(H,28,29,30)',
               inchi_key='VYLDEYYOISNGST-UHFFFAOYSA-N')
 
+dsso = ihm.ChemDescriptor('DSSO', chemical_name='disuccinimidyl sulfoxide',
+              smiles='O=C(CCS(CCC(ON1C(CCC1=O)=O)=O)=O)ON2C(CCC2=O)=O',
+              inchi='1S/C14H16N2O9S/c17-9-1-2-10(18)15(9)24-13(21)5-7-'
+                    '26(23)8-6-14(22)25-16-11(19)3-4-12(16)20/h1-8H2',
+              inchi_key='XJSVVHDQSGMHAJ-UHFFFAOYSA-N')
+
 edc = ihm.ChemDescriptor('EDC',
               chemical_name='1-ethyl-3-(3-dimethylaminopropyl)carbodiimide',
               smiles='CCN=C=NCCCN(C)C',
               inchi='1S/C8H17N3/c1-4-9-8-10-6-5-7-11(2)3/h4-7H2,1-3H3',
               inchi_key='LMDZBCPBFSXMTL-UHFFFAOYSA-N')
```

### Comparing `ihm-0.8/ihm/dataset.py` & `ihm-0.9/ihm/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,20 +47,33 @@
         root.parents.append(dataset)
 
 
 class DatasetGroup(list):
     """A set of :class:`Dataset` objects that are handled together.
        This is implemented as a simple list.
 
+       :param sequence elements: Initial set of datasets.
+       :param str name: Short text name of this group.
+       :param str application: Text that shows how this group is used.
+       :param str details: Longer text that describes this group.
+
        Normally a group is passed to one or more :class:`~ihm.protocol.Protocol`
        or :class:`~ihm.analysis.Analysis` objects, although unused groups
        can still be included in the file if desired by adding them to
        :attr:`ihm.System.orphan_dataset_groups`.
     """
-    pass
+
+    # For backwards compatibility with earlier versions of this class which
+    # didn't specify name/application/details
+    name = application = details = None
+
+    def __init__(self, elements=(), name=None, application=None, details=None):
+        super(DatasetGroup, self).__init__(elements)
+        self.name, self.application = name, application
+        self.details = details
 
 
 class CXMSDataset(Dataset):
     """Processed cross-links from a CX-MS experiment"""
     data_type = 'CX-MS data'
```

### Comparing `ihm-0.8/ihm/dictionary.py` & `ihm-0.9/ihm/dictionary.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/dumper.py` & `ihm-0.9/ihm/dumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,53 @@
             for entity in system.entities:
                 if not entity.is_polymeric():
                     continue
                 for num, comp in enumerate(entity.sequence):
                     l.write(entity_id=entity._id, num=num + 1, mon_id=comp.id)
 
 
+class _EntityPolySegmentDumper(Dumper):
+    def finalize(self, system):
+        seen_ranges = {}
+        self._ranges_by_id = []
+        # Need to assign ranges for all starting models too
+        for sm in system._all_starting_models():
+            rng = sm._get_seq_id_range_all_templates()
+            util._remove_id(rng, attr='_range_id')
+            sm._all_template_rng = rng
+
+        for rng in system._all_entity_ranges():
+            util._remove_id(rng, attr='_range_id')
+        for rng in itertools.chain(system._all_entity_ranges(),
+                                   (sm._all_template_rng
+                                    for sm in system._all_starting_models())):
+            entity = rng.entity if hasattr(rng, 'entity') else rng
+            if entity.is_polymeric():
+                util._assign_id(rng, seen_ranges, self._ranges_by_id,
+                                attr='_range_id',
+                                # Two ranges are considered the same if they
+                                # have the same entity ID and refer to
+                                # the same residue range
+                                seen_obj=(entity._id, rng.seq_id_range))
+            else:
+                rng._range_id = None
+
+    def dump(self, system, writer):
+        with writer.loop("_ihm_entity_poly_segment",
+                         ["id", "entity_id", "seq_id_begin", "seq_id_end",
+                          "comp_id_begin", "comp_id_end"]) as l:
+            for rng in self._ranges_by_id:
+                entity = rng.entity if hasattr(rng, 'entity') else rng
+                l.write(id=rng._range_id, entity_id=entity._id,
+                        seq_id_begin=rng.seq_id_range[0],
+                        seq_id_end=rng.seq_id_range[1],
+                        comp_id_begin=entity.sequence[rng.seq_id_range[0]-1].id,
+                        comp_id_end=entity.sequence[rng.seq_id_range[1]-1].id)
+
+
 class _PolySeqSchemeDumper(Dumper):
     """Output the _pdbx_poly_seq_scheme table.
        This is needed because it is a parent category of atom_site.
        For now we assume we're using auth_seq_num==pdb_seq_num."""
     def dump(self, system, writer):
         with writer.loop("_pdbx_poly_seq_scheme",
                          ["asym_id", "entity_id", "seq_id", "mon_id",
@@ -493,17 +532,14 @@
             for asym in system.asym_units:
                 l.write(id=asym._id, entity_id=asym.entity._id,
                         details=asym.details)
 
 
 class _AssemblyDumper(Dumper):
     def finalize(self, system):
-        # Fill in complete assembly
-        system._make_complete_assembly()
-
         # Sort each assembly by entity/asym id/range
         def component_key(comp):
             if hasattr(comp, 'entity'): # asymmetric unit or range
                 return (comp.entity._id, comp._ordinal, comp.seq_id_range)
             else: # entity or range
                 return (comp._id, 0, comp.seq_id_range)
         for a in system._all_assemblies():
@@ -535,44 +571,42 @@
         # composite description
         for a_id, description in description_by_id.items():
             description_by_id[a_id] = ' & '.join(description) \
                                       if description else None
         for a in all_assemblies:
             a.description = description_by_id[a._id]
 
-    def dump_details(self, system, writer):
-        with writer.loop("_ihm_struct_assembly_details",
-                         ["assembly_id", "assembly_name",
-                          "assembly_description"]) as l:
-            for a in self._assembly_by_id:
-                l.write(assembly_id=a._id, assembly_name=a.name,
-                        assembly_description=a.description)
-
     def dump(self, system, writer):
+        self.dump_summary(system, writer)
         self.dump_details(system, writer)
-        ordinal = 1
+
+    def dump_summary(self, system, writer):
         with writer.loop("_ihm_struct_assembly",
-                         ["ordinal_id", "assembly_id", "parent_assembly_id",
-                          "entity_description",
-                          "entity_id", "asym_id", "seq_id_begin",
-                          "seq_id_end"]) as l:
+                         ["id", "name", "description"]) as l:
+            for a in self._assembly_by_id:
+                l.write(id=a._id, name=a.name, description=a.description)
+
+    def dump_details(self, system, writer):
+        ordinal = 1
+        with writer.loop("_ihm_struct_assembly_details",
+                         ["id", "assembly_id", "parent_assembly_id",
+                          "entity_description", "entity_id", "asym_id",
+                          "entity_poly_segment_id"]) as l:
             for a in self._assembly_by_id:
                 for comp in a:
                     entity = comp.entity if hasattr(comp, 'entity') else comp
-                    seqrange = comp.seq_id_range
-                    l.write(ordinal_id=ordinal, assembly_id=a._id,
+                    l.write(id=ordinal, assembly_id=a._id,
                             # if no hierarchy then assembly is self-parent
                             parent_assembly_id=a.parent._id if a.parent
                                                else a._id,
                             entity_description=entity.description,
                             entity_id=entity._id,
                             asym_id=comp._id if hasattr(comp, 'entity')
                                              else None,
-                            seq_id_begin=seqrange[0],
-                            seq_id_end=seqrange[1])
+                            entity_poly_segment_id=comp._range_id)
                     ordinal += 1
 
 class _ExternalReferenceDumper(Dumper):
     """Output information on externally referenced files
        (i.e. anything that refers to a Location that isn't
        a DatabaseLocation)."""
 
@@ -677,33 +711,42 @@
                           "details"]) as l:
             for d in self._dataset_by_id:
                 l.write(id=d._id, data_type=d.data_type, details=d.details,
                         database_hosted=isinstance(d.location,
                                                    location.DatabaseLocation))
         self.dump_groups(writer)
         self.dump_other((d for d in self._dataset_by_id
-                         if not isinstance(d.location,
+                         if d.location is not None
+                         and not isinstance(d.location,
                                            location.DatabaseLocation)),
                         writer)
         self.dump_rel_dbs((d for d in self._dataset_by_id
                            if isinstance(d.location,
                                          location.DatabaseLocation)),
                           writer)
         self.dump_related(system, writer)
 
     def dump_groups(self, writer):
-        ordinal = 1
+        self.dump_group_summary(writer)
+        self.dump_group_links(writer)
+
+    def dump_group_summary(self, writer):
         with writer.loop("_ihm_dataset_group",
-                         ["ordinal_id", "group_id", "dataset_list_id"]) as l:
+                         ["id", "name", "application", "details"]) as l:
+            for g in self._dataset_group_by_id:
+                l.write(id=g._id, name=g.name, application=g.application,
+                        details=g.details)
+
+    def dump_group_links(self, writer):
+        with writer.loop("_ihm_dataset_group_link",
+                         ["group_id", "dataset_list_id"]) as l:
             for g in self._dataset_group_by_id:
                 # Don't duplicate IDs, and output in sorted order
                 for dataset_id in sorted(set(d._id for d in g)):
-                    l.write(ordinal_id=ordinal, group_id=g._id,
-                            dataset_list_id=dataset_id)
-                    ordinal += 1
+                    l.write(group_id=g._id, dataset_list_id=dataset_id)
 
     def dump_other(self, datasets, writer):
         ordinal = 1
         with writer.loop("_ihm_dataset_external_reference",
                          ["id", "dataset_list_id", "file_id"]) as l:
             for d in datasets:
                 l.write(id=ordinal, dataset_list_id=d._id,
@@ -720,53 +763,58 @@
                         db_name=d.location.db_name,
                         accession_code=d.location.access_code,
                         version=d.location.version,
                         details=d.location.details)
                 ordinal += 1
 
     def dump_related(self, system, writer):
-        ordinal = 1
         with writer.loop("_ihm_related_datasets",
-                         ["ordinal_id", "dataset_list_id_derived",
+                         ["dataset_list_id_derived",
                           "dataset_list_id_primary"]) as l:
             for derived in self._dataset_by_id:
                 # Don't duplicate IDs, and output in sorted order
                 for parent_id in sorted(set(d._id for d in derived.parents)):
-                    l.write(ordinal_id=ordinal,
-                            dataset_list_id_derived=derived._id,
+                    l.write(dataset_list_id_derived=derived._id,
                             dataset_list_id_primary=parent_id)
-                    ordinal += 1
 
 class _ModelRepresentationDumper(Dumper):
     def finalize(self, system):
         # Assign IDs to representations and segments
         for nr, r in enumerate(system._all_representations()):
             r._id = nr + 1
             for ns, s in enumerate(r):
                 s._id = ns + 1
 
     def dump(self, system, writer):
-        ordinal_id = 1
+        self.dump_summary(system, writer)
+        self.dump_details(system, writer)
+
+    def dump_summary(self, system, writer):
         with writer.loop("_ihm_model_representation",
-                         ["ordinal_id", "representation_id",
-                          "segment_id", "entity_id", "entity_description",
-                          "entity_asym_id",
-                          "seq_id_begin", "seq_id_end",
+                         ["id", "name", "details"]) as l:
+            for r in system._all_representations():
+                l.write(id=r._id, name=r.name, details=r.details)
+
+    def dump_details(self, system, writer):
+        ordinal_id = 1
+        with writer.loop("_ihm_model_representation_details",
+                         ["id", "representation_id",
+                          "entity_id", "entity_description",
+                          "entity_asym_id", "entity_poly_segment_id",
                           "model_object_primitive", "starting_model_id",
                           "model_mode", "model_granularity",
                           "model_object_count"]) as l:
             for r in system._all_representations():
                 for segment in r:
                     entity = segment.asym_unit.entity
-                    l.write(ordinal_id=ordinal_id, representation_id=r._id,
-                            segment_id=segment._id, entity_id=entity._id,
+                    l.write(id=ordinal_id, representation_id=r._id,
+                            entity_id=entity._id,
                             entity_description=entity.description,
                             entity_asym_id=segment.asym_unit._id,
-                            seq_id_begin=segment.asym_unit.seq_id_range[0],
-                            seq_id_end=segment.asym_unit.seq_id_range[1],
+                            entity_poly_segment_id=segment.asym_unit._range_id,
                             model_object_primitive=segment.primitive,
                             starting_model_id=segment.starting_model._id
                                                   if segment.starting_model
                                                   else None,
                             model_mode='rigid' if segment.rigid else 'flexible',
                             model_granularity=segment.granularity,
                             model_object_count=segment.count)
@@ -790,27 +838,25 @@
         # Map dataset types to starting model sources
         source_map = {'Comparative model': 'comparative model',
                       'Integrative model': 'integrative model',
                       'Experimental model': 'experimental model',
                       'De Novo model': 'ab initio model'}
         with writer.loop("_ihm_starting_model_details",
                      ["starting_model_id", "entity_id", "entity_description",
-                      "asym_id", "seq_id_begin",
-                      "seq_id_end", "starting_model_source",
+                      "asym_id", "entity_poly_segment_id",
+                      "starting_model_source",
                       "starting_model_auth_asym_id",
                       "starting_model_sequence_offset",
                       "dataset_list_id"]) as l:
             for sm in system._all_starting_models():
-                seq_id_range = sm._get_seq_id_range_all_templates()
                 l.write(starting_model_id=sm._id,
                         entity_id=sm.asym_unit.entity._id,
                         entity_description=sm.asym_unit.entity.description,
                         asym_id=sm.asym_unit._id,
-                        seq_id_begin=seq_id_range[0],
-                        seq_id_end=seq_id_range[1],
+                        entity_poly_segment_id=sm._all_template_rng._range_id,
                         starting_model_source=source_map[sm.dataset.data_type],
                         starting_model_auth_asym_id=sm.asym_id,
                         dataset_list_id=sm.dataset._id,
                         starting_model_sequence_offset=sm.offset)
 
     def dump_computational(self, system, writer):
         """Dump details on computational models."""
@@ -824,39 +870,40 @@
                                         if sm.software else None,
                             script_file_id=sm.script_file._id
                                             if sm.script_file else None)
 
     def dump_comparative(self, system, writer):
         """Dump details on comparative models."""
         with writer.loop("_ihm_starting_comparative_models",
-                     ["ordinal_id", "starting_model_id",
+                     ["id", "starting_model_id",
                       "starting_model_auth_asym_id",
                       "starting_model_seq_id_begin",
                       "starting_model_seq_id_end",
                       "template_auth_asym_id", "template_seq_id_begin",
                       "template_seq_id_end", "template_sequence_identity",
                       "template_sequence_identity_denominator",
                       "template_dataset_list_id",
                       "alignment_file_id"]) as l:
             ordinal = 1
             for sm in system._all_starting_models():
                 off = sm.offset
                 for template in sm.templates:
-                    l.write(ordinal_id=ordinal,
+                    denom = template.sequence_identity.denominator
+                    l.write(id=ordinal,
                       starting_model_id=sm._id,
                       starting_model_auth_asym_id=sm.asym_id,
                       starting_model_seq_id_begin=template.seq_id_range[0]+off,
                       starting_model_seq_id_end=template.seq_id_range[1]+off,
                       template_auth_asym_id=template.asym_id,
                       template_seq_id_begin=template.template_seq_id_range[0],
                       template_seq_id_end=template.template_seq_id_range[1],
                       template_sequence_identity=
                                   float(template.sequence_identity),
                       template_sequence_identity_denominator=
-                                  int(template.sequence_identity.denominator),
+                                  None if denom is None else int(denom),
                       template_dataset_list_id=template.dataset._id
                                                if template.dataset else None,
                       alignment_file_id=template.alignment_file._id
                                         if template.alignment_file else None)
                     ordinal += 1
 
     def dump_coords(self, system, writer):
@@ -885,22 +932,22 @@
                             ordinal_id=ordinal)
                     ordinal += 1
 
     def dump_seq_dif(self, system, writer):
         """Write out sequence difference information"""
         ordinal = 1
         with writer.loop("_ihm_starting_model_seq_dif",
-                     ["ordinal_id", "entity_id", "asym_id",
+                     ["id", "entity_id", "asym_id",
                       "seq_id", "comp_id", "starting_model_id",
                       "db_asym_id", "db_seq_id", "db_comp_id",
                       "details"]) as l:
             for model in system._all_starting_models():
                 for sd in model.get_seq_dif():
                     comp = model.asym_unit.entity.sequence[sd.seq_id-1]
-                    l.write(ordinal_id=ordinal,
+                    l.write(id=ordinal,
                         entity_id=model.asym_unit.entity._id,
                         asym_id=model.asym_unit._id,
                         seq_id=sd.seq_id, comp_id=comp.id,
                         db_asym_id=model.asym_id, db_seq_id=sd.db_seq_id,
                         db_comp_id=sd.db_comp_id, starting_model_id=model._id,
                         details=sd.details)
                     ordinal += 1
@@ -911,32 +958,42 @@
         # Assign IDs to protocols and steps
         for np, p in enumerate(system._all_protocols()):
             p._id = np + 1
             for ns, s in enumerate(p.steps):
                 s._id = ns + 1
 
     def dump(self, system, writer):
-        ordinal = 1
+        self.dump_summary(system, writer)
+        self.dump_details(system, writer)
+
+    def dump_summary(self, system, writer):
         with writer.loop("_ihm_modeling_protocol",
-                         ["ordinal_id", "protocol_id", "step_id",
+                         ["id", "protocol_name", "num_steps"]) as l:
+            for p in system._all_protocols():
+                l.write(id=p._id,
+                        protocol_name=p.name, num_steps=len(p.steps))
+
+    def dump_details(self, system, writer):
+        ordinal = 1
+        with writer.loop("_ihm_modeling_protocol_details",
+                         ["id", "protocol_id", "step_id",
                           "struct_assembly_id", "dataset_group_id",
-                          "struct_assembly_description", "protocol_name",
+                          "struct_assembly_description",
                           "step_name", "step_method", "num_models_begin",
                           "num_models_end", "multi_scale_flag",
                           "multi_state_flag", "ordered_flag",
                           "software_id", "script_file_id"]) as l:
             for p in system._all_protocols():
                 for s in p.steps:
-                    l.write(ordinal_id=ordinal, protocol_id=p._id,
+                    l.write(id=ordinal, protocol_id=p._id,
                             step_id=s._id,
                             struct_assembly_id=s.assembly._id,
                             dataset_group_id=s.dataset_group._id
                                              if s.dataset_group else None,
                             struct_assembly_description=s.assembly.description,
-                            protocol_name=p.name,
                             step_name=s.name, step_method=s.method,
                             num_models_begin=s.num_models_begin,
                             num_models_end=s.num_models_end,
                             multi_state_flag=s.multi_state,
                             ordered_flag=s.ordered,
                             multi_scale_flag=s.multi_scale,
                             software_id=s.software._id if s.software else None,
@@ -1138,34 +1195,46 @@
             if not hasattr(g, '_id'):
                 raise ValueError("%s is referenced only by an Ensemble or "
                                  "OrderedProcess. ModelGroups should be "
                                  "stored in State objects." % g)
 
     def dump(self, system, writer):
         self.dump_model_list(system, writer)
+        self.dump_model_groups(system, writer)
         seen_types = self.dump_atoms(system, writer)
         self.dump_spheres(system, writer)
         self.dump_atom_type(seen_types, system, writer)
 
     def dump_model_list(self, system, writer):
-        ordinal = 1
         with writer.loop("_ihm_model_list",
-                         ["ordinal_id", "model_id", "model_group_id",
-                          "model_name", "model_group_name", "assembly_id",
+                         ["model_id", "model_name","assembly_id",
                           "protocol_id", "representation_id"]) as l:
             for group, model in system._all_models():
-                l.write(ordinal_id=ordinal, model_id=model._id,
-                        model_group_id=group._id,
+                l.write(model_id=model._id,
                         model_name=model.name,
-                        model_group_name=group.name,
                         assembly_id=model.assembly._id,
                         protocol_id=model.protocol._id
                                     if model.protocol else None,
                         representation_id=model.representation._id)
-                ordinal += 1
+
+    def dump_model_groups(self, system, writer):
+        self.dump_model_group_summary(system, writer)
+        self.dump_model_group_link(system, writer)
+
+    def dump_model_group_summary(self, system, writer):
+        with writer.loop("_ihm_model_group", ["id", "name", "details"]) as l:
+            for group in system._all_model_groups():
+                l.write(id=group._id, name=group.name)
+
+    def dump_model_group_link(self, system, writer):
+        with writer.loop("_ihm_model_group_link",
+                         ["group_id", "model_id"]) as l:
+            for group in system._all_model_groups():
+                for model_id in sorted(set(model._id for model in group)):
+                    l.write(model_id=model_id, group_id=group._id)
 
     def dump_atom_type(self, seen_types, system, writer):
         """Output the atom_type table with a list of elements used in atom_site.
            This table is needed by atom_site. Note that we output it *after*
            atom_site (otherwise we would need to iterate through all atoms in
            the system twice)."""
         elements = [x for x in sorted(seen_types.keys()) if x is not None]
@@ -1185,15 +1254,16 @@
                           "auth_asym_id",
                           "B_iso_or_equiv", "pdbx_PDB_model_num",
                           "ihm_model_id"]) as l:
             for group, model in system._all_models():
                 rngcheck = _RangeChecker(model)
                 for atom in model.get_atoms():
                     rngcheck(atom)
-                    comp = atom.asym_unit.entity.sequence[atom.seq_id-1]
+                    seq_id = 1 if atom.seq_id is None else atom.seq_id
+                    comp = atom.asym_unit.entity.sequence[seq_id-1]
                     seen_types[atom.type_symbol] = None
                     l.write(id=ordinal,
                             type_symbol=atom.type_symbol,
                             group_PDB='HETATM' if atom.het else 'ATOM',
                             label_atom_id=atom.atom_id,
                             label_comp_id=comp.id,
                             label_asym_id=atom.asym_unit._id,
@@ -1206,23 +1276,23 @@
                             ihm_model_id=model._id)
                     ordinal += 1
         return seen_types
 
     def dump_spheres(self, system, writer):
         ordinal = 1
         with writer.loop("_ihm_sphere_obj_site",
-                         ["ordinal_id", "entity_id", "seq_id_begin",
+                         ["id", "entity_id", "seq_id_begin",
                           "seq_id_end", "asym_id", "Cartn_x",
                           "Cartn_y", "Cartn_z", "object_radius", "rmsf",
                           "model_id"]) as l:
             for group, model in system._all_models():
                 rngcheck = _RangeChecker(model)
                 for sphere in model.get_spheres():
                     rngcheck(sphere)
-                    l.write(ordinal_id=ordinal,
+                    l.write(id=ordinal,
                             entity_id=sphere.asym_unit.entity._id,
                             seq_id_begin=sphere.seq_id_range[0],
                             seq_id_end=sphere.seq_id_range[1],
                             asym_id=sphere.asym_unit._id,
                             Cartn_x=sphere.x, Cartn_y=sphere.y,
                             Cartn_z=sphere.z, object_radius=sphere.radius,
                             rmsf=sphere.rmsf, model_id=model._id)
@@ -1265,23 +1335,22 @@
             for d in e.densities:
                 d._id = did
                 did += 1
 
     def dump(self, system, writer):
         with writer.loop("_ihm_localization_density_files",
                          ["id", "file_id", "ensemble_id", "entity_id",
-                          "asym_id", "seq_id_begin", "seq_id_end"]) as l:
+                          "asym_id", "entity_poly_segment_id"]) as l:
             for ensemble in system.ensembles:
                 for density in ensemble.densities:
                     l.write(id=density._id, file_id=density.file._id,
                             ensemble_id=ensemble._id,
                             entity_id=density.asym_unit.entity._id,
                             asym_id=density.asym_unit._id,
-                            seq_id_begin=density.asym_unit.seq_id_range[0],
-                            seq_id_end=density.asym_unit.seq_id_range[1])
+                            entity_poly_segment_id=density.asym_unit._range_id)
 
 
 class _MultiStateDumper(Dumper):
     def finalize(self, system):
         state_id = 1
         # Assign IDs
         for ng, g in enumerate(system.state_groups):
@@ -1290,31 +1359,40 @@
                 state._id = state_id
                 state_id += 1
 
     def dump(self, system, writer):
         # Nothing to do for single state modeling
         if len(system.state_groups) == 1 and len(system.state_groups[0]) <= 1:
             return
+        self.dump_summary(system, writer)
+        self.dump_model_groups(system, writer)
+
+    def dump_summary(self, system, writer):
         with writer.loop("_ihm_multi_state_modeling",
-                         ["ordinal_id", "state_id", "state_group_id",
+                         ["state_id", "state_group_id",
                           "population_fraction", "state_type", "state_name",
-                          "model_group_id", "experiment_type", "details"]) as l:
-            ordinal = 1
+                          "experiment_type", "details"]) as l:
+            for state_group in system.state_groups:
+                for state in state_group:
+                    l.write(state_id=state._id,
+                            state_group_id=state_group._id,
+                            population_fraction=state.population_fraction,
+                            state_type=state.type,
+                            state_name=state.name,
+                            experiment_type=state.experiment_type,
+                            details=state.details)
+
+    def dump_model_groups(self, system, writer):
+        with writer.loop("_ihm_multi_state_model_group_link",
+                         ["state_id", "model_group_id"]) as l:
             for state_group in system.state_groups:
                 for state in state_group:
                     for model_group in state:
-                        l.write(ordinal_id=ordinal, state_id=state._id,
-                                state_group_id=state_group._id,
-                                population_fraction=state.population_fraction,
-                                model_group_id=model_group._id,
-                                state_type=state.type,
-                                state_name=state.name,
-                                experiment_type=state.experiment_type,
-                                details=state.details)
-                        ordinal += 1
+                        l.write(state_id=state._id,
+                                model_group_id=model_group._id)
 
 
 class _OrderedDumper(Dumper):
     def finalize(self, system):
         for nproc, proc in enumerate(system.ordered_processes):
             proc._id = nproc + 1
             edge_id = 1
@@ -1640,15 +1718,14 @@
                         entity_id_1=entity1._id,
                         seq_id_1=xl.residue1.seq_id,
                         comp_id_1=seq1[xl.residue1.seq_id-1].id,
                         entity_description_2=entity2.description,
                         entity_id_2=entity2._id,
                         seq_id_2=xl.residue2.seq_id,
                         comp_id_2=seq2[xl.residue2.seq_id-1].id,
-                        linker_descriptor_id=r.linker._id,
                         linker_chem_comp_descriptor_id=r.linker._id,
                         linker_type=r.linker.auth_name,
                         dataset_list_id=r.dataset._id)
 
     def dump_restraint(self, system, writer):
         with writer.loop("_ihm_cross_link_restraint",
                          ["id", "group_id", "entity_id_1", "asym_id_1",
@@ -1677,23 +1754,23 @@
                         conditional_crosslink_flag=condmap[xl.restrain_all],
                         model_granularity=xl.granularity,
                         distance_threshold=xl.distance.distance,
                         psi=xl.psi, sigma_1=xl.sigma1, sigma_2=xl.sigma2)
 
     def dump_results(self, system, writer):
         with writer.loop("_ihm_cross_link_result_parameters",
-                         ["ordinal_id", "restraint_id", "model_id",
+                         ["id", "restraint_id", "model_id",
                           "psi", "sigma_1", "sigma_2"]) as l:
             ordinal = 1
             for r in self._all_restraints(system):
                 for xl in r.cross_links:
                     # all fits ordered by model ID
                     for model, fit in sorted(xl.fits.items(),
                                              key=lambda i: i[0]._id):
-                        l.write(ordinal_id=ordinal, restraint_id=xl._id,
+                        l.write(id=ordinal, restraint_id=xl._id,
                                 model_id=model._id, psi=fit.psi,
                                 sigma_1=fit.sigma1, sigma_2=fit.sigma2)
                         ordinal += 1
 
 
 class _GeometricRestraintDumper(Dumper):
     def _all_restraints(self, system):
@@ -1785,16 +1862,16 @@
         (self._restraints_by_id,
          self._group_for_id) = _finalize_restraints_and_groups(system,
                                          restraint.PredictedContactRestraint)
 
     def dump(self, system, writer):
         with writer.loop("_ihm_predicted_contact_restraint",
                          ["id", "group_id", "entity_id_1", "asym_id_1",
-                          "comp_id_1", "seq_id_1", "atom_id_1", "entity_id_2",
-                          "asym_id_2", "comp_id_2", "seq_id_2", "atom_id_2",
+                          "comp_id_1", "seq_id_1", "rep_atom_1", "entity_id_2",
+                          "asym_id_2", "comp_id_2", "seq_id_2", "rep_atom_2",
                           "restraint_type", "distance_lower_limit",
                           "distance_upper_limit", "probability",
                           "model_granularity", "dataset_list_id",
                           "software_id"]) as l:
             for r in self._restraints_by_id:
                 comp1 = r.resatom1.asym.entity.sequence[r.resatom1.seq_id-1].id
                 comp2 = r.resatom2.asym.entity.sequence[r.resatom2.seq_id-1].id
@@ -1803,19 +1880,19 @@
                     atom1 = r.resatom1.id
                 if isinstance(r.resatom2, ihm.Atom):
                     atom2 = r.resatom2.id
                 l.write(id=r._id, group_id=self._group_for_id.get(r._id, None),
                         entity_id_1=r.resatom1.asym.entity._id,
                         asym_id_1=r.resatom1.asym._id,
                         comp_id_1=comp1, seq_id_1=r.resatom1.seq_id,
-                        atom_id_1=atom1,
+                        rep_atom_1=atom1,
                         entity_id_2=r.resatom2.asym.entity._id,
                         asym_id_2=r.resatom2.asym._id,
                         comp_id_2=comp2, seq_id_2=r.resatom2.seq_id,
-                        atom_id_2=atom2,
+                        rep_atom_2=atom2,
                         restraint_type=r.distance.restraint_type,
                         distance_lower_limit=r.distance.distance_lower_limit,
                         distance_upper_limit=r.distance.distance_upper_limit,
                         probability=r.probability,
                         model_granularity="by-residue" if r.by_residue
                                           else 'by-feature',
                         dataset_list_id=r.dataset._id if r.dataset else None,
@@ -1830,29 +1907,29 @@
     def finalize(self, system):
         for nr, r in enumerate(self._all_restraints(system)):
             r._id = nr + 1
 
     def dump(self, system, writer):
         ordinal = 1
         with writer.loop("_ihm_3dem_restraint",
-                         ["ordinal_id", "dataset_list_id", "fitting_method",
+                         ["id", "dataset_list_id", "fitting_method",
                           "fitting_method_citation_id",
                           "struct_assembly_id",
                           "number_of_gaussians", "model_id",
                           "cross_correlation_coefficient"]) as l:
             for r in self._all_restraints(system):
                 if r.fitting_method_citation:
                     citation_id = r.fitting_method_citation._id
                 else:
                     citation_id = None
                 # all fits ordered by model ID
                 for model, fit in sorted(r.fits.items(),
                                          key=lambda i: i[0]._id):
                     ccc = fit.cross_correlation_coefficient
-                    l.write(ordinal_id=ordinal,
+                    l.write(id=ordinal,
                             dataset_list_id=r.dataset._id,
                             fitting_method=r.fitting_method,
                             fitting_method_citation_id=citation_id,
                             struct_assembly_id=r.assembly._id,
                             number_of_gaussians=r.number_of_gaussians,
                             model_id=model._id,
                             cross_correlation_coefficient=ccc)
@@ -1889,15 +1966,15 @@
                         struct_assembly_id=r.assembly._id,
                         image_segment_flag=r.segment,
                         details=r.details)
 
     def dump_fitting(self, system, writer):
         ordinal = 1
         with writer.loop("_ihm_2dem_class_average_fitting",
-                ["ordinal_id", "restraint_id", "model_id",
+                ["id", "restraint_id", "model_id",
                  "cross_correlation_coefficient", "rot_matrix[1][1]",
                  "rot_matrix[2][1]", "rot_matrix[3][1]", "rot_matrix[1][2]",
                  "rot_matrix[2][2]", "rot_matrix[3][2]", "rot_matrix[1][3]",
                  "rot_matrix[2][3]", "rot_matrix[3][3]", "tr_vector[1]",
                  "tr_vector[2]", "tr_vector[3]"]) as l:
             for r in self._all_restraints(system):
                 # all fits ordered by model ID
@@ -1912,15 +1989,15 @@
                         rm = [[None] * 3] * 3
                     else:
                         # mmCIF writer usually outputs floats to 3 decimal
                         # places, but we need more precision for rotation
                         # matrices
                         rm = [["%.6f" % e for e in fit.rot_matrix[i]]
                               for i in range(3)]
-                    l.write(ordinal_id=ordinal, restraint_id=r._id,
+                    l.write(id=ordinal, restraint_id=r._id,
                             model_id=model._id,
                             cross_correlation_coefficient=ccc,
                             rot_matrix11=rm[0][0], rot_matrix21=rm[1][0],
                             rot_matrix31=rm[2][0], rot_matrix12=rm[0][1],
                             rot_matrix22=rm[1][1], rot_matrix32=rm[2][1],
                             rot_matrix13=rm[0][2], rot_matrix23=rm[1][2],
                             rot_matrix33=rm[2][2], tr_vector1=t[0],
@@ -1936,24 +2013,24 @@
     def finalize(self, system):
         for nr, r in enumerate(self._all_restraints(system)):
             r._id = nr + 1
 
     def dump(self, system, writer):
         ordinal = 1
         with writer.loop("_ihm_sas_restraint",
-                         ["ordinal_id", "dataset_list_id", "model_id",
+                         ["id", "dataset_list_id", "model_id",
                           "struct_assembly_id", "profile_segment_flag",
                           "fitting_atom_type", "fitting_method",
                           "fitting_state", "radius_of_gyration",
                           "chi_value", "details"]) as l:
             for r in self._all_restraints(system):
                 # all fits ordered by model ID
                 for model, fit in sorted(r.fits.items(),
                                          key=lambda i: i[0]._id):
-                    l.write(ordinal_id=ordinal,
+                    l.write(id=ordinal,
                             dataset_list_id=r.dataset._id,
                             fitting_method=r.fitting_method,
                             fitting_atom_type=r.fitting_atom_type,
                             fitting_state='Multiple' if r.multi_state
                                                      else 'Single',
                             profile_segment_flag=r.segment,
                             radius_of_gyration=r.radius_of_gyration,
@@ -2578,15 +2655,15 @@
                _AuditConformDumper(), _SoftwareDumper(),
                _CitationDumper(),
                _AuditAuthorDumper(), _GrantDumper(),
                _ChemCompDumper(), _ChemDescriptorDumper(),
                _EntityDumper(), _EntitySrcGenDumper(), _EntitySrcNatDumper(),
                _EntitySrcSynDumper(), _EntityPolyDumper(),
                _EntityNonPolyDumper(),
-               _EntityPolySeqDumper(),
+               _EntityPolySeqDumper(), _EntityPolySegmentDumper(),
                _StructAsymDumper(),
                _PolySeqSchemeDumper(),
                _NonPolySchemeDumper(),
                _AssemblyDumper(),
                _ExternalReferenceDumper(),
                _DatasetDumper(),
                _ModelRepresentationDumper(),
@@ -2617,13 +2694,16 @@
                _FLRFPSMPPModelingDumper()] + [d() for d in dumpers]
     writer_map = {'mmCIF': ihm.format.CifWriter,
                   'BCIF': ihm.format_bcif.BinaryCifWriter}
 
     writer = writer_map[format](fh)
     for system in systems:
         _init_restraint_groups(system)
+        # Fill in complete assembly
+        system._make_complete_assembly()
+
         for d in dumpers:
             d.finalize(system)
         _check_restraint_groups(system)
         for d in dumpers:
             d.dump(system, writer)
     writer.flush()
```

### Comparing `ihm-0.8/ihm/flr.py` & `ihm-0.9/ihm/flr.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/format.py` & `ihm-0.9/ihm/format.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/format_bcif.py` & `ihm-0.9/ihm/format_bcif.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/geometry.py` & `ihm-0.9/ihm/geometry.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/location.py` & `ihm-0.9/ihm/location.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/metadata.py` & `ihm-0.9/ihm/metadata.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/model.py` & `ihm-0.9/ihm/model.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/protocol.py` & `ihm-0.9/ihm/protocol.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/reader.py` & `ihm-0.9/ihm/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,49 @@
             return newcls(None)
         elif newcls is ihm.WaterChemComp:
             return newcls()
         else:
             return newcls(*self._cls_args, **self._cls_keys)
 
 
+class RangeIDMapper(object):
+    """Utility class to handle mapping from mmCIF IDs to
+       :class:`ihm.AsymUnitRange` or :class:`EntityRange` objects."""
+
+    def __init__(self):
+        self._id_map = {}
+
+    def set(self, range_id, seq_id_begin, seq_id_end):
+        """Add a range.
+
+           :param str range_id: mmCIF ID
+           :param int seq_id_begin: Index of the start of the range
+           :param int seq_id_end: Index of the end of the range
+        """
+        self._id_map[range_id] = (seq_id_begin, seq_id_end)
+
+    def get(self, asym_or_entity, range_id):
+        """Get a range from an ID.
+
+           :param asym_or_entity: An :class:`ihm.Entity` or
+                  :class:`ihm.AsymUnit` object representing the part of
+                  the system to which the range will be applied.
+           :param str range_id: mmCIF ID
+           :return: A range as a :class:`ihm.Entity`, :class:`ihm.AsymUnit`,
+                    :class:`ihm.EntityRange` or :class:`ihm.AsymUnitRange`
+                    object.
+        """
+        # range_id can be None if the entire asym/entity should be selected
+        # (e.g. for a non-polymer)
+        if range_id is None:
+            return asym_or_entity
+        else:
+            return asym_or_entity(*self._id_map[range_id])
+
+
 class _AnalysisIDMapper(IDMapper):
     """Add extra handling to IDMapper for the post processing category"""
 
     def _make_new_object(self, newcls=None):
         if newcls is None:
             newcls = self._cls
         if newcls is ihm.analysis.EmptyStep:
@@ -371,14 +406,18 @@
 
         #: Mapping from ID to :class:`ihm.ChemComp` objects
         self.chem_comps = _ChemCompIDMapper(None, ihm.ChemComp, *(None,)*3)
 
         #: Mapping from ID to :class:`ihm.Assembly` objects
         self.assemblies = IDMapper(self.system.orphan_assemblies, ihm.Assembly)
 
+        #: Mapping from ID to :class:`ihm.AsymUnitRange`
+        #: or :class:`EntityRange` objects
+        self.ranges = RangeIDMapper()
+
         #: Mapping from ID to :class:`ihm.location.Repository` objects
         self.repos = IDMapper(None, ihm.location.Repository, None)
 
         #: Mapping from ID to :class:`ihm.location.FileLocation` objects
         self.external_files = IDMapper(self.system.locations,
                                  ihm.location.FileLocation,
                                  '/') # should always exist?
@@ -949,14 +988,16 @@
     def __init__(self, *args):
         super(_EntityPolyHandler, self).__init__(*args)
         self._entity_info = {}
 
     def _get_codes(self, codestr):
         """Convert a one-letter-code string into a sequence of individual
            codes"""
+        if codestr is None:
+            return
         i = 0
         while i < len(codestr):
             # Strip out linebreaks
             if codestr[i] == '\n':
                 pass
             elif codestr[i] == '(':
                 end = codestr.index(')', i)
@@ -989,14 +1030,22 @@
                 if comp.code is None and i < len(ei.one_letter):
                     comp.code = ei.one_letter[i]
                 if (comp.code_canonical is None
                     and i < len(ei.one_letter_can)):
                     comp.code_canonical = ei.one_letter_can[i]
 
 
+class _EntityPolySegmentHandler(Handler):
+    category = '_ihm_entity_poly_segment'
+
+    def __call__(self, id, seq_id_begin, seq_id_end):
+        self.sysr.ranges.set(id, self.get_int(seq_id_begin),
+                             self.get_int(seq_id_end))
+
+
 class _EntityNonPolyHandler(Handler):
     category = '_pdbx_entity_nonpoly'
 
     def __call__(self, entity_id, comp_id):
         s = self.sysr.entities.get_by_id(entity_id)
         s.sequence = (self.sysr.chem_comps.get_by_id(comp_id),)
 
@@ -1008,47 +1057,39 @@
         s = self.sysr.asym_units.get_by_id(id)
         # Keep this ID (like a user-assigned ID); don't reassign it on output
         s.id = id
         s.entity = self.sysr.entities.get_by_id(entity_id)
         self.copy_if_present(s, locals(), keys=('details',))
 
 
-class _AssemblyDetailsHandler(Handler):
-    category = '_ihm_struct_assembly_details'
+class _AssemblyHandler(Handler):
+    category = '_ihm_struct_assembly'
 
-    def __call__(self, assembly_id, assembly_name, assembly_description):
-        s = self.sysr.assemblies.get_by_id(assembly_id)
-        self.copy_if_present(s, locals(),
-                mapkeys={'assembly_name':'name',
-                         'assembly_description':'description'})
+    def __call__(self, id, name, description):
+        s = self.sysr.assemblies.get_by_id(id)
+        self.copy_if_present(s, locals(), keys=('name', 'description'))
 
 
-class _AssemblyHandler(Handler):
+class _AssemblyDetailsHandler(Handler):
     # todo: figure out how to populate System.complete_assembly
-    category = '_ihm_struct_assembly'
+    category = '_ihm_struct_assembly_details'
     ignored_keywords = ['ordinal_id', 'entity_description']
 
-    def __call__(self, assembly_id, parent_assembly_id, seq_id_begin,
-                 seq_id_end, asym_id, entity_id):
+    def __call__(self, assembly_id, parent_assembly_id, entity_poly_segment_id,
+                 asym_id, entity_id):
         a_id = assembly_id
         a = self.sysr.assemblies.get_by_id(a_id)
         parent_id = parent_assembly_id
         if parent_id and parent_id != a_id and not a.parent:
             a.parent = self.sysr.assemblies.get_by_id(parent_id)
-        def handle_range(obj):
-            # seq_id_range can be None for assemblies of nonpolymers - treat as
-            # complete entity/asym
-            if seq_id_begin is None or seq_id_end is None:
-                return obj
-            else:
-                return obj(int(seq_id_begin), int(seq_id_end))
         if asym_id:
-            a.append(handle_range(self.sysr.asym_units.get_by_id(asym_id)))
+            obj = self.sysr.asym_units.get_by_id(asym_id)
         else:
-            a.append(handle_range(self.sysr.entities.get_by_id(entity_id)))
+            obj = self.sysr.entities.get_by_id(entity_id)
+        a.append(self.sysr.ranges.get(obj, entity_poly_segment_id))
 
     def finalize(self):
         # Any EntityRange or AsymUnitRange which covers an entire entity,
         # replace with Entity or AsymUnit object
         for a in self.system.orphan_assemblies:
             a[:] = [self._handle_component(x) for x in a]
 
@@ -1141,14 +1182,23 @@
         f.details = details
 
 
 class _DatasetGroupHandler(Handler):
     category = '_ihm_dataset_group'
     ignored_keywords = ['ordinal_id']
 
+    def __call__(self, id, name, application, details):
+        g = self.sysr.dataset_groups.get_by_id(id)
+        self.copy_if_present(g, locals(),
+                             keys=('name', 'application', 'details'))
+
+
+class _DatasetGroupLinkHandler(Handler):
+    category = '_ihm_dataset_group_link'
+
     def __call__(self, group_id, dataset_list_id):
         g = self.sysr.dataset_groups.get_by_id(group_id)
         ds = self.sysr.datasets.get_by_id(dataset_list_id)
         g.append(ds)
 
 
 class _DatasetExtRefHandler(Handler):
@@ -1191,14 +1241,22 @@
 
     def __call__(self, dataset_list_id_derived, dataset_list_id_primary):
         derived = self.sysr.datasets.get_by_id(dataset_list_id_derived)
         primary = self.sysr.datasets.get_by_id(dataset_list_id_primary)
         derived.parents.append(primary)
 
 
+class _ModelRepresentationHandler(Handler):
+    category = '_ihm_model_representation'
+
+    def __call__(self, id, name, details):
+        rep = self.sysr.representations.get_by_id(id)
+        self.copy_if_present(rep, locals(), keys=('name', 'details'))
+
+
 def _make_atom_segment(asym, rigid, primitive, count, smodel):
     return ihm.representation.AtomicSegment(
                 asym_unit=asym, rigid=rigid, starting_model=smodel)
 
 def _make_residue_segment(asym, rigid, primitive, count, smodel):
     return ihm.representation.ResidueSegment(
                 asym_unit=asym, rigid=rigid, primitive=primitive,
@@ -1210,30 +1268,31 @@
                 starting_model=smodel)
 
 def _make_feature_segment(asym, rigid, primitive, count, smodel):
     return ihm.representation.FeatureSegment(
                 asym_unit=asym, rigid=rigid, primitive=primitive,
                 count=count, starting_model=smodel)
 
-class _ModelRepresentationHandler(Handler):
-    category = '_ihm_model_representation'
+
+class _ModelRepresentationDetailsHandler(Handler):
+    category = '_ihm_model_representation_details'
     ignored_keywords = ['entity_description']
 
     _rigid_map = {'rigid': True, 'flexible': False, None: None}
     _segment_factory = {'by-atom': _make_atom_segment,
                         'by-residue': _make_residue_segment,
                         'multi-residue': _make_multi_residue_segment,
                         'by-feature': _make_feature_segment}
 
-    def __call__(self, entity_asym_id, seq_id_begin, seq_id_end,
+    def __call__(self, entity_asym_id, entity_poly_segment_id,
                  representation_id, starting_model_id, model_object_primitive,
                  model_granularity, model_object_count, model_mode):
-        asym = self.sysr.asym_units.get_by_id(entity_asym_id)
-        if seq_id_begin is not None and seq_id_end is not None:
-            asym = asym(int(seq_id_begin), int(seq_id_end))
+        asym = self.sysr.ranges.get(
+                       self.sysr.asym_units.get_by_id(entity_asym_id),
+                       entity_poly_segment_id)
         rep = self.sysr.representations.get_by_id(representation_id)
         smodel = self.sysr.starting_models.get_by_id_or_none(
                                             starting_model_id)
         primitive = self.get_lower(model_object_primitive)
         gran = self.get_lower(model_granularity)
         primitive = self.get_lower(model_object_primitive)
         count = self.get_int(model_object_count)
@@ -1244,21 +1303,21 @@
 
 
 # todo: support user subclass of StartingModel, pass it coordinates, seqdif
 class _StartingModelDetailsHandler(Handler):
     category = '_ihm_starting_model_details'
     ignored_keywords = ['entity_description']
 
-    def __call__(self, starting_model_id, asym_id, seq_id_begin, seq_id_end,
+    def __call__(self, starting_model_id, asym_id, entity_poly_segment_id,
                  dataset_list_id, starting_model_auth_asym_id,
                  starting_model_sequence_offset):
         m = self.sysr.starting_models.get_by_id(starting_model_id)
-        asym = self.sysr.asym_units.get_by_id(asym_id)
-        if seq_id_begin is not None and seq_id_end is not None:
-            asym = asym(int(seq_id_begin), int(seq_id_end))
+        asym = self.sysr.ranges.get(
+                       self.sysr.asym_units.get_by_id(asym_id),
+                       entity_poly_segment_id)
         m.asym_unit = asym
         m.dataset = self.sysr.datasets.get_by_id(dataset_list_id)
         self.copy_if_present(m, locals(),
                     mapkeys={'starting_model_auth_asym_id':'asym_id'})
         if starting_model_sequence_offset is not None:
             m.offset = int(starting_model_sequence_offset)
 
@@ -1301,20 +1360,27 @@
         m.templates.append(t)
 
 
 class _ProtocolHandler(Handler):
     category = '_ihm_modeling_protocol'
     ignored_keywords = ['ordinal_id', 'struct_assembly_description']
 
-    def __call__(self, protocol_id, step_id, protocol_name, num_models_begin,
+    def __call__(self, id, protocol_name, num_steps):
+        p = self.sysr.protocols.get_by_id(id)
+        self.copy_if_present(p, locals(), mapkeys={'protocol_name':'name'})
+
+
+class _ProtocolDetailsHandler(Handler):
+    category = '_ihm_modeling_protocol_details'
+
+    def __call__(self, protocol_id, step_id, num_models_begin,
                  num_models_end, multi_scale_flag, multi_state_flag,
                  ordered_flag, struct_assembly_id, dataset_group_id,
                  software_id, script_file_id, step_name, step_method):
         p = self.sysr.protocols.get_by_id(protocol_id)
-        self.copy_if_present(p, locals(),  mapkeys={'protocol_name':'name'})
         nbegin = self.get_int(num_models_begin)
         nend = self.get_int(num_models_end)
         mscale = self.get_bool(multi_scale_flag)
         mstate = self.get_bool(multi_state_flag)
         ordered = self.get_bool(ordered_flag)
         assembly = self.sysr.assemblies.get_by_id_or_none(
                                             struct_assembly_id)
@@ -1375,33 +1441,34 @@
                                             script_file_id)
             self.copy_if_present(step, locals(), keys=['feature'])
 
 
 class _ModelListHandler(Handler):
     category = '_ihm_model_list'
 
-    def __call__(self, model_group_id, model_group_name, model_id, model_name,
+    def __call__(self, model_id, model_name,
                  assembly_id, representation_id, protocol_id):
-        model_group = self.sysr.model_groups.get_by_id(model_group_id)
-        self.copy_if_present(model_group, locals(),
-                             mapkeys={'model_group_name':'name'})
-
         model = self.sysr.models.get_by_id(model_id)
 
-        assert model._id not in (m._id for m in model_group)
-        model_group.append(model)
-
         self.copy_if_present(model, locals(), mapkeys={'model_name':'name'})
         model.assembly = self.sysr.assemblies.get_by_id_or_none(
                                             assembly_id)
         model.representation = self.sysr.representations.get_by_id_or_none(
                                             representation_id)
         model.protocol = self.sysr.protocols.get_by_id_or_none(
                                             protocol_id)
 
+
+class _ModelGroupHandler(Handler):
+    category = '_ihm_model_group'
+
+    def __call__(self, id, name, details):
+        model_group = self.sysr.model_groups.get_by_id(id)
+        self.copy_if_present(model_group, locals(), keys=('name', 'details'))
+
     def finalize(self):
         # Put all model groups not assigned to a state in their own state
         # todo: handle models not in model groups too?
         model_groups_in_states = set()
         for sg in self.system.state_groups:
             for state in sg:
                 for model_group in state:
@@ -1409,35 +1476,48 @@
         mgs = [mg for mgid, mg in self.sysr.model_groups._obj_by_id.items()
                if mgid not in model_groups_in_states]
         if mgs:
             s = ihm.model.State(mgs)
             self.system.state_groups.append(ihm.model.StateGroup([s]))
 
 
+class _ModelGroupLinkHandler(Handler):
+    category = '_ihm_model_group_link'
+
+    def __call__(self, group_id, model_id):
+        model_group = self.sysr.model_groups.get_by_id(group_id)
+        model = self.sysr.models.get_by_id(model_id)
+        model_group.append(model)
+
+
 class _MultiStateHandler(Handler):
     category = '_ihm_multi_state_modeling'
 
-    def __call__(self, state_group_id, state_id, model_group_id,
+    def __call__(self, state_group_id, state_id,
                  population_fraction, experiment_type, details, state_name,
                  state_type):
         state_group = self.sysr.state_groups.get_by_id(state_group_id)
         state = self.sysr.states.get_by_id(state_id)
-
-        if state._id not in [s._id for s in state_group]:
-            state_group.append(state)
-
-        model_group = self.sysr.model_groups.get_by_id(model_group_id)
-        state.append(model_group)
+        state_group.append(state)
 
         state.population_fraction = self.get_float(population_fraction)
         self.copy_if_present(state, locals(),
                 keys=['experiment_type', 'details'],
                 mapkeys={'state_name':'name', 'state_type':'type'})
 
 
+class _MultiStateLinkHandler(Handler):
+    category = '_ihm_multi_state_model_group_link'
+
+    def __call__(self, state_id, model_group_id):
+        state = self.sysr.states.get_by_id(state_id)
+        model_group = self.sysr.model_groups.get_by_id(model_group_id)
+        state.append(model_group)
+
+
 class _EnsembleHandler(Handler):
     category = '_ihm_ensemble_info'
 
     def __call__(self, ensemble_id, model_group_id, post_process_id,
                  ensemble_file_id, num_ensemble_models,
                  ensemble_precision_value, ensemble_name,
                  ensemble_clustering_method, ensemble_clustering_feature):
@@ -1458,24 +1538,23 @@
                          'ensemble_clustering_method':'clustering_method',
                          'ensemble_clustering_feature':'clustering_feature'})
 
 
 class _DensityHandler(Handler):
     category = '_ihm_localization_density_files'
 
-    def __call__(self, id, ensemble_id, file_id, asym_id, seq_id_begin,
-                 seq_id_end):
+    def __call__(self, id, ensemble_id, file_id, asym_id,
+                 entity_poly_segment_id):
         density = self.sysr.densities.get_by_id(id)
         ensemble = self.sysr.ensembles.get_by_id(ensemble_id)
         f = self.sysr.external_files.get_by_id(file_id)
 
-        asym = self.sysr.asym_units.get_by_id(asym_id)
-        if seq_id_begin is not None and seq_id_end is not None:
-            asym = asym(int(seq_id_begin), int(seq_id_end))
-
+        asym = self.sysr.ranges.get(
+                       self.sysr.asym_units.get_by_id(asym_id),
+                       entity_poly_segment_id)
         density.asym_unit = asym
         density.file = f
         ensemble.densities.append(density)
 
 
 class _EM3DRestraintHandler(Handler):
     category = '_ihm_3dem_restraint'
@@ -1751,24 +1830,24 @@
         seq_id = self.get_int(seq_id)
         resatom = asym.residue(seq_id)
         if atom_id:
             resatom = resatom.atom(atom_id)
         return resatom
 
     def __call__(self, id, group_id, dataset_list_id, asym_id_1,
-                 seq_id_1, atom_id_1, asym_id_2, seq_id_2, atom_id_2,
+                 seq_id_1, rep_atom_1, asym_id_2, seq_id_2, rep_atom_2,
                  restraint_type, probability, distance_lower_limit,
                  distance_upper_limit, model_granularity, software_id):
         r = self.sysr.pred_cont_restraints.get_by_id(id)
         if group_id is not None:
             rg = self.sysr.pred_cont_restraint_groups.get_by_id(group_id)
             rg.append(r)
         r.dataset = self.sysr.datasets.get_by_id_or_none(dataset_list_id)
-        r.resatom1 = self._get_resatom(asym_id_1, seq_id_1, atom_id_1)
-        r.resatom2 = self._get_resatom(asym_id_2, seq_id_2, atom_id_2)
+        r.resatom1 = self._get_resatom(asym_id_1, seq_id_1, rep_atom_1)
+        r.resatom2 = self._get_resatom(asym_id_2, seq_id_2, rep_atom_2)
         r.distance = _handle_distance[restraint_type](distance_lower_limit,
                                                       distance_upper_limit,
                                                       self.get_float)
         r.by_residue = self.get_lower(model_granularity) == 'by-residue'
         r.probability = self.get_float(probability)
         r.software = self.sysr.software.get_by_id_or_none(software_id)
 
@@ -2633,24 +2712,30 @@
         hs = [_StructHandler(s), _SoftwareHandler(s), _CitationHandler(s),
               _AuditAuthorHandler(s), _GrantHandler(s),
               _CitationAuthorHandler(s), _ChemCompHandler(s),
               _ChemDescriptorHandler(s), _EntityHandler(s),
               _EntitySrcNatHandler(s), _EntitySrcGenHandler(s),
               _EntitySrcSynHandler(s), _EntityPolyHandler(s),
               _EntityPolySeqHandler(s), _EntityNonPolyHandler(s),
+              _EntityPolySegmentHandler(s),
               _StructAsymHandler(s), _AssemblyDetailsHandler(s),
               _AssemblyHandler(s), _ExtRefHandler(s), _ExtFileHandler(s),
               _DatasetListHandler(s), _DatasetGroupHandler(s),
+              _DatasetGroupLinkHandler(s),
               _DatasetExtRefHandler(s), _DatasetDBRefHandler(s),
               _RelatedDatasetsHandler(s), _ModelRepresentationHandler(s),
+              _ModelRepresentationDetailsHandler(s),
               _StartingModelDetailsHandler(s),
               _StartingComputationalModelsHandler(s),
               _StartingComparativeModelsHandler(s),
-              _ProtocolHandler(s), _PostProcessHandler(s), _ModelListHandler(s),
-              _MultiStateHandler(s), _EnsembleHandler(s), _DensityHandler(s),
+              _ProtocolHandler(s), _ProtocolDetailsHandler(s),
+              _PostProcessHandler(s), _ModelListHandler(s),
+              _ModelGroupHandler(s), _ModelGroupLinkHandler(s),
+              _MultiStateHandler(s), _MultiStateLinkHandler(s),
+              _EnsembleHandler(s), _DensityHandler(s),
               _EM3DRestraintHandler(s), _EM2DRestraintHandler(s),
               _EM2DFittingHandler(s), _SASRestraintHandler(s),
               _SphereObjSiteHandler(s), _AtomSiteHandler(s),
               _PolyResidueFeatureHandler(s), _PolyAtomFeatureHandler(s),
               _NonPolyFeatureHandler(s), _PseudoSiteFeatureHandler(s),
               _DerivedDistanceRestraintHandler(s),
               _PredictedContactRestraintHandler(s), _CenterHandler(s),
```

### Comparing `ihm-0.8/ihm/representation.py` & `ihm-0.9/ihm/representation.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,16 +108,26 @@
 
 
 class Representation(list):
     """Part of the system modeled as a set of geometric objects, such as
        spheres or atoms. This is implemented as a simple list of
        :class:`Segment` objects.
 
+       :param sequence elements: Initial set of segments.
+       :param str name: A short descriptive name.
+       :param str details: A longer description of the representation.
+
        Typically a Representation is assigned to a
        :class:`~ihm.model.Model`. See also
        :attr:`ihm.System.orphan_representations`.
 
        Multiple representations of the same system are possible (multi-scale).
     """
 
+    # For backwards compatibility with earlier versions of this class which
+    # didn't specify name/details
+    name = details = None
+
     # todo: use set rather than list?
-    pass
+    def __init__(self, elements=(), name=None, details=None):
+        super(Representation, self).__init__(elements)
+        self.name, self.details = name, details
```

### Comparing `ihm-0.8/ihm/restraint.py` & `ihm-0.9/ihm/restraint.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/source.py` & `ihm-0.9/ihm/source.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/ihm/startmodel.py` & `ihm-0.9/ihm/startmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Classes to handle starting models."""
 
+import ihm
 from .format import CifWriter
 try:
     from enum import IntEnum
 except ImportError:
     IntEnum = object
 
 
@@ -160,31 +161,32 @@
 
            See :meth:`get_atoms` for more details.
         """
         self._seq_difs.append(seq_dif)
 
     def _get_seq_id_range_all_templates(self):
         """Get the seq_id range covered by all templates in this starting
-           model. Where there are multiple templates, consolidate
-           them; template info is given in starting_comparative_models."""
+           model, as an AsymUnit or AsymUnitRange object. Where there are
+           multiple templates, consolidate them; template info is given in
+           starting_comparative_models."""
         def get_seq_id_range(template, full):
             # The template may cover more than the current starting model
             rng = template.seq_id_range
             return (max(rng[0]+self.offset, full[0]),
                     min(rng[1]+self.offset, full[1]))
 
         if self.templates:
             full = self.asym_unit.seq_id_range
             rng = get_seq_id_range(self.templates[0], full)
             for template in self.templates[1:]:
                 this_rng = get_seq_id_range(template, full)
                 rng = (min(rng[0], this_rng[0]), max(rng[1], this_rng[1]))
-            return rng
+            return ihm.AsymUnit(self.asym_unit.entity)(*rng)
         else:
-            return self.asym_unit.seq_id_range
+            return self.asym_unit
 
 
 class PDBHelix(object):
     """Represent a HELIX record from a PDB file."""
     def __init__(self, line):
         self.helix_id = line[11:14].strip()
         self.start_resnam = line[14:18].strip()
```

### Comparing `ihm-0.8/ihm/util.py` & `ihm-0.9/ihm/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,28 +15,30 @@
         while ind >= lc:
             ids.append(chars[ind % lc])
             ind = ind // lc - 1
         ids.append(chars[ind])
         return "".join(reversed(ids))
 
 
-def _remove_id(obj):
+def _remove_id(obj, attr='_id'):
     """Remove any unique ID from obj"""
-    if hasattr(obj, '_id'):
-        del obj._id
+    if hasattr(obj, attr):
+        delattr(obj, attr)
 
-def _assign_id(obj, seen_objs, obj_by_id):
+def _assign_id(obj, seen_objs, obj_by_id, attr='_id', seen_obj=None):
     """Assign a unique ID to obj, and track all ids in obj_by_id."""
-    if obj not in seen_objs:
-        if not hasattr(obj, '_id'):
+    if seen_obj is None:
+        seen_obj = obj
+    if seen_obj not in seen_objs:
+        if not hasattr(obj, attr):
             obj_by_id.append(obj)
-            obj._id = len(obj_by_id)
-        seen_objs[obj] = obj._id
+            setattr(obj, attr, len(obj_by_id))
+        seen_objs[seen_obj] = getattr(obj, attr)
     else:
-        obj._id = seen_objs[obj]
+        setattr(obj, attr, seen_objs[seen_obj])
 
 def _get_relative_path(reference, path):
     """Return `path` interpreted relative to `reference`"""
     if os.path.isabs(path):
         return path
     else:
         return os.path.join(os.path.dirname(reference), path)
```

### Comparing `ihm-0.8/ihm.egg-info/PKG-INFO` & `ihm-0.9/ihm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihm
-Version: 0.8
+Version: 0.9
 Summary: Package for handling IHM mmCIF and BinaryCIF files
 Home-page: https://github.com/ihmwg/python-ihm
 Author: Ben Webb
 Author-email: ben@salilab.org
 License: UNKNOWN
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2603378.svg)](https://doi.org/10.5281/zenodo.2603378)
         [![docs](https://readthedocs.org/projects/python-ihm/badge/)](https://python-ihm.readthedocs.org/)
```

### Comparing `ihm-0.8/ihm.egg-info/SOURCES.txt` & `ihm-0.9/ihm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ihm.egg-info/SOURCES.txt
 ihm.egg-info/dependency_links.txt
 ihm.egg-info/requires.txt
 ihm.egg-info/top_level.txt
 src/ihm_format.c
 src/ihm_format.h
 src/ihm_format.i
-src/ihm_format_wrap_0.8.c
+src/ihm_format_wrap_0.9.c
 test/test_analysis.py
 test/test_cross_linkers.py
 test/test_dataset.py
 test/test_dictionary.py
 test/test_dumper.py
 test/test_edit.py
 test/test_examples.py
```

### Comparing `ihm-0.8/setup.py` & `ihm-0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from setuptools import setup, Extension
 except ImportError:
     from distutils.core import setup, Extension
 import sys
 import os
 
-VERSION = "0.8"
+VERSION = "0.9"
 
 copy_args = sys.argv[1:]
 
 # Allow building without the C extension
 build_ext = True
 if '--without-ext' in copy_args:
     build_ext = False
```

### Comparing `ihm-0.8/src/ihm_format.c` & `ihm-0.9/src/ihm_format.c`

 * *Files identical despite different names*

### Comparing `ihm-0.8/src/ihm_format.h` & `ihm-0.9/src/ihm_format.h`

 * *Files identical despite different names*

### Comparing `ihm-0.8/src/ihm_format.i` & `ihm-0.9/src/ihm_format.i`

 * *Files identical despite different names*

### Comparing `ihm-0.8/src/ihm_format_wrap_0.8.c` & `ihm-0.9/src/ihm_format_wrap_0.9.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /* ----------------------------------------------------------------------------
  * This file was automatically generated by SWIG (http://www.swig.org).
- * Version 4.0.0
+ * Version 3.0.12
  *
  * This file is not intended to be easily readable and contains a number of
  * coding conventions designed to improve portability and efficiency. Do not make
  * changes to this file unless you know what you are doing--modify the SWIG
  * interface file instead.
  * ----------------------------------------------------------------------------- */
 
@@ -136,24 +136,19 @@
  * See: https://github.com/swig/swig/issues/192 for more discussion.
  */
 #ifdef __INTEL_COMPILER
 # pragma warning disable 592
 #endif
 
 
-#if defined(__GNUC__) && defined(_WIN32) && !defined(SWIG_PYTHON_NO_HYPOT_WORKAROUND)
-/* Workaround for '::hypot' has not been declared', see https://bugs.python.org/issue11566 */
-# include <math.h>
-#endif
-
 #if defined(_DEBUG) && defined(SWIG_PYTHON_INTERPRETER_NO_DEBUG)
 /* Use debug wrappers with the Python release dll */
 # undef _DEBUG
 # include <Python.h>
-# define _DEBUG 1
+# define _DEBUG
 #else
 # include <Python.h>
 #endif
 
 /* -----------------------------------------------------------------------------
  * swigrun.swg
  *
@@ -195,15 +190,14 @@
 #ifndef SWIG_BUFFER_SIZE
 # define SWIG_BUFFER_SIZE 1024
 #endif
 
 /* Flags for pointer conversions */
 #define SWIG_POINTER_DISOWN        0x1
 #define SWIG_CAST_NEW_MEMORY       0x2
-#define SWIG_POINTER_NO_NULL       0x4
 
 /* Flags for new pointer objects */
 #define SWIG_POINTER_OWN           0x1
 
 
 /*
    Flags/methods for returning states.
@@ -781,24 +775,22 @@
 /* Warning: This function will allocate a new string in Python 3,
  * so please call SWIG_Python_str_DelForPy3(x) to free the space.
  */
 SWIGINTERN char*
 SWIG_Python_str_AsChar(PyObject *str)
 {
 #if PY_VERSION_HEX >= 0x03000000
-  char *newstr = 0;
+  char *cstr;
+  char *newstr;
+  Py_ssize_t len;
   str = PyUnicode_AsUTF8String(str);
-  if (str) {
-    char *cstr;
-    Py_ssize_t len;
-    PyBytes_AsStringAndSize(str, &cstr, &len);
-    newstr = (char *) malloc(len+1);
-    memcpy(newstr, cstr, len+1);
-    Py_XDECREF(str);
-  }
+  PyBytes_AsStringAndSize(str, &cstr, &len);
+  newstr = (char *) malloc(len+1);
+  memcpy(newstr, cstr, len+1);
+  Py_XDECREF(str);
   return newstr;
 #else
   return PyString_AsString(str);
 #endif
 }
 
 #if PY_VERSION_HEX >= 0x03000000
@@ -814,22 +806,152 @@
 #if PY_VERSION_HEX >= 0x03000000
   return PyUnicode_FromString(c); 
 #else
   return PyString_FromString(c);
 #endif
 }
 
+/* Add PyOS_snprintf for old Pythons */
+#if PY_VERSION_HEX < 0x02020000
+# if defined(_MSC_VER) || defined(__BORLANDC__) || defined(_WATCOM)
+#  define PyOS_snprintf _snprintf
+# else
+#  define PyOS_snprintf snprintf
+# endif
+#endif
+
+/* A crude PyString_FromFormat implementation for old Pythons */
+#if PY_VERSION_HEX < 0x02020000
+
+#ifndef SWIG_PYBUFFER_SIZE
+# define SWIG_PYBUFFER_SIZE 1024
+#endif
+
+static PyObject *
+PyString_FromFormat(const char *fmt, ...) {
+  va_list ap;
+  char buf[SWIG_PYBUFFER_SIZE * 2];
+  int res;
+  va_start(ap, fmt);
+  res = vsnprintf(buf, sizeof(buf), fmt, ap);
+  va_end(ap);
+  return (res < 0 || res >= (int)sizeof(buf)) ? 0 : PyString_FromString(buf);
+}
+#endif
+
 #ifndef PyObject_DEL
 # define PyObject_DEL PyObject_Del
 #endif
 
-// SWIGPY_USE_CAPSULE is no longer used within SWIG itself, but some user
-// interface files check for it.
+/* A crude PyExc_StopIteration exception for old Pythons */
+#if PY_VERSION_HEX < 0x02020000
+# ifndef PyExc_StopIteration
+#  define PyExc_StopIteration PyExc_RuntimeError
+# endif
+# ifndef PyObject_GenericGetAttr
+#  define PyObject_GenericGetAttr 0
+# endif
+#endif
+
+/* Py_NotImplemented is defined in 2.1 and up. */
+#if PY_VERSION_HEX < 0x02010000
+# ifndef Py_NotImplemented
+#  define Py_NotImplemented PyExc_RuntimeError
+# endif
+#endif
+
+/* A crude PyString_AsStringAndSize implementation for old Pythons */
+#if PY_VERSION_HEX < 0x02010000
+# ifndef PyString_AsStringAndSize
+#  define PyString_AsStringAndSize(obj, s, len) {*s = PyString_AsString(obj); *len = *s ? strlen(*s) : 0;}
+# endif
+#endif
+
+/* PySequence_Size for old Pythons */
+#if PY_VERSION_HEX < 0x02000000
+# ifndef PySequence_Size
+#  define PySequence_Size PySequence_Length
+# endif
+#endif
+
+/* PyBool_FromLong for old Pythons */
+#if PY_VERSION_HEX < 0x02030000
+static
+PyObject *PyBool_FromLong(long ok)
+{
+  PyObject *result = ok ? Py_True : Py_False;
+  Py_INCREF(result);
+  return result;
+}
+#endif
+
+/* Py_ssize_t for old Pythons */
+/* This code is as recommended by: */
+/* http://www.python.org/dev/peps/pep-0353/#conversion-guidelines */
+#if PY_VERSION_HEX < 0x02050000 && !defined(PY_SSIZE_T_MIN)
+typedef int Py_ssize_t;
+# define PY_SSIZE_T_MAX INT_MAX
+# define PY_SSIZE_T_MIN INT_MIN
+typedef inquiry lenfunc;
+typedef intargfunc ssizeargfunc;
+typedef intintargfunc ssizessizeargfunc;
+typedef intobjargproc ssizeobjargproc;
+typedef intintobjargproc ssizessizeobjargproc;
+typedef getreadbufferproc readbufferproc;
+typedef getwritebufferproc writebufferproc;
+typedef getsegcountproc segcountproc;
+typedef getcharbufferproc charbufferproc;
+static long PyNumber_AsSsize_t (PyObject *x, void *SWIGUNUSEDPARM(exc))
+{
+  long result = 0;
+  PyObject *i = PyNumber_Int(x);
+  if (i) {
+    result = PyInt_AsLong(i);
+    Py_DECREF(i);
+  }
+  return result;
+}
+#endif
+
+#if PY_VERSION_HEX < 0x02050000
+#define PyInt_FromSize_t(x) PyInt_FromLong((long)x)
+#endif
+
+#if PY_VERSION_HEX < 0x02040000
+#define Py_VISIT(op)				\
+  do { 						\
+    if (op) {					\
+      int vret = visit((op), arg);		\
+      if (vret)					\
+        return vret;				\
+    }						\
+  } while (0)
+#endif
+
+#if PY_VERSION_HEX < 0x02030000
+typedef struct {
+  PyTypeObject type;
+  PyNumberMethods as_number;
+  PyMappingMethods as_mapping;
+  PySequenceMethods as_sequence;
+  PyBufferProcs as_buffer;
+  PyObject *name, *slots;
+} PyHeapTypeObject;
+#endif
+
+#if PY_VERSION_HEX < 0x02030000
+typedef destructor freefunc;
+#endif
+
+#if ((PY_MAJOR_VERSION == 2 && PY_MINOR_VERSION > 6) || \
+     (PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION > 0) || \
+     (PY_MAJOR_VERSION > 3))
 # define SWIGPY_USE_CAPSULE
-# define SWIGPY_CAPSULE_NAME ("swig_runtime_data" SWIG_RUNTIME_VERSION ".type_pointer_capsule" SWIG_TYPE_TABLE_NAME)
+# define SWIGPY_CAPSULE_NAME ((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION ".type_pointer_capsule" SWIG_TYPE_TABLE_NAME)
+#endif
 
 #if PY_VERSION_HEX < 0x03020000
 #define PyDescr_TYPE(x) (((PyDescrObject *)(x))->d_type)
 #define PyDescr_NAME(x) (((PyDescrObject *)(x))->d_name)
 #define Py_hash_t long
 #endif
 
@@ -884,72 +1006,40 @@
 SWIGRUNTIME void
 SWIG_Python_AddErrorMsg(const char* mesg)
 {
   PyObject *type = 0;
   PyObject *value = 0;
   PyObject *traceback = 0;
 
-  if (PyErr_Occurred())
-    PyErr_Fetch(&type, &value, &traceback);
+  if (PyErr_Occurred()) PyErr_Fetch(&type, &value, &traceback);
   if (value) {
+    char *tmp;
     PyObject *old_str = PyObject_Str(value);
-    const char *tmp = SWIG_Python_str_AsChar(old_str);
     PyErr_Clear();
     Py_XINCREF(type);
-    if (tmp)
-      PyErr_Format(type, "%s %s", tmp, mesg);
-    else
-      PyErr_Format(type, "%s", mesg);
+
+    PyErr_Format(type, "%s %s", tmp = SWIG_Python_str_AsChar(old_str), mesg);
     SWIG_Python_str_DelForPy3(tmp);
     Py_DECREF(old_str);
     Py_DECREF(value);
   } else {
     PyErr_SetString(PyExc_RuntimeError, mesg);
   }
 }
 
-SWIGRUNTIME int
-SWIG_Python_TypeErrorOccurred(PyObject *obj)
-{
-  PyObject *error;
-  if (obj)
-    return 0;
-  error = PyErr_Occurred();
-  return error && PyErr_GivenExceptionMatches(error, PyExc_TypeError);
-}
-
-SWIGRUNTIME void
-SWIG_Python_RaiseOrModifyTypeError(const char *message)
-{
-  if (SWIG_Python_TypeErrorOccurred(NULL)) {
-    /* Use existing TypeError to preserve stacktrace and enhance with given message */
-    PyObject *newvalue;
-    PyObject *type = NULL, *value = NULL, *traceback = NULL;
-    PyErr_Fetch(&type, &value, &traceback);
-#if PY_VERSION_HEX >= 0x03000000
-    newvalue = PyUnicode_FromFormat("%S\nAdditional information:\n%s", value, message);
-#else
-    newvalue = PyString_FromFormat("%s\nAdditional information:\n%s", PyString_AsString(value), message);
-#endif
-    Py_XDECREF(value);
-    PyErr_Restore(type, newvalue, traceback);
-  } else {
-    /* Raise TypeError using given message */
-    PyErr_SetString(PyExc_TypeError, message);
-  }
-}
-
 #if defined(SWIG_PYTHON_NO_THREADS)
 #  if defined(SWIG_PYTHON_THREADS)
 #    undef SWIG_PYTHON_THREADS
 #  endif
 #endif
 #if defined(SWIG_PYTHON_THREADS) /* Threading support is enabled */
 #  if !defined(SWIG_PYTHON_USE_GIL) && !defined(SWIG_PYTHON_NO_USE_GIL)
-#    define SWIG_PYTHON_USE_GIL
+#    if (PY_VERSION_HEX >= 0x02030000) /* For 2.3 or later, use the PyGILState calls */
+#      define SWIG_PYTHON_USE_GIL
+#    endif
 #  endif
 #  if defined(SWIG_PYTHON_USE_GIL) /* Use PyGILState threads calls */
 #    ifndef SWIG_PYTHON_INITIALIZE_THREADS
 #     define SWIG_PYTHON_INITIALIZE_THREADS  PyEval_InitThreads() 
 #    endif
 #    ifdef __cplusplus /* C++ code */
        class SWIG_Python_Thread_Block {
@@ -1018,43 +1108,52 @@
 /* Constant Types */
 #define SWIG_PY_POINTER 4
 #define SWIG_PY_BINARY  5
 
 /* Constant information structure */
 typedef struct swig_const_info {
   int type;
-  const char *name;
+  char *name;
   long lvalue;
   double dvalue;
   void   *pvalue;
   swig_type_info **ptype;
 } swig_const_info;
 
+
+/* -----------------------------------------------------------------------------
+ * Wrapper of PyInstanceMethod_New() used in Python 3
+ * It is exported to the generated module, used for -fastproxy
+ * ----------------------------------------------------------------------------- */
+#if PY_VERSION_HEX >= 0x03000000
+SWIGRUNTIME PyObject* SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func)
+{
+  return PyInstanceMethod_New(func);
+}
+#else
+SWIGRUNTIME PyObject* SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *SWIGUNUSEDPARM(func))
+{
+  return NULL;
+}
+#endif
+
 #ifdef __cplusplus
 }
 #endif
 
 
 /* -----------------------------------------------------------------------------
  * pyrun.swg
  *
  * This file contains the runtime support for Python modules
  * and includes code for managing global variables and pointer
  * type checking.
  *
  * ----------------------------------------------------------------------------- */
 
-#if PY_VERSION_HEX < 0x02070000 /* 2.7.0 */
-# error "This version of SWIG only supports Python >= 2.7"
-#endif
-
-#if PY_VERSION_HEX >= 0x03000000 && PY_VERSION_HEX < 0x03020000
-# error "This version of SWIG only supports Python 3 >= 3.2"
-#endif
-
 /* Common SWIG API */
 
 /* for raw pointers */
 #define SWIG_Python_ConvertPtr(obj, pptr, type, flags)  SWIG_Python_ConvertPtrAndOwn(obj, pptr, type, flags, 0)
 #define SWIG_ConvertPtr(obj, pptr, type, flags)         SWIG_Python_ConvertPtr(obj, pptr, type, flags)
 #define SWIG_ConvertPtrAndOwn(obj,pptr,type,flags,own)  SWIG_Python_ConvertPtrAndOwn(obj, pptr, type, flags, own)
 
@@ -1130,34 +1229,43 @@
   PyObject *s = PyString_InternFromString(key);
   PyList_Append(seq, s);
   Py_DECREF(s);
 }
 
 SWIGINTERN void
 SWIG_Python_SetConstant(PyObject *d, PyObject *public_interface, const char *name, PyObject *obj) {   
+#if PY_VERSION_HEX < 0x02030000
+  PyDict_SetItemString(d, (char *)name, obj);
+#else
   PyDict_SetItemString(d, name, obj);
+#endif
   Py_DECREF(obj);
   if (public_interface)
     SwigPyBuiltin_AddPublicSymbol(public_interface, name);
 }
 
 #else
 
 SWIGINTERN void
 SWIG_Python_SetConstant(PyObject *d, const char *name, PyObject *obj) {   
+#if PY_VERSION_HEX < 0x02030000
+  PyDict_SetItemString(d, (char *)name, obj);
+#else
   PyDict_SetItemString(d, name, obj);
+#endif
   Py_DECREF(obj);                            
 }
 
 #endif
 
 /* Append a value to the result obj */
 
 SWIGINTERN PyObject*
 SWIG_Python_AppendOutput(PyObject* result, PyObject* obj) {
+#if !defined(SWIG_PYTHON_OUTPUT_TUPLE)
   if (!result) {
     result = obj;
   } else if (result == Py_None) {
     Py_DECREF(result);
     result = obj;
   } else {
     if (!PyList_Check(result)) {
@@ -1165,14 +1273,37 @@
       result = PyList_New(1);
       PyList_SetItem(result, 0, o2);
     }
     PyList_Append(result,obj);
     Py_DECREF(obj);
   }
   return result;
+#else
+  PyObject*   o2;
+  PyObject*   o3;
+  if (!result) {
+    result = obj;
+  } else if (result == Py_None) {
+    Py_DECREF(result);
+    result = obj;
+  } else {
+    if (!PyTuple_Check(result)) {
+      o2 = result;
+      result = PyTuple_New(1);
+      PyTuple_SET_ITEM(result, 0, o2);
+    }
+    o3 = PyTuple_New(1);
+    PyTuple_SET_ITEM(o3, 0, obj);
+    o2 = result;
+    result = PySequence_Concat(o2, o3);
+    Py_DECREF(o2);
+    Py_DECREF(o3);
+  }
+  return result;
+#endif
 }
 
 /* Unpack the argument tuple */
 
 SWIGINTERN Py_ssize_t
 SWIG_Python_UnpackTuple(PyObject *args, const char *name, Py_ssize_t min, Py_ssize_t max, PyObject **objs)
 {
@@ -1216,15 +1347,19 @@
       }
       return i + 1;
     }    
   }
 }
 
 /* A functor is a function object with one single object argument */
-#define SWIG_Python_CallFunctor(functor, obj)	        PyObject_CallFunction(functor, (char *)"O", obj);
+#if PY_VERSION_HEX >= 0x02020000
+#define SWIG_Python_CallFunctor(functor, obj)	        PyObject_CallFunctionObjArgs(functor, obj, NULL);
+#else
+#define SWIG_Python_CallFunctor(functor, obj)	        PyObject_CallFunction(functor, "O", obj);
+#endif
 
 /*
   Helper for static pointer initialization for both C and C++ code, for example
   static PyObject *SWIG_STATIC_POINTER(MyVar) = NewSomething(...);
 */
 #ifdef __cplusplus
 #define SWIG_STATIC_POINTER(var)  var
@@ -1245,14 +1380,43 @@
 #define SWIG_BUILTIN_TP_INIT	    (SWIG_POINTER_OWN << 2)
 #define SWIG_BUILTIN_INIT	    (SWIG_BUILTIN_TP_INIT | SWIG_POINTER_OWN)
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
+/*  How to access Py_None */
+#if defined(_WIN32) || defined(__WIN32__) || defined(__CYGWIN__)
+#  ifndef SWIG_PYTHON_NO_BUILD_NONE
+#    ifndef SWIG_PYTHON_BUILD_NONE
+#      define SWIG_PYTHON_BUILD_NONE
+#    endif
+#  endif
+#endif
+
+#ifdef SWIG_PYTHON_BUILD_NONE
+#  ifdef Py_None
+#   undef Py_None
+#   define Py_None SWIG_Py_None()
+#  endif
+SWIGRUNTIMEINLINE PyObject * 
+_SWIG_Py_None(void)
+{
+  PyObject *none = Py_BuildValue((char*)"");
+  Py_DECREF(none);
+  return none;
+}
+SWIGRUNTIME PyObject * 
+SWIG_Py_None(void)
+{
+  static PyObject *SWIG_STATIC_POINTER(none) = _SWIG_Py_None();
+  return none;
+}
+#endif
+
 /* The python void return value */
 
 SWIGRUNTIMEINLINE PyObject * 
 SWIG_Py_Void(void)
 {
   PyObject *none = Py_None;
   Py_INCREF(none);
@@ -1271,18 +1435,15 @@
   PyTypeObject *pytype;
 } SwigPyClientData;
 
 SWIGRUNTIMEINLINE int 
 SWIG_Python_CheckImplicit(swig_type_info *ty)
 {
   SwigPyClientData *data = (SwigPyClientData *)ty->clientdata;
-  int fail = data ? data->implicitconv : 0;
-  if (fail)
-    PyErr_SetString(PyExc_TypeError, "Implicit conversion is prohibited for explicit constructors.");
-  return fail;
+  return data ? data->implicitconv : 0;
 }
 
 SWIGRUNTIMEINLINE PyObject *
 SWIG_Python_ExceptionType(swig_type_info *desc) {
   SwigPyClientData *data = desc ? (SwigPyClientData *) desc->clientdata : 0;
   PyObject *klass = data ? data->klass : 0;
   return (klass ? klass : PyExc_RuntimeError);
@@ -1301,35 +1462,43 @@
     Py_INCREF(data->klass);
     /* the newraw method and newargs arguments used to create a new raw instance */
     if (PyClass_Check(obj)) {
       data->newraw = 0;
       data->newargs = obj;
       Py_INCREF(obj);
     } else {
-      data->newraw = PyObject_GetAttrString(data->klass, "__new__");
+#if (PY_VERSION_HEX < 0x02020000)
+      data->newraw = 0;
+#else
+      data->newraw = PyObject_GetAttrString(data->klass, (char *)"__new__");
+#endif
       if (data->newraw) {
 	Py_INCREF(data->newraw);
 	data->newargs = PyTuple_New(1);
 	PyTuple_SetItem(data->newargs, 0, obj);
       } else {
 	data->newargs = obj;
       }
       Py_INCREF(data->newargs);
     }
     /* the destroy method, aka as the C++ delete method */
-    data->destroy = PyObject_GetAttrString(data->klass, "__swig_destroy__");
+    data->destroy = PyObject_GetAttrString(data->klass, (char *)"__swig_destroy__");
     if (PyErr_Occurred()) {
       PyErr_Clear();
       data->destroy = 0;
     }
     if (data->destroy) {
       int flags;
       Py_INCREF(data->destroy);
       flags = PyCFunction_GET_FLAGS(data->destroy);
+#ifdef METH_O
       data->delargs = !(flags & (METH_O));
+#else
+      data->delargs = 0;
+#endif
     } else {
       data->delargs = 0;
     }
     data->implicitconv = 0;
     data->pytype = 0;
     return data;
   }
@@ -1409,40 +1578,40 @@
 SWIGRUNTIME PyObject *
 SwigPyObject_hex(SwigPyObject *v)
 {
   return SwigPyObject_format("%x",v);
 }
 
 SWIGRUNTIME PyObject *
+#ifdef METH_NOARGS
 SwigPyObject_repr(SwigPyObject *v)
+#else
+SwigPyObject_repr(SwigPyObject *v, PyObject *args)
+#endif
 {
   const char *name = SWIG_TypePrettyName(v->ty);
   PyObject *repr = SWIG_Python_str_FromFormat("<Swig Object of type '%s' at %p>", (name ? name : "unknown"), (void *)v);
   if (v->next) {
+# ifdef METH_NOARGS
     PyObject *nrep = SwigPyObject_repr((SwigPyObject *)v->next);
+# else
+    PyObject *nrep = SwigPyObject_repr((SwigPyObject *)v->next, args);
+# endif
 # if PY_VERSION_HEX >= 0x03000000
     PyObject *joined = PyUnicode_Concat(repr, nrep);
     Py_DecRef(repr);
     Py_DecRef(nrep);
     repr = joined;
 # else
     PyString_ConcatAndDel(&repr,nrep);
 # endif
   }
   return repr;  
 }
 
-/* We need a version taking two PyObject* parameters so it's a valid
- * PyCFunction to use in swigobject_methods[]. */
-SWIGRUNTIME PyObject *
-SwigPyObject_repr2(PyObject *v, PyObject *SWIGUNUSEDPARM(args))
-{
-  return SwigPyObject_repr((SwigPyObject*)v);
-}
-
 SWIGRUNTIME int
 SwigPyObject_compare(SwigPyObject *v, SwigPyObject *w)
 {
   void *i = v->ptr;
   void *j = w->ptr;
   return (i < j) ? -1 : ((i > j) ? 1 : 0);
 }
@@ -1508,37 +1677,37 @@
     SwigPyClientData *data = ty ? (SwigPyClientData *) ty->clientdata : 0;
     PyObject *destroy = data ? data->destroy : 0;
     if (destroy) {
       /* destroy is always a VARARGS method */
       PyObject *res;
 
       /* PyObject_CallFunction() has the potential to silently drop
-         the active exception.  In cases of unnamed temporary
+         the active active exception.  In cases of unnamed temporary
          variable or where we just finished iterating over a generator
          StopIteration will be active right now, and this needs to
          remain true upon return from SwigPyObject_dealloc.  So save
          and restore. */
       
-      PyObject *type = NULL, *value = NULL, *traceback = NULL;
-      PyErr_Fetch(&type, &value, &traceback);
+      PyObject *val = NULL, *type = NULL, *tb = NULL;
+      PyErr_Fetch(&val, &type, &tb);
 
       if (data->delargs) {
         /* we need to create a temporary object to carry the destroy operation */
         PyObject *tmp = SwigPyObject_New(sobj->ptr, ty, 0);
         res = SWIG_Python_CallFunctor(destroy, tmp);
         Py_DECREF(tmp);
       } else {
         PyCFunction meth = PyCFunction_GET_FUNCTION(destroy);
         PyObject *mself = PyCFunction_GET_SELF(destroy);
         res = ((*meth)(mself, v));
       }
       if (!res)
         PyErr_WriteUnraisable(destroy);
 
-      PyErr_Restore(type, value, traceback);
+      PyErr_Restore(val, type, tb);
 
       Py_XDECREF(res);
     } 
 #if !defined(SWIG_PYTHON_SILENT_MEMLEAK)
     else {
       const char *name = SWIG_TypePrettyName(ty);
       printf("swig/python detected a memory leak of type '%s', no destructor found.\n", (name ? name : "unknown"));
@@ -1549,81 +1718,136 @@
   PyObject_DEL(v);
 }
 
 SWIGRUNTIME PyObject* 
 SwigPyObject_append(PyObject* v, PyObject* next)
 {
   SwigPyObject *sobj = (SwigPyObject *) v;
+#ifndef METH_O
+  PyObject *tmp = 0;
+  if (!PyArg_ParseTuple(next,(char *)"O:append", &tmp)) return NULL;
+  next = tmp;
+#endif
   if (!SwigPyObject_Check(next)) {
     PyErr_SetString(PyExc_TypeError, "Attempt to append a non SwigPyObject");
     return NULL;
   }
   sobj->next = next;
   Py_INCREF(next);
   return SWIG_Py_Void();
 }
 
 SWIGRUNTIME PyObject* 
+#ifdef METH_NOARGS
+SwigPyObject_next(PyObject* v)
+#else
 SwigPyObject_next(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
+#endif
 {
   SwigPyObject *sobj = (SwigPyObject *) v;
   if (sobj->next) {    
     Py_INCREF(sobj->next);
     return sobj->next;
   } else {
     return SWIG_Py_Void();
   }
 }
 
 SWIGINTERN PyObject*
+#ifdef METH_NOARGS
+SwigPyObject_disown(PyObject *v)
+#else
 SwigPyObject_disown(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
+#endif
 {
   SwigPyObject *sobj = (SwigPyObject *)v;
   sobj->own = 0;
   return SWIG_Py_Void();
 }
 
 SWIGINTERN PyObject*
+#ifdef METH_NOARGS
+SwigPyObject_acquire(PyObject *v)
+#else
 SwigPyObject_acquire(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
+#endif
 {
   SwigPyObject *sobj = (SwigPyObject *)v;
   sobj->own = SWIG_POINTER_OWN;
   return SWIG_Py_Void();
 }
 
 SWIGINTERN PyObject*
 SwigPyObject_own(PyObject *v, PyObject *args)
 {
   PyObject *val = 0;
-  if (!PyArg_UnpackTuple(args, "own", 0, 1, &val)) {
-    return NULL;
-  } else {
-    SwigPyObject *sobj = (SwigPyObject *)v;
-    PyObject *obj = PyBool_FromLong(sobj->own);
-    if (val) {
-      if (PyObject_IsTrue(val)) {
-        SwigPyObject_acquire(v,args);
-      } else {
-        SwigPyObject_disown(v,args);
-      }
+#if (PY_VERSION_HEX < 0x02020000)
+  if (!PyArg_ParseTuple(args,(char *)"|O:own",&val))
+#elif (PY_VERSION_HEX < 0x02050000)
+  if (!PyArg_UnpackTuple(args, (char *)"own", 0, 1, &val)) 
+#else
+  if (!PyArg_UnpackTuple(args, "own", 0, 1, &val)) 
+#endif
+    {
+      return NULL;
     } 
-    return obj;
-  }
+  else
+    {
+      SwigPyObject *sobj = (SwigPyObject *)v;
+      PyObject *obj = PyBool_FromLong(sobj->own);
+      if (val) {
+#ifdef METH_NOARGS
+	if (PyObject_IsTrue(val)) {
+	  SwigPyObject_acquire(v);
+	} else {
+	  SwigPyObject_disown(v);
+	}
+#else
+	if (PyObject_IsTrue(val)) {
+	  SwigPyObject_acquire(v,args);
+	} else {
+	  SwigPyObject_disown(v,args);
+	}
+#endif
+      } 
+      return obj;
+    }
 }
 
+#ifdef METH_O
 static PyMethodDef
 swigobject_methods[] = {
-  {"disown",  SwigPyObject_disown,  METH_NOARGS,  "releases ownership of the pointer"},
-  {"acquire", SwigPyObject_acquire, METH_NOARGS,  "acquires ownership of the pointer"},
-  {"own",     SwigPyObject_own,     METH_VARARGS, "returns/sets ownership of the pointer"},
-  {"append",  SwigPyObject_append,  METH_O,       "appends another 'this' object"},
-  {"next",    SwigPyObject_next,    METH_NOARGS,  "returns the next 'this' object"},
-  {"__repr__",SwigPyObject_repr2,   METH_NOARGS,  "returns object representation"},
+  {(char *)"disown",  (PyCFunction)SwigPyObject_disown,  METH_NOARGS,  (char *)"releases ownership of the pointer"},
+  {(char *)"acquire", (PyCFunction)SwigPyObject_acquire, METH_NOARGS,  (char *)"acquires ownership of the pointer"},
+  {(char *)"own",     (PyCFunction)SwigPyObject_own,     METH_VARARGS, (char *)"returns/sets ownership of the pointer"},
+  {(char *)"append",  (PyCFunction)SwigPyObject_append,  METH_O,       (char *)"appends another 'this' object"},
+  {(char *)"next",    (PyCFunction)SwigPyObject_next,    METH_NOARGS,  (char *)"returns the next 'this' object"},
+  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr,    METH_NOARGS,  (char *)"returns object representation"},
   {0, 0, 0, 0}  
 };
+#else
+static PyMethodDef
+swigobject_methods[] = {
+  {(char *)"disown",  (PyCFunction)SwigPyObject_disown,  METH_VARARGS,  (char *)"releases ownership of the pointer"},
+  {(char *)"acquire", (PyCFunction)SwigPyObject_acquire, METH_VARARGS,  (char *)"acquires ownership of the pointer"},
+  {(char *)"own",     (PyCFunction)SwigPyObject_own,     METH_VARARGS,  (char *)"returns/sets ownership of the pointer"},
+  {(char *)"append",  (PyCFunction)SwigPyObject_append,  METH_VARARGS,  (char *)"appends another 'this' object"},
+  {(char *)"next",    (PyCFunction)SwigPyObject_next,    METH_VARARGS,  (char *)"returns the next 'this' object"},
+  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr,   METH_VARARGS,  (char *)"returns object representation"},
+  {0, 0, 0, 0}  
+};
+#endif
+
+#if PY_VERSION_HEX < 0x02020000
+SWIGINTERN PyObject *
+SwigPyObject_getattr(SwigPyObject *sobj,char *name)
+{
+  return Py_FindMethod(swigobject_methods, (PyObject *)sobj, name);
+}
+#endif
 
 SWIGRUNTIME PyTypeObject*
 SwigPyObject_TypeOnce(void) {
   static char swigobject_doc[] = "Swig object carries a C/C++ instance pointer";
 
   static PyNumberMethods SwigPyObject_as_number = {
     (binaryfunc)0, /*nb_add*/
@@ -1660,35 +1884,43 @@
     (unaryfunc)SwigPyObject_oct,  /*nb_oct*/
     (unaryfunc)SwigPyObject_hex,  /*nb_hex*/
 #endif
 #if PY_VERSION_HEX >= 0x03050000 /* 3.5 */
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_matrix_multiply */
 #elif PY_VERSION_HEX >= 0x03000000 /* 3.0 */
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_index, nb_inplace_divide removed */
-#else
+#elif PY_VERSION_HEX >= 0x02050000 /* 2.5.0 */
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_index */
+#elif PY_VERSION_HEX >= 0x02020000 /* 2.2.0 */
+    0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_true_divide */
+#elif PY_VERSION_HEX >= 0x02000000 /* 2.0.0 */
+    0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_or */
 #endif
   };
 
   static PyTypeObject swigpyobject_type;
   static int type_init = 0;
   if (!type_init) {
     const PyTypeObject tmp = {
 #if PY_VERSION_HEX >= 0x03000000
       PyVarObject_HEAD_INIT(NULL, 0)
 #else
       PyObject_HEAD_INIT(NULL)
       0,                                    /* ob_size */
 #endif
-      "SwigPyObject",                       /* tp_name */
+      (char *)"SwigPyObject",               /* tp_name */
       sizeof(SwigPyObject),                 /* tp_basicsize */
       0,                                    /* tp_itemsize */
       (destructor)SwigPyObject_dealloc,     /* tp_dealloc */
       0,                                    /* tp_print */
+#if PY_VERSION_HEX < 0x02020000
+      (getattrfunc)SwigPyObject_getattr,    /* tp_getattr */
+#else
       (getattrfunc)0,                       /* tp_getattr */
+#endif
       (setattrfunc)0,                       /* tp_setattr */
 #if PY_VERSION_HEX >= 0x03000000
       0, /* tp_reserved in 3.0.1, tp_compare in 3.0.0 but not used */
 #else
       (cmpfunc)SwigPyObject_compare,        /* tp_compare */
 #endif
       (reprfunc)SwigPyObject_repr,          /* tp_repr */
@@ -1703,14 +1935,15 @@
       0,                                    /* tp_as_buffer */
       Py_TPFLAGS_DEFAULT,                   /* tp_flags */
       swigobject_doc,                       /* tp_doc */
       0,                                    /* tp_traverse */
       0,                                    /* tp_clear */
       (richcmpfunc)SwigPyObject_richcompare,/* tp_richcompare */
       0,                                    /* tp_weaklistoffset */
+#if PY_VERSION_HEX >= 0x02020000
       0,                                    /* tp_iter */
       0,                                    /* tp_iternext */
       swigobject_methods,                   /* tp_methods */
       0,                                    /* tp_members */
       0,                                    /* tp_getset */
       0,                                    /* tp_base */
       0,                                    /* tp_dict */
@@ -1723,31 +1956,42 @@
       0,                                    /* tp_free */
       0,                                    /* tp_is_gc */
       0,                                    /* tp_bases */
       0,                                    /* tp_mro */
       0,                                    /* tp_cache */
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
+#endif
+#if PY_VERSION_HEX >= 0x02030000
       0,                                    /* tp_del */
+#endif
+#if PY_VERSION_HEX >= 0x02060000
       0,                                    /* tp_version_tag */
+#endif
 #if PY_VERSION_HEX >= 0x03040000
       0,                                    /* tp_finalize */
 #endif
 #ifdef COUNT_ALLOCS
       0,                                    /* tp_allocs */
       0,                                    /* tp_frees */
       0,                                    /* tp_maxalloc */
+#if PY_VERSION_HEX >= 0x02050000
       0,                                    /* tp_prev */
+#endif
       0                                     /* tp_next */
 #endif
     };
     swigpyobject_type = tmp;
     type_init = 1;
+#if PY_VERSION_HEX < 0x02020000
+    swigpyobject_type.ob_type = &PyType_Type;
+#else
     if (PyType_Ready(&swigpyobject_type) < 0)
       return NULL;
+#endif
   }
   return &swigpyobject_type;
 }
 
 SWIGRUNTIME PyObject *
 SwigPyObject_New(void *ptr, swig_type_info *ty, int own)
 {
@@ -1768,14 +2012,28 @@
 typedef struct {
   PyObject_HEAD
   void *pack;
   swig_type_info *ty;
   size_t size;
 } SwigPyPacked;
 
+SWIGRUNTIME int
+SwigPyPacked_print(SwigPyPacked *v, FILE *fp, int SWIGUNUSEDPARM(flags))
+{
+  char result[SWIG_BUFFER_SIZE];
+  fputs("<Swig Packed ", fp); 
+  if (SWIG_PackDataName(result, v->pack, v->size, 0, sizeof(result))) {
+    fputs("at ", fp); 
+    fputs(result, fp); 
+  }
+  fputs(v->ty->name,fp); 
+  fputs(">", fp);
+  return 0; 
+}
+  
 SWIGRUNTIME PyObject *
 SwigPyPacked_repr(SwigPyPacked *v)
 {
   char result[SWIG_BUFFER_SIZE];
   if (SWIG_PackDataName(result, v->pack, v->size, 0, sizeof(result))) {
     return SWIG_Python_str_FromFormat("<Swig Packed at %s%s>", result, v->ty->name);
   } else {
@@ -1796,15 +2054,15 @@
 
 SWIGRUNTIME int
 SwigPyPacked_compare(SwigPyPacked *v, SwigPyPacked *w)
 {
   size_t i = v->size;
   size_t j = w->size;
   int s = (i < j) ? -1 : ((i > j) ? 1 : 0);
-  return s ? s : strncmp((const char *)v->pack, (const char *)w->pack, 2*v->size);
+  return s ? s : strncmp((char *)v->pack, (char *)w->pack, 2*v->size);
 }
 
 SWIGRUNTIME PyTypeObject* SwigPyPacked_TypeOnce(void);
 
 SWIGRUNTIME PyTypeObject*
 SwigPyPacked_type(void) {
   static PyTypeObject *SWIG_STATIC_POINTER(type) = SwigPyPacked_TypeOnce();
@@ -1836,19 +2094,19 @@
     const PyTypeObject tmp = {
 #if PY_VERSION_HEX>=0x03000000
       PyVarObject_HEAD_INIT(NULL, 0)
 #else
       PyObject_HEAD_INIT(NULL)
       0,                                    /* ob_size */
 #endif
-      "SwigPyPacked",                       /* tp_name */
+      (char *)"SwigPyPacked",               /* tp_name */
       sizeof(SwigPyPacked),                 /* tp_basicsize */
       0,                                    /* tp_itemsize */
       (destructor)SwigPyPacked_dealloc,     /* tp_dealloc */
-      0,                                    /* tp_print */
+      (printfunc)SwigPyPacked_print,        /* tp_print */
       (getattrfunc)0,                       /* tp_getattr */
       (setattrfunc)0,                       /* tp_setattr */
 #if PY_VERSION_HEX>=0x03000000
       0, /* tp_reserved in 3.0.1 */
 #else
       (cmpfunc)SwigPyPacked_compare,        /* tp_compare */
 #endif
@@ -1864,14 +2122,15 @@
       0,                                    /* tp_as_buffer */
       Py_TPFLAGS_DEFAULT,                   /* tp_flags */
       swigpacked_doc,                       /* tp_doc */
       0,                                    /* tp_traverse */
       0,                                    /* tp_clear */
       0,                                    /* tp_richcompare */
       0,                                    /* tp_weaklistoffset */
+#if PY_VERSION_HEX >= 0x02020000
       0,                                    /* tp_iter */
       0,                                    /* tp_iternext */
       0,                                    /* tp_methods */
       0,                                    /* tp_members */
       0,                                    /* tp_getset */
       0,                                    /* tp_base */
       0,                                    /* tp_dict */
@@ -1884,31 +2143,42 @@
       0,                                    /* tp_free */
       0,                                    /* tp_is_gc */
       0,                                    /* tp_bases */
       0,                                    /* tp_mro */
       0,                                    /* tp_cache */
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
+#endif
+#if PY_VERSION_HEX >= 0x02030000
       0,                                    /* tp_del */
+#endif
+#if PY_VERSION_HEX >= 0x02060000
       0,                                    /* tp_version_tag */
+#endif
 #if PY_VERSION_HEX >= 0x03040000
       0,                                    /* tp_finalize */
 #endif
 #ifdef COUNT_ALLOCS
       0,                                    /* tp_allocs */
       0,                                    /* tp_frees */
       0,                                    /* tp_maxalloc */
+#if PY_VERSION_HEX >= 0x02050000
       0,                                    /* tp_prev */
+#endif
       0                                     /* tp_next */
 #endif
     };
     swigpypacked_type = tmp;
     type_init = 1;
+#if PY_VERSION_HEX < 0x02020000
+    swigpypacked_type.ob_type = &PyType_Type;
+#else
     if (PyType_Ready(&swigpypacked_type) < 0)
       return NULL;
+#endif
   }
   return &swigpypacked_type;
 }
 
 SWIGRUNTIME PyObject *
 SwigPyPacked_New(void *ptr, size_t size, swig_type_info *ty)
 {
@@ -1941,22 +2211,28 @@
   }
 }
 
 /* -----------------------------------------------------------------------------
  * pointers/data manipulation
  * ----------------------------------------------------------------------------- */
 
-static PyObject *Swig_This_global = NULL;
+SWIGRUNTIMEINLINE PyObject *
+_SWIG_This(void)
+{
+    return SWIG_Python_str_FromChar("this");
+}
+
+static PyObject *swig_this = NULL;
 
 SWIGRUNTIME PyObject *
 SWIG_This(void)
 {
-  if (Swig_This_global == NULL)
-    Swig_This_global = SWIG_Python_str_FromChar("this");
-  return Swig_This_global;
+  if (swig_this == NULL)
+    swig_this = _SWIG_This();
+  return swig_this;
 }
 
 /* #define SWIG_PYTHON_SLOW_GETSET_THIS */
 
 /* TODO: I don't know how to implement the fast getset in Python 3 right now */
 #if PY_VERSION_HEX>=0x03000000
 #define SWIG_PYTHON_SLOW_GETSET_THIS 
@@ -1980,15 +2256,15 @@
   }
 # endif
   return NULL;
 #else
 
   obj = 0;
 
-#if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
+#if (!defined(SWIG_PYTHON_SLOW_GETSET_THIS) && (PY_VERSION_HEX >= 0x02030000))
   if (PyInstance_Check(pyobj)) {
     obj = _PyInstance_Lookup(pyobj, SWIG_This());      
   } else {
     PyObject **dictptr = _PyObject_GetDictPtr(pyobj);
     if (dictptr != NULL) {
       PyObject *dict = *dictptr;
       obj = dict ? PyDict_GetItem(dict, SWIG_This()) : 0;
@@ -2050,15 +2326,15 @@
   int implicit_conv = (flags & SWIG_POINTER_IMPLICIT_CONV) != 0;
 
   if (!obj)
     return SWIG_ERROR;
   if (obj == Py_None && !implicit_conv) {
     if (ptr)
       *ptr = 0;
-    return (flags & SWIG_POINTER_NO_NULL) ? SWIG_NullReferenceError : SWIG_OK;
+    return SWIG_OK;
   }
 
   res = SWIG_ERROR;
 
   sobj = SWIG_Python_GetSwigThis(obj);
   if (own)
     *own = 0;
@@ -2130,21 +2406,21 @@
                 }
               }
             }
             Py_DECREF(impconv);
           }
         }
       }
-      if (!SWIG_IsOK(res) && obj == Py_None) {
-        if (ptr)
-          *ptr = 0;
-        if (PyErr_Occurred())
-          PyErr_Clear();
-        res = SWIG_OK;
-      }
+    }
+    if (!SWIG_IsOK(res) && obj == Py_None) {
+      if (ptr)
+        *ptr = 0;
+      if (PyErr_Occurred())
+        PyErr_Clear();
+      res = SWIG_OK;
     }
   }
   return res;
 }
 
 /* Convert a function ptr value */
 
@@ -2171,15 +2447,15 @@
     } else {
       return SWIG_ERROR;
     }
     return SWIG_OK;
   }
 }
 
-/* Convert a packed pointer value */
+/* Convert a packed value value */
 
 SWIGRUNTIME int
 SWIG_Python_ConvertPacked(PyObject *obj, void *ptr, size_t sz, swig_type_info *ty) {
   swig_type_info *to = SwigPyPacked_UnpackData(obj, ptr, sz);
   if (!to) return SWIG_ERROR;
   if (ty) {
     if (to != ty) {
@@ -2199,14 +2475,15 @@
   Create a new instance object, without calling __init__, and set the
   'this' attribute.
 */
 
 SWIGRUNTIME PyObject* 
 SWIG_Python_NewShadowInstance(SwigPyClientData *data, PyObject *swig_this)
 {
+#if (PY_VERSION_HEX >= 0x02020000)
   PyObject *inst = 0;
   PyObject *newraw = data->newraw;
   if (newraw) {
     inst = PyObject_Call(newraw, data->newargs, NULL);
     if (inst) {
 #if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
       PyObject **dictptr = _PyObject_GetDictPtr(inst);
@@ -2221,56 +2498,80 @@
 #else
       PyObject *key = SWIG_This();
       PyObject_SetAttr(inst, key, swig_this);
 #endif
     }
   } else {
 #if PY_VERSION_HEX >= 0x03000000
-    PyObject *empty_args = PyTuple_New(0);
-    if (empty_args) {
-      PyObject *empty_kwargs = PyDict_New();
-      if (empty_kwargs) {
-        inst = ((PyTypeObject *)data->newargs)->tp_new((PyTypeObject *)data->newargs, empty_args, empty_kwargs);
-        Py_DECREF(empty_kwargs);
-        if (inst) {
-          PyObject_SetAttr(inst, SWIG_This(), swig_this);
-          Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
-        }
-      }
-      Py_DECREF(empty_args);
+    inst = ((PyTypeObject*) data->newargs)->tp_new((PyTypeObject*) data->newargs, Py_None, Py_None);
+    if (inst) {
+      PyObject_SetAttr(inst, SWIG_This(), swig_this);
+      Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
     }
 #else
     PyObject *dict = PyDict_New();
     if (dict) {
       PyDict_SetItem(dict, SWIG_This(), swig_this);
       inst = PyInstance_NewRaw(data->newargs, dict);
       Py_DECREF(dict);
     }
 #endif
   }
   return inst;
+#else
+#if (PY_VERSION_HEX >= 0x02010000)
+  PyObject *inst = 0;
+  PyObject *dict = PyDict_New();
+  if (dict) {
+    PyDict_SetItem(dict, SWIG_This(), swig_this);
+    inst = PyInstance_NewRaw(data->newargs, dict);
+    Py_DECREF(dict);
+  }
+  return (PyObject *) inst;
+#else
+  PyInstanceObject *inst = PyObject_NEW(PyInstanceObject, &PyInstance_Type);
+  if (inst == NULL) {
+    return NULL;
+  }
+  inst->in_class = (PyClassObject *)data->newargs;
+  Py_INCREF(inst->in_class);
+  inst->in_dict = PyDict_New();
+  if (inst->in_dict == NULL) {
+    Py_DECREF(inst);
+    return NULL;
+  }
+#ifdef Py_TPFLAGS_HAVE_WEAKREFS
+  inst->in_weakreflist = NULL;
+#endif
+#ifdef Py_TPFLAGS_GC
+  PyObject_GC_Init(inst);
+#endif
+  PyDict_SetItem(inst->in_dict, SWIG_This(), swig_this);
+  return (PyObject *) inst;
+#endif
+#endif
 }
 
 SWIGRUNTIME void
 SWIG_Python_SetSwigThis(PyObject *inst, PyObject *swig_this)
 {
  PyObject *dict;
-#if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
+#if (PY_VERSION_HEX >= 0x02020000) && !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
  PyObject **dictptr = _PyObject_GetDictPtr(inst);
  if (dictptr != NULL) {
    dict = *dictptr;
    if (dict == NULL) {
      dict = PyDict_New();
      *dictptr = dict;
    }
    PyDict_SetItem(dict, SWIG_This(), swig_this);
    return;
  }
 #endif
- dict = PyObject_GetAttrString(inst, "__dict__");
+ dict = PyObject_GetAttrString(inst, (char*)"__dict__");
  PyDict_SetItem(dict, SWIG_This(), swig_this);
  Py_DECREF(dict);
 } 
 
 
 SWIGINTERN PyObject *
 SWIG_Python_InitShadowInstance(PyObject *args) {
@@ -2361,56 +2662,108 @@
 SWIG_Python_GetModule(void *SWIGUNUSEDPARM(clientdata)) {
   static void *type_pointer = (void *)0;
   /* first check if module already created */
   if (!type_pointer) {
 #ifdef SWIG_LINK_RUNTIME
     type_pointer = SWIG_ReturnGlobalTypeList((void *)0);
 #else
+# ifdef SWIGPY_USE_CAPSULE
     type_pointer = PyCapsule_Import(SWIGPY_CAPSULE_NAME, 0);
+# else
+    type_pointer = PyCObject_Import((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION,
+				    (char*)"type_pointer" SWIG_TYPE_TABLE_NAME);
+# endif
     if (PyErr_Occurred()) {
       PyErr_Clear();
       type_pointer = (void *)0;
     }
 #endif
   }
   return (swig_module_info *) type_pointer;
 }
 
+#if PY_MAJOR_VERSION < 2
+/* PyModule_AddObject function was introduced in Python 2.0.  The following function
+   is copied out of Python/modsupport.c in python version 2.3.4 */
+SWIGINTERN int
+PyModule_AddObject(PyObject *m, char *name, PyObject *o)
+{
+  PyObject *dict;
+  if (!PyModule_Check(m)) {
+    PyErr_SetString(PyExc_TypeError, "PyModule_AddObject() needs module as first arg");
+    return SWIG_ERROR;
+  }
+  if (!o) {
+    PyErr_SetString(PyExc_TypeError, "PyModule_AddObject() needs non-NULL value");
+    return SWIG_ERROR;
+  }
+  
+  dict = PyModule_GetDict(m);
+  if (dict == NULL) {
+    /* Internal error -- modules must have a dict! */
+    PyErr_Format(PyExc_SystemError, "module '%s' has no __dict__",
+		 PyModule_GetName(m));
+    return SWIG_ERROR;
+  }
+  if (PyDict_SetItemString(dict, name, o))
+    return SWIG_ERROR;
+  Py_DECREF(o);
+  return SWIG_OK;
+}
+#endif
+
 SWIGRUNTIME void
+#ifdef SWIGPY_USE_CAPSULE
 SWIG_Python_DestroyModule(PyObject *obj)
+#else
+SWIG_Python_DestroyModule(void *vptr)
+#endif
 {
+#ifdef SWIGPY_USE_CAPSULE
   swig_module_info *swig_module = (swig_module_info *) PyCapsule_GetPointer(obj, SWIGPY_CAPSULE_NAME);
+#else
+  swig_module_info *swig_module = (swig_module_info *) vptr;
+#endif
   swig_type_info **types = swig_module->types;
   size_t i;
   for (i =0; i < swig_module->size; ++i) {
     swig_type_info *ty = types[i];
     if (ty->owndata) {
       SwigPyClientData *data = (SwigPyClientData *) ty->clientdata;
       if (data) SwigPyClientData_Del(data);
     }
   }
   Py_DECREF(SWIG_This());
-  Swig_This_global = NULL;
+  swig_this = NULL;
 }
 
 SWIGRUNTIME void
 SWIG_Python_SetModule(swig_module_info *swig_module) {
 #if PY_VERSION_HEX >= 0x03000000
  /* Add a dummy module object into sys.modules */
-  PyObject *module = PyImport_AddModule("swig_runtime_data" SWIG_RUNTIME_VERSION);
+  PyObject *module = PyImport_AddModule((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION);
 #else
   static PyMethodDef swig_empty_runtime_method_table[] = { {NULL, NULL, 0, NULL} }; /* Sentinel */
-  PyObject *module = Py_InitModule("swig_runtime_data" SWIG_RUNTIME_VERSION, swig_empty_runtime_method_table);
+  PyObject *module = Py_InitModule((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION, swig_empty_runtime_method_table);
 #endif
+#ifdef SWIGPY_USE_CAPSULE
   PyObject *pointer = PyCapsule_New((void *) swig_module, SWIGPY_CAPSULE_NAME, SWIG_Python_DestroyModule);
   if (pointer && module) {
-    PyModule_AddObject(module, "type_pointer_capsule" SWIG_TYPE_TABLE_NAME, pointer);
+    PyModule_AddObject(module, (char*)"type_pointer_capsule" SWIG_TYPE_TABLE_NAME, pointer);
   } else {
     Py_XDECREF(pointer);
   }
+#else
+  PyObject *pointer = PyCObject_FromVoidPtr((void *) swig_module, SWIG_Python_DestroyModule);
+  if (pointer && module) {
+    PyModule_AddObject(module, (char*)"type_pointer" SWIG_TYPE_TABLE_NAME, pointer);
+  } else {
+    Py_XDECREF(pointer);
+  }
+#endif
 }
 
 /* The python cached type query */
 SWIGRUNTIME PyObject *
 SWIG_Python_TypeCache(void) {
   static PyObject *SWIG_STATIC_POINTER(cache) = PyDict_New();
   return cache;
@@ -2420,20 +2773,28 @@
 SWIG_Python_TypeQuery(const char *type)
 {
   PyObject *cache = SWIG_Python_TypeCache();
   PyObject *key = SWIG_Python_str_FromChar(type); 
   PyObject *obj = PyDict_GetItem(cache, key);
   swig_type_info *descriptor;
   if (obj) {
+#ifdef SWIGPY_USE_CAPSULE
     descriptor = (swig_type_info *) PyCapsule_GetPointer(obj, NULL);
+#else
+    descriptor = (swig_type_info *) PyCObject_AsVoidPtr(obj);
+#endif
   } else {
     swig_module_info *swig_module = SWIG_GetModule(0);
     descriptor = SWIG_TypeQueryModule(swig_module, swig_module, type);
     if (descriptor) {
+#ifdef SWIGPY_USE_CAPSULE
       obj = PyCapsule_New((void*) descriptor, NULL, NULL);
+#else
+      obj = PyCObject_FromVoidPtr(descriptor, NULL);
+#endif
       PyDict_SetItem(cache, key, obj);
       Py_DECREF(obj);
     }
   }
   Py_DECREF(key);
   return descriptor;
 }
@@ -2450,23 +2811,22 @@
 {  
   if (PyErr_Occurred()) {
     PyObject *type = 0;
     PyObject *value = 0;
     PyObject *traceback = 0;
     PyErr_Fetch(&type, &value, &traceback);
     if (value) {
+      char *tmp;
       PyObject *old_str = PyObject_Str(value);
-      const char *tmp = SWIG_Python_str_AsChar(old_str);
-      const char *errmesg = tmp ? tmp : "Invalid error message";
       Py_XINCREF(type);
       PyErr_Clear();
       if (infront) {
-	PyErr_Format(type, "%s %s", mesg, errmesg);
+	PyErr_Format(type, "%s %s", mesg, tmp = SWIG_Python_str_AsChar(old_str));
       } else {
-	PyErr_Format(type, "%s %s", errmesg, mesg);
+	PyErr_Format(type, "%s %s", tmp = SWIG_Python_str_AsChar(old_str), mesg);
       }
       SWIG_Python_str_DelForPy3(tmp);
       Py_DECREF(old_str);
     }
     return 1;
   } else {
     return 0;
@@ -2584,16 +2944,14 @@
     f = descr->ob_type->tp_descr_set;
   if (!f) {
     if (PyString_Check(name)) {
       encoded_name = name;
       Py_INCREF(name);
     } else {
       encoded_name = PyUnicode_AsUTF8String(name);
-      if (!encoded_name)
-        return -1;
     }
     PyErr_Format(PyExc_AttributeError, "'%.100s' object has no attribute '%.200s'", tp->tp_name, PyString_AsString(encoded_name));
     Py_DECREF(encoded_name);
   } else {
     res = f(descr, obj, value);
   }
   
@@ -2612,29 +2970,14 @@
 
 #define SWIG_exception_fail(code, msg) do { SWIG_Error(code, msg); SWIG_fail; } while(0) 
 
 #define SWIG_contract_assert(expr, msg) if (!(expr)) { SWIG_Error(SWIG_RuntimeError, msg); SWIG_fail; } else 
 
 
 
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-/* Method creation and docstring support functions */
-
-SWIGINTERN PyMethodDef *SWIG_PythonGetProxyDoc(const char *name);
-SWIGINTERN PyObject *SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func);
-SWIGINTERN PyObject *SWIG_PyStaticMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func);
-
-#ifdef __cplusplus
-}
-#endif
-
-
 /* -------- TYPES TABLE (BEGIN) -------- */
 
 #define SWIGTYPE_p_IHMErrorCode swig_types[0]
 #define SWIGTYPE_p_char swig_types[1]
 #define SWIGTYPE_p_f_p_char_size_t_p_void_p_p_struct_ihm_error__ssize_t swig_types[2]
 #define SWIGTYPE_p_f_p_struct_ihm_reader_p_q_const__char_int_p_void_p_p_struct_ihm_error__void swig_types[3]
 #define SWIGTYPE_p_f_p_struct_ihm_reader_p_q_const__char_p_q_const__char_int_p_void_p_p_struct_ihm_error__void swig_types[4]
@@ -2652,32 +2995,33 @@
 static swig_type_info *swig_types[17];
 static swig_module_info swig_module = {swig_types, 16, 0, 0, 0, 0};
 #define SWIG_TypeQuery(name) SWIG_TypeQueryModule(&swig_module, &swig_module, name)
 #define SWIG_MangledTypeQuery(name) SWIG_MangledTypeQueryModule(&swig_module, &swig_module, name)
 
 /* -------- TYPES TABLE (END) -------- */
 
-#ifdef SWIG_TypeQuery
-# undef SWIG_TypeQuery
+#if (PY_VERSION_HEX <= 0x02000000)
+# if !defined(SWIG_PYTHON_CLASSIC)
+#  error "This python version requires swig to be run with the '-classic' option"
+# endif
 #endif
-#define SWIG_TypeQuery SWIG_Python_TypeQuery
 
 /*-----------------------------------------------
               @(target):= _format.so
   ------------------------------------------------*/
 #if PY_VERSION_HEX >= 0x03000000
 #  define SWIG_init    PyInit__format
 
 #else
 #  define SWIG_init    init_format
 
 #endif
 #define SWIG_name    "_format"
 
-#define SWIGVERSION 0x040000 
+#define SWIGVERSION 0x030012 
 #define SWIG_VERSION SWIGVERSION
 
 
 #define SWIG_as_voidptr(a) (void *)((const void *)(a)) 
 #define SWIG_as_voidptrptr(a) ((void)SWIG_as_voidptr(*a),(void**)(a)) 
 
 
@@ -3082,37 +3426,47 @@
   if (PyUnicode_Check(obj))
 #endif
 #else  
   if (PyString_Check(obj))
 #endif
   {
     char *cstr; Py_ssize_t len;
-    int ret = SWIG_OK;
 #if PY_VERSION_HEX>=0x03000000
 #if !defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
     if (!alloc && cptr) {
         /* We can't allow converting without allocation, since the internal
            representation of string in Python 3 is UCS-2/UCS-4 but we require
            a UTF-8 representation.
            TODO(bhy) More detailed explanation */
         return SWIG_RuntimeError;
     }
     obj = PyUnicode_AsUTF8String(obj);
-    if (!obj)
-      return SWIG_TypeError;
-    if (alloc)
-      *alloc = SWIG_NEWOBJ;
+    if(alloc) *alloc = SWIG_NEWOBJ;
 #endif
     PyBytes_AsStringAndSize(obj, &cstr, &len);
 #else
     PyString_AsStringAndSize(obj, &cstr, &len);
 #endif
     if (cptr) {
       if (alloc) {
-	if (*alloc == SWIG_NEWOBJ) {
+	/* 
+	   In python the user should not be able to modify the inner
+	   string representation. To warranty that, if you define
+	   SWIG_PYTHON_SAFE_CSTRINGS, a new/copy of the python string
+	   buffer is always returned.
+
+	   The default behavior is just to return the pointer value,
+	   so, be careful.
+	*/ 
+#if defined(SWIG_PYTHON_SAFE_CSTRINGS)
+	if (*alloc != SWIG_OLDOBJ) 
+#else
+	if (*alloc == SWIG_NEWOBJ) 
+#endif
+	{
 	  *cptr = (char *)memcpy(malloc((len + 1)*sizeof(char)), cstr, sizeof(char)*(len + 1));
 	  *alloc = SWIG_NEWOBJ;
 	} else {
 	  *cptr = cstr;
 	  *alloc = SWIG_OLDOBJ;
 	}
       } else {
@@ -3120,38 +3474,34 @@
 #if defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
 	*cptr = PyBytes_AsString(obj);
 #else
 	assert(0); /* Should never reach here with Unicode strings in Python 3 */
 #endif
 #else
 	*cptr = SWIG_Python_str_AsChar(obj);
-        if (!*cptr)
-          ret = SWIG_TypeError;
 #endif
       }
     }
     if (psize) *psize = len + 1;
 #if PY_VERSION_HEX>=0x03000000 && !defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
     Py_XDECREF(obj);
 #endif
-    return ret;
+    return SWIG_OK;
   } else {
 #if defined(SWIG_PYTHON_2_UNICODE)
 #if defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
 #error "Cannot use both SWIG_PYTHON_2_UNICODE and SWIG_PYTHON_STRICT_BYTE_CHAR at once"
 #endif
 #if PY_VERSION_HEX<0x03000000
     if (PyUnicode_Check(obj)) {
       char *cstr; Py_ssize_t len;
       if (!alloc && cptr) {
         return SWIG_RuntimeError;
       }
       obj = PyUnicode_AsUTF8String(obj);
-      if (!obj)
-        return SWIG_TypeError;
       if (PyString_AsStringAndSize(obj, &cstr, &len) != -1) {
         if (cptr) {
           if (alloc) *alloc = SWIG_NEWOBJ;
           *cptr = (char *)memcpy(malloc((len + 1)*sizeof(char)), cstr, sizeof(char)*(len + 1));
         }
         if (psize) *psize = len + 1;
 
@@ -3408,15 +3758,19 @@
       return pchar_descriptor ? 
 	SWIG_InternalNewPointerObj((char *)(carray), pchar_descriptor, 0) : SWIG_Py_Void();
     } else {
 #if PY_VERSION_HEX >= 0x03000000
 #if defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
       return PyBytes_FromStringAndSize(carray, (Py_ssize_t)(size));
 #else
+#if PY_VERSION_HEX >= 0x03010000
       return PyUnicode_DecodeUTF8(carray, (Py_ssize_t)(size), "surrogateescape");
+#else
+      return PyUnicode_FromStringAndSize(carray, (Py_ssize_t)(size));
+#endif
 #endif
 #else
       return PyString_FromStringAndSize(carray, (Py_ssize_t)(size));
 #endif
     }
   } else {
     return SWIG_Py_Void();
@@ -3587,24 +3941,24 @@
 #endif
 SWIGINTERN PyObject *_wrap_ihm_file_new_from_python(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0;
   PyObject *arg1 = (PyObject *) 0 ;
   struct ihm_error **arg2 = (struct ihm_error **) 0 ;
   struct ihm_error *temp2 ;
   PyObject * obj0 = 0 ;
-  char * kwnames[] = {
-    (char *)"pyfile",  NULL 
+  char *  kwnames[] = {
+    (char *) "pyfile", NULL 
   };
   struct ihm_file *result = 0 ;
   
   {
     temp2 = NULL;
     arg2 = &temp2;
   }
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:ihm_file_new_from_python", kwnames, &obj0)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"O:ihm_file_new_from_python",kwnames,&obj0)) SWIG_fail;
   arg1 = obj0;
   result = (struct ihm_file *)ihm_file_new_from_python(arg1,arg2);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ihm_file, 0 |  0 );
   {
     if (*arg2) {
       handle_error(*arg2);
       Py_DECREF(resultobj);
@@ -3623,23 +3977,23 @@
   PyObject *arg2 = (PyObject *) 0 ;
   struct ihm_error **arg3 = (struct ihm_error **) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   struct ihm_error *temp3 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"callable",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "callable", NULL 
   };
   
   {
     temp3 = NULL;
     arg3 = &temp3;
   }
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OO:add_unknown_category_handler", kwnames, &obj0, &obj1)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OO:add_unknown_category_handler",kwnames,&obj0,&obj1)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "add_unknown_category_handler" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   arg2 = obj1;
   add_unknown_category_handler(arg1,arg2,arg3);
@@ -3663,23 +4017,23 @@
   PyObject *arg2 = (PyObject *) 0 ;
   struct ihm_error **arg3 = (struct ihm_error **) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   struct ihm_error *temp3 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"callable",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "callable", NULL 
   };
   
   {
     temp3 = NULL;
     arg3 = &temp3;
   }
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OO:add_unknown_keyword_handler", kwnames, &obj0, &obj1)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OO:add_unknown_keyword_handler",kwnames,&obj0,&obj1)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "add_unknown_keyword_handler" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   arg2 = obj1;
   add_unknown_keyword_handler(arg1,arg2,arg3);
@@ -3710,23 +4064,23 @@
   char *buf2 = 0 ;
   int alloc2 = 0 ;
   struct ihm_error *temp5 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"name",  (char *)"keywords",  (char *)"callable",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "name",(char *) "keywords",(char *) "callable", NULL 
   };
   
   {
     temp5 = NULL;
     arg5 = &temp5;
   }
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OOOO:add_category_handler", kwnames, &obj0, &obj1, &obj2, &obj3)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OOOO:add_category_handler",kwnames,&obj0,&obj1,&obj2,&obj3)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "add_category_handler" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   res2 = SWIG_AsCharPtrAndSize(obj1, &buf2, NULL, &alloc2);
   if (!SWIG_IsOK(res2)) {
@@ -3765,23 +4119,23 @@
   char *buf2 = 0 ;
   int alloc2 = 0 ;
   struct ihm_error *temp5 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"name",  (char *)"keywords",  (char *)"callable",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "name",(char *) "keywords",(char *) "callable", NULL 
   };
   
   {
     temp5 = NULL;
     arg5 = &temp5;
   }
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OOOO:add_poly_seq_scheme_handler", kwnames, &obj0, &obj1, &obj2, &obj3)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OOOO:add_poly_seq_scheme_handler",kwnames,&obj0,&obj1,&obj2,&obj3)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "add_poly_seq_scheme_handler" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   res2 = SWIG_AsCharPtrAndSize(obj1, &buf2, NULL, &alloc2);
   if (!SWIG_IsOK(res2)) {
@@ -3820,23 +4174,23 @@
   char *buf2 = 0 ;
   int alloc2 = 0 ;
   struct ihm_error *temp5 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"name",  (char *)"keywords",  (char *)"callable",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "name",(char *) "keywords",(char *) "callable", NULL 
   };
   
   {
     temp5 = NULL;
     arg5 = &temp5;
   }
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OOOO:_test_finalize_callback", kwnames, &obj0, &obj1, &obj2, &obj3)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OOOO:_test_finalize_callback",kwnames,&obj0,&obj1,&obj2,&obj3)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "_test_finalize_callback" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   res2 = SWIG_AsCharPtrAndSize(obj1, &buf2, NULL, &alloc2);
   if (!SWIG_IsOK(res2)) {
@@ -3866,23 +4220,24 @@
   PyObject *resultobj = 0;
   struct ihm_error *arg1 = (struct ihm_error *) 0 ;
   IHMErrorCode arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_error_code_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_error_code_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_error_code_set" "', argument " "1"" of type '" "struct ihm_error *""'"); 
   }
   arg1 = (struct ihm_error *)(argp1);
-  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
+  ecode2 = SWIG_AsVal_int(obj1, &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ihm_error_code_set" "', argument " "2"" of type '" "IHMErrorCode""'");
   } 
   arg2 = (IHMErrorCode)(val2);
   if (arg1) (arg1)->code = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
@@ -3892,20 +4247,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_error_code_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_error *arg1 = (struct ihm_error *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   IHMErrorCode result;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_error_code_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_error_code_get" "', argument " "1"" of type '" "struct ihm_error *""'"); 
   }
   arg1 = (struct ihm_error *)(argp1);
   result = (IHMErrorCode) ((arg1)->code);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
@@ -3919,23 +4273,24 @@
   struct ihm_error *arg1 = (struct ihm_error *) 0 ;
   char *arg2 = (char *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res2 ;
   char *buf2 = 0 ;
   int alloc2 = 0 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_error_msg_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_error_msg_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_error_msg_set" "', argument " "1"" of type '" "struct ihm_error *""'"); 
   }
   arg1 = (struct ihm_error *)(argp1);
-  res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
+  res2 = SWIG_AsCharPtrAndSize(obj1, &buf2, NULL, &alloc2);
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "ihm_error_msg_set" "', argument " "2"" of type '" "char *""'");
   }
   arg2 = (char *)(buf2);
   if (arg1->msg) free((char*)arg1->msg);
   if (arg2) {
     size_t size = strlen((const char *)(arg2)) + 1;
@@ -3953,20 +4308,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_error_msg_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_error *arg1 = (struct ihm_error *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   char *result = 0 ;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_error_msg_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_error_msg_get" "', argument " "1"" of type '" "struct ihm_error *""'"); 
   }
   arg1 = (struct ihm_error *)(argp1);
   result = (char *) ((arg1)->msg);
   resultobj = SWIG_FromCharPtr((const char *)result);
   return resultobj;
@@ -3977,19 +4331,19 @@
 
 SWIGINTERN PyObject *_wrap_ihm_error_free(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0;
   struct ihm_error *arg1 = (struct ihm_error *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject * obj0 = 0 ;
-  char * kwnames[] = {
-    (char *)"err",  NULL 
+  char *  kwnames[] = {
+    (char *) "err", NULL 
   };
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:ihm_error_free", kwnames, &obj0)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"O:ihm_error_free",kwnames,&obj0)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_error, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_error_free" "', argument " "1"" of type '" "struct ihm_error *""'"); 
   }
   arg1 = (struct ihm_error *)(argp1);
   ihm_error_free(arg1);
   resultobj = SWIG_Py_Void();
@@ -4017,20 +4371,20 @@
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
   PyObject * obj4 = 0 ;
   PyObject * obj5 = 0 ;
   PyObject * obj6 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"name",  (char *)"data_callback",  (char *)"end_frame_callback",  (char *)"finalize_callback",  (char *)"data",  (char *)"free_func",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "name",(char *) "data_callback",(char *) "end_frame_callback",(char *) "finalize_callback",(char *) "data",(char *) "free_func", NULL 
   };
   struct ihm_category *result = 0 ;
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OOOOOOO:ihm_category_new", kwnames, &obj0, &obj1, &obj2, &obj3, &obj4, &obj5, &obj6)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OOOOOOO:ihm_category_new",kwnames,&obj0,&obj1,&obj2,&obj3,&obj4,&obj5,&obj6)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_category_new" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   res2 = SWIG_AsCharPtrAndSize(obj1, &buf2, NULL, &alloc2);
   if (!SWIG_IsOK(res2)) {
@@ -4084,19 +4438,19 @@
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res3 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"callback",  (char *)"data",  (char *)"free_func",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "callback",(char *) "data",(char *) "free_func", NULL 
   };
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OOOO:ihm_reader_unknown_category_callback_set", kwnames, &obj0, &obj1, &obj2, &obj3)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OOOO:ihm_reader_unknown_category_callback_set",kwnames,&obj0,&obj1,&obj2,&obj3)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_reader_unknown_category_callback_set" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   {
     int res = SWIG_ConvertFunctionPtr(obj1, (void**)(&arg2), SWIGTYPE_p_f_p_struct_ihm_reader_p_q_const__char_int_p_void_p_p_struct_ihm_error__void);
@@ -4131,19 +4485,19 @@
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res3 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
   PyObject * obj3 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  (char *)"callback",  (char *)"data",  (char *)"free_func",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader",(char *) "callback",(char *) "data",(char *) "free_func", NULL 
   };
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OOOO:ihm_reader_unknown_keyword_callback_set", kwnames, &obj0, &obj1, &obj2, &obj3)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OOOO:ihm_reader_unknown_keyword_callback_set",kwnames,&obj0,&obj1,&obj2,&obj3)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_reader_unknown_keyword_callback_set" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   {
     int res = SWIG_ConvertFunctionPtr(obj1, (void**)(&arg2), SWIGTYPE_p_f_p_struct_ihm_reader_p_q_const__char_p_q_const__char_int_p_void_p_p_struct_ihm_error__void);
@@ -4171,19 +4525,19 @@
 
 SWIGINTERN PyObject *_wrap_ihm_reader_remove_all_categories(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0;
   struct ihm_reader *arg1 = (struct ihm_reader *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject * obj0 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader", NULL 
   };
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:ihm_reader_remove_all_categories", kwnames, &obj0)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"O:ihm_reader_remove_all_categories",kwnames,&obj0)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_reader_remove_all_categories" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   ihm_reader_remove_all_categories(arg1);
   resultobj = SWIG_Py_Void();
@@ -4200,20 +4554,20 @@
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res2 ;
   char *buf2 = 0 ;
   int alloc2 = 0 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
-  char * kwnames[] = {
-    (char *)"category",  (char *)"name",  NULL 
+  char *  kwnames[] = {
+    (char *) "category",(char *) "name", NULL 
   };
   struct ihm_keyword *result = 0 ;
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OO:ihm_keyword_new", kwnames, &obj0, &obj1)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OO:ihm_keyword_new",kwnames,&obj0,&obj1)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_category, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_keyword_new" "', argument " "1"" of type '" "struct ihm_category *""'"); 
   }
   arg1 = (struct ihm_category *)(argp1);
   res2 = SWIG_AsCharPtrAndSize(obj1, &buf2, NULL, &alloc2);
   if (!SWIG_IsOK(res2)) {
@@ -4234,23 +4588,24 @@
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   struct ihm_string *arg2 = (struct ihm_string *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   void *argp2 = 0 ;
   int res2 = 0 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_file_buffer_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_file_buffer_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_buffer_set" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
-  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_ihm_string, SWIG_POINTER_DISOWN |  0 );
+  res2 = SWIG_ConvertPtr(obj1, &argp2,SWIGTYPE_p_ihm_string, SWIG_POINTER_DISOWN |  0 );
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "ihm_file_buffer_set" "', argument " "2"" of type '" "struct ihm_string *""'"); 
   }
   arg2 = (struct ihm_string *)(argp2);
   if (arg1) (arg1)->buffer = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
@@ -4260,20 +4615,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_file_buffer_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   struct ihm_string *result = 0 ;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_file_buffer_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_buffer_get" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   result = (struct ihm_string *) ((arg1)->buffer);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ihm_string, 0 |  0 );
   return resultobj;
@@ -4286,23 +4640,24 @@
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   size_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   size_t val2 ;
   int ecode2 = 0 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_file_line_start_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_file_line_start_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_line_start_set" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
-  ecode2 = SWIG_AsVal_size_t(swig_obj[1], &val2);
+  ecode2 = SWIG_AsVal_size_t(obj1, &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ihm_file_line_start_set" "', argument " "2"" of type '" "size_t""'");
   } 
   arg2 = (size_t)(val2);
   if (arg1) (arg1)->line_start = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
@@ -4312,20 +4667,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_file_line_start_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   size_t result;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_file_line_start_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_line_start_get" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   result =  ((arg1)->line_start);
   resultobj = SWIG_From_size_t((size_t)(result));
   return resultobj;
@@ -4338,23 +4692,24 @@
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   size_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   size_t val2 ;
   int ecode2 = 0 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_file_next_line_start_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_file_next_line_start_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_next_line_start_set" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
-  ecode2 = SWIG_AsVal_size_t(swig_obj[1], &val2);
+  ecode2 = SWIG_AsVal_size_t(obj1, &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ihm_file_next_line_start_set" "', argument " "2"" of type '" "size_t""'");
   } 
   arg2 = (size_t)(val2);
   if (arg1) (arg1)->next_line_start = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
@@ -4364,20 +4719,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_file_next_line_start_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   size_t result;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_file_next_line_start_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_next_line_start_get" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   result =  ((arg1)->next_line_start);
   resultobj = SWIG_From_size_t((size_t)(result));
   return resultobj;
@@ -4388,24 +4742,25 @@
 
 SWIGINTERN PyObject *_wrap_ihm_file_read_callback_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   ihm_file_read_callback arg2 = (ihm_file_read_callback) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_file_read_callback_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_file_read_callback_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_read_callback_set" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   {
-    int res = SWIG_ConvertFunctionPtr(swig_obj[1], (void**)(&arg2), SWIGTYPE_p_f_p_char_size_t_p_void_p_p_struct_ihm_error__ssize_t);
+    int res = SWIG_ConvertFunctionPtr(obj1, (void**)(&arg2), SWIGTYPE_p_f_p_char_size_t_p_void_p_p_struct_ihm_error__ssize_t);
     if (!SWIG_IsOK(res)) {
       SWIG_exception_fail(SWIG_ArgError(res), "in method '" "ihm_file_read_callback_set" "', argument " "2"" of type '" "ihm_file_read_callback""'"); 
     }
   }
   if (arg1) (arg1)->read_callback = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
@@ -4415,20 +4770,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_file_read_callback_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   ihm_file_read_callback result;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_file_read_callback_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_read_callback_get" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   result = (ihm_file_read_callback) ((arg1)->read_callback);
   resultobj = SWIG_NewFunctionPtrObj((void *)(result), SWIGTYPE_p_f_p_char_size_t_p_void_p_p_struct_ihm_error__ssize_t);
   return resultobj;
@@ -4440,23 +4794,24 @@
 SWIGINTERN PyObject *_wrap_ihm_file_data_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *arg2 = (void *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res2 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_file_data_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_file_data_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_data_set" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
-  res2 = SWIG_ConvertPtr(swig_obj[1],SWIG_as_voidptrptr(&arg2), 0, SWIG_POINTER_DISOWN);
+  res2 = SWIG_ConvertPtr(obj1,SWIG_as_voidptrptr(&arg2), 0, SWIG_POINTER_DISOWN);
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "ihm_file_data_set" "', argument " "2"" of type '" "void *""'"); 
   }
   if (arg1) (arg1)->data = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
@@ -4465,20 +4820,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_file_data_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   void *result = 0 ;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_file_data_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_data_get" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   result = (void *) ((arg1)->data);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_void, 0 |  0 );
   return resultobj;
@@ -4489,24 +4843,25 @@
 
 SWIGINTERN PyObject *_wrap_ihm_file_free_func_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   ihm_free_callback arg2 = (ihm_free_callback) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[2] ;
+  PyObject * obj0 = 0 ;
+  PyObject * obj1 = 0 ;
   
-  if (!SWIG_Python_UnpackTuple(args, "ihm_file_free_func_set", 2, 2, swig_obj)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"OO:ihm_file_free_func_set",&obj0,&obj1)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_free_func_set" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   {
-    int res = SWIG_ConvertFunctionPtr(swig_obj[1], (void**)(&arg2), SWIGTYPE_p_f_p_void__void);
+    int res = SWIG_ConvertFunctionPtr(obj1, (void**)(&arg2), SWIGTYPE_p_f_p_void__void);
     if (!SWIG_IsOK(res)) {
       SWIG_exception_fail(SWIG_ArgError(res), "in method '" "ihm_file_free_func_set" "', argument " "2"" of type '" "ihm_free_callback""'"); 
     }
   }
   if (arg1) (arg1)->free_func = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
@@ -4516,20 +4871,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ihm_file_free_func_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject *swig_obj[1] ;
+  PyObject * obj0 = 0 ;
   ihm_free_callback result;
   
-  if (!args) SWIG_fail;
-  swig_obj[0] = args;
-  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
+  if (!PyArg_ParseTuple(args,(char *)"O:ihm_file_free_func_get",&obj0)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_file_free_func_get" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   result = (ihm_free_callback) ((arg1)->free_func);
   resultobj = SWIG_NewFunctionPtrObj((void *)(result), SWIGTYPE_p_f_p_void__void);
   return resultobj;
@@ -4543,20 +4897,20 @@
   ihm_file_read_callback arg1 = (ihm_file_read_callback) 0 ;
   void *arg2 = (void *) 0 ;
   ihm_free_callback arg3 = (ihm_free_callback) 0 ;
   int res2 ;
   PyObject * obj0 = 0 ;
   PyObject * obj1 = 0 ;
   PyObject * obj2 = 0 ;
-  char * kwnames[] = {
-    (char *)"read_callback",  (char *)"data",  (char *)"free_func",  NULL 
+  char *  kwnames[] = {
+    (char *) "read_callback",(char *) "data",(char *) "free_func", NULL 
   };
   struct ihm_file *result = 0 ;
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "OOO:ihm_file_new", kwnames, &obj0, &obj1, &obj2)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"OOO:ihm_file_new",kwnames,&obj0,&obj1,&obj2)) SWIG_fail;
   {
     int res = SWIG_ConvertFunctionPtr(obj0, (void**)(&arg1), SWIGTYPE_p_f_p_char_size_t_p_void_p_p_struct_ihm_error__ssize_t);
     if (!SWIG_IsOK(res)) {
       SWIG_exception_fail(SWIG_ArgError(res), "in method '" "ihm_file_new" "', argument " "1"" of type '" "ihm_file_read_callback""'"); 
     }
   }
   res2 = SWIG_ConvertPtr(obj1,SWIG_as_voidptrptr(&arg2), 0, 0);
@@ -4579,20 +4933,20 @@
 
 SWIGINTERN PyObject *_wrap_ihm_file_new_from_fd(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0;
   int arg1 ;
   int val1 ;
   int ecode1 = 0 ;
   PyObject * obj0 = 0 ;
-  char * kwnames[] = {
-    (char *)"fd",  NULL 
+  char *  kwnames[] = {
+    (char *) "fd", NULL 
   };
   struct ihm_file *result = 0 ;
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:ihm_file_new_from_fd", kwnames, &obj0)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"O:ihm_file_new_from_fd",kwnames,&obj0)) SWIG_fail;
   ecode1 = SWIG_AsVal_int(obj0, &val1);
   if (!SWIG_IsOK(ecode1)) {
     SWIG_exception_fail(SWIG_ArgError(ecode1), "in method '" "ihm_file_new_from_fd" "', argument " "1"" of type '" "int""'");
   } 
   arg1 = (int)(val1);
   result = (struct ihm_file *)ihm_file_new_from_fd(arg1);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ihm_file, 0 |  0 );
@@ -4604,20 +4958,20 @@
 
 SWIGINTERN PyObject *_wrap_ihm_reader_new(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0;
   struct ihm_file *arg1 = (struct ihm_file *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject * obj0 = 0 ;
-  char * kwnames[] = {
-    (char *)"fh",  NULL 
+  char *  kwnames[] = {
+    (char *) "fh", NULL 
   };
   struct ihm_reader *result = 0 ;
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:ihm_reader_new", kwnames, &obj0)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"O:ihm_reader_new",kwnames,&obj0)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_file, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_reader_new" "', argument " "1"" of type '" "struct ihm_file *""'"); 
   }
   arg1 = (struct ihm_file *)(argp1);
   result = (struct ihm_reader *)ihm_reader_new(arg1);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ihm_reader, 0 |  0 );
@@ -4629,19 +4983,19 @@
 
 SWIGINTERN PyObject *_wrap_ihm_reader_free(PyObject *SWIGUNUSEDPARM(self), PyObject *args, PyObject *kwargs) {
   PyObject *resultobj = 0;
   struct ihm_reader *arg1 = (struct ihm_reader *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject * obj0 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader", NULL 
   };
   
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:ihm_reader_free", kwnames, &obj0)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"O:ihm_reader_free",kwnames,&obj0)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_reader_free" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   ihm_reader_free(arg1);
   resultobj = SWIG_Py_Void();
@@ -4658,25 +5012,25 @@
   struct ihm_error **arg3 = (struct ihm_error **) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int temp2 ;
   int res2 = SWIG_TMPOBJ ;
   struct ihm_error *temp3 ;
   PyObject * obj0 = 0 ;
-  char * kwnames[] = {
-    (char *)"reader",  NULL 
+  char *  kwnames[] = {
+    (char *) "reader", NULL 
   };
   int result;
   
   arg2 = &temp2;
   {
     temp3 = NULL;
     arg3 = &temp3;
   }
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:ihm_read_file", kwnames, &obj0)) SWIG_fail;
+  if (!PyArg_ParseTupleAndKeywords(args,kwargs,(char *)"O:ihm_read_file",kwnames,&obj0)) SWIG_fail;
   res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ihm_reader, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ihm_read_file" "', argument " "1"" of type '" "struct ihm_reader *""'"); 
   }
   arg1 = (struct ihm_reader *)(argp1);
   result = (int)ihm_read_file(arg1,arg2,arg3);
   resultobj = SWIG_From_int((int)(result));
@@ -4696,52 +5050,48 @@
   return resultobj;
 fail:
   return NULL;
 }
 
 
 static PyMethodDef SwigMethods[] = {
-	 { "SWIG_PyInstanceMethod_New", SWIG_PyInstanceMethod_New, METH_O, NULL},
-	 { "ihm_file_new_from_python", (PyCFunction)(void(*)(void))_wrap_ihm_file_new_from_python, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "add_unknown_category_handler", (PyCFunction)(void(*)(void))_wrap_add_unknown_category_handler, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "add_unknown_keyword_handler", (PyCFunction)(void(*)(void))_wrap_add_unknown_keyword_handler, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "add_category_handler", (PyCFunction)(void(*)(void))_wrap_add_category_handler, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "add_poly_seq_scheme_handler", (PyCFunction)(void(*)(void))_wrap_add_poly_seq_scheme_handler, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "_test_finalize_callback", (PyCFunction)(void(*)(void))_wrap__test_finalize_callback, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_error_code_set", _wrap_ihm_error_code_set, METH_VARARGS, NULL},
-	 { "ihm_error_code_get", _wrap_ihm_error_code_get, METH_O, NULL},
-	 { "ihm_error_msg_set", _wrap_ihm_error_msg_set, METH_VARARGS, NULL},
-	 { "ihm_error_msg_get", _wrap_ihm_error_msg_get, METH_O, NULL},
-	 { "ihm_error_free", (PyCFunction)(void(*)(void))_wrap_ihm_error_free, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_category_new", (PyCFunction)(void(*)(void))_wrap_ihm_category_new, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_reader_unknown_category_callback_set", (PyCFunction)(void(*)(void))_wrap_ihm_reader_unknown_category_callback_set, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_reader_unknown_keyword_callback_set", (PyCFunction)(void(*)(void))_wrap_ihm_reader_unknown_keyword_callback_set, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_reader_remove_all_categories", (PyCFunction)(void(*)(void))_wrap_ihm_reader_remove_all_categories, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_keyword_new", (PyCFunction)(void(*)(void))_wrap_ihm_keyword_new, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_file_buffer_set", _wrap_ihm_file_buffer_set, METH_VARARGS, NULL},
-	 { "ihm_file_buffer_get", _wrap_ihm_file_buffer_get, METH_O, NULL},
-	 { "ihm_file_line_start_set", _wrap_ihm_file_line_start_set, METH_VARARGS, NULL},
-	 { "ihm_file_line_start_get", _wrap_ihm_file_line_start_get, METH_O, NULL},
-	 { "ihm_file_next_line_start_set", _wrap_ihm_file_next_line_start_set, METH_VARARGS, NULL},
-	 { "ihm_file_next_line_start_get", _wrap_ihm_file_next_line_start_get, METH_O, NULL},
-	 { "ihm_file_read_callback_set", _wrap_ihm_file_read_callback_set, METH_VARARGS, NULL},
-	 { "ihm_file_read_callback_get", _wrap_ihm_file_read_callback_get, METH_O, NULL},
-	 { "ihm_file_data_set", _wrap_ihm_file_data_set, METH_VARARGS, NULL},
-	 { "ihm_file_data_get", _wrap_ihm_file_data_get, METH_O, NULL},
-	 { "ihm_file_free_func_set", _wrap_ihm_file_free_func_set, METH_VARARGS, NULL},
-	 { "ihm_file_free_func_get", _wrap_ihm_file_free_func_get, METH_O, NULL},
-	 { "ihm_file_new", (PyCFunction)(void(*)(void))_wrap_ihm_file_new, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_file_new_from_fd", (PyCFunction)(void(*)(void))_wrap_ihm_file_new_from_fd, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_reader_new", (PyCFunction)(void(*)(void))_wrap_ihm_reader_new, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_reader_free", (PyCFunction)(void(*)(void))_wrap_ihm_reader_free, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { "ihm_read_file", (PyCFunction)(void(*)(void))_wrap_ihm_read_file, METH_VARARGS|METH_KEYWORDS, NULL},
-	 { NULL, NULL, 0, NULL }
-};
-
-static PyMethodDef SwigMethods_proxydocs[] = {
+	 { (char *)"SWIG_PyInstanceMethod_New", (PyCFunction)SWIG_PyInstanceMethod_New, METH_O, NULL},
+	 { (char *)"ihm_file_new_from_python", (PyCFunction) _wrap_ihm_file_new_from_python, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"add_unknown_category_handler", (PyCFunction) _wrap_add_unknown_category_handler, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"add_unknown_keyword_handler", (PyCFunction) _wrap_add_unknown_keyword_handler, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"add_category_handler", (PyCFunction) _wrap_add_category_handler, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"add_poly_seq_scheme_handler", (PyCFunction) _wrap_add_poly_seq_scheme_handler, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"_test_finalize_callback", (PyCFunction) _wrap__test_finalize_callback, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_error_code_set", _wrap_ihm_error_code_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_error_code_get", _wrap_ihm_error_code_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_error_msg_set", _wrap_ihm_error_msg_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_error_msg_get", _wrap_ihm_error_msg_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_error_free", (PyCFunction) _wrap_ihm_error_free, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_category_new", (PyCFunction) _wrap_ihm_category_new, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_reader_unknown_category_callback_set", (PyCFunction) _wrap_ihm_reader_unknown_category_callback_set, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_reader_unknown_keyword_callback_set", (PyCFunction) _wrap_ihm_reader_unknown_keyword_callback_set, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_reader_remove_all_categories", (PyCFunction) _wrap_ihm_reader_remove_all_categories, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_keyword_new", (PyCFunction) _wrap_ihm_keyword_new, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_file_buffer_set", _wrap_ihm_file_buffer_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_buffer_get", _wrap_ihm_file_buffer_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_line_start_set", _wrap_ihm_file_line_start_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_line_start_get", _wrap_ihm_file_line_start_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_next_line_start_set", _wrap_ihm_file_next_line_start_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_next_line_start_get", _wrap_ihm_file_next_line_start_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_read_callback_set", _wrap_ihm_file_read_callback_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_read_callback_get", _wrap_ihm_file_read_callback_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_data_set", _wrap_ihm_file_data_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_data_get", _wrap_ihm_file_data_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_free_func_set", _wrap_ihm_file_free_func_set, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_free_func_get", _wrap_ihm_file_free_func_get, METH_VARARGS, NULL},
+	 { (char *)"ihm_file_new", (PyCFunction) _wrap_ihm_file_new, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_file_new_from_fd", (PyCFunction) _wrap_ihm_file_new_from_fd, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_reader_new", (PyCFunction) _wrap_ihm_reader_new, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_reader_free", (PyCFunction) _wrap_ihm_reader_free, METH_VARARGS | METH_KEYWORDS, NULL},
+	 { (char *)"ihm_read_file", (PyCFunction) _wrap_ihm_read_file, METH_VARARGS | METH_KEYWORDS, NULL},
 	 { NULL, NULL, 0, NULL }
 };
 
 
 /* -------- TYPE CONVERSION AND EQUIVALENCE RULES (BEGIN) -------- */
 
 static swig_type_info _swigt__p_IHMErrorCode = {"_p_IHMErrorCode", "enum IHMErrorCode *|IHMErrorCode *", 0, 0, (void*)0, 0};
@@ -4921,23 +5271,23 @@
        a different interpreter, but not yet have a pointer in this interpreter.
        In this case, we do not want to continue adding types... everything should be
        set up already */
   if (init == 0) return;
   
   /* Now work on filling in swig_module.types */
 #ifdef SWIGRUNTIME_DEBUG
-  printf("SWIG_InitializeModule: size %lu\n", (unsigned long)swig_module.size);
+  printf("SWIG_InitializeModule: size %d\n", swig_module.size);
 #endif
   for (i = 0; i < swig_module.size; ++i) {
     swig_type_info *type = 0;
     swig_type_info *ret;
     swig_cast_info *cast;
     
 #ifdef SWIGRUNTIME_DEBUG
-    printf("SWIG_InitializeModule: type %lu %s\n", (unsigned long)i, swig_module.type_initial[i]->name);
+    printf("SWIG_InitializeModule: type %d %s\n", i, swig_module.type_initial[i]->name);
 #endif
     
     /* if there is another module already loaded */
     if (swig_module.next != &swig_module) {
       type = SWIG_MangledTypeQueryModule(swig_module.next, &swig_module, swig_module.type_initial[i]->name);
     }
     if (type) {
@@ -5004,15 +5354,15 @@
   swig_module.types[i] = 0;
   
 #ifdef SWIGRUNTIME_DEBUG
   printf("**** SWIG_InitializeModule: Cast List ******\n");
   for (i = 0; i < swig_module.size; ++i) {
     int j = 0;
     swig_cast_info *cast = swig_module.cast_initial[i];
-    printf("SWIG_InitializeModule: type %lu %s\n", (unsigned long)i, swig_module.type_initial[i]->name);
+    printf("SWIG_InitializeModule: type %d %s\n", i, swig_module.type_initial[i]->name);
     while (cast->type) {
       printf("SWIG_InitializeModule: cast type %s\n", cast->type->name);
       cast++;
       ++j;
     }
     printf("---- Total casts: %d\n",j);
   }
@@ -5126,14 +5476,25 @@
       if (var->next) PyString_ConcatAndDel(&str,PyString_FromString(", "));
     }
     PyString_ConcatAndDel(&str,PyString_FromString(")"));
 #endif
     return str;
   }
   
+  SWIGINTERN int
+  swig_varlink_print(swig_varlinkobject *v, FILE *fp, int SWIGUNUSEDPARM(flags)) {
+    char *tmp;
+    PyObject *str = swig_varlink_str(v);
+    fprintf(fp,"Swig global variables ");
+    fprintf(fp,"%s\n", tmp = SWIG_Python_str_AsChar(str));
+    SWIG_Python_str_DelForPy3(tmp);
+    Py_DECREF(str);
+    return 0;
+  }
+  
   SWIGINTERN void
   swig_varlink_dealloc(swig_varlinkobject *v) {
     swig_globalvar *var = v->vars;
     while (var) {
       swig_globalvar *n = var->next;
       free(var->name);
       free(var);
@@ -5184,19 +5545,19 @@
       const PyTypeObject tmp = {
 #if PY_VERSION_HEX >= 0x03000000
         PyVarObject_HEAD_INIT(NULL, 0)
 #else
         PyObject_HEAD_INIT(NULL)
         0,                                  /* ob_size */
 #endif
-        "swigvarlink",                      /* tp_name */
+        (char *)"swigvarlink",              /* tp_name */
         sizeof(swig_varlinkobject),         /* tp_basicsize */
         0,                                  /* tp_itemsize */
         (destructor) swig_varlink_dealloc,  /* tp_dealloc */
-        0,                                  /* tp_print */
+        (printfunc) swig_varlink_print,     /* tp_print */
         (getattrfunc) swig_varlink_getattr, /* tp_getattr */
         (setattrfunc) swig_varlink_setattr, /* tp_setattr */
         0,                                  /* tp_compare */
         (reprfunc) swig_varlink_repr,       /* tp_repr */
         0,                                  /* tp_as_number */
         0,                                  /* tp_as_sequence */
         0,                                  /* tp_as_mapping */
@@ -5208,32 +5569,44 @@
         0,                                  /* tp_as_buffer */
         0,                                  /* tp_flags */
         varlink__doc__,                     /* tp_doc */
         0,                                  /* tp_traverse */
         0,                                  /* tp_clear */
         0,                                  /* tp_richcompare */
         0,                                  /* tp_weaklistoffset */
+#if PY_VERSION_HEX >= 0x02020000
         0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0, /* tp_iter -> tp_weaklist */
+#endif
+#if PY_VERSION_HEX >= 0x02030000
         0,                                  /* tp_del */
+#endif
+#if PY_VERSION_HEX >= 0x02060000
         0,                                  /* tp_version_tag */
+#endif
 #if PY_VERSION_HEX >= 0x03040000
         0,                                  /* tp_finalize */
 #endif
 #ifdef COUNT_ALLOCS
         0,                                  /* tp_allocs */
         0,                                  /* tp_frees */
         0,                                  /* tp_maxalloc */
+#if PY_VERSION_HEX >= 0x02050000
         0,                                  /* tp_prev */
+#endif
         0                                   /* tp_next */
 #endif
       };
       varlink_type = tmp;
       type_init = 1;
+#if PY_VERSION_HEX < 0x02020000
+      varlink_type.ob_type = &PyType_Type;
+#else
       if (PyType_Ready(&varlink_type) < 0)
       return NULL;
+#endif
     }
     return &varlink_type;
   }
   
   /* Create a variable linking object for use later */
   SWIGINTERN PyObject *
   SWIG_Python_newvarlink(void) {
@@ -5241,37 +5614,35 @@
     if (result) {
       result->vars = 0;
     }
     return ((PyObject*) result);
   }
   
   SWIGINTERN void 
-  SWIG_Python_addvarlink(PyObject *p, const char *name, PyObject *(*get_attr)(void), int (*set_attr)(PyObject *p)) {
+  SWIG_Python_addvarlink(PyObject *p, char *name, PyObject *(*get_attr)(void), int (*set_attr)(PyObject *p)) {
     swig_varlinkobject *v = (swig_varlinkobject *) p;
     swig_globalvar *gv = (swig_globalvar *) malloc(sizeof(swig_globalvar));
     if (gv) {
       size_t size = strlen(name)+1;
       gv->name = (char *)malloc(size);
       if (gv->name) {
-        memcpy(gv->name, name, size);
+        strncpy(gv->name,name,size);
         gv->get_attr = get_attr;
         gv->set_attr = set_attr;
         gv->next = v->vars;
       }
     }
     v->vars = gv;
   }
   
   SWIGINTERN PyObject *
   SWIG_globals(void) {
-    static PyObject *globals = 0;
-    if (!globals) {
-      globals = SWIG_newvarlink();
-    }
-    return globals;
+    static PyObject *_SWIG_globals = 0; 
+    if (!_SWIG_globals) _SWIG_globals = SWIG_newvarlink();  
+    return _SWIG_globals;
   }
   
   /* -----------------------------------------------------------------------------
    * constants/methods manipulation
    * ----------------------------------------------------------------------------- */
   
   /* Install Constants */
@@ -5342,72 +5713,14 @@
             }
           }
         }
       }
     }
   } 
   
-  /* -----------------------------------------------------------------------------
-   * Method creation and docstring support functions
-   * ----------------------------------------------------------------------------- */
-  
-  /* -----------------------------------------------------------------------------
-   * Function to find the method definition with the correct docstring for the
-   * proxy module as opposed to the low-level API
-   * ----------------------------------------------------------------------------- */
-  
-  SWIGINTERN PyMethodDef *SWIG_PythonGetProxyDoc(const char *name) {
-    /* Find the function in the modified method table */
-    size_t offset = 0;
-    int found = 0;
-    while (SwigMethods_proxydocs[offset].ml_meth != NULL) {
-      if (strcmp(SwigMethods_proxydocs[offset].ml_name, name) == 0) {
-        found = 1;
-        break;
-      }
-      offset++;
-    }
-    /* Use the copy with the modified docstring if available */
-    return found ? &SwigMethods_proxydocs[offset] : NULL;
-  }
-  
-  /* -----------------------------------------------------------------------------
-   * Wrapper of PyInstanceMethod_New() used in Python 3
-   * It is exported to the generated module, used for -fastproxy
-   * ----------------------------------------------------------------------------- */
-  
-  SWIGINTERN PyObject *SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func) {
-    if (PyCFunction_Check(func)) {
-      PyCFunctionObject *funcobj = (PyCFunctionObject *)func;
-      PyMethodDef *ml = SWIG_PythonGetProxyDoc(funcobj->m_ml->ml_name);
-      if (ml)
-      func = PyCFunction_NewEx(ml, funcobj->m_self, funcobj->m_module);
-    }
-#if PY_VERSION_HEX >= 0x03000000
-    return PyInstanceMethod_New(func);
-#else
-    return PyMethod_New(func, NULL, NULL);
-#endif
-  }
-  
-  /* -----------------------------------------------------------------------------
-   * Wrapper of PyStaticMethod_New()
-   * It is exported to the generated module, used for -fastproxy
-   * ----------------------------------------------------------------------------- */
-  
-  SWIGINTERN PyObject *SWIG_PyStaticMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func) {
-    if (PyCFunction_Check(func)) {
-      PyCFunctionObject *funcobj = (PyCFunctionObject *)func;
-      PyMethodDef *ml = SWIG_PythonGetProxyDoc(funcobj->m_ml->ml_name);
-      if (ml)
-      func = PyCFunction_NewEx(ml, funcobj->m_self, funcobj->m_module);
-    }
-    return PyStaticMethod_New(func);
-  }
-  
 #ifdef __cplusplus
 }
 #endif
 
 /* -----------------------------------------------------------------------------*
  *  Partial Init method
  * -----------------------------------------------------------------------------*/
@@ -5419,20 +5732,28 @@
 SWIGEXPORT 
 #if PY_VERSION_HEX >= 0x03000000
 PyObject*
 #else
 void
 #endif
 SWIG_init(void) {
-  PyObject *m, *d, *md, *globals;
-  
+  PyObject *m, *d, *md;
 #if PY_VERSION_HEX >= 0x03000000
   static struct PyModuleDef SWIG_module = {
+# if PY_VERSION_HEX >= 0x03020000
     PyModuleDef_HEAD_INIT,
-    SWIG_name,
+# else
+    {
+      PyObject_HEAD_INIT(NULL)
+      NULL, /* m_init */
+      0,    /* m_index */
+      NULL, /* m_copy */
+    },
+# endif
+    (char *) SWIG_name,
     NULL,
     -1,
     SwigMethods,
     NULL,
     NULL,
     NULL,
     NULL
@@ -5443,16 +5764,16 @@
   static SwigPyClientData SwigPyObject_clientdata = {
     0, 0, 0, 0, 0, 0, 0
   };
   static PyGetSetDef this_getset_def = {
     (char *)"this", &SwigPyBuiltin_ThisClosure, NULL, NULL, NULL
   };
   static SwigPyGetSet thisown_getset_closure = {
-    SwigPyObject_own,
-    SwigPyObject_own
+    (PyCFunction) SwigPyObject_own,
+    (PyCFunction) SwigPyObject_own
   };
   static PyGetSetDef thisown_getset_def = {
     (char *)"thisown", SwigPyBuiltin_GetterClosure, SwigPyBuiltin_SetterClosure, NULL, &thisown_getset_closure
   };
   PyTypeObject *builtin_pytype;
   int builtin_base_count;
   swig_type_info *builtin_basetype;
@@ -5475,31 +5796,21 @@
   (void)self;
   
   /* Metaclass is used to implement static member variables */
   metatype = SwigPyObjectType();
   assert(metatype);
 #endif
   
-  (void)globals;
-  
-  /* Create singletons now to avoid potential deadlocks with multi-threaded usage after module initialization */
-  SWIG_This();
-  SWIG_Python_TypeCache();
-  SwigPyPacked_type();
-#ifndef SWIGPYTHON_BUILTIN
-  SwigPyObject_type();
-#endif
-  
   /* Fix SwigMethods to carry the callback ptrs when needed */
   SWIG_Python_FixMethods(SwigMethods, swig_const_table, swig_types, swig_type_initial);
   
 #if PY_VERSION_HEX >= 0x03000000
   m = PyModule_Create(&SWIG_module);
 #else
-  m = Py_InitModule(SWIG_name, SwigMethods);
+  m = Py_InitModule((char *) SWIG_name, SwigMethods);
 #endif
   
   md = d = PyModule_GetDict(m);
   (void)md;
   
   SWIG_InitializeModule(0);
```

### Comparing `ihm-0.8/test/test_analysis.py` & `ihm-0.9/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_cross_linkers.py` & `ihm-0.9/test/test_cross_linkers.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_dataset.py` & `ihm-0.9/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_dictionary.py` & `ihm-0.9/test/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_dumper.py` & `ihm-0.9/test/test_dumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,16 +699,16 @@
         system.asym_units.extend((a1, a2))
         dumper = ihm.dumper._StructAsymDumper()
         self.assertRaises(ValueError, dumper.finalize, system)
 
     def test_assembly_all_modeled(self):
         """Test AssemblyDumper, all components modeled"""
         system = ihm.System()
-        e1 = ihm.Entity('AAA', description='foo')
-        e2 = ihm.Entity('AA', description='baz')
+        e1 = ihm.Entity('ACG', description='foo')
+        e2 = ihm.Entity('AW', description='baz')
         a1 = ihm.AsymUnit(e1)
         a2 = ihm.AsymUnit(e1)
         a3 = ihm.AsymUnit(e2)
         system.entities.extend((e1, e2))
         system.asym_units.extend((a1, a2, a3))
 
         system.orphan_assemblies.append(ihm.Assembly((a1, a2(2,3)), name='foo'))
@@ -723,89 +723,126 @@
         a = ihm.Assembly((a2, a3), description='desc2')
         system.orphan_assemblies.append(a)
 
         # Duplicate (identical) assembly (should be ignored, including
         # description)
         system.orphan_assemblies.append(a)
 
-        # Assign entity and asym IDs
+        # Assign entity, asym and range IDs
         ihm.dumper._EntityDumper().finalize(system)
         ihm.dumper._StructAsymDumper().finalize(system)
 
+        system._make_complete_assembly()
+
+        # Assign and check segment IDs
+        dumper = ihm.dumper._EntityPolySegmentDumper()
+        dumper.finalize(system)
+        out = _get_dumper_output(dumper, system)
+        self.assertEqual(out, """#
+loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+_ihm_entity_poly_segment.comp_id_begin
+_ihm_entity_poly_segment.comp_id_end
+1 1 1 3 ALA GLY
+2 2 1 2 ALA TRP
+3 1 2 3 CYS GLY
+#
+""")
+
         d = ihm.dumper._AssemblyDumper()
         d.finalize(system)
         self.assertEqual(system.complete_assembly._id, 1)
         self.assertEqual([a._id for a in system.orphan_assemblies], [2,3,3,3,3])
         out = _get_dumper_output(d, system)
         self.assertEqual(out, """#
 loop_
-_ihm_struct_assembly_details.assembly_id
-_ihm_struct_assembly_details.assembly_name
-_ihm_struct_assembly_details.assembly_description
+_ihm_struct_assembly.id
+_ihm_struct_assembly.name
+_ihm_struct_assembly.description
 1 'Complete assembly' 'All known components'
 2 foo .
 3 bar 'desc1 & desc2'
 #
 #
 loop_
-_ihm_struct_assembly.ordinal_id
-_ihm_struct_assembly.assembly_id
-_ihm_struct_assembly.parent_assembly_id
-_ihm_struct_assembly.entity_description
-_ihm_struct_assembly.entity_id
-_ihm_struct_assembly.asym_id
-_ihm_struct_assembly.seq_id_begin
-_ihm_struct_assembly.seq_id_end
-1 1 1 foo 1 A 1 3
-2 1 1 foo 1 B 1 3
-3 1 1 baz 2 C 1 2
-4 2 2 foo 1 A 1 3
-5 2 2 foo 1 B 2 3
-6 3 3 foo 1 B 1 3
-7 3 3 baz 2 C 1 2
+_ihm_struct_assembly_details.id
+_ihm_struct_assembly_details.assembly_id
+_ihm_struct_assembly_details.parent_assembly_id
+_ihm_struct_assembly_details.entity_description
+_ihm_struct_assembly_details.entity_id
+_ihm_struct_assembly_details.asym_id
+_ihm_struct_assembly_details.entity_poly_segment_id
+1 1 1 foo 1 A 1
+2 1 1 foo 1 B 1
+3 1 1 baz 2 C 2
+4 2 2 foo 1 A 1
+5 2 2 foo 1 B 3
+6 3 3 foo 1 B 1
+7 3 3 baz 2 C 2
 #
 """)
 
     def test_assembly_subset_modeled(self):
         """Test AssemblyDumper, subset of components modeled"""
         system = ihm.System()
-        e1 = ihm.Entity('AAA', description='foo')
-        e2 = ihm.Entity('AA', description='bar')
+        e1 = ihm.Entity('ACG', description='foo')
+        e2 = ihm.Entity('EW', description='bar')
         a1 = ihm.AsymUnit(e1)
         system.entities.extend((e1, e2))
         system.asym_units.append(a1)
         # Note that no asym unit uses entity e2, so the assembly
         # should omit the chain ID ('.')
 
         # Assign entity and asym IDs
         ihm.dumper._EntityDumper().finalize(system)
         ihm.dumper._StructAsymDumper().finalize(system)
 
+        system._make_complete_assembly()
+
+        # Assign and check segment IDs
+        dumper = ihm.dumper._EntityPolySegmentDumper()
+        dumper.finalize(system)
+        out = _get_dumper_output(dumper, system)
+        self.assertEqual(out, """#
+loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+_ihm_entity_poly_segment.comp_id_begin
+_ihm_entity_poly_segment.comp_id_end
+1 1 1 3 ALA GLY
+2 2 1 2 GLU TRP
+#
+""")
+
         d = ihm.dumper._AssemblyDumper()
         d.finalize(system)
         out = _get_dumper_output(d, system)
         self.assertEqual(out, """#
 loop_
-_ihm_struct_assembly_details.assembly_id
-_ihm_struct_assembly_details.assembly_name
-_ihm_struct_assembly_details.assembly_description
+_ihm_struct_assembly.id
+_ihm_struct_assembly.name
+_ihm_struct_assembly.description
 1 'Complete assembly' 'All known components'
 #
 #
 loop_
-_ihm_struct_assembly.ordinal_id
-_ihm_struct_assembly.assembly_id
-_ihm_struct_assembly.parent_assembly_id
-_ihm_struct_assembly.entity_description
-_ihm_struct_assembly.entity_id
-_ihm_struct_assembly.asym_id
-_ihm_struct_assembly.seq_id_begin
-_ihm_struct_assembly.seq_id_end
-1 1 1 foo 1 A 1 3
-2 1 1 bar 2 . 1 2
+_ihm_struct_assembly_details.id
+_ihm_struct_assembly_details.assembly_id
+_ihm_struct_assembly_details.parent_assembly_id
+_ihm_struct_assembly_details.entity_description
+_ihm_struct_assembly_details.entity_id
+_ihm_struct_assembly_details.asym_id
+_ihm_struct_assembly_details.entity_poly_segment_id
+1 1 1 foo 1 A 1
+2 1 1 bar 2 . 2
 #
 """)
 
     def test_external_reference_dumper(self):
         """Test ExternalReferenceDumper"""
         system = ihm.System()
         repo1 = ihm.location.Repository(doi="foo")
@@ -985,53 +1022,66 @@
         system = ihm.System()
         l = ihm.location.InputFileLocation(repo='foo', path='bar')
         l._id = 97
         ds1 = ihm.dataset.CXMSDataset(l)
         system.orphan_datasets.append(ds1)
 
         # group1 contains just the first dataset (but duplicated)
-        group1 = ihm.dataset.DatasetGroup([ds1, ds1])
+        group1 = ihm.dataset.DatasetGroup([ds1, ds1], name="first")
         system.orphan_dataset_groups.append(group1)
 
         l = ihm.location.InputFileLocation(repo='foo2', path='bar2')
         l._id = 98
         ds2 = ihm.dataset.CXMSDataset(l)
 
         # group2 contains all datasets so far (ds1 & ds2)
-        group2 = ihm.dataset.DatasetGroup([ds1, ds2])
+        group2 = ihm.dataset.DatasetGroup([ds1, ds2], name="all so far")
         system.orphan_dataset_groups.append(group2)
 
         l = ihm.location.PDBLocation('1abc', '1.0', 'test details')
         ds3 = ihm.dataset.PDBDataset(l, details='test dataset details')
         system.orphan_datasets.append(ds3)
         ds3.parents.append(ds2)
         # Ignore duplicates
         ds3.parents.append(ds2)
 
+        # Dataset with no location
+        ds4 = ihm.dataset.PDBDataset(None)
+        system.orphan_datasets.append(ds4)
+
         d = ihm.dumper._DatasetDumper()
         d.finalize(system) # Assign IDs
         out = _get_dumper_output(d, system)
         self.assertEqual(out, """#
 loop_
 _ihm_dataset_list.id
 _ihm_dataset_list.data_type
 _ihm_dataset_list.database_hosted
 _ihm_dataset_list.details
 1 'CX-MS data' NO .
 2 'CX-MS data' NO .
 3 'Experimental model' YES 'test dataset details'
+4 'Experimental model' NO .
+#
+#
+loop_
+_ihm_dataset_group.id
+_ihm_dataset_group.name
+_ihm_dataset_group.application
+_ihm_dataset_group.details
+1 first . .
+2 'all so far' . .
 #
 #
 loop_
-_ihm_dataset_group.ordinal_id
-_ihm_dataset_group.group_id
-_ihm_dataset_group.dataset_list_id
-1 1 1
-2 2 1
-3 2 2
+_ihm_dataset_group_link.group_id
+_ihm_dataset_group_link.dataset_list_id
+1 1
+2 1
+2 2
 #
 #
 loop_
 _ihm_dataset_external_reference.id
 _ihm_dataset_external_reference.dataset_list_id
 _ihm_dataset_external_reference.file_id
 1 1 97
@@ -1045,18 +1095,17 @@
 _ihm_dataset_related_db_reference.accession_code
 _ihm_dataset_related_db_reference.version
 _ihm_dataset_related_db_reference.details
 1 3 PDB 1abc 1.0 'test details'
 #
 #
 loop_
-_ihm_related_datasets.ordinal_id
 _ihm_related_datasets.dataset_list_id_derived
 _ihm_related_datasets.dataset_list_id_primary
-1 3 2
+3 2
 #
 """)
 
     def test_model_representation_dump(self):
         """Test ModelRepresentationDumper"""
         system = ihm.System()
         e1 = ihm.Entity('AAAAAAAA', description='bar')
@@ -1071,43 +1120,53 @@
                     rigid=False, primitive='sphere')
         s3 = ihm.representation.MultiResidueSegment(
                     asym(1,2), starting_model=None,
                     rigid=False, primitive='gaussian')
         s4 = ihm.representation.FeatureSegment(
                     asym(3,4), starting_model=None,
                     rigid=True, primitive='other', count=3)
-        r1 = ihm.representation.Representation((s1, s2))
-        r2 = ihm.representation.Representation((s3, s4))
+        r1 = ihm.representation.Representation((s1, s2), name='foo',
+                                               details='foo details')
+        r2 = ihm.representation.Representation((s3, s4), name='bar')
         system.orphan_representations.extend((r1, r2))
 
         e1._id = 42
         asym._id = 'X'
 
+        # Assign segment IDs
+        ihm.dumper._EntityPolySegmentDumper().finalize(system)
+
         dumper = ihm.dumper._ModelRepresentationDumper()
         dumper.finalize(system) # assign IDs
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_model_representation.ordinal_id
-_ihm_model_representation.representation_id
-_ihm_model_representation.segment_id
-_ihm_model_representation.entity_id
-_ihm_model_representation.entity_description
-_ihm_model_representation.entity_asym_id
-_ihm_model_representation.seq_id_begin
-_ihm_model_representation.seq_id_end
-_ihm_model_representation.model_object_primitive
-_ihm_model_representation.starting_model_id
-_ihm_model_representation.model_mode
-_ihm_model_representation.model_granularity
-_ihm_model_representation.model_object_count
-1 1 1 42 bar X 1 2 atomistic . rigid by-atom .
-2 1 2 42 bar X 3 4 sphere . flexible by-residue .
-3 2 1 42 bar X 1 2 gaussian . flexible multi-residue .
-4 2 2 42 bar X 3 4 other . rigid by-feature 3
+_ihm_model_representation.id
+_ihm_model_representation.name
+_ihm_model_representation.details
+1 foo 'foo details'
+2 bar .
+#
+#
+loop_
+_ihm_model_representation_details.id
+_ihm_model_representation_details.representation_id
+_ihm_model_representation_details.entity_id
+_ihm_model_representation_details.entity_description
+_ihm_model_representation_details.entity_asym_id
+_ihm_model_representation_details.entity_poly_segment_id
+_ihm_model_representation_details.model_object_primitive
+_ihm_model_representation_details.starting_model_id
+_ihm_model_representation_details.model_mode
+_ihm_model_representation_details.model_granularity
+_ihm_model_representation_details.model_object_count
+1 1 42 bar X 1 atomistic . rigid by-atom .
+2 1 42 bar X 2 sphere . flexible by-residue .
+3 2 42 bar X 1 gaussian . flexible multi-residue .
+4 2 42 bar X 2 other . rigid by-feature 3
 #
 """)
 
     def test_starting_model_dumper(self):
         """Test StartingModelDumper"""
         class TestStartingModel(ihm.startmodel.StartingModel):
             def get_atoms(self):
@@ -1139,15 +1198,16 @@
         s1 = ihm.startmodel.Template(dataset=dstemplate, asym_id='C',
                              seq_id_range=(-9,0), # 1,10 in IHM numbering
                              template_seq_id_range=(101,110),
                              sequence_identity=30.)
         s2 = ihm.startmodel.Template(dataset=dstemplate, asym_id='D',
                              seq_id_range=(-5,2), # 5,12 in IHM numbering
                              template_seq_id_range=(201,210),
-                             sequence_identity=40.,
+                             sequence_identity
+                                    =ihm.startmodel.SequenceIdentity(40., None),
                              alignment_file=ali)
 
         sm = TestStartingModel(asym(1,15), dstarget, 'A', [s1, s2], offset=10,
                                script_file=script, software=software)
         system.orphan_starting_models.append(sm)
 
         sm = TestStartingModel(asym(1,15), dstarget, 'A', [])
@@ -1156,55 +1216,71 @@
         e1._id = 42
         asym._id = 99
         dstemplate._id = 101
         dstarget._id = 102
         ali._id = 5
         script._id = 8
         software._id = 99
+        # Assign and check segment IDs
+        dumper = ihm.dumper._EntityPolySegmentDumper()
+        dumper.finalize(system)
+        out = _get_dumper_output(dumper, system)
+        self.assertEqual(out, """#
+loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+_ihm_entity_poly_segment.comp_id_begin
+_ihm_entity_poly_segment.comp_id_end
+1 42 1 15 ALA ALA
+2 42 1 12 ALA ALA
+#
+""")
+
         dumper = ihm.dumper._StartingModelDumper()
         dumper.finalize(system) # assign IDs
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
 _ihm_starting_model_details.starting_model_id
 _ihm_starting_model_details.entity_id
 _ihm_starting_model_details.entity_description
 _ihm_starting_model_details.asym_id
-_ihm_starting_model_details.seq_id_begin
-_ihm_starting_model_details.seq_id_end
+_ihm_starting_model_details.entity_poly_segment_id
 _ihm_starting_model_details.starting_model_source
 _ihm_starting_model_details.starting_model_auth_asym_id
 _ihm_starting_model_details.starting_model_sequence_offset
 _ihm_starting_model_details.dataset_list_id
-1 42 foo 99 1 12 'experimental model' A 10 102
-2 42 foo 99 1 15 'experimental model' A 0 102
+1 42 foo 99 2 'experimental model' A 10 102
+2 42 foo 99 1 'experimental model' A 0 102
 #
 #
 loop_
 _ihm_starting_computational_models.starting_model_id
 _ihm_starting_computational_models.software_id
 _ihm_starting_computational_models.script_file_id
 1 99 8
 #
 #
 loop_
-_ihm_starting_comparative_models.ordinal_id
+_ihm_starting_comparative_models.id
 _ihm_starting_comparative_models.starting_model_id
 _ihm_starting_comparative_models.starting_model_auth_asym_id
 _ihm_starting_comparative_models.starting_model_seq_id_begin
 _ihm_starting_comparative_models.starting_model_seq_id_end
 _ihm_starting_comparative_models.template_auth_asym_id
 _ihm_starting_comparative_models.template_seq_id_begin
 _ihm_starting_comparative_models.template_seq_id_end
 _ihm_starting_comparative_models.template_sequence_identity
 _ihm_starting_comparative_models.template_sequence_identity_denominator
 _ihm_starting_comparative_models.template_dataset_list_id
 _ihm_starting_comparative_models.alignment_file_id
 1 1 A 1 10 C 101 110 30.000 1 101 .
-2 1 A 5 12 D 201 210 40.000 1 101 5
+2 1 A 5 12 D 201 210 40.000 . 101 5
 #
 #
 loop_
 _ihm_starting_model_coord.starting_model_id
 _ihm_starting_model_coord.group_PDB
 _ihm_starting_model_coord.id
 _ihm_starting_model_coord.type_symbol
@@ -1219,15 +1295,15 @@
 _ihm_starting_model_coord.B_iso_or_equiv
 _ihm_starting_model_coord.ordinal_id
 1 ATOM 1 C CA ALA 42 99 1 -8.000 -5.000 91.000 42.000 1
 2 ATOM 1 C CA ALA 42 99 1 -8.000 -5.000 91.000 42.000 2
 #
 #
 loop_
-_ihm_starting_model_seq_dif.ordinal_id
+_ihm_starting_model_seq_dif.id
 _ihm_starting_model_seq_dif.entity_id
 _ihm_starting_model_seq_dif.asym_id
 _ihm_starting_model_seq_dif.seq_id
 _ihm_starting_model_seq_dif.comp_id
 _ihm_starting_model_seq_dif.starting_model_id
 _ihm_starting_model_seq_dif.db_asym_id
 _ihm_starting_model_seq_dif.db_seq_id
@@ -1272,33 +1348,40 @@
         system.orphan_protocols.append(p2)
 
         dumper = ihm.dumper._ProtocolDumper()
         dumper.finalize(system) # assign IDs
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_modeling_protocol.ordinal_id
-_ihm_modeling_protocol.protocol_id
-_ihm_modeling_protocol.step_id
-_ihm_modeling_protocol.struct_assembly_id
-_ihm_modeling_protocol.dataset_group_id
-_ihm_modeling_protocol.struct_assembly_description
+_ihm_modeling_protocol.id
 _ihm_modeling_protocol.protocol_name
-_ihm_modeling_protocol.step_name
-_ihm_modeling_protocol.step_method
-_ihm_modeling_protocol.num_models_begin
-_ihm_modeling_protocol.num_models_end
-_ihm_modeling_protocol.multi_scale_flag
-_ihm_modeling_protocol.multi_state_flag
-_ihm_modeling_protocol.ordered_flag
-_ihm_modeling_protocol.software_id
-_ihm_modeling_protocol.script_file_id
-1 1 1 42 99 foo equilibration s1 'Monte Carlo' 0 500 YES NO NO . .
-2 1 2 42 99 foo equilibration . 'Replica exchange' 500 2000 YES NO NO . .
-3 2 1 42 101 foo sampling . 'Replica exchange' 2000 1000 YES NO NO 80 90
+_ihm_modeling_protocol.num_steps
+1 equilibration 2
+2 sampling 1
+#
+#
+loop_
+_ihm_modeling_protocol_details.id
+_ihm_modeling_protocol_details.protocol_id
+_ihm_modeling_protocol_details.step_id
+_ihm_modeling_protocol_details.struct_assembly_id
+_ihm_modeling_protocol_details.dataset_group_id
+_ihm_modeling_protocol_details.struct_assembly_description
+_ihm_modeling_protocol_details.step_name
+_ihm_modeling_protocol_details.step_method
+_ihm_modeling_protocol_details.num_models_begin
+_ihm_modeling_protocol_details.num_models_end
+_ihm_modeling_protocol_details.multi_scale_flag
+_ihm_modeling_protocol_details.multi_state_flag
+_ihm_modeling_protocol_details.ordered_flag
+_ihm_modeling_protocol_details.software_id
+_ihm_modeling_protocol_details.script_file_id
+1 1 1 42 99 foo s1 'Monte Carlo' 0 500 YES NO NO . .
+2 1 2 42 99 foo . 'Replica exchange' 500 2000 YES NO NO . .
+3 2 1 42 101 foo . 'Replica exchange' 2000 1000 YES NO NO 80 90
 #
 """)
 
     def test_post_process(self):
         """Test PostProcessDumper"""
         class MockObject(object):
             pass
@@ -1390,25 +1473,38 @@
 
         dumper = ihm.dumper._ModelDumper()
         dumper.finalize(system) # assign model/group IDs
 
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 'test model' Group1 99 42 32
-2 2 1 'test model2' Group1 99 42 32
-3 3 2 'test model3' 'Group 2' 99 42 32
+1 'test model' 99 42 32
+2 'test model2' 99 42 32
+3 'test model3' 99 42 32
+#
+#
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 Group1 .
+2 'Group 2' .
+#
+#
+loop_
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
+1 2
+2 3
 #
 """)
 
     def _make_test_model(self):
         class MockObject(object):
             pass
         system = ihm.System()
@@ -1703,27 +1799,37 @@
 
         dumper = ihm.dumper._ModelDumper()
         dumper.finalize(system) # assign model/group IDs
 
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 'test model' . 99 42 32
+1 'test model' 99 42 32
+#
+#
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 . .
+#
+#
+loop_
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
 #
 #
 loop_
-_ihm_sphere_obj_site.ordinal_id
+_ihm_sphere_obj_site.id
 _ihm_sphere_obj_site.entity_id
 _ihm_sphere_obj_site.seq_id_begin
 _ihm_sphere_obj_site.seq_id_end
 _ihm_sphere_obj_site.asym_id
 _ihm_sphere_obj_site.Cartn_x
 _ihm_sphere_obj_site.Cartn_y
 _ihm_sphere_obj_site.Cartn_z
@@ -1756,23 +1862,33 @@
 
         dumper = ihm.dumper._ModelDumper()
         dumper.finalize(system) # assign model/group IDs
 
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 'test model' . 99 42 32
+1 'test model' 99 42 32
+#
+#
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 . .
+#
+#
+loop_
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
 #
 #
 loop_
 _atom_site.group_PDB
 _atom_site.id
 _atom_site.type_symbol
 _atom_site.label_atom_id
@@ -1861,29 +1977,71 @@
         loc = ihm.location.OutputFileLocation(repo='foo', path='bar')
         loc._id = 3
         ens.densities.append(ihm.model.LocalizationDensity(loc, asym(1,2)))
         ens.densities.append(ihm.model.LocalizationDensity(loc, asym))
         ens._id = 5
         system.ensembles.append(ens)
 
+        # Assign segment IDs
+        ihm.dumper._EntityPolySegmentDumper().finalize(system)
+
         dumper = ihm.dumper._DensityDumper()
         dumper.finalize(system) # assign IDs
 
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
 _ihm_localization_density_files.id
 _ihm_localization_density_files.file_id
 _ihm_localization_density_files.ensemble_id
 _ihm_localization_density_files.entity_id
 _ihm_localization_density_files.asym_id
-_ihm_localization_density_files.seq_id_begin
-_ihm_localization_density_files.seq_id_end
-1 3 5 9 X 1 2
-2 3 5 9 X 1 4
+_ihm_localization_density_files.entity_poly_segment_id
+1 3 5 9 X 1
+2 3 5 9 X 2
+#
+""")
+
+    def test_entity_poly_segment_dumper(self):
+        """Test EntityPolySegmentDumper"""
+        system = ihm.System()
+        e1 = ihm.Entity('AHCD')
+        e2 = ihm.Entity('ACG')
+        e3 = ihm.Entity([ihm.NonPolymerChemComp('HEM')])
+        a1 = ihm.AsymUnit(e1)
+        a1._id = 'X'
+        system.entities.extend((e1, e2, e3))
+        system.asym_units.append(a1)
+
+        system._make_complete_assembly()
+
+        ihm.dumper._EntityDumper().finalize(system) # assign entity IDs
+
+        dumper = ihm.dumper._EntityPolySegmentDumper()
+        dumper.finalize(system) # assign IDs
+
+        # e1 isn't directly used in the assembly (a1 is used instead) so
+        # should have no range ID
+        self.assertFalse(hasattr(e1, '_range_id'))
+        self.assertEqual(a1._range_id, 1)
+        self.assertEqual(e2._range_id, 2)
+        # non-polymers don't have ranges
+        self.assertEqual(e3._range_id, None)
+
+        out = _get_dumper_output(dumper, system)
+        self.assertEqual(out, """#
+loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+_ihm_entity_poly_segment.comp_id_begin
+_ihm_entity_poly_segment.comp_id_end
+1 1 1 4 ALA ASP
+2 2 1 3 ALA GLY
 #
 """)
 
     def test_single_state(self):
         """Test MultiStateDumper with a single state"""
         system = ihm.System()
         state = ihm.model.State()
@@ -1924,27 +2082,33 @@
 
         dumper = ihm.dumper._MultiStateDumper()
         dumper.finalize(system) # assign IDs
 
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_multi_state_modeling.ordinal_id
 _ihm_multi_state_modeling.state_id
 _ihm_multi_state_modeling.state_group_id
 _ihm_multi_state_modeling.population_fraction
 _ihm_multi_state_modeling.state_type
 _ihm_multi_state_modeling.state_name
-_ihm_multi_state_modeling.model_group_id
 _ihm_multi_state_modeling.experiment_type
 _ihm_multi_state_modeling.details
-1 1 1 . 'complex formation' unbound 1 'Fraction of bulk' 'Unbound molecule 1'
-2 1 1 . 'complex formation' unbound 2 'Fraction of bulk' 'Unbound molecule 1'
-3 2 1 . 'complex formation' bound 3 'Fraction of bulk' 'Unbound molecule 2'
-4 3 2 0.400 . . 4 . .
+1 1 . 'complex formation' unbound 'Fraction of bulk' 'Unbound molecule 1'
+2 1 . 'complex formation' bound 'Fraction of bulk' 'Unbound molecule 2'
+3 2 0.400 . . . .
+#
+#
+loop_
+_ihm_multi_state_model_group_link.state_id
+_ihm_multi_state_model_group_link.model_group_id
+1 1
+1 2
+2 3
+3 4
 #
 """)
 
     def test_orphan_model_groups(self):
         """Test detection of ModelGroups not in States"""
         system = ihm.System()
         m1 = ihm.model.Model(assembly='a1', protocol='p1', representation='r1')
@@ -2040,15 +2204,15 @@
 
         dumper = ihm.dumper._EM3DDumper()
         dumper.finalize(system) # assign IDs
 
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_3dem_restraint.ordinal_id
+_ihm_3dem_restraint.id
 _ihm_3dem_restraint.dataset_list_id
 _ihm_3dem_restraint.fitting_method
 _ihm_3dem_restraint.fitting_method_citation_id
 _ihm_3dem_restraint.struct_assembly_id
 _ihm_3dem_restraint.number_of_gaussians
 _ihm_3dem_restraint.model_id
 _ihm_3dem_restraint.cross_correlation_coefficient
@@ -2086,15 +2250,15 @@
 
         dumper = ihm.dumper._SASDumper()
         dumper.finalize(system) # assign IDs
 
         out = _get_dumper_output(dumper, system)
         self.assertEqual(out, """#
 loop_
-_ihm_sas_restraint.ordinal_id
+_ihm_sas_restraint.id
 _ihm_sas_restraint.dataset_list_id
 _ihm_sas_restraint.model_id
 _ihm_sas_restraint.struct_assembly_id
 _ihm_sas_restraint.profile_segment_flag
 _ihm_sas_restraint.fitting_atom_type
 _ihm_sas_restraint.fitting_method
 _ihm_sas_restraint.fitting_state
@@ -2152,15 +2316,15 @@
 _ihm_2dem_class_average_restraint.number_of_projections
 _ihm_2dem_class_average_restraint.struct_assembly_id
 _ihm_2dem_class_average_restraint.details
 1 97 400 0.600 0.500 30.000 NO 100 99 'Test fit'
 #
 #
 loop_
-_ihm_2dem_class_average_fitting.ordinal_id
+_ihm_2dem_class_average_fitting.id
 _ihm_2dem_class_average_fitting.restraint_id
 _ihm_2dem_class_average_fitting.model_id
 _ihm_2dem_class_average_fitting.cross_correlation_coefficient
 _ihm_2dem_class_average_fitting.rot_matrix[1][1]
 _ihm_2dem_class_average_fitting.rot_matrix[2][1]
 _ihm_2dem_class_average_fitting.rot_matrix[3][1]
 _ihm_2dem_class_average_fitting.rot_matrix[1][2]
@@ -2273,15 +2437,15 @@
 _ihm_cross_link_restraint.sigma_2
 1 1 1 A 2 THR 1 A 3 CYS . . 'upper bound' ALL by-residue 25.000 0.500 1.000
 2.000
 2 3 1 A 2 THR 2 B 2 GLU C N 'lower bound' ANY by-atom 34.000 . . .
 #
 #
 loop_
-_ihm_cross_link_result_parameters.ordinal_id
+_ihm_cross_link_result_parameters.id
 _ihm_cross_link_result_parameters.restraint_id
 _ihm_cross_link_result_parameters.model_id
 _ihm_cross_link_result_parameters.psi
 _ihm_cross_link_result_parameters.sigma_1
 _ihm_cross_link_result_parameters.sigma_2
 1 1 201 0.100 4.200 2.100
 #
@@ -2688,34 +2852,33 @@
 loop_
 _ihm_predicted_contact_restraint.id
 _ihm_predicted_contact_restraint.group_id
 _ihm_predicted_contact_restraint.entity_id_1
 _ihm_predicted_contact_restraint.asym_id_1
 _ihm_predicted_contact_restraint.comp_id_1
 _ihm_predicted_contact_restraint.seq_id_1
-_ihm_predicted_contact_restraint.atom_id_1
+_ihm_predicted_contact_restraint.rep_atom_1
 _ihm_predicted_contact_restraint.entity_id_2
 _ihm_predicted_contact_restraint.asym_id_2
 _ihm_predicted_contact_restraint.comp_id_2
 _ihm_predicted_contact_restraint.seq_id_2
-_ihm_predicted_contact_restraint.atom_id_2
+_ihm_predicted_contact_restraint.rep_atom_2
 _ihm_predicted_contact_restraint.restraint_type
 _ihm_predicted_contact_restraint.distance_lower_limit
 _ihm_predicted_contact_restraint.distance_upper_limit
 _ihm_predicted_contact_restraint.probability
 _ihm_predicted_contact_restraint.model_granularity
 _ihm_predicted_contact_restraint.dataset_list_id
 _ihm_predicted_contact_restraint.software_id
 1 . 1 A ALA 1 . 2 B TRP 2 . 'lower bound' 25.000 . 0.800 by-residue 97 34
 2 1 1 A ALA 1 CA 2 B TRP 2 CB 'lower bound' 25.000 . 0.400 by-residue 97 .
 3 1 1 A ALA 1 . 2 B TRP 2 . 'upper bound' . 14.000 0.600 by-feature 97 .
 #
 """)
 
-
     def test_FLRDumper(self):
         """Test FLR dumpers"""
 
         class MockObject(object):
             pass
 
         cur_state = MockObject()
```

### Comparing `ihm-0.8/test/test_examples.py` & `ihm-0.9/test/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                                    get_example_path("simple-docking.py")],
                                   cwd=tmpdir)
 
             # Make sure that a complete output file was produced and that we
             # can read it
             with open(os.path.join(tmpdir, 'output.cif')) as fh:
                 contents = fh.readlines()
-            self.assertEqual(len(contents), 272)
+            self.assertEqual(len(contents), 309)
             with open(os.path.join(tmpdir, 'output.cif')) as fh:
                 s, = ihm.reader.read(fh)
 
     def test_locations_example(self):
         """Test locations example"""
         subprocess.check_call([sys.executable, "locations.py"],
                               cwd=get_example_dir())
@@ -54,15 +54,15 @@
                               cwd=get_example_dir())
         out = get_example_path("output.cif")
 
         # Make sure that a complete output file was produced and that we
         # can read it
         with open(out) as fh:
             contents = fh.readlines()
-        self.assertEqual(len(contents), 147)
+        self.assertEqual(len(contents), 158)
         with open(out) as fh:
             s, = ihm.reader.read(fh)
         # Make sure that resulting Python objects are picklable
         testpck = 'test-lig-wat.pck'
         with open(testpck, 'wb') as fh:
             pickle.dump(s, fh, protocol=-1)
         with open(testpck, 'rb') as fh:
@@ -76,15 +76,15 @@
                               cwd=get_example_dir())
         out = get_example_path("output.cif")
 
         # Make sure that a complete output file was produced and that we
         # can read it
         with open(out) as fh:
             contents = fh.readlines()
-        self.assertEqual(len(contents), 77)
+        self.assertEqual(len(contents), 87)
         with open(out) as fh:
             s, = ihm.reader.read(fh)
         os.unlink(out)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ihm-0.8/test/test_flr.py` & `ihm-0.9/test/test_flr.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_format.py` & `ihm-0.9/test/test_format.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_format_bcif.py` & `ihm-0.9/test/test_format_bcif.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_geometry.py` & `ihm-0.9/test/test_geometry.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_location.py` & `ihm-0.9/test/test_location.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_main.py` & `ihm-0.9/test/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -817,14 +817,51 @@
         conj = ihm.flr.PolyProbeConjugate(sample_probe=None, chem_descriptor=d4,
                                           ambiguous_stoichiometry=False)
         f.poly_probe_conjugates.append(conj)
 
         # duplicates should not be filtered
         self.assertEqual(list(s._all_chem_descriptors()), [d1, d2, d1, d3, d4])
 
+    def test_all_entity_ranges(self):
+        """Test _all_entity_ranges() method"""
+        class MockObject(object):
+            pass
+
+        s = ihm.System()
+        e1 = ihm.Entity('AHCD', description='foo')
+        a1 = ihm.AsymUnit(e1)
+        s.entities.append(e1)
+        s.asym_units.append(a1)
+        e1rng = e1(1,3)
+        a1rng = a1(1,2)
+
+        sm1 = MockObject()
+        sm1.asym_unit = e1rng
+        s.orphan_starting_models.append(sm1)
+
+        rep = ihm.representation.Representation()
+        seg1 = ihm.representation.Segment()
+        seg1.starting_model = None
+        seg1.asym_unit = a1
+        rep.append(seg1)
+        s.orphan_representations.append(rep)
+
+        asmb1 = ihm.Assembly([e1, a1])
+        s.orphan_assemblies.append(asmb1)
+
+        ensemble = MockObject()
+        density = MockObject()
+        density.asym_unit = a1rng
+        ensemble.densities = [density]
+        s.ensembles.append(ensemble)
+
+        # duplicates should not be filtered
+        self.assertEqual(list(s._all_entity_ranges()),
+                         [e1rng, a1, e1, a1, a1rng])
+
     def test_update_locations_in_repositories(self):
         """Test update_locations_in_repositories() method"""
         s = ihm.System()
         loc = ihm.location.InputFileLocation(path='foo', repo='bar')
         s.locations.append(loc)
         r = ihm.location.Repository(doi='foo', root='..')
         s.update_locations_in_repositories([r])
```

### Comparing `ihm-0.8/test/test_metadata.py` & `ihm-0.9/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_model.py` & `ihm-0.9/test/test_model.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_protocol.py` & `ihm-0.9/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_reader.py` & `ihm-0.9/test/test_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,28 +321,30 @@
 _entity_poly_seq.num
 _entity_poly_seq.mon_id
 _entity_poly_seq.hetero
 1 1 OCS .
 1 2 MET .
 1 3 ACE .
 2 1 MET .
+3 1 MET .
 #
 loop_
 _entity_poly.entity_id
 _entity_poly.type
 _entity_poly.pdbx_seq_one_letter_code
 _entity_poly.pdbx_seq_one_letter_code_can
 1 'polypeptide(L)'
 ;(OCS)
 M
 ;
 SM
+3 other . .
 """)
         s, = ihm.reader.read(fh)
-        e1, e2 = s.entities
+        e1, e2, e3 = s.entities
         c1, c2, c3 = e1.sequence
         self.assertEqual(c1.id, 'OCS')
         # Missing information should be filled in from entity_poly
         self.assertEqual(c1.code, 'OCS')
         self.assertEqual(c1.code_canonical, 'S')
         # No info in entity_poly for this component
         self.assertEqual(c3.id, 'ACE')
@@ -573,63 +575,73 @@
             self.assertEqual(a1.details, 'Nup84')
             self.assertEqual(a2.entity._id, '1')
             self.assertEqual(a2._id, 'B')
             self.assertEqual(a2.id, 'B')
             self.assertEqual(a2.details, 'Nup85')
             self.assertEqual(id(a1.entity), id(a2.entity))
 
-    def test_assembly_details_handler(self):
-        """Test AssemblyDetailsHandler"""
+    def test_assembly_handler(self):
+        """Test AssemblyHandler"""
         cif = """
 loop_
-_ihm_struct_assembly_details.assembly_id
-_ihm_struct_assembly_details.assembly_name
-_ihm_struct_assembly_details.assembly_description
+_ihm_struct_assembly.id
+_ihm_struct_assembly.name
+_ihm_struct_assembly.description
 1 'Complete assembly' 'All known components'
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             a1, = s.orphan_assemblies
             self.assertEqual(a1._id, '1')
             self.assertEqual(a1.name, 'Complete assembly')
             self.assertEqual(a1.description, 'All known components')
 
-    def test_assembly_handler(self):
-        """Test AssemblyHandler"""
+    def test_assembly_details_handler(self):
+        """Test AssemblyDetailsHandler"""
         cif = """
 loop_
 _entity_poly_seq.entity_id
 _entity_poly_seq.num
 _entity_poly_seq.mon_id
 1 1 ALA
 2 1 ALA
 #
 loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+1 1 1 726
+2 2 1 744
+3 1 1 1
+4 2 1 50
+5 2 1 1
+#
+loop_
 _struct_asym.id
 _struct_asym.entity_id
 _struct_asym.details
 A 1 Nup84
 B 2 Nup85
 #
 loop_
-_ihm_struct_assembly.ordinal_id
-_ihm_struct_assembly.assembly_id
-_ihm_struct_assembly.parent_assembly_id
-_ihm_struct_assembly.entity_description
-_ihm_struct_assembly.entity_id
-_ihm_struct_assembly.asym_id
-_ihm_struct_assembly.seq_id_begin
-_ihm_struct_assembly.seq_id_end
-1 1 1 Nup84 1 A 1 726
-2 1 1 Nup85 2 B 1 744
-3 1 1 Nup84 1 A 1 1
-4 2 1 Nup86 2 . 1 50
-5 2 1 Nup85 2 . 1 1
-6 3 1 Nup84 1 A . .
-7 3 1 Nup85 2 . . .
+_ihm_struct_assembly_details.id
+_ihm_struct_assembly_details.assembly_id
+_ihm_struct_assembly_details.parent_assembly_id
+_ihm_struct_assembly_details.entity_description
+_ihm_struct_assembly_details.entity_id
+_ihm_struct_assembly_details.asym_id
+_ihm_struct_assembly_details.entity_poly_segment_id
+1 1 1 Nup84 1 A 1
+2 1 1 Nup85 2 B 2
+3 1 1 Nup84 1 A 3
+4 2 1 Nup86 2 . 4
+5 2 1 Nup85 2 . 5
+6 3 1 Nup84 1 A .
+7 3 1 Nup85 2 . .
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             a1, a2, a3 = s.orphan_assemblies
             self.assertEqual(a1._id, '1')
             self.assertIsNone(a1.parent)
             self.assertEqual(len(a1), 3)
@@ -736,19 +748,36 @@
             self.assertIsNone(d1.details)
             self.assertEqual(d3.details, 'test details')
 
     def test_dataset_group_handler(self):
         """Test DatasetGroupHandler"""
         cif = """
 loop_
-_ihm_dataset_group.ordinal_id
-_ihm_dataset_group.group_id
-_ihm_dataset_group.dataset_list_id
-1 1 1
-2 1 2
+_ihm_dataset_group.id
+_ihm_dataset_group.name
+_ihm_dataset_group.application
+_ihm_dataset_group.details
+1 "foo" "foo app" "foo details"
+"""
+        for fh in cif_file_handles(cif):
+            s, = ihm.reader.read(fh)
+            g1, = s.orphan_dataset_groups
+            self.assertEqual(len(g1), 0) # no datasets read yet
+            self.assertEqual(g1.name, 'foo')
+            self.assertEqual(g1.application, 'foo app')
+            self.assertEqual(g1.details, 'foo details')
+
+    def test_dataset_group_link_handler(self):
+        """Test DatasetGroupLinkHandler"""
+        cif = """
+loop_
+_ihm_dataset_group_link.group_id
+_ihm_dataset_group_link.dataset_list_id
+1 1
+1 2
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             d1, d2 = s.orphan_datasets
             g1, = s.orphan_dataset_groups
             self.assertEqual(len(g1), 2)
             self.assertEqual(g1[0], d1)
@@ -811,48 +840,69 @@
                              ihm.location.DatabaseLocation)
             self.assertIsNone(d4.location.access_code)
 
     def test_related_datasets_handler(self):
         """Test RelatedDatasetsHandler"""
         cif = """
 loop_
-_ihm_related_datasets.ordinal_id
 _ihm_related_datasets.dataset_list_id_derived
 _ihm_related_datasets.dataset_list_id_primary
-1 4 1
+4 1
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             d1, d2 = s.orphan_datasets
             self.assertEqual(d1._id, '4')
             self.assertEqual(d2._id, '1')
             self.assertEqual(d1.parents, [d2])
             self.assertEqual(d2.parents, [])
 
     def test_model_representation_handler(self):
         """Test ModelRepresentationHandler"""
         cif = """
 loop_
-_ihm_model_representation.ordinal_id
-_ihm_model_representation.representation_id
-_ihm_model_representation.segment_id
-_ihm_model_representation.entity_id
-_ihm_model_representation.entity_description
-_ihm_model_representation.entity_asym_id
-_ihm_model_representation.seq_id_begin
-_ihm_model_representation.seq_id_end
-_ihm_model_representation.model_object_primitive
-_ihm_model_representation.starting_model_id
-_ihm_model_representation.model_mode
-_ihm_model_representation.model_granularity
-_ihm_model_representation.model_object_count
-1 1 1 1 Nup84 A 1 6 sphere . flexible by-feature 1
-2 1 2 1 Nup84 A 7 20 sphere 1 rigid by-residue .
-3 2 1 1 Nup84 A . . atomistic . flexible by-atom .
-4 3 1 2 Nup85 B . . sphere . . multi-residue .
+_ihm_model_representation.id
+_ihm_model_representation.name
+_ihm_model_representation.details
+1 "rep A" "rep A details"
+"""
+        for fh in cif_file_handles(cif):
+            s, = ihm.reader.read(fh)
+            r1, = s.orphan_representations
+            self.assertEqual(len(r1), 0) # no segments read yet
+            self.assertEqual(r1.name, 'rep A')
+            self.assertEqual(r1.details, 'rep A details')
+
+    def test_model_representation_details_handler(self):
+        """Test ModelRepresentationDetailsHandler"""
+        cif = """
+loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+1 1 1 6
+2 1 7 20
+#
+loop_
+_ihm_model_representation_details.id
+_ihm_model_representation_details.representation_id
+_ihm_model_representation_details.entity_id
+_ihm_model_representation_details.entity_description
+_ihm_model_representation_details.entity_asym_id
+_ihm_model_representation_details.entity_poly_segment_id
+_ihm_model_representation_details.model_object_primitive
+_ihm_model_representation_details.starting_model_id
+_ihm_model_representation_details.model_mode
+_ihm_model_representation_details.model_granularity
+_ihm_model_representation_details.model_object_count
+1 1 1 Nup84 A 1 sphere . flexible by-feature 1
+2 1 1 Nup84 A 2 sphere 1 rigid by-residue .
+3 2 1 Nup84 A . atomistic . flexible by-atom .
+4 3 2 Nup85 B . sphere . . multi-residue .
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             r1, r2, r3 = s.orphan_representations
             self.assertEqual(len(r1), 2)
             s1, s2 = r1
             self.assertEqual(s1.__class__, ihm.representation.FeatureSegment)
@@ -878,26 +928,32 @@
             self.assertEqual(s1.__class__,
                              ihm.representation.MultiResidueSegment)
 
     def test_starting_model_details_handler(self):
         """Test StartingModelDetailsHandler"""
         cif = """
 loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+1 1 7 483
+#
+loop_
 _ihm_starting_model_details.starting_model_id
 _ihm_starting_model_details.entity_id
 _ihm_starting_model_details.entity_description
 _ihm_starting_model_details.asym_id
-_ihm_starting_model_details.seq_id_begin
-_ihm_starting_model_details.seq_id_end
+_ihm_starting_model_details.entity_poly_segment_id
 _ihm_starting_model_details.starting_model_source
 _ihm_starting_model_details.starting_model_auth_asym_id
 _ihm_starting_model_details.starting_model_sequence_offset
 _ihm_starting_model_details.dataset_list_id
-1 1 Nup84 A 7 483 'comparative model' Q 8 4
-2 1 Nup84 A . . 'comparative model' X . 6
+1 1 Nup84 A 1 'comparative model' Q 8 4
+2 1 Nup84 A . 'comparative model' X . 6
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             m1, m2 = s.orphan_starting_models
             self.assertEqual(m1.asym_unit._id, 'A')
             self.assertEqual(m1.asym_unit.seq_id_range, (7,483))
             self.assertEqual(m1.asym_id, 'Q')
@@ -927,15 +983,15 @@
             self.assertIsNone(m2.script_file)
             self.assertIsNone(m2.software)
 
     def test_starting_comparative_models_handler(self):
         """Test StartingComparativeModelsHandler"""
         cif = """
 loop_
-_ihm_starting_comparative_models.ordinal_id
+_ihm_starting_comparative_models.id
 _ihm_starting_comparative_models.starting_model_id
 _ihm_starting_comparative_models.starting_model_auth_asym_id
 _ihm_starting_comparative_models.starting_model_seq_id_begin
 _ihm_starting_comparative_models.starting_model_seq_id_end
 _ihm_starting_comparative_models.template_auth_asym_id
 _ihm_starting_comparative_models.template_seq_id_begin
 _ihm_starting_comparative_models.template_seq_id_end
@@ -959,37 +1015,51 @@
             self.assertEqual(t1.alignment_file._id, '2')
             self.assertIsNone(t2.alignment_file)
 
     def test_protocol_handler(self):
         """Test ProtocolHandler"""
         cif = """
 loop_
-_ihm_modeling_protocol.ordinal_id
-_ihm_modeling_protocol.protocol_id
-_ihm_modeling_protocol.step_id
-_ihm_modeling_protocol.struct_assembly_id
-_ihm_modeling_protocol.dataset_group_id
-_ihm_modeling_protocol.struct_assembly_description
+_ihm_modeling_protocol.id
 _ihm_modeling_protocol.protocol_name
-_ihm_modeling_protocol.step_name
-_ihm_modeling_protocol.step_method
-_ihm_modeling_protocol.num_models_begin
-_ihm_modeling_protocol.num_models_end
-_ihm_modeling_protocol.multi_scale_flag
-_ihm_modeling_protocol.multi_state_flag
-_ihm_modeling_protocol.ordered_flag
-_ihm_modeling_protocol.software_id
-_ihm_modeling_protocol.script_file_id
-1 1 1 1 1 . Prot1 Sampling 'Monte Carlo' 0 500 YES NO NO . .
-2 1 2 1 2 . Prot1 Sampling 'Monte Carlo' 500 5000 YES . NO 401 501
+_ihm_modeling_protocol.num_steps
+1 Prot1 5
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             p1, = s.orphan_protocols
             self.assertEqual(p1.name, "Prot1")
+            # no step objects read yet, num_steps ignored
+            self.assertEqual(len(p1.steps), 0)
+
+    def test_protocol_details_handler(self):
+        """Test ProtocolDetailsHandler"""
+        cif = """
+loop_
+_ihm_modeling_protocol_details.id
+_ihm_modeling_protocol_details.protocol_id
+_ihm_modeling_protocol_details.step_id
+_ihm_modeling_protocol_details.struct_assembly_id
+_ihm_modeling_protocol_details.dataset_group_id
+_ihm_modeling_protocol_details.struct_assembly_description
+_ihm_modeling_protocol_details.step_name
+_ihm_modeling_protocol_details.step_method
+_ihm_modeling_protocol_details.num_models_begin
+_ihm_modeling_protocol_details.num_models_end
+_ihm_modeling_protocol_details.multi_scale_flag
+_ihm_modeling_protocol_details.multi_state_flag
+_ihm_modeling_protocol_details.ordered_flag
+_ihm_modeling_protocol_details.software_id
+_ihm_modeling_protocol_details.script_file_id
+1 1 1 1 1 . Sampling 'Monte Carlo' 0 500 YES NO NO . .
+2 1 2 1 2 . Sampling 'Monte Carlo' 500 5000 YES . NO 401 501
+"""
+        for fh in cif_file_handles(cif):
+            s, = ihm.reader.read(fh)
+            p1, = s.orphan_protocols
             self.assertEqual(len(p1.steps), 2)
             self.assertEqual(p1.steps[0]._id, '1')
             self.assertEqual(p1.steps[0].assembly._id, '1')
             self.assertEqual(p1.steps[0].dataset_group._id, '1')
             self.assertEqual(p1.steps[0].name, 'Sampling')
             self.assertEqual(p1.steps[0].method, 'Monte Carlo')
             self.assertEqual(p1.steps[0].num_models_begin, 0)
@@ -1051,27 +1121,37 @@
             self.assertEqual(len(a1.steps), 1)
             self.assertEqual(a1.steps[0].__class__, ihm.analysis.EmptyStep)
             self.assertEqual(a1.steps[0].feature, 'none')
             self.assertIsNone(a1.steps[0].num_models_begin)
             self.assertIsNone(a1.steps[0].num_models_end)
 
     def test_model_list_handler(self):
-        """Test ModelListHandler"""
+        """Test ModelListHandler and ModelGroupHandler"""
         cif = """
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 'Best scoring model' 'Cluster 1' 1 2 3
-2 2 2 'Best scoring model' 'Cluster 2' 1 1 1
+1 'Best scoring model' 1 2 3
+2 'Best scoring model' 1 1 1
+#
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 "Cluster 1" .
+2 "Cluster 2" .
+#
+loop_
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
+2 2
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             sg, = s.state_groups
             state, = sg
             self.assertIsNone(state.name) # auto-created state
             mg1, mg2 = state
@@ -1085,42 +1165,54 @@
             self.assertEqual(m.representation._id, '3')
             self.assertEqual(mg2.name, 'Cluster 2')
             self.assertEqual(mg2._id, '2')
             m, = mg2
             self.assertEqual(m._id, '2')
 
     def test_multi_state_handler(self):
-        """Test MultiStateHandler"""
+        """Test MultiStateHandler and MultiStateLinkHandler"""
         cif = """
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 'Best scoring model' 'Cluster 1' 1 2 3
+1 'Best scoring model' 1 2 3
 #
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 "Cluster 1" .
+#
+loop_
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
 #
 loop_
-_ihm_multi_state_modeling.ordinal_id
 _ihm_multi_state_modeling.state_id
 _ihm_multi_state_modeling.state_group_id
 _ihm_multi_state_modeling.population_fraction
 _ihm_multi_state_modeling.state_type
 _ihm_multi_state_modeling.state_name
-_ihm_multi_state_modeling.model_group_id
 _ihm_multi_state_modeling.experiment_type
 _ihm_multi_state_modeling.details
-1 1 1 0.4 'complex formation' 'unbound' 1  'Fraction of bulk'  'unbound molecule 1'
-2 2 1 .  'complex formation' 'unbound' 2  'Fraction of bulk'  'unbound molecule 2'
-3 3 1 .  'complex formation' 'bound'   3  'Fraction of bulk'  'bound molecules 1 and 2'
-4 3 1 .  'complex formation' 'bound'   4  'Fraction of bulk'  'bound molecules 1 and 2'
+1 1 0.4 'complex formation' 'unbound' 'Fraction of bulk'  'unbound molecule 1'
+2 1 .  'complex formation' 'unbound' 'Fraction of bulk'  'unbound molecule 2'
+3 1 .  'complex formation' 'bound' 'Fraction of bulk'  'bound molecules 1 and 2'
+#
+loop_
+_ihm_multi_state_model_group_link.state_id
+_ihm_multi_state_model_group_link.model_group_id
+1 1
+2 2
+3 3
+3 4
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             sg, = s.state_groups
             s1, s2, s3, = sg
             self.assertAlmostEqual(s1.population_fraction, 0.4, places=1)
             self.assertEqual(s1.type, 'complex formation')
@@ -1163,23 +1255,29 @@
             self.assertAlmostEqual(e.precision, 15.4, places=1)
             self.assertEqual(e.file._id, '9')
 
     def test_density_handler(self):
         """Test DensityHandler"""
         cif = """
 loop_
+_ihm_entity_poly_segment.id
+_ihm_entity_poly_segment.entity_id
+_ihm_entity_poly_segment.seq_id_begin
+_ihm_entity_poly_segment.seq_id_end
+1 1 1 726
+#
+loop_
 _ihm_localization_density_files.id
 _ihm_localization_density_files.file_id
 _ihm_localization_density_files.ensemble_id
 _ihm_localization_density_files.entity_id
 _ihm_localization_density_files.asym_id
-_ihm_localization_density_files.seq_id_begin
-_ihm_localization_density_files.seq_id_end
-1 22 9 1 A 1 726
-2 23 9 2 B . .
+_ihm_localization_density_files.entity_poly_segment_id
+1 22 9 1 A 1
+2 23 9 2 B .
 """
         for fh in cif_file_handles(cif):
             s, = ihm.reader.read(fh)
             e, = s.ensembles
             self.assertEqual(e._id, '9')
             d1, d2 = e.densities
             self.assertEqual(d1._id, '1')
@@ -1189,15 +1287,15 @@
             self.assertEqual(d2._id, '2')
             self.assertEqual(d2.asym_unit.__class__, ihm.AsymUnit)
 
     def test_em3d_restraint_handler(self):
         """Test EM3DRestraintHandler"""
         fh = StringIO("""
 loop_
-_ihm_3dem_restraint.ordinal_id
+_ihm_3dem_restraint.id
 _ihm_3dem_restraint.dataset_list_id
 _ihm_3dem_restraint.fitting_method
 _ihm_3dem_restraint.fitting_method_citation_id
 _ihm_3dem_restraint.struct_assembly_id
 _ihm_3dem_restraint.number_of_gaussians
 _ihm_3dem_restraint.model_id
 _ihm_3dem_restraint.cross_correlation_coefficient
@@ -1322,15 +1420,15 @@
 _ihm_2dem_class_average_restraint.image_segment_flag
 _ihm_2dem_class_average_restraint.number_of_projections
 _ihm_2dem_class_average_restraint.struct_assembly_id
 _ihm_2dem_class_average_restraint.details
 1 65 800 2.030 4.030 35.000 NO 10000 42 .
 #
 loop_
-_ihm_2dem_class_average_fitting.ordinal_id
+_ihm_2dem_class_average_fitting.id
 _ihm_2dem_class_average_fitting.restraint_id
 _ihm_2dem_class_average_fitting.model_id
 _ihm_2dem_class_average_fitting.cross_correlation_coefficient
 _ihm_2dem_class_average_fitting.rot_matrix[1][1]
 _ihm_2dem_class_average_fitting.rot_matrix[2][1]
 _ihm_2dem_class_average_fitting.rot_matrix[3][1]
 _ihm_2dem_class_average_fitting.rot_matrix[1][2]
@@ -1364,15 +1462,15 @@
         self.assertAlmostEqual(fit[1].rot_matrix[1][2], 0.988628, places=2)
         self.assertEqual([int(x) for x in fit[1].tr_vector], [327, 83, -227])
 
     def test_sas_restraint_handler(self):
         """Test SASRestraintHandler"""
         fh = StringIO("""
 loop_
-_ihm_sas_restraint.ordinal_id
+_ihm_sas_restraint.id
 _ihm_sas_restraint.dataset_list_id
 _ihm_sas_restraint.model_id
 _ihm_sas_restraint.struct_assembly_id
 _ihm_sas_restraint.profile_segment_flag
 _ihm_sas_restraint.fitting_atom_type
 _ihm_sas_restraint.fitting_method
 _ihm_sas_restraint.fitting_state
@@ -1399,26 +1497,34 @@
         class MyModel(ihm.model.Model):
             def add_sphere(self, sphere):
                 super(MyModel, self).add_sphere(sphere)
                 self.sphere_count = len(self._spheres)
 
         fh = StringIO("""
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 . 'Cluster 1' 1 1 1
+1 . 1 1 1
+#
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 "Cluster 1" .
 #
 loop_
-_ihm_sphere_obj_site.ordinal_id
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
+#
+loop_
+_ihm_sphere_obj_site.id
 _ihm_sphere_obj_site.entity_id
 _ihm_sphere_obj_site.seq_id_begin
 _ihm_sphere_obj_site.seq_id_end
 _ihm_sphere_obj_site.asym_id
 _ihm_sphere_obj_site.Cartn_x
 _ihm_sphere_obj_site.Cartn_y
 _ihm_sphere_obj_site.Cartn_z
@@ -1441,23 +1547,31 @@
         self.assertIsNone(s1.rmsf)
         self.assertAlmostEqual(s2.rmsf, 1.34, places=1)
 
     def test_atom_site_handler(self):
         """Test AtomSiteHandler"""
         fh = StringIO("""
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 . 'Cluster 1' 1 1 1
+1 . 1 1 1
+#
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 "Cluster 1" .
+#
+loop_
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
 #
 loop_
 _atom_site.group_PDB
 _atom_site.id
 _atom_site.type_symbol
 _atom_site.label_atom_id
 _atom_site.label_alt_id
@@ -1495,23 +1609,31 @@
         self.assertEqual(a2.het, True)
         self.assertAlmostEqual(a2.biso, 42.0, places=0)
 
     def test_atom_site_handler_auth_seq_id(self):
         """Test AtomSiteHandler handling of auth_seq_id"""
         fh = StringIO(ASYM_ENTITY + """
 loop_
-_ihm_model_list.ordinal_id
 _ihm_model_list.model_id
-_ihm_model_list.model_group_id
 _ihm_model_list.model_name
-_ihm_model_list.model_group_name
 _ihm_model_list.assembly_id
 _ihm_model_list.protocol_id
 _ihm_model_list.representation_id
-1 1 1 . 'Cluster 1' 1 1 1
+1 . 1 1 1
+#
+loop_
+_ihm_model_group.id
+_ihm_model_group.name
+_ihm_model_group.details
+1 "Cluster 1" .
+#
+loop_
+_ihm_model_group_link.group_id
+_ihm_model_group_link.model_id
+1 1
 #
 loop_
 _atom_site.group_PDB
 _atom_site.id
 _atom_site.type_symbol
 _atom_site.label_atom_id
 _atom_site.label_alt_id
@@ -2205,15 +2327,15 @@
 _ihm_cross_link_restraint.sigma_1
 _ihm_cross_link_restraint.sigma_2
 1 1 1 A 2 THR 1 B 3 CYS . . 'upper bound' ALL by-residue 25.000 0.500 1.000
 2.000
 """
         xl_fit = """
 loop_
-_ihm_cross_link_result_parameters.ordinal_id
+_ihm_cross_link_result_parameters.id
 _ihm_cross_link_result_parameters.restraint_id
 _ihm_cross_link_result_parameters.model_id
 _ihm_cross_link_result_parameters.psi
 _ihm_cross_link_result_parameters.sigma_1
 _ihm_cross_link_result_parameters.sigma_2
 1 1 201 0.100 4.200 2.100
 2 1 301 . . .
@@ -2348,20 +2470,20 @@
 loop_
 _ihm_predicted_contact_restraint.id
 _ihm_predicted_contact_restraint.group_id
 _ihm_predicted_contact_restraint.entity_id_1
 _ihm_predicted_contact_restraint.asym_id_1
 _ihm_predicted_contact_restraint.comp_id_1
 _ihm_predicted_contact_restraint.seq_id_1
-_ihm_predicted_contact_restraint.atom_id_1
+_ihm_predicted_contact_restraint.rep_atom_1
 _ihm_predicted_contact_restraint.entity_id_2
 _ihm_predicted_contact_restraint.asym_id_2
 _ihm_predicted_contact_restraint.comp_id_2
 _ihm_predicted_contact_restraint.seq_id_2
-_ihm_predicted_contact_restraint.atom_id_2
+_ihm_predicted_contact_restraint.rep_atom_2
 _ihm_predicted_contact_restraint.restraint_type
 _ihm_predicted_contact_restraint.distance_lower_limit
 _ihm_predicted_contact_restraint.distance_upper_limit
 _ihm_predicted_contact_restraint.probability
 _ihm_predicted_contact_restraint.model_granularity
 _ihm_predicted_contact_restraint.dataset_list_id
 _ihm_predicted_contact_restraint.software_id
```

### Comparing `ihm-0.8/test/test_representation.py` & `ihm-0.9/test/test_representation.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_restraint.py` & `ihm-0.9/test/test_restraint.py`

 * *Files identical despite different names*

### Comparing `ihm-0.8/test/test_startmodel.py` & `ihm-0.9/test/test_startmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         self.assertEqual(p.length, 18)
 
     def test_starting_model(self):
         """Test StartingModel class, no templates"""
         e1 = ihm.Entity('AAAA')
         asym = ihm.AsymUnit(e1)
         s = ihm.startmodel.StartingModel(asym, 'mock_dataset', 'A', offset=10)
-        self.assertEqual(s._get_seq_id_range_all_templates(), (1,4))
+        r = s._get_seq_id_range_all_templates()
+        self.assertEqual(r.seq_id_range, (1,4))
         self.assertEqual(s.get_atoms(), [])
         self.assertEqual(s.get_seq_dif(), [])
 
     def test_starting_model_templates(self):
         """Test StartingModel class, with templates"""
         e1 = ihm.Entity('A' * 30)
         asym = ihm.AsymUnit(e1)
@@ -53,15 +54,16 @@
         # This should extend the range to 20
         s2 = ihm.startmodel.Template(dataset='2xyz', asym_id='D',
                              seq_id_range=(14, 19), # 15,20 in IHM numbering
                              template_seq_id_range=(115,120),
                              sequence_identity=40.)
         s = ihm.startmodel.StartingModel(asym(5,25), 'mock_dataset', 'A',
                                          [s1, s2], offset=1)
-        self.assertEqual(s._get_seq_id_range_all_templates(), (5,20))
+        self.assertEqual(s._get_seq_id_range_all_templates().seq_id_range,
+                         (5,20))
 
     def test_seq_dif(self):
         """Test SeqDif class"""
         sd = ihm.startmodel.SeqDif(db_seq_id=10, seq_id=20, db_comp_id='PHE')
         self.assertEqual(sd.db_seq_id, 10)
 
     def test_mse_seq_dif(self):
```

### Comparing `ihm-0.8/test/test_util.py` & `ihm-0.9/test/test_util.py`

 * *Files identical despite different names*

