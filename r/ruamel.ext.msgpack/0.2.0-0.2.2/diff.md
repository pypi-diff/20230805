# Comparing `tmp/ruamel.ext.msgpack-0.2.0.tar.gz` & `tmp/ruamel.ext.msgpack-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruamel.ext.msgpack-0.2.0.tar", last modified: Sun Feb 19 09:51:11 2023, max compression
+gzip compressed data, was "ruamel.ext.msgpack-0.2.2.tar", last modified: Sat Aug  5 09:29:51 2023, max compression
```

## Comparing `ruamel.ext.msgpack-0.2.0.tar` & `ruamel.ext.msgpack-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-02-19 09:51:11.420722 ruamel.ext.msgpack-0.2.0/
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-02-19 09:51:11.419567 ruamel.ext.msgpack-0.2.0/.ruamel/
--rw-r--r--   0 anthon    (1000) users      (500)       63 2023-02-16 14:50:27.000000 ruamel.ext.msgpack-0.2.0/.ruamel/__init__.py
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-02-19 09:51:11.419682 ruamel.ext.msgpack-0.2.0/.ruamel/ext/
--rw-r--r--   0 anthon    (1000) users      (500)       63 2023-02-16 14:50:27.000000 ruamel.ext.msgpack-0.2.0/.ruamel/ext/__init__.py
--rw-r--r--   0 anthon    (1000) users      (500)     5236 2023-02-19 09:51:11.420612 ruamel.ext.msgpack-0.2.0/PKG-INFO
--rw-r--r--   0 anthon    (1000) users      (500)     4578 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/README.rst
--rw-r--r--   0 anthon    (1000) users      (500)     2827 2023-02-19 09:50:12.000000 ruamel.ext.msgpack-0.2.0/__init__.py
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-02-19 09:51:11.420463 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/
--rw-r--r--   0 anthon    (1000) users      (500)     5236 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/PKG-INFO
--rw-r--r--   0 anthon    (1000) users      (500)      382 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/SOURCES.txt
--rw-r--r--   0 anthon    (1000) users      (500)        1 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/dependency_links.txt
--rw-r--r--   0 anthon    (1000) users      (500)       61 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/entry_points.txt
--rw-r--r--   0 anthon    (1000) users      (500)       18 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/namespace_packages.txt
--rw-r--r--   0 anthon    (1000) users      (500)       15 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/requires.txt
--rw-r--r--   0 anthon    (1000) users      (500)        7 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/top_level.txt
--rw-r--r--   0 anthon    (1000) users      (500)       38 2023-02-19 09:51:11.420755 ruamel.ext.msgpack-0.2.0/setup.cfg
--rw-rw-r--   0 anthon    (1000) users      (500)    35813 2023-02-19 09:51:11.000000 ruamel.ext.msgpack-0.2.0/setup.py
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-08-05 09:29:51.918778 ruamel.ext.msgpack-0.2.2/
+-rw-r--r--   0 anthon    (1000) users      (500)     5670 2023-08-05 09:29:51.918648 ruamel.ext.msgpack-0.2.2/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)     5012 2023-08-05 09:28:52.000000 ruamel.ext.msgpack-0.2.2/README.rst
+-rw-r--r--   0 anthon    (1000) users      (500)     7315 2023-08-05 09:29:23.000000 ruamel.ext.msgpack-0.2.2/__init__.py
+-rw-r--r--   0 anthon    (1000) users      (500)       97 2023-08-05 09:29:51.000000 ruamel.ext.msgpack-0.2.2/pyproject.toml
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-08-05 09:29:51.918468 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/
+-rw-r--r--   0 anthon    (1000) users      (500)     5670 2023-08-05 09:29:51.000000 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)      343 2023-08-05 09:29:51.000000 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/SOURCES.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-08-05 09:29:51.000000 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/dependency_links.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       61 2023-08-05 09:29:51.000000 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/entry_points.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-08-05 09:29:26.000000 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/not-zip-safe
+-rw-r--r--   0 anthon    (1000) users      (500)       15 2023-08-05 09:29:51.000000 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/requires.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        7 2023-08-05 09:29:51.000000 ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/top_level.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       38 2023-08-05 09:29:51.918815 ruamel.ext.msgpack-0.2.2/setup.cfg
+-rw-rw-r--   0 anthon    (1000) users      (500)    33415 2023-08-05 04:59:28.000000 ruamel.ext.msgpack-0.2.2/setup.py
```

### Comparing `ruamel.ext.msgpack-0.2.0/PKG-INFO` & `ruamel.ext.msgpack-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.ext.msgpack
-Version: 0.2.0
+Version: 0.2.2
 Summary: thin wrapper around msgpack to deal with naive datetime and ruamel defined extension types
 Home-page: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: Copyright Ruamel bvba 2007-2023
 Keywords: pypi statistics
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,23 @@
 Description-Content-Type: text/x-rst
 
 
 ruamel.ext.msgpack
 ==================
 
 ruamel.ext.msgpack is  a thin wrapper around msgpack, that deals with naive datetime instances and ruamel defined 
-extension types (date). 
+extension types (date).
+
+.. image:: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree/_doc/_static/license.svg?format=raw
+     :target: https://opensource.org/licenses/MIT
+.. image:: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree/_doc/_static/pypi.svg?format=raw
+     :target: https://pypi.org/project/ruamel.ext.msgpack
+.. image:: https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw
+   :target: https://pypi.org/project/oitnb/
+
 
 naive datetime.datetime
 +++++++++++++++++++++++
 
 If you try to pack a naive datetime.datetime instance, you'll get an error:
 
 .. code:: python
@@ -63,15 +71,15 @@
 which will print:
 
 .. code::
 
   2011-10-02 17:15:01+00:00
 
 
-as you can see from the output this will make the instance timezone aware.
+as you can see from the output this will make the instance, that was read back, timezone aware.
 
 use_bin_type=True
 ++++++++++++++++++
 
 The ``pack`` and ``packb`` routines do not change the default ``use_bin_type=True``.
 So the UTF-8 "bytestrings" get dumped as bin 8/16/32 and not as the slightly more
 efficient "fixstr" for strings up to a length of 31 bytes.
@@ -98,15 +106,15 @@
   こんにちは世界
   \xc4\x15\xe3\x81\x93\xe3\x82\x93\xe3\x81\xab\xe3\x81\xa1\xe3\x81\xaf\xe4\xb8\x96\xe7\x95\x8c 23
   b'\xe3\x81\x93\xe3\x82\x93\xe3\x81\xab\xe3\x81\xa1\xe3\x81\xaf\xe4\xb8\x96\xe7\x95\x8c'
 
 
 If you don't need byte arrays, and want conversion done of ``bytes`` to ``str`` on msgpack-roundtrip,
 an alternate version of ``pack``/``unpack``  can be constructed,
-that still handle naive datetime objects, and the other types provided by ``ruamel.ext.msgpack``:
+that still handles naive datetime objects, and the other types provided by ``ruamel.ext.msgpack``:
 
 .. code:: python
 
 
   from functools import partial
   from ruamel.ext.msgpack import hex, unpackb, msgpack_default
   import msgpack
@@ -166,11 +174,10 @@
 which will print:
 
 .. code::
 
   hex: \xd5\x11\x17\x82 4
   2011-10-02
   msgpack_default.date=17
-  hex: \xd5\x2a\x17\x82 4
+  hex: \xd5\x11\x17\x82 4
   2011-10-02
-  exception: <class 'ValueError'> year out of range 2000-2126
```

### Comparing `ruamel.ext.msgpack-0.2.0/README.rst` & `ruamel.ext.msgpack-0.2.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 
 ruamel.ext.msgpack
 ==================
 
 ruamel.ext.msgpack is  a thin wrapper around msgpack, that deals with naive datetime instances and ruamel defined 
-extension types (date). 
+extension types (date).
+
+.. image:: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree/_doc/_static/license.svg?format=raw
+     :target: https://opensource.org/licenses/MIT
+.. image:: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree/_doc/_static/pypi.svg?format=raw
+     :target: https://pypi.org/project/ruamel.ext.msgpack
+.. image:: https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw
+   :target: https://pypi.org/project/oitnb/
+
 
 naive datetime.datetime
 +++++++++++++++++++++++
 
 If you try to pack a naive datetime.datetime instance, you'll get an error:
 
 .. code:: python
@@ -46,15 +54,15 @@
 which will print:
 
 .. code::
 
   2011-10-02 17:15:01+00:00
 
 
-as you can see from the output this will make the instance timezone aware.
+as you can see from the output this will make the instance, that was read back, timezone aware.
 
 use_bin_type=True
 ++++++++++++++++++
 
 The ``pack`` and ``packb`` routines do not change the default ``use_bin_type=True``.
 So the UTF-8 "bytestrings" get dumped as bin 8/16/32 and not as the slightly more
 efficient "fixstr" for strings up to a length of 31 bytes.
@@ -81,15 +89,15 @@
   こんにちは世界
   \xc4\x15\xe3\x81\x93\xe3\x82\x93\xe3\x81\xab\xe3\x81\xa1\xe3\x81\xaf\xe4\xb8\x96\xe7\x95\x8c 23
   b'\xe3\x81\x93\xe3\x82\x93\xe3\x81\xab\xe3\x81\xa1\xe3\x81\xaf\xe4\xb8\x96\xe7\x95\x8c'
 
 
 If you don't need byte arrays, and want conversion done of ``bytes`` to ``str`` on msgpack-roundtrip,
 an alternate version of ``pack``/``unpack``  can be constructed,
-that still handle naive datetime objects, and the other types provided by ``ruamel.ext.msgpack``:
+that still handles naive datetime objects, and the other types provided by ``ruamel.ext.msgpack``:
 
 .. code:: python
 
 
   from functools import partial
   from ruamel.ext.msgpack import hex, unpackb, msgpack_default
   import msgpack
@@ -149,11 +157,10 @@
 which will print:
 
 .. code::
 
   hex: \xd5\x11\x17\x82 4
   2011-10-02
   msgpack_default.date=17
-  hex: \xd5\x2a\x17\x82 4
+  hex: \xd5\x11\x17\x82 4
   2011-10-02
-  exception: <class 'ValueError'> year out of range 2000-2126
```

### Comparing `ruamel.ext.msgpack-0.2.0/ruamel.ext.msgpack.egg-info/PKG-INFO` & `ruamel.ext.msgpack-0.2.2/ruamel.ext.msgpack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.ext.msgpack
-Version: 0.2.0
+Version: 0.2.2
 Summary: thin wrapper around msgpack to deal with naive datetime and ruamel defined extension types
 Home-page: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: Copyright Ruamel bvba 2007-2023
 Keywords: pypi statistics
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,23 @@
 Description-Content-Type: text/x-rst
 
 
 ruamel.ext.msgpack
 ==================
 
 ruamel.ext.msgpack is  a thin wrapper around msgpack, that deals with naive datetime instances and ruamel defined 
-extension types (date). 
+extension types (date).
+
+.. image:: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree/_doc/_static/license.svg?format=raw
+     :target: https://opensource.org/licenses/MIT
+.. image:: https://sourceforge.net/p/ruamel-ext-msgpack/code/ci/default/tree/_doc/_static/pypi.svg?format=raw
+     :target: https://pypi.org/project/ruamel.ext.msgpack
+.. image:: https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw
+   :target: https://pypi.org/project/oitnb/
+
 
 naive datetime.datetime
 +++++++++++++++++++++++
 
 If you try to pack a naive datetime.datetime instance, you'll get an error:
 
 .. code:: python
@@ -63,15 +71,15 @@
 which will print:
 
 .. code::
 
   2011-10-02 17:15:01+00:00
 
 
-as you can see from the output this will make the instance timezone aware.
+as you can see from the output this will make the instance, that was read back, timezone aware.
 
 use_bin_type=True
 ++++++++++++++++++
 
 The ``pack`` and ``packb`` routines do not change the default ``use_bin_type=True``.
 So the UTF-8 "bytestrings" get dumped as bin 8/16/32 and not as the slightly more
 efficient "fixstr" for strings up to a length of 31 bytes.
@@ -98,15 +106,15 @@
   こんにちは世界
   \xc4\x15\xe3\x81\x93\xe3\x82\x93\xe3\x81\xab\xe3\x81\xa1\xe3\x81\xaf\xe4\xb8\x96\xe7\x95\x8c 23
   b'\xe3\x81\x93\xe3\x82\x93\xe3\x81\xab\xe3\x81\xa1\xe3\x81\xaf\xe4\xb8\x96\xe7\x95\x8c'
 
 
 If you don't need byte arrays, and want conversion done of ``bytes`` to ``str`` on msgpack-roundtrip,
 an alternate version of ``pack``/``unpack``  can be constructed,
-that still handle naive datetime objects, and the other types provided by ``ruamel.ext.msgpack``:
+that still handles naive datetime objects, and the other types provided by ``ruamel.ext.msgpack``:
 
 .. code:: python
 
 
   from functools import partial
   from ruamel.ext.msgpack import hex, unpackb, msgpack_default
   import msgpack
@@ -166,11 +174,10 @@
 which will print:
 
 .. code::
 
   hex: \xd5\x11\x17\x82 4
   2011-10-02
   msgpack_default.date=17
-  hex: \xd5\x2a\x17\x82 4
+  hex: \xd5\x11\x17\x82 4
   2011-10-02
-  exception: <class 'ValueError'> year out of range 2000-2126
```

### Comparing `ruamel.ext.msgpack-0.2.0/setup.py` & `ruamel.ext.msgpack-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # # header
 # coding: utf-8
-# dd: 20200903
-
-from __future__ import print_function, absolute_import, division, unicode_literals
+# dd: 20230418
 
 # # __init__.py parser
 
 import sys
 import os
 import datetime
-import traceback
+from textwrap import dedent
 
 sys.path = [path for path in sys.path if path not in [os.getcwd(), ""]]
 import platform  # NOQA
 from _ast import *  # NOQA
 from ast import parse  # NOQA
 
 from setuptools import setup, Extension, Distribution  # NOQA
 from setuptools.command import install_lib  # NOQA
 from setuptools.command.sdist import sdist as _sdist  # NOQA
 
-try:
-    from setuptools.namespaces import Installer as NameSpaceInstaller # NOQA
-except ImportError:
-    msg = ('You should use the latest setuptools. The namespaces.py file that this setup.py'
-           ' uses was added in setuptools 28.7.0 (Oct 2016)')
-    print(msg)
-    sys.exit()
+# try:
+#     from setuptools.namespaces import Installer as NameSpaceInstaller # NOQA
+# except ImportError:
+#     msg = ('You should use the latest setuptools. The namespaces.py file that this setup.py'
+#            ' uses was added in setuptools 28.7.0 (Oct 2016)')
+#     print(msg)
+#     sys.exit()
 
 if __name__ != '__main__':
     raise NotImplementedError('should never include setup.py')
 
 # # definitions
 
 full_package_name = None
@@ -47,17 +45,17 @@
         pass
 
     class NameConstant:
         pass
 
 
 if sys.version_info < (3,):
-    open_kw = dict()
+    open_kw = {}
 else:
-    open_kw = dict(encoding='utf-8')
+    open_kw = dict(encoding='utf-8')  # NOQA: C408
 
 
 if sys.version_info < (2, 7) or platform.python_implementation() == 'Jython':
 
     class Set:
         pass
 
@@ -111,15 +109,15 @@
         elif isinstance(node, Tuple):
             return tuple(map(_convert, node.elts))
         elif isinstance(node, List):
             return list(map(_convert, node.elts))
         elif isinstance(node, Set):
             return set(map(_convert, node.elts))
         elif isinstance(node, Dict):
-            return dict((_convert(k), _convert(v)) for k, v in zip(node.keys, node.values))
+            return {_convert(k): _convert(v) for k, v in zip(node.keys, node.values)}
         elif isinstance(node, NameConstant):
             return node.value
         elif sys.version_info < (3, 4) and isinstance(node, Name):
             if node.id in _safe_names:
                 return _safe_names[node.id]
         elif (
             isinstance(node, UnaryOp)
@@ -142,15 +140,15 @@
             if isinstance(node.op, Add):
                 return left + right
             else:
                 return left - right
         elif isinstance(node, Call):
             func_id = getattr(node.func, 'id', None)
             if func_id == 'dict':
-                return dict((k.arg, _convert(k.value)) for k in node.keywords)
+                return {k.arg: _convert(k.value) for k in node.keywords}
             elif func_id == 'set':
                 return set(_convert(node.args[0]))
             elif func_id == 'date':
                 return datetime.date(*[_convert(k) for k in node.args])
             elif func_id == 'datetime':
                 return datetime.datetime(*[_convert(k) for k in node.args])
         err = SyntaxError('malformed node or string: ' + repr(node))
@@ -200,16 +198,16 @@
                                 print(
                                     '{0:{1}}: {2}'.format(index, w, line).encode('utf-8'),
                                     end="",
                                 )
                                 if index == e.lineno - 1:
                                     print(
                                         '{0:{1}}  {2}^--- {3}'.format(
-                                            ' ', w, ' ' * e.offset, e.node
-                                        )
+                                            ' ', w, ' ' * e.offset, e.node,
+                                        ),
                                     )
                         raise
                     break
                 lines.append(line)
             else:
                 raise NotImplementedError
     return data
@@ -274,16 +272,15 @@
                 alt_files.append(x)
         return alt_files
 
 
 class MySdist(_sdist):
     def initialize_options(self):
         _sdist.initialize_options(self)
-        # see pep 527, new uploads should be tar.gz or .zip
-        # fmt = getattr(self, 'tarfmt',  None)
+        # failed expiriment, see pep 527, new uploads should be tar.gz or .zip
         # because of unicode_literals
         # self.formats = fmt if fmt else [b'bztar'] if sys.version_info < (3, ) else ['bztar']
         dist_base = os.environ.get('PYDISTBASE')
         fpn = getattr(getattr(self, 'nsp', self), 'full_package_name', None)
         if fpn and dist_base:
             print('setting  distdir {}/{}'.format(dist_base, fpn))
             self.dist_dir = os.path.join(dist_base, fpn)
@@ -313,16 +310,16 @@
     def __init__(self, pkg_data):
         assert isinstance(pkg_data, dict)
         self._pkg_data = pkg_data
         self.full_package_name = self.pn(self._pkg_data['full_package_name'])
         self._split = None
         self.depth = self.full_package_name.count('.')
         self.nested = self._pkg_data.get('nested', False)
-        if self.nested:
-            NameSpaceInstaller.install_namespaces = lambda x: None
+        # if self.nested:
+        #     NameSpaceInstaller.install_namespaces = lambda x: None
         self.command = None
         self.python_version()
         self._pkg = [None, None]  # required and pre-installable packages
         if sys.argv[0] == 'setup.py' and sys.argv[1] == 'install':
             debug('calling setup.py', sys.argv)
             if '-h' in sys.argv:
                 pass
@@ -383,17 +380,14 @@
         if skip:
             # this interferes with output checking
             # print('skipping sub-packages:', ', '.join(skip))
             pass
         return self._split
 
     @property
-    def namespace_packages(self):
-        return self.split[: self.depth]
-
     def namespace_directories(self, depth=None):
         """return list of directories where the namespace should be created /
         can be found
         """
         res = []
         for index, d in enumerate(self.split[:depth]):
             # toplevel gets a dot
@@ -402,35 +396,23 @@
             res.append('.' + d)
         return res
 
     @property
     def package_dir(self):
         d = {
             # don't specify empty dir, clashes with package_data spec
-            self.full_package_name: '.'
+            self.full_package_name: '.',
         }
         if 'extra_packages' in self._pkg_data:
             return d
-        if len(self.split) > 1:  # only if package namespace
-            d[self.split[0]] = self.namespace_directories(1)[0]
+        # if len(self.split) > 1:  # only if package namespace
+        #     d[self.split[0]] = self.namespace_directories(1)[0]
+        # print('d', d, os.getcwd())
         return d
 
-    def create_dirs(self):
-        """create the directories necessary for namespace packaging"""
-        directories = self.namespace_directories(self.depth)
-        if not directories:
-            return
-        if not os.path.exists(directories[0]):
-            for d in directories:
-                os.mkdir(d)
-                with open(os.path.join(d, '__init__.py'), 'w') as fp:
-                    fp.write(
-                        'import pkg_resources\n' 'pkg_resources.declare_namespace(__name__)\n'
-                    )
-
     def python_version(self):
         supported = self._pkg_data.get('supported')
         if supported is None:
             return
         if len(supported) == 1:
             minimum = supported[0]
         else:
@@ -452,15 +434,15 @@
             return
 
         # if hgi and hgi.base are both in namespace_packages matching
         # against the top (hgi.) it suffices to find minus-e and non-minus-e
         # installed packages. As we don't know the order in namespace_packages
         # do some magic
         prefix = self.split[0]
-        prefixes = set([prefix, prefix.replace('_', '-')])
+        prefixes = {prefix, prefix.replace('_', '-')}
         for p in sys.path:
             if not p:
                 continue  # directory with setup.py
             if os.path.exists(os.path.join(p, 'setup.py')):
                 continue  # some linked in stuff might not be hgi based
             if not os.path.isdir(p):
                 continue
@@ -475,27 +457,27 @@
                 full_name = os.path.join(p, fn)
                 # not in prefixes the toplevel is never changed from _ to -
                 if fn == prefix and os.path.isdir(full_name):
                     # directory -> other, non-minus-e, install
                     if self.command == 'develop':
                         raise InstallationError(
                             'Cannot mix develop (pip install -e),\nwith '
-                            'non-develop installs for package name {0}'.format(fn)
+                            'non-develop installs for package name {0}'.format(fn),
                         )
                 elif fn == prefix:
                     raise InstallationError('non directory package {0} in {1}'.format(fn, p))
                 for pre in [x + '.' for x in prefixes]:
                     if fn.startswith(pre):
                         break
                 else:
                     continue  # hgiabc instead of hgi.
                 if fn.endswith('-link') and self.command == 'install':
                     raise InstallationError(
                         'Cannot mix non-develop with develop\n(pip install -e)'
-                        ' installs for package name {0}'.format(fn)
+                        ' installs for package name {0}'.format(fn),
                     )
 
     def entry_points(self, script_name=None, package_name=None):
         """normally called without explicit script_name and package name
         the default console_scripts entry depends on the existence of __main__.py:
         if that file exists then the function main() in there is used, otherwise
         the in __init__.py.
@@ -505,15 +487,15 @@
         scriptname is the last part of the full package path (split on '.')
         if the ep entry is a simple string without "=", that is assumed to be
         the name of the script.
         """
 
         def pckg_entry_point(name):
             return '{0}{1}:main'.format(
-                name, '.__main__' if os.path.exists('__main__.py') else ""
+                name, '.__main__' if os.path.exists('__main__.py') else "",
             )
 
         ep = self._pkg_data.get('entry_points', True)
         if isinstance(ep, dict):
             return ep
         if ep is None:
             return None
@@ -526,16 +508,16 @@
             script_name = ep
         if package_name is None:
             package_name = self.full_package_name
         if not script_name:
             script_name = package_name.rsplit('.', 1)[-1]
         return {
             'console_scripts': [
-                '{0} = {1}'.format(script_name, pckg_entry_point(package_name))
-            ]
+                '{0} = {1}'.format(script_name, pckg_entry_point(package_name)),
+            ],
         }
 
     @property
     def url(self):
         url = self._pkg_data.get('url')
         if url:
             return url
@@ -600,16 +582,16 @@
                     'Intended Audience :: Developers',
                     'License :: '
                     + ('OSI Approved :: MIT' if self.has_mit_lic() else 'Other/Proprietary')
                     + ' License',
                     'Operating System :: OS Independent',
                     'Programming Language :: Python',
                 ]
-                + [self.pn(x) for x in self._pkg_data.get('classifiers', [])]
-            )
+                + [self.pn(x) for x in self._pkg_data.get('classifiers', [])],
+            ),
         )
 
     @property
     def keywords(self):
         return self.pn(self._pkg_data.get('keywords', []))
 
     @property
@@ -714,15 +696,16 @@
                     pd[str(k)] = pd.pop(k)
             # for k in pd:
             #     pd[k] = [e.encode('utf-8') for e in pd[k]]  # de-unicode
         return pd
 
     @property
     def packages(self):
-        s = self.split
+        # s = self.split
+        s = [self._pkg_data['full_package_name']]
         # fixed this in package_data, the keys there must be non-unicode for py27
         # if sys.version_info < (3, 0):
         #     s = [x.encode('utf-8') for x in self.split]
         return s + self._pkg_data.get('extra_packages', [])
 
     @property
     def python_requires(self):
@@ -750,99 +733,29 @@
         try:
             plat = sys.argv.index('--plat-name')
             if 'win' in sys.argv[plat + 1]:
                 return None
         except ValueError:
             pass
         self._ext_modules = []
-        no_test_compile = False
+        no_test_compile = True
         if '--restructuredtext' in sys.argv:
             no_test_compile = True
         elif 'sdist' in sys.argv:
             no_test_compile = True
         if no_test_compile:
             for target in self._pkg_data.get('ext_modules', []):
                 ext = Extension(
                     self.pn(target['name']),
                     sources=[self.pn(x) for x in target['src']],
                     libraries=[self.pn(x) for x in target.get('lib')],
                 )
                 self._ext_modules.append(ext)
             return self._ext_modules
-
-        print('sys.argv', sys.argv)
-        import tempfile
-        import shutil
-        from textwrap import dedent
-
-        import distutils.sysconfig
-        import distutils.ccompiler
-        from distutils.errors import CompileError, LinkError
-
-        for target in self._pkg_data.get('ext_modules', []):  # list of dicts
-            ext = Extension(
-                self.pn(target['name']),
-                sources=[self.pn(x) for x in target['src']],
-                libraries=[self.pn(x) for x in target.get('lib')],
-            )
-            # debug('test1 in target', 'test' in target, target)
-            if 'test' not in target:  # no test, just hope it works
-                self._ext_modules.append(ext)
-                continue
-            if sys.version_info[:2] == (3, 4) and platform.system() == 'Windows':
-                # this is giving problems on appveyor, so skip
-                if 'FORCE_C_BUILD_TEST' not in os.environ:
-                    self._ext_modules.append(ext)
-                    continue
-            # write a temporary .c file to compile
-            c_code = dedent(target['test'])
-            try:
-                tmp_dir = tempfile.mkdtemp(prefix='tmp_ruamel_')
-                bin_file_name = 'test' + self.pn(target['name'])
-                file_name = os.path.join(tmp_dir, bin_file_name + '.c')
-                print('test compiling', file_name, '->', bin_file_name, end=' ')
-                with open(file_name, 'w') as fp:  # write source
-                    fp.write(c_code)
-                # and try to compile it
-                compiler = distutils.ccompiler.new_compiler()
-                assert isinstance(compiler, distutils.ccompiler.CCompiler)
-                # do any platform specific initialisations
-                distutils.sysconfig.customize_compiler(compiler)
-                # make sure you can reach header files because compile does change dir
-                compiler.add_include_dir(os.getcwd())
-                if sys.version_info < (3,):
-                    tmp_dir = tmp_dir.encode('utf-8')
-                # used to be a different directory, not necessary
-                compile_out_dir = tmp_dir
-                try:
-                    compiler.link_executable(
-                        compiler.compile([file_name], output_dir=compile_out_dir),
-                        bin_file_name,
-                        output_dir=tmp_dir,
-                        libraries=ext.libraries,
-                    )
-                except CompileError:
-                    debug('compile error:', file_name)
-                    print('compile error:', file_name)
-                    raise
-                except LinkError:
-                    debug('link error', file_name)
-                    print('link error', file_name)
-                    raise
-                print('OK')
-                self._ext_modules.append(ext)
-            except Exception as e:  # NOQA
-                debug('Exception:', e)
-                print('Exception:', e)
-                sys.exit(1)
-                if sys.version_info[:2] == (3, 4) and platform.system() == 'Windows':
-                    traceback.print_exc()
-            finally:
-                shutil.rmtree(tmp_dir)
-        return self._ext_modules
+        # this used to use distutils
 
     @property
     def test_suite(self):
         return self._pkg_data.get('test_suite')
 
     def wheel(self, kw, setup):
         """temporary add setup.cfg if creating a wheel to include LICENSE file
@@ -850,56 +763,97 @@
         """
         if 'bdist_wheel' not in sys.argv:
             return False
         file_name = 'setup.cfg'
         if os.path.exists(file_name):  # add it if not in there?
             return False
         with open(file_name, 'w') as fp:
-            if os.path.exists('LICENSE'):
-                fp.write('[metadata]\nlicense_file = LICENSE\n')
-            else:
-                print('\n\n>>>>>> LICENSE file not found <<<<<\n\n')
             if self._pkg_data.get('universal'):
                 fp.write('[bdist_wheel]\nuniversal = 1\n')
         try:
             setup(**kw)
         except Exception:
             raise
         finally:
             os.remove(file_name)
         return True
 
 
-# # call setup
+class TmpFiles:
+    def __init__(self, pkg_data, py_project=True, keep=False):
+        self._rm_after = []
+        self._pkg_data = pkg_data
+        self._py_project = py_project
+        self._bdist_wheel = 'bdist_wheel' in sys.argv
+        self._keep = keep
+
+    def __enter__(self):
+        self.bdist_wheel()
+        self.py_project()
+
+    def bdist_wheel(self):
+        """pyproject doesn't allow for universal, so use setup.cfg if necessary
+        """
+        file_name = 'setup.cfg'
+        if not self._bdist_wheel or os.path.exists(file_name):
+            return
+        if self._pkg_data.get('universal'):
+            self._rm_after.append(file_name)
+            with open(file_name, 'w') as fp:
+                fp.write('[bdist_wheel]\nuniversal = 1\n')
+
+    def py_project(self):
+        """
+        to prevent pip from complaining, or is it too late to create it from setup.py
+        """
+        file_name = 'pyproject.toml'
+        if not self._py_project or os.path.exists(file_name):
+            return
+        self._rm_after.append(file_name)
+        with open(file_name, 'w') as fp:
+            fp.write(dedent("""\
+            [build-system]
+            requires = ["setuptools", "wheel"]
+            # test
+            build-backend = "setuptools.build_meta"
+            """))
+
+    def __exit__(self, typ, value, traceback):
+        if self._keep:
+            return
+        for p in self._rm_after:
+            if not os.path.exists(p):
+                print('file {} already removed'.format(p))
+            else:
+                os.unlink(p)
+
+
+# call setup
 def main():
     dump_kw = '--dump-kw'
     if dump_kw in sys.argv:
         import wheel
-        import distutils
         import setuptools
+        import pip
 
         print('python:    ', sys.version)
+        print('pip:       ', pip.__version__)
         print('setuptools:', setuptools.__version__)
-        print('distutils: ', distutils.__version__)
         print('wheel:     ', wheel.__version__)
     nsp = NameSpacePackager(pkg_data)
     nsp.check()
-    nsp.create_dirs()
+    # nsp.create_dirs()
     MySdist.nsp = nsp
-    if pkg_data.get('tarfmt'):
-        MySdist.tarfmt = pkg_data.get('tarfmt')
-
-    cmdclass = dict(install_lib=MyInstallLib, sdist=MySdist)
+    cmdclass = dict(install_lib=MyInstallLib, sdist=MySdist)  # NOQA: C408
     if _bdist_wheel_available:
         MyBdistWheel.nsp = nsp
         cmdclass['bdist_wheel'] = MyBdistWheel
 
-    kw = dict(
+    kw = dict(  # NOQA: C408
         name=nsp.full_package_name,
-        namespace_packages=nsp.namespace_packages,
         version=version_str,
         packages=nsp.packages,
         python_requires=nsp.python_requires,
         url=nsp.url,
         author=nsp.author,
         author_email=nsp.author_email,
         cmdclass=cmdclass,
@@ -910,52 +864,54 @@
         extras_require=nsp.extras_require,  # available since setuptools 18.0 / 2015-06
         license=nsp.license,
         classifiers=nsp.classifiers,
         keywords=nsp.keywords,
         package_data=nsp.package_data,
         ext_modules=nsp.ext_modules,
         test_suite=nsp.test_suite,
+        zip_safe=False,
     )
 
     if '--version' not in sys.argv and ('--verbose' in sys.argv or dump_kw in sys.argv):
         for k in sorted(kw):
             v = kw[k]
-            print('  "{0}": "{1}",'.format(k, v))
+            print('  "{0}": {1},'.format(k, repr(v)))
     # if '--record' in sys.argv:
     #     return
     if dump_kw in sys.argv:
         sys.argv.remove(dump_kw)
     try:
         with open('README.rst') as fp:
             kw['long_description'] = fp.read()
             kw['long_description_content_type'] = 'text/x-rst'
     except Exception:
         pass
 
-    if nsp.wheel(kw, setup):
-        return
-    for x in ['-c', 'egg_info', '--egg-base', 'pip-egg-info']:
-        if x not in sys.argv:
-            break
-    else:
-        # we're doing a tox setup install any starred package by searching up the source tree
-        # until you match your/package/name for your.package.name
-        for p in nsp.install_pre:
-            import subprocess
-
-            # search other source
-            setup_path = os.path.join(*p.split('.') + ['setup.py'])
-            try_dir = os.path.dirname(sys.executable)
-            while len(try_dir) > 1:
-                full_path_setup_py = os.path.join(try_dir, setup_path)
-                if os.path.exists(full_path_setup_py):
-                    pip = sys.executable.replace('python', 'pip')
-                    cmd = [pip, 'install', os.path.dirname(full_path_setup_py)]
-                    # with open('/var/tmp/notice', 'a') as fp:
-                    #     print('installing', cmd, file=fp)
-                    subprocess.check_output(cmd)
-                    break
-                try_dir = os.path.dirname(try_dir)
-    setup(**kw)
+    # if nsp.wheel(kw, setup):
+    #     return
+    with TmpFiles(pkg_data, keep=True):
+        for x in ['-c', 'egg_info', '--egg-base', 'pip-egg-info']:
+            if x not in sys.argv:
+                break
+        else:
+            # we're doing a tox setup install any starred package by searching up the
+            # source tree until you match your/package/name for your.package.name
+            for p in nsp.install_pre:
+                import subprocess
+
+                # search other source
+                setup_path = os.path.join(*p.split('.') + ['setup.py'])
+                try_dir = os.path.dirname(sys.executable)
+                while len(try_dir) > 1:
+                    full_path_setup_py = os.path.join(try_dir, setup_path)
+                    if os.path.exists(full_path_setup_py):
+                        pip = sys.executable.replace('python', 'pip')
+                        cmd = [pip, 'install', os.path.dirname(full_path_setup_py)]
+                        # with open('/var/tmp/notice', 'a') as fp:
+                        #     print('installing', cmd, file=fp)
+                        subprocess.check_output(cmd)
+                        break
+                    try_dir = os.path.dirname(try_dir)
+        setup(**kw)
 
 
 main()
```

