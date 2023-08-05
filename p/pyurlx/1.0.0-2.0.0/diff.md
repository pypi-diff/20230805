# Comparing `tmp/pyurlx-1.0.0.tar.gz` & `tmp/pyurlx-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyurlx-1.0.0.tar", last modified: Thu Jun 29 16:53:09 2023, max compression
+gzip compressed data, was "pyurlx-2.0.0.tar", last modified: Sat Aug  5 08:52:34 2023, max compression
```

## Comparing `pyurlx-1.0.0.tar` & `pyurlx-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-29 16:53:09.333709 pyurlx-1.0.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1300 2023-06-29 15:38:44.000000 pyurlx-1.0.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      576 2023-06-29 16:53:09.333709 pyurlx-1.0.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      178 2023-06-29 16:48:18.000000 pyurlx-1.0.0/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      527 2023-06-29 16:52:54.000000 pyurlx-1.0.0/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-29 16:53:09.333709 pyurlx-1.0.0/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-29 16:53:09.329709 pyurlx-1.0.0/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-29 16:53:09.329709 pyurlx-1.0.0/src/pyurlx/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-29 15:39:07.000000 pyurlx-1.0.0/src/pyurlx/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      290 2023-06-29 15:38:44.000000 pyurlx-1.0.0/src/pyurlx/shorten.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-29 16:53:09.333709 pyurlx-1.0.0/src/pyurlx.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      576 2023-06-29 16:53:09.000000 pyurlx-1.0.0/src/pyurlx.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      246 2023-06-29 16:53:09.000000 pyurlx-1.0.0/src/pyurlx.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-29 16:53:09.000000 pyurlx-1.0.0/src/pyurlx.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       55 2023-06-29 16:53:09.000000 pyurlx-1.0.0/src/pyurlx.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-29 16:53:09.000000 pyurlx-1.0.0/src/pyurlx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 08:52:34.192618 pyurlx-2.0.0/
+-rw-rw-rw-   0        0        0     1326 2023-08-05 08:39:25.000000 pyurlx-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      613 2023-08-05 08:52:34.189106 pyurlx-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-08-05 08:51:26.000000 pyurlx-2.0.0/README.md
+-rw-rw-rw-   0        0        0      554 2023-08-05 08:38:16.000000 pyurlx-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 08:52:34.193634 pyurlx-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 08:52:34.055829 pyurlx-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 08:52:34.109584 pyurlx-2.0.0/src/pyurlx/
+-rw-rw-rw-   0        0        0        0 2023-08-05 08:37:32.000000 pyurlx-2.0.0/src/pyurlx/__init__.py
+-rw-rw-rw-   0        0        0      800 2023-08-05 08:41:35.000000 pyurlx-2.0.0/src/pyurlx/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-05 08:52:34.183562 pyurlx-2.0.0/src/pyurlx.egg-info/
+-rw-rw-rw-   0        0        0      613 2023-08-05 08:52:33.000000 pyurlx-2.0.0/src/pyurlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-05 08:52:34.000000 pyurlx-2.0.0/src/pyurlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 08:52:33.000000 pyurlx-2.0.0/src/pyurlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-05 08:52:33.000000 pyurlx-2.0.0/src/pyurlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 08:52:33.000000 pyurlx-2.0.0/src/pyurlx.egg-info/top_level.txt
```

### Comparing `pyurlx-1.0.0/LICENSE` & `pyurlx-2.0.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-BSD 2-Clause License
-
-Copyright (c) 2023, James Marke
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 2-Clause License
+
+Copyright (c) 2023, The URLx Team
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

