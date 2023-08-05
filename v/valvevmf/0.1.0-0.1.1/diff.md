# Comparing `tmp/valvevmf-0.1.0.tar.gz` & `tmp/valvevmf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valvevmf-0.1.0.tar", last modified: Thu Dec 30 10:17:23 2021, max compression
+gzip compressed data, was "valvevmf-0.1.1.tar", last modified: Sat Aug  5 03:27:26 2023, max compression
```

## Comparing `valvevmf-0.1.0.tar` & `valvevmf-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-12-30 10:17:23.668918 valvevmf-0.1.0/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      970 2021-12-30 10:17:23.668918 valvevmf-0.1.0/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       39 2021-12-16 13:29:08.262350 valvevmf-0.1.0/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1104 2021-12-30 10:16:15.761329 valvevmf-0.1.0/setup.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2021-12-30 10:17:23.668918 valvevmf-0.1.0/valvevmf/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      284 2021-12-30 09:17:02.489380 valvevmf-0.1.0/valvevmf/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1758 2021-12-30 09:54:16.212829 valvevmf-0.1.0/valvevmf/node.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2960 2021-12-29 04:14:58.674308 valvevmf-0.1.0/valvevmf/parser.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     3644 2021-12-29 03:52:53.165569 valvevmf-0.1.0/valvevmf/property_parser.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1973 2021-12-30 07:44:38.772536 valvevmf-0.1.0/valvevmf/property_writer.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1466 2021-12-30 09:51:26.909181 valvevmf-0.1.0/valvevmf/vmf.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      372 2021-12-16 13:37:59.033000 valvevmf-0.1.0/valvevmf/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:27:26.504578 valvevmf-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 03:27:18.000000 valvevmf-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-05 03:27:26.504578 valvevmf-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-05 03:27:18.000000 valvevmf-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 03:27:26.504578 valvevmf-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-05 03:27:25.000000 valvevmf-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:27:26.504578 valvevmf-0.1.1/valvevmf/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-05 03:27:18.000000 valvevmf-0.1.1/valvevmf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-08-05 03:27:18.000000 valvevmf-0.1.1/valvevmf/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-08-05 03:27:18.000000 valvevmf-0.1.1/valvevmf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-05 03:27:18.000000 valvevmf-0.1.1/valvevmf/property_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-05 03:27:18.000000 valvevmf-0.1.1/valvevmf/property_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-05 03:27:18.000000 valvevmf-0.1.1/valvevmf/vmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-05 03:27:18.000000 valvevmf-0.1.1/valvevmf/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:27:26.504578 valvevmf-0.1.1/valvevmf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-05 03:27:26.000000 valvevmf-0.1.1/valvevmf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-05 03:27:26.000000 valvevmf-0.1.1/valvevmf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:27:26.000000 valvevmf-0.1.1/valvevmf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 03:27:26.000000 valvevmf-0.1.1/valvevmf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 03:27:26.000000 valvevmf-0.1.1/valvevmf.egg-info/top_level.txt
```

### Comparing `valvevmf-0.1.0/valvevmf/parser.py` & `valvevmf-0.1.1/valvevmf/parser.py`

 * *Files identical despite different names*

### Comparing `valvevmf-0.1.0/valvevmf/property_parser.py` & `valvevmf-0.1.1/valvevmf/property_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     return [tuple(data.asList()[0])]
 
 
 # Property parsing
 pp_bool = Word(nums+'-').setParseAction(lambda p: bool(int(p[0])))
 pp_int = Word(nums+'-').setParseAction(lambda p: int(p[0]))
 pp_uint8 = Word(nums).setParseAction(lambda p: min(255, max(0, int(p[0]))))
-pp_float = Word(nums+'-.').setParseAction(lambda p: Decimal(p[0]))
+pp_float = Word(nums+'-.e').setParseAction(lambda p: Decimal(p[0]))
 
 pp_angle = Group(pp_float + pp_float + pp_float).setParseAction(asTuple)
 pp_origin = pp_angle
 
 pp_vertex_content = Group(pp_float + pp_float +
                           pp_float).setParseAction(asTuple)
 pp_vertex_tup = Suppress('(') + pp_vertex_content + Suppress(')')
```

### Comparing `valvevmf-0.1.0/valvevmf/property_writer.py` & `valvevmf-0.1.1/valvevmf/property_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from decimal import Decimal
 
 
 def _repr_prop_value(val, wrapper=None):
     vstr = val
     if isinstance(val, str):
         vstr = val
-    elif isinstance(val, Decimal):
+    elif isinstance(val, Decimal) or isinstance(val, float):
         vstr = '{:.6g}'.format(val)
     elif isinstance(val, bool):
         vstr = '1' if val else '0'
     elif isinstance(val, int):
         vstr = str(val)
     elif isinstance(val, list) or isinstance(val, tuple):
         vstr = ' '.join([_repr_prop_value(c) for c in val])
```

### Comparing `valvevmf-0.1.0/valvevmf/vmf.py` & `valvevmf-0.1.1/valvevmf/vmf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
+from valvevmf.node import HoldsNodesAbstract
+from valvevmf.writer import VmfWrite
+from valvevmf.parser import VmfParse
 from builtins import object
 from builtins import super
 from future import standard_library
 standard_library.install_aliases()
 
-from valvevmf.parser import VmfParse
-from valvevmf.writer import VmfWrite
-
 
-class Vmf(object):
+class Vmf(HoldsNodesAbstract):
     """
     This is the basic class to interact with vmf files, it is mostly a collection of VmfNodes.
     """
 
     def __init__(self, path=None):
         """
         initalize a Vmf file.
@@ -23,16 +23,15 @@
         :param path: The location of the vmf file to be parsed, saved as :any:`source_path<Vmf.source_path>`.
         :type path: str, optional
         """
 
         #: :type: (str) - The location of the parsed file
         self.source_path = path
 
-        #: :type: (list[VmfNode]) - The list of nodes at the Vmf root
-        self.nodes = []
+        HoldsNodesAbstract.__init__(self, None)
 
         if self.source_path:
             self.nodes = VmfParse(self.source_path)
 
     def save(self, destination=None):
         """Saves the current instance of the Vmf. Overwrites original vmf file if no destination is provided.
```

