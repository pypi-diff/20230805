# Comparing `tmp/cellmaps_utils-0.1.0a7.tar.gz` & `tmp/cellmaps_utils-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_utils-0.1.0a7.tar", last modified: Thu May 11 22:07:40 2023, max compression
+gzip compressed data, was "dist/cellmaps_utils-0.1.0a8.tar", last modified: Fri May 12 22:41:39 2023, max compression
```

## Comparing `cellmaps_utils-0.1.0a7.tar` & `cellmaps_utils-0.1.0a8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.431299 cellmaps_utils-0.1.0a7/
--rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a7/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a7/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 22:07:40.431436 cellmaps_utils-0.1.0a7/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a7/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.422410 cellmaps_utils-0.1.0a7/cellmaps_utils/
--rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-11 22:06:22.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     3858 2023-05-11 18:35:27.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/constants.py
--rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/logutils.py
--rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/music_utils.py
--rw-r--r--   0 churas     (504) staff       (20)    12991 2023-05-11 21:55:18.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/provenance.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.423871 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       60 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.429479 cellmaps_utils-0.1.0a7/docs/
--rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.417825 cellmaps_utils-0.1.0a7/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.417893 cellmaps_utils-0.1.0a7/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.430283 cellmaps_utils-0.1.0a7/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a7/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a7/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a7/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a7/docs/cellmaps_utils.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a7/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-11 22:07:40.432051 cellmaps_utils-0.1.0a7/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1796 2023-05-11 20:55:28.000000 cellmaps_utils-0.1.0a7/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.431040 cellmaps_utils-0.1.0a7/tests/
--rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a7/tests/test_logutils.py
--rw-r--r--   0 churas     (504) staff       (20)     7029 2023-05-11 21:02:45.000000 cellmaps_utils-0.1.0a7/tests/test_provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.931318 cellmaps_utils-0.1.0a8/
+-rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a8/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a8/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-12 22:41:39.931465 cellmaps_utils-0.1.0a8/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a8/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.923452 cellmaps_utils-0.1.0a8/cellmaps_utils/
+-rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-12 20:32:13.000000 cellmaps_utils-0.1.0a8/cellmaps_utils/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     3995 2023-05-12 18:00:09.000000 cellmaps_utils-0.1.0a8/cellmaps_utils/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a8/cellmaps_utils/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a8/cellmaps_utils/logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a8/cellmaps_utils/music_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)    15018 2023-05-12 21:25:57.000000 cellmaps_utils-0.1.0a8/cellmaps_utils/provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.925178 cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-12 22:41:39.000000 cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-12 22:41:39.000000 cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-12 22:41:39.000000 cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-12 22:41:39.000000 cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       60 2023-05-12 22:41:39.000000 cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-12 22:41:39.000000 cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.929559 cellmaps_utils-0.1.0a8/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.919083 cellmaps_utils-0.1.0a8/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.919226 cellmaps_utils-0.1.0a8/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.930313 cellmaps_utils-0.1.0a8/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a8/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a8/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a8/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a8/docs/cellmaps_utils.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a8/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-12 22:41:39.931980 cellmaps_utils-0.1.0a8/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1796 2023-05-11 20:55:28.000000 cellmaps_utils-0.1.0a8/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-12 22:41:39.931092 cellmaps_utils-0.1.0a8/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a8/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a8/tests/test_logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     8343 2023-05-12 20:32:39.000000 cellmaps_utils-0.1.0a8/tests/test_provenance.py
```

### Comparing `cellmaps_utils-0.1.0a7/CONTRIBUTING.rst` & `cellmaps_utils-0.1.0a8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/LICENSE` & `cellmaps_utils-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/PKG-INFO` & `cellmaps_utils-0.1.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_utils
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a7/README.rst` & `cellmaps_utils-0.1.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/cellmaps_utils/constants.py` & `cellmaps_utils-0.1.0a8/cellmaps_utils/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
 LOG_FORMAT = "%(asctime)-15s %(levelname)s %(relativeCreated)dms " \
              "%(filename)s::%(funcName)s():%(lineno)d %(message)s"
 """
 Sets format of logging messages
 """
 
+RO_CRATE_METADATA_FILE = 'ro-crate-metadata.json'
+"""
+`rocrate <https://www.researchobject.org/ro-crate>`__ metadata JSON file name
+"""
+
 TASK_FILE_PREFIX = 'task_'
 """
 Prefix for task file
 """
 
 TASK_START_FILE_SUFFIX = '_start.json'
 """
```

### Comparing `cellmaps_utils-0.1.0a7/cellmaps_utils/logutils.py` & `cellmaps_utils-0.1.0a8/cellmaps_utils/logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/cellmaps_utils/music_utils.py` & `cellmaps_utils-0.1.0a8/cellmaps_utils/music_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/cellmaps_utils/provenance.py` & `cellmaps_utils-0.1.0a8/cellmaps_utils/provenance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 import os
 import subprocess
 import logging
 import uuid
 from datetime import date
+import json
 
+from cellmaps_utils import constants
 from cellmaps_utils.exceptions import CellMapsProvenanceError
 logger = logging.getLogger(__name__)
 
 
 class ProvenanceUtil(object):
     """
     Wrapper around `FAIRSCAPE <https://fairscape.github.io>`__ calls
@@ -77,14 +79,77 @@
             field_dict.update({'url': 'URL of datset',
                                'used-by': '?',
                                'derived-from': '?',
                                'associated-publication': '?',
                                'additional-documentation': '?'})
         return field_dict
 
+    def get_rocrate_as_dict(self, rocrate_path):
+        """
+        Loads rocrate as a dict
+
+        :param rocrate_path: Directory containing `ro-crate-metadata.json` file or
+                             path to file assumed to be ro-crate meta data file
+        :type rocrate_path: str
+        :return:
+        """
+        if rocrate_path is None:
+            raise CellMapsProvenanceError('rocrate_path is None')
+
+        if os.path.isdir(rocrate_path):
+            rocrate_file = os.path.join(rocrate_path, constants.RO_CRATE_METADATA_FILE)
+        else:
+            rocrate_file = rocrate_path
+
+        try:
+            with open(rocrate_file, 'r') as f:
+                data = json.load(f)
+            return data
+        except Exception as e:
+            raise CellMapsProvenanceError('Error parsing ' + str(rocrate_file) +
+                                          ' ' + str(e))
+
+    def get_id_of_rocrate(self, rocrate):
+        """
+        Gets id of rocrate
+
+        :param rocrate:
+        :return:
+        """
+        if isinstance(rocrate, dict):
+            data = rocrate
+        else:
+            data = self.get_rocrate_as_dict(rocrate)
+        return data['@id']
+
+    def get_name_project_org_of_rocrate(self, rocrate):
+        """
+        Gets name, project, and organization name of rocrate
+
+        :param rocrate:
+        :type rocrate: str or dict
+        :return: (name, project, organization-name)
+        :rtype: tuple
+        """
+        if isinstance(rocrate, dict):
+            data = rocrate
+        else:
+            data = self.get_rocrate_as_dict(rocrate)
+
+        name = data['name']
+        org_name = None
+        proj_name = None
+        for entry in data['isPartOf']:
+            if '@type' in entry:
+                if entry['@type'] == 'Organization':
+                    org_name = entry['name']
+                elif entry['@type'] == 'Project':
+                    proj_name = entry['name']
+        return name, proj_name, org_name
+
     def register_rocrate(self, rocrate_path, name='',
                          organization_name='', project_name='',
                          guid=None):
         """
         Creates/registers rocreate in directory specified by **rocrate_path**
         Upon completion a ``ro-crate-metadata.json`` file will be created
         in the directory
```

### Comparing `cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/PKG-INFO` & `cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-utils
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/SOURCES.txt` & `cellmaps_utils-0.1.0a8/cellmaps_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/Makefile` & `cellmaps_utils-0.1.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/cellmaps_utils.rst` & `cellmaps_utils-0.1.0a8/docs/cellmaps_utils.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/conf.py` & `cellmaps_utils-0.1.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/index.rst` & `cellmaps_utils-0.1.0a8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/installation.rst` & `cellmaps_utils-0.1.0a8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/make.bat` & `cellmaps_utils-0.1.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/newrelease.rst` & `cellmaps_utils-0.1.0a8/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/pypircfile.rst` & `cellmaps_utils-0.1.0a8/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/docs/versioningscheme.rst` & `cellmaps_utils-0.1.0a8/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/setup.py` & `cellmaps_utils-0.1.0a8/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/tests/test_logutils.py` & `cellmaps_utils-0.1.0a8/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a7/tests/test_provenance.py` & `cellmaps_utils-0.1.0a8/tests/test_provenance.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 """Tests for `cellmaps_utils.cellmaps_io` package."""
 
 import os
 import sys
 import shutil
 import tempfile
+import json
 from datetime import date
 import unittest
 from unittest.mock import patch
 
+from cellmaps_utils import constants
 from cellmaps_utils.provenance import ProvenanceUtil
 from cellmaps_utils.exceptions import CellMapsProvenanceError
 
 
 class TestProvenanceUtil(unittest.TestCase):
     """Tests for `cellmaps_utils` package."""
 
@@ -66,26 +68,25 @@
                           'additional-documentation': '?'}
         self.assertEqual(expected_full, example)
 
         # with required only None
         example = ProvenanceUtil.example_dataset_provenance(requiredonly=None)
         self.assertEqual(expected_full, example)
 
-
     def test_register_rocrate_actual_invocation(self):
         """
         Registers temp directory as a crate
         with all default values
         :return:
         """
         temp_dir = tempfile.mkdtemp()
         try:
             prov = ProvenanceUtil()
             prov.register_rocrate(temp_dir)
-            crate_file = os.path.join(temp_dir, 'ro-crate-metadata.json')
+            crate_file = os.path.join(temp_dir, constants.RO_CRATE_METADATA_FILE)
             self.assertTrue(os.path.isfile(crate_file))
             self.assertTrue(os.path.getsize(crate_file) > 0)
         finally:
             shutil.rmtree(temp_dir)
 
     def test_register_computation_actual_invocation(self):
         temp_dir = tempfile.mkdtemp()
@@ -119,15 +120,15 @@
                                              used_dataset=used_dataset,
                                              used_software=used_software,
                                              generated=generated)
             self.assertTrue(len(c_id) > 0)
         finally:
             shutil.rmtree(temp_dir)
 
-    def test_register_software_actual_invocation(self):
+    def test_register_software(self):
         # Todo: due to fairscape-cli bug this is failing
         #       and the test expects the failure for now
         #       once fairscape-cli fixes
         #       https://github.com/fairscape/fairscape-cli/issues/7
         #       remove the exception check
         temp_dir = tempfile.mkdtemp()
         try:
@@ -138,15 +139,15 @@
                                           url='http://foo.com')
             # this is never reached due to
             # https://github.com/fairscape/fairscape-cli/issues/7
             self.assertTrue(len(s_id) > 0)
         finally:
             shutil.rmtree(temp_dir)
 
-    def test_register_dataset_actual_invocation(self):
+    def test_register_dataset(self):
 
         temp_dir = tempfile.mkdtemp()
         try:
             subdir = os.path.join(temp_dir, 'input')
             os.makedirs(subdir, mode=0o755)
             src_file = os.path.join(subdir, 'xx')
             with open(src_file, 'w') as f:
@@ -160,14 +161,43 @@
                                          data_dict={'name': 'Name of dataset',
                                                     'author': 'Author of dataset',
                                                     'version': 'Version of dataset',
                                                     'date-published': 'Date dataset was published MM-DD-YYYY',
                                                     'description': 'Description of dataset',
                                                     'data-format': 'Format of data'})
             self.assertTrue(len(d_id) > 0)
+
+        except CellMapsProvenanceError as ce:
+            print(str(ce))
+            self.assertEqual('', str(ce))
+            self.assertTrue('Error adding dataset' in str(ce))
+        finally:
+            shutil.rmtree(temp_dir)
+
+    def test_register_dataset_skipcopy_true(self):
+
+        temp_dir = tempfile.mkdtemp()
+        try:
+            src_file = os.path.join(temp_dir, 'xx')
+            with open(src_file, 'w') as f:
+                f.write('hi')
+
+            prov = ProvenanceUtil()
+            prov.register_rocrate(temp_dir)
+            d_id = prov.register_dataset(temp_dir,
+                                         source_file=src_file,
+                                         skip_copy=True,
+                                         data_dict={'name': 'Name of dataset',
+                                                    'author': 'Author of dataset',
+                                                    'version': 'Version of dataset',
+                                                    'date-published': 'Date dataset was published MM-DD-YYYY',
+                                                    'description': 'Description of dataset',
+                                                    'data-format': 'Format of data'})
+            self.assertTrue(len(d_id) > 0)
+
         except CellMapsProvenanceError as ce:
             print(str(ce))
             self.assertEqual('', str(ce))
             self.assertTrue('Error adding dataset' in str(ce))
         finally:
             shutil.rmtree(temp_dir)
```

