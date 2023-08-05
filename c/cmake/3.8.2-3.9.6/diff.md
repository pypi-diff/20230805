# Comparing `tmp/cmake-3.8.2.tar.gz` & `tmp/cmake-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmake-3.8.2.tar", last modified: Mon Jul 23 07:07:23 2018, max compression
+gzip compressed data, was "dist/cmake-3.9.6.tar", last modified: Mon Jul 23 06:55:27 2018, max compression
```

## Comparing `cmake-3.8.2.tar` & `cmake-3.9.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-23 07:07:23.000000 cmake-3.8.2/
--rw-r--r--   0 root         (0) root         (0)    10430 2018-07-23 07:07:03.000000 cmake-3.8.2/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1356 2018-07-23 07:07:04.000000 cmake-3.8.2/CMakeUrls.cmake
--rw-r--r--   0 root         (0) root         (0)      261 2018-07-23 07:07:03.000000 cmake-3.8.2/HISTORY.rst
--rw-r--r--   0 root         (0) root         (0)    10274 2018-07-23 07:07:03.000000 cmake-3.8.2/LICENSE_Apache_20
--rw-r--r--   0 root         (0) root         (0)     1669 2018-07-23 07:07:03.000000 cmake-3.8.2/LICENSE_BSD_3
--rw-r--r--   0 root         (0) root         (0)      266 2018-07-23 07:07:03.000000 cmake-3.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4976 2018-07-23 07:07:23.000000 cmake-3.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3344 2018-07-23 07:07:04.000000 cmake-3.8.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake/
--rw-r--r--   0 root         (0) root         (0)     1138 2018-07-23 07:07:03.000000 cmake-3.8.2/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4976 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      335 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2018-07-23 07:07:23.000000 cmake-3.8.2/cmake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      189 2018-07-23 07:07:03.000000 cmake-3.8.2/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      458 2018-07-23 07:07:23.000000 cmake-3.8.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2090 2018-07-23 07:07:03.000000 cmake-3.8.2/setup.py
--rw-r--r--   0 root         (0) root         (0)    68587 2018-07-23 07:07:03.000000 cmake-3.8.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-23 06:55:27.000000 cmake-3.9.6/
+-rw-r--r--   0 root         (0) root         (0)    10430 2018-07-23 06:55:05.000000 cmake-3.9.6/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1356 2018-07-23 06:55:07.000000 cmake-3.9.6/CMakeUrls.cmake
+-rw-r--r--   0 root         (0) root         (0)      261 2018-07-23 06:55:05.000000 cmake-3.9.6/HISTORY.rst
+-rw-r--r--   0 root         (0) root         (0)    10274 2018-07-23 06:55:05.000000 cmake-3.9.6/LICENSE_Apache_20
+-rw-r--r--   0 root         (0) root         (0)     1669 2018-07-23 06:55:05.000000 cmake-3.9.6/LICENSE_BSD_3
+-rw-r--r--   0 root         (0) root         (0)      266 2018-07-23 06:55:05.000000 cmake-3.9.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4976 2018-07-23 06:55:27.000000 cmake-3.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3344 2018-07-23 06:55:07.000000 cmake-3.9.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake/
+-rw-r--r--   0 root         (0) root         (0)     1138 2018-07-23 06:55:05.000000 cmake-3.9.6/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4976 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      335 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2018-07-23 06:55:27.000000 cmake-3.9.6/cmake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2018-07-23 06:55:05.000000 cmake-3.9.6/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      458 2018-07-23 06:55:27.000000 cmake-3.9.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2090 2018-07-23 06:55:05.000000 cmake-3.9.6/setup.py
+-rw-r--r--   0 root         (0) root         (0)    68587 2018-07-23 06:55:05.000000 cmake-3.9.6/versioneer.py
```

### Comparing `cmake-3.8.2/CMakeLists.txt` & `cmake-3.9.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-3.8.2/CMakeUrls.cmake` & `cmake-3.9.6/CMakeUrls.cmake`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 #-----------------------------------------------------------------------------
 # CMake sources
-set(unix_source_url       "https://cmake.org/files/v3.8/cmake-3.8.2.tar.gz")
-set(unix_source_sha256    "da3072794eb4c09f2d782fcee043847b99bb4cf8d4573978d9b2024214d6e92d")
+set(unix_source_url       "https://cmake.org/files/v3.9/cmake-3.9.6.tar.gz")
+set(unix_source_sha256    "7410851a783a41b521214ad987bb534a7e4a65e059651a2514e6ebfc8f46b218")
 
-set(windows_source_url    "https://cmake.org/files/v3.8/cmake-3.8.2.zip")
-set(windows_source_sha256 "4b40927383b84c1a8dfdca55dddfb8431486462c8df3439a74b6b22be135175b")
+set(windows_source_url    "https://cmake.org/files/v3.9/cmake-3.9.6.zip")
+set(windows_source_sha256 "15af7cb123d9c939ac159ade831ea312e242a5a8fe5682646a69607a6b450ea3")
 
 #-----------------------------------------------------------------------------
 # CMake binaries
 
 set(linux32_binary_url    "NA")  # Linux 32-bit binaries not available
 set(linux32_binary_sha256 "NA")
 
-set(linux64_binary_url    "https://cmake.org/files/v3.8/cmake-3.8.2-Linux-x86_64.tar.gz")
-set(linux64_binary_sha256 "33e4851d3219b720f4b64fcf617151168f1bffdf5afad25eb4b7f5f58cee3a08")
+set(linux64_binary_url    "https://cmake.org/files/v3.9/cmake-3.9.6-Linux-x86_64.tar.gz")
+set(linux64_binary_sha256 "062bf45bee36ce7c2a55ae26b8b5324720f370d420a05cba91b9448c64ffdbea")
 
-set(macosx_binary_url    "https://cmake.org/files/v3.8/cmake-3.8.2-Darwin-x86_64.tar.gz")
-set(macosx_binary_sha256 "d164a1fa2a3d2f276c83ab55c7014b14b501b939d1a5a56f6788eb5cddc7acb6")
+set(macosx_binary_url    "https://cmake.org/files/v3.9/cmake-3.9.6-Darwin-x86_64.tar.gz")
+set(macosx_binary_sha256 "1694f3e183954ab6aadb2d7f85552aa2e050fab97ef4cbc817b1165255703599")
 
-set(win32_binary_url    "https://cmake.org/files/v3.8/cmake-3.8.2-win32-x86.zip")
-set(win32_binary_sha256 "3fa45a8ad473a8e0579ec826b3355f864750a7455987ed425a9c6fdf4820b5f2")
+set(win32_binary_url    "https://cmake.org/files/v3.9/cmake-3.9.6-win32-x86.zip")
+set(win32_binary_sha256 "8dd4b6c35afa8e0c044789b55645327cc4bb75276f87c6758f9997c08f559256")
 
-set(win64_binary_url    "https://cmake.org/files/v3.8/cmake-3.8.2-win64-x64.zip")
-set(win64_binary_sha256 "202c2416c964fb7199e5d7ce92336a44c7ba65d5ccca36246f41d7d09bd8ffe2")
+set(win64_binary_url    "https://cmake.org/files/v3.9/cmake-3.9.6-win64-x64.zip")
+set(win64_binary_sha256 "fa667bf658fa526e4e2489a9704f83f851e5ded66a18904424ba1b8505fd4dc0")
```

### Comparing `cmake-3.8.2/LICENSE_Apache_20` & `cmake-3.9.6/LICENSE_Apache_20`

 * *Files identical despite different names*

### Comparing `cmake-3.8.2/LICENSE_BSD_3` & `cmake-3.9.6/LICENSE_BSD_3`

 * *Files identical despite different names*

### Comparing `cmake-3.8.2/PKG-INFO` & `cmake-3.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cmake
-Version: 3.8.2
+Version: 3.9.6
 Summary: CMake is an open-source, cross-platform family of tools designed to build, test and package software
 Home-page: http://cmake.org/
 Author: Jean-Christophe Fillion-Robin
 Author-email: jchris.fillionr@kitware.com
 License: Apache 2.0
 Download-URL: https://cmake.org/download
 Description: ==========================
@@ -16,15 +16,15 @@
         and generate native makefiles and workspaces that can be used in the
         compiler environment of your choice.
         
         The suite of CMake tools were created by Kitware in response to the need
         for a powerful, cross-platform build environment for open-source projects
         such as ITK and VTK.
         
-        The CMake python wheels provide `CMake 3.8.2 <https://cmake.org/cmake/help/v3.8/index.html>`_.
+        The CMake python wheels provide `CMake 3.9.6 <https://cmake.org/cmake/help/v3.9/index.html>`_.
         
         Build Status
         ------------
         
         .. table::
         
           +---------------+------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
```

### Comparing `cmake-3.8.2/README.rst` & `cmake-3.9.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 and generate native makefiles and workspaces that can be used in the
 compiler environment of your choice.
 
 The suite of CMake tools were created by Kitware in response to the need
 for a powerful, cross-platform build environment for open-source projects
 such as ITK and VTK.
 
-The CMake python wheels provide `CMake 3.8.2 <https://cmake.org/cmake/help/v3.8/index.html>`_.
+The CMake python wheels provide `CMake 3.9.6 <https://cmake.org/cmake/help/v3.9/index.html>`_.
 
 Build Status
 ------------
 
 .. table::
 
   +---------------+------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
```

### Comparing `cmake-3.8.2/cmake/__init__.py` & `cmake-3.9.6/cmake/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake-3.8.2/cmake.egg-info/PKG-INFO` & `cmake-3.9.6/cmake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cmake
-Version: 3.8.2
+Version: 3.9.6
 Summary: CMake is an open-source, cross-platform family of tools designed to build, test and package software
 Home-page: http://cmake.org/
 Author: Jean-Christophe Fillion-Robin
 Author-email: jchris.fillionr@kitware.com
 License: Apache 2.0
 Download-URL: https://cmake.org/download
 Description: ==========================
@@ -16,15 +16,15 @@
         and generate native makefiles and workspaces that can be used in the
         compiler environment of your choice.
         
         The suite of CMake tools were created by Kitware in response to the need
         for a powerful, cross-platform build environment for open-source projects
         such as ITK and VTK.
         
-        The CMake python wheels provide `CMake 3.8.2 <https://cmake.org/cmake/help/v3.8/index.html>`_.
+        The CMake python wheels provide `CMake 3.9.6 <https://cmake.org/cmake/help/v3.9/index.html>`_.
         
         Build Status
         ------------
         
         .. table::
         
           +---------------+------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------+
```

### Comparing `cmake-3.8.2/setup.py` & `cmake-3.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `cmake-3.8.2/versioneer.py` & `cmake-3.9.6/versioneer.py`

 * *Files identical despite different names*

