# Comparing `tmp/daqpp-2.0.1.tar.gz` & `tmp/daqpp-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daqpp-2.0.1.tar", last modified: Thu May 11 22:02:19 2023, max compression
+gzip compressed data, was "daqpp-2.0.3.tar", last modified: Sat Aug  5 08:21:04 2023, max compression
```

## Comparing `daqpp-2.0.1.tar` & `daqpp-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 22:02:19.813732 daqpp-2.0.1/
--rw-r--r--   0 lacasta    (503) staff       (20)      476 2023-05-11 22:02:19.813382 daqpp-2.0.1/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)       60 2023-05-11 15:52:01.000000 daqpp-2.0.1/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 22:02:19.808918 daqpp-2.0.1/daqpp/
--rw-r--r--   0 lacasta    (503) staff       (20)       22 2023-05-11 22:01:54.000000 daqpp-2.0.1/daqpp/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6794 2020-12-01 07:54:55.000000 daqpp-2.0.1/daqpp/daq.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20114 2022-09-27 17:00:12.000000 daqpp-2.0.1/daqpp/soap.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-11 22:02:19.812681 daqpp-2.0.1/daqpp.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)      476 2023-05-11 22:02:19.000000 daqpp-2.0.1/daqpp.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      213 2023-05-11 22:02:19.000000 daqpp-2.0.1/daqpp.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-11 22:02:19.000000 daqpp-2.0.1/daqpp.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       12 2023-05-11 22:02:19.000000 daqpp-2.0.1/daqpp.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        6 2023-05-11 22:02:19.000000 daqpp-2.0.1/daqpp.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      574 2023-05-11 21:58:50.000000 daqpp-2.0.1/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-11 22:02:19.813815 daqpp-2.0.1/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-05 08:21:04.314660 daqpp-2.0.3/
+-rw-r--r--   0 lacasta    (503) staff       (20)      414 2023-08-05 08:21:04.314241 daqpp-2.0.3/PKG-INFO
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-05 08:21:04.309046 daqpp-2.0.3/daqpp/
+-rw-r--r--   0 lacasta    (503) staff       (20)       22 2023-08-04 18:25:21.000000 daqpp-2.0.3/daqpp/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6683 2023-07-31 15:20:25.000000 daqpp-2.0.3/daqpp/daq.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    20248 2023-08-04 18:36:43.000000 daqpp-2.0.3/daqpp/soap.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-08-05 08:21:04.311403 daqpp-2.0.3/daqpp.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)      414 2023-08-05 08:21:04.000000 daqpp-2.0.3/daqpp.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      203 2023-08-05 08:21:04.000000 daqpp-2.0.3/daqpp.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-08-05 08:21:04.000000 daqpp-2.0.3/daqpp.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       12 2023-08-05 08:21:04.000000 daqpp-2.0.3/daqpp.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        6 2023-08-05 08:21:04.000000 daqpp-2.0.3/daqpp.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      574 2023-08-04 18:24:56.000000 daqpp-2.0.3/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-08-05 08:21:04.314744 daqpp-2.0.3/setup.cfg
```

### Comparing `daqpp-2.0.1/daqpp/daq.py` & `daqpp-2.0.3/daqpp/daq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 #!/usr/bin/env python3
 
-"""daqpp.
+"""daqpp
 
-This module defines a wrapper for the DAQ++ package, allowing to
-build a data acquisition system from python taking advantage of
-DAQ++.
-One can also interface with existing libraries that implement
-different models for Module and RunManager objects. For that daqpp
-provides load_lib that will return a Hook object from with you can
-call the Module and RunManager factories. daqpp uses dl for loading
-the shared libraries. It also 'borrows' the RTLD_* constants from
-the dl module.
-Note: The libraries should provide Object factories, that is,
-functions declared with extern 'C' that are able to create your
-objects from the arguments passed. They should be something like:
-extern 'C' void create_module(const char *type) {
-   if ( type=='type1') {
-      new ModuleType1(...)
+   This module defines a wrapper for the DAQ++ package, allowing to
+   build a data acquisition system from python taking advantage of
+   DAQ++.
+
+   One can also interface with existing libraries that implement
+   different models for Module and RunManager objects. For that daqpp
+   provides load_lib that will return a Hook object from with you can
+   call the Module and RunManager factories. daqpp uses dl for loading
+   the shared libraries. It also 'borrows' the RTLD_* constants from
+   the dl module.
+
+   Note: The libraries should provide Object factories, that is,
+   functions declared with extern 'C' that are able to create your
+   objects from the arguments passed. They should be something like:
+
+   extern 'C' void create_module(const char *type) {
+      if ( type=='type1') {
+         new ModuleType1(...)
+      }
+      else if ( type='...') {
+          ...
+      }
    }
-   else if ( type='...') {
-       ...
-   }
-}
-The idea behind is that you can afterwards access the module with
-the DAQmanager.find_module() or DAQmanager.find_runmanager() functions.
-This module also provides a helper function that does exactly that:
-- create_module
-- create_runmanager
-"""
 
+   The idea behind is that you can afterwards access the module with
+   the DAQmanager.find_module() or DAQmanager.find_runmanager() functions.
+
+   This module also provides a helper function that does exactly that:
+   - create_module
+   - create_runmanager
+"""
 import sys
 import ctypes
 import re
 from pathlib import Path
 
 from daqpp.DAQpp import *
 
@@ -41,64 +45,49 @@
     """HookList.
 
     Maintains a list of all the existing Hooks. This is implemented as
     a singleton. The basic idea behind is that we do not want the
     libraries to be unloaded until the very end, so that all their
     routines are available.
     """
-
     def __new__(cls, *args, **kwargs):
-        """That makes the class a singleton."""
+        """That makes the class a singleton"""
         if '_inst' not in vars(cls):
             cls._inst = dict.__new__(cls, *args, **kwargs)
 
         return cls._inst
 
     def __init__(self):
-        """Initialization."""
         super(HookList, self).__init__()
 
     def __setitem__(self, key, value):
-        """Item setter.
-
-        Args:
-        ----
-            key (str): the item key
-            value : The item value
-
-        """
         if value.handler:
             super(HookList, self).__setitem__(key, value)
         else:
             print('Invalid handler. Hook not stored')
 
     def __del__(self):
-        """Delete."""
         print('Deleting the list of Hooks')
         self.clear()
 
 
 def load_lib(lib):
-    """Load a library.
+    """load_lib(lib)
 
-    Load a shared library into the system. It will return a
-    reference to a Hook object that contains the library handler
-    that will allow to access to the library symbols.
-
-    Args:
-    ----
-    lib: the path of the shared library
-
-    Returns
-    -------
-    A Hook object that will allow to access the library symbols
+       Load a shared library into the system. It will return a
+       reference to a Hook object that contains the library handler
+       that will allow to access to the library symbols.
+
+       @param lib: the path of the shared library
+       @return: A Hook object that will allow to access the
+                library symbols
 
     """
     class Hook(object):
-        """Hook.
+        """Hook,
 
         This class defines what I call a hook. It is in fact a holder
         of a shared library handler as given by the dl module.
 
         To access the symbols or routines exported by the library, just
         call
```

### Comparing `daqpp-2.0.1/daqpp/soap.py` & `daqpp-2.0.3/daqpp/soap.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,16 +143,16 @@
 
     xsd_valueType = xsd.ComplexType(
         xsd.Sequence([
             xsd.Element('item',
                         xsd.Any,
                         min_occurs=1,
                         max_occurs='unbounded')
-        ]),
-        qname=etree.QName("{http://localhost/daqpp/}valueType"))
+            ]),
+         qname=etree.QName("{http://localhost/daqpp/}valueType"))
 
     def __init__(self, server, value, type):
         """Initializtion.
 
         Args:
         ----
             server (DAQppClient): The zeep client
@@ -368,16 +368,15 @@
         ----
         value: the new value
 
         """
         if self.server is None:
             return
 
-        par_value = SOAPParam(self.server, self.obj,
-                              self.name, value, self.type)
+        par_value = SOAPParam(self.server, self.obj, self.name, value, self.type)
 
         self.server.setParameter(par_value.element())
 
     def decode(self, par):
         """Decode the parameter.
 
         Helper function to parse the Parameter as returned by the SOAP server.
@@ -542,14 +541,19 @@
         rc = self.server.getMonitorData(daqid=self.name)
         return rc
 
     def resetMonitorData(self, flags=0):
         """Reset the monitor data in the server."""
         self.server.resetMonitorData(daqid=self.name, flags=flags)
 
+    def getParameter(self, parName):
+        """Get the parameter with given name."""
+        P = Parameter(parName, self.name, self.server)
+        return P
+
 
 class Module(DAQObject):
     """A Module"""
 
     def __init__(self, name, server):
         """Initialization.
```

### Comparing `daqpp-2.0.1/pyproject.toml` & `daqpp-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daqpp"
-version = "2.0.1"
+version = "2.0.3"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "Communication with daqpp via soap.."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

