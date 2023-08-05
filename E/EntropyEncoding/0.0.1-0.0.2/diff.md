# Comparing `tmp/EntropyEncoding-0.0.1.tar.gz` & `tmp/EntropyEncoding-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EntropyEncoding-0.0.1.tar", last modified: Fri Aug  4 20:15:18 2023, max compression
+gzip compressed data, was "EntropyEncoding-0.0.2.tar", last modified: Fri Aug  4 20:26:26 2023, max compression
```

## Comparing `EntropyEncoding-0.0.1.tar` & `EntropyEncoding-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-04 20:15:18.631242 EntropyEncoding-0.0.1/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-04 20:15:18.631242 EntropyEncoding-0.0.1/EntropyEncoding.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2644 2023-08-04 20:15:18.000000 EntropyEncoding-0.0.1/EntropyEncoding.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      242 2023-08-04 20:15:18.000000 EntropyEncoding-0.0.1/EntropyEncoding.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-04 20:15:18.000000 EntropyEncoding-0.0.1/EntropyEncoding.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-08-04 20:15:18.000000 EntropyEncoding-0.0.1/EntropyEncoding.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    49221 2023-08-04 20:00:06.000000 EntropyEncoding-0.0.1/EntropyEncoding.py
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.1/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       60 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.1/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2644 2023-08-04 20:15:18.631242 EntropyEncoding-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1232 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.1/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1778 2023-08-04 20:07:48.000000 EntropyEncoding-0.0.1/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)     1444 2023-08-04 20:15:18.631242 EntropyEncoding-0.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1783 2023-08-04 20:04:48.000000 EntropyEncoding-0.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2357 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      242 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    49272 2023-08-04 20:21:36.000000 EntropyEncoding-0.0.2/EntropyEncoding.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.2/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       60 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.2/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     2357 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      939 2023-08-04 20:21:04.000000 EntropyEncoding-0.0.2/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1778 2023-08-04 20:26:22.000000 EntropyEncoding-0.0.2/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1444 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1783 2023-08-04 20:04:48.000000 EntropyEncoding-0.0.2/setup.py
```

### Comparing `EntropyEncoding-0.0.1/EntropyEncoding.egg-info/PKG-INFO` & `EntropyEncoding-0.0.2/EntropyEncoding.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EntropyEncoding
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package implements an encoding to bypass entropy antivirus check.
 Home-page: https://github.com/mauricelambert/EntropyEncoding
 Author: Maurice Lambert
 Author-email: Maurice Lambert <mauricelambert434@gmail.com>
 Maintainer: Maurice Lambert
 Maintainer-email: Maurice Lambert <mauricelambert434@gmail.com>
 License: GPL-3.0 License
@@ -55,33 +55,27 @@
 git clone "https://github.com/mauricelambert/EntropyEncoding.git"
 cd "EntropyEncoding"
 python3 -m pip install .
 ```
 
 ## Usages
 
-### Command line
+```python
+from EntropyEncoding import *
 
-```bash
-EntropyEncoding              # Using CLI package executable
-python3 -m EntropyEncoding   # Using python module
-python3 EntropyEncoding.pyz  # Using python executable
-EntropyEncoding.exe          # Using python Windows executable
-```
+encoded_shellcode = entropy_encode(b"shellcode_payload")
+print(encoded_shellcode)
 
-### Python script
+entropy_decode(encoded_shellcode) == b"shellcode_payload"
 
-```python
-from EntropyEncoding import *
+print(shannon_entropy)
 ```
 
 ## Links
 
  - [Pypi](https://pypi.org/project/EntropyEncoding)
- - [Github](https://github.com/user/EntropyEncoding)
+ - [Github](https://github.com/mauricelambert/EntropyEncoding)
  - [Documentation](https://user.github.io/info/python/security/EntropyEncoding.html)
- - [Python executable](https://user.github.io/info/python/security/EntropyEncoding.pyz)
- - [Python Windows executable](https://user.github.io/info/python/security/EntropyEncoding.exe)
 
 ## License
 
 Licensed under the [GPL, version 3](https://www.gnu.org/licenses/).
```

### Comparing `EntropyEncoding-0.0.1/EntropyEncoding.py` & `EntropyEncoding-0.0.2/EntropyEncoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,25 +35,25 @@
 Entropy for entropy-encoded encrypted secrets: 5.774096152750044
 Entropy for non-encoded exe: 5.22055339277441
 Entropy for non-encoded encrypted exe: 7.914685739354301
 Entropy for entropy-encoded encrypted exe: 5.759477906043907
 ~# 
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an encoding to bypass entropy antivirus check.
 """
 __url__ = "https://github.com/mauricelambert/EntropyEncoding"
 
-# __all__ = []
+__all__ = ["entropy_encode", "entropy_decode", "shannon_entropy"]
 
 __license__ = "GPL-3.0 License"
 __copyright__ = """
 EntropyEncoding  Copyright (C) 2023  Maurice Lambert
 This program comes with ABSOLUTELY NO WARRANTY.
 This is free software, and you are welcome to redistribute it
 under certain conditions.
```

### Comparing `EntropyEncoding-0.0.1/LICENSE.txt` & `EntropyEncoding-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EntropyEncoding-0.0.1/PKG-INFO` & `EntropyEncoding-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EntropyEncoding
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package implements an encoding to bypass entropy antivirus check.
 Home-page: https://github.com/mauricelambert/EntropyEncoding
 Author: Maurice Lambert
 Author-email: Maurice Lambert <mauricelambert434@gmail.com>
 Maintainer: Maurice Lambert
 Maintainer-email: Maurice Lambert <mauricelambert434@gmail.com>
 License: GPL-3.0 License
@@ -55,33 +55,27 @@
 git clone "https://github.com/mauricelambert/EntropyEncoding.git"
 cd "EntropyEncoding"
 python3 -m pip install .
 ```
 
 ## Usages
 
-### Command line
+```python
+from EntropyEncoding import *
 
-```bash
-EntropyEncoding              # Using CLI package executable
-python3 -m EntropyEncoding   # Using python module
-python3 EntropyEncoding.pyz  # Using python executable
-EntropyEncoding.exe          # Using python Windows executable
-```
+encoded_shellcode = entropy_encode(b"shellcode_payload")
+print(encoded_shellcode)
 
-### Python script
+entropy_decode(encoded_shellcode) == b"shellcode_payload"
 
-```python
-from EntropyEncoding import *
+print(shannon_entropy)
 ```
 
 ## Links
 
  - [Pypi](https://pypi.org/project/EntropyEncoding)
- - [Github](https://github.com/user/EntropyEncoding)
+ - [Github](https://github.com/mauricelambert/EntropyEncoding)
  - [Documentation](https://user.github.io/info/python/security/EntropyEncoding.html)
- - [Python executable](https://user.github.io/info/python/security/EntropyEncoding.pyz)
- - [Python Windows executable](https://user.github.io/info/python/security/EntropyEncoding.exe)
 
 ## License
 
 Licensed under the [GPL, version 3](https://www.gnu.org/licenses/).
```

### Comparing `EntropyEncoding-0.0.1/pyproject.toml` & `EntropyEncoding-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EntropyEncoding"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = []
 authors = [
     {name = "Maurice Lambert", email = "mauricelambert434@gmail.com"},
 ]
 maintainers = [
     {name = "Maurice Lambert", email = "mauricelambert434@gmail.com"},
 ]
```

### Comparing `EntropyEncoding-0.0.1/setup.cfg` & `EntropyEncoding-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EntropyEncoding
-version = 0.0.1
+version = 0.0.2
 author = Maurice Lambert
 author_email = mauricelambert434@gmail.com
 maintainer = Maurice Lambert
 maintainer_email = mauricelambert434@gmail.com
 description = This package implements an encoding to bypass entropy antivirus check.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `EntropyEncoding-0.0.1/setup.py` & `EntropyEncoding-0.0.2/setup.py`

 * *Files identical despite different names*

