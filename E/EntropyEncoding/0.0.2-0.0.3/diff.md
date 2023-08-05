# Comparing `tmp/EntropyEncoding-0.0.2.tar.gz` & `tmp/EntropyEncoding-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EntropyEncoding-0.0.2.tar", last modified: Fri Aug  4 20:26:26 2023, max compression
+gzip compressed data, was "EntropyEncoding-0.0.3.tar", last modified: Sat Aug  5 08:03:52 2023, max compression
```

## Comparing `EntropyEncoding-0.0.2.tar` & `EntropyEncoding-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2357 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      242 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-08-04 20:26:26.000000 EntropyEncoding-0.0.2/EntropyEncoding.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    49272 2023-08-04 20:21:36.000000 EntropyEncoding-0.0.2/EntropyEncoding.py
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.2/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       60 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.2/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2357 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      939 2023-08-04 20:21:04.000000 EntropyEncoding-0.0.2/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     1778 2023-08-04 20:26:22.000000 EntropyEncoding-0.0.2/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)     1444 2023-08-04 20:26:26.669095 EntropyEncoding-0.0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1783 2023-08-04 20:04:48.000000 EntropyEncoding-0.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-05 08:03:52.511734 EntropyEncoding-0.0.3/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-05 08:03:52.511734 EntropyEncoding-0.0.3/EntropyEncoding.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3394 2023-08-05 08:03:52.000000 EntropyEncoding-0.0.3/EntropyEncoding.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      242 2023-08-05 08:03:52.000000 EntropyEncoding-0.0.3/EntropyEncoding.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-05 08:03:52.000000 EntropyEncoding-0.0.3/EntropyEncoding.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-08-05 08:03:52.000000 EntropyEncoding-0.0.3/EntropyEncoding.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    52409 2023-08-05 07:50:08.000000 EntropyEncoding-0.0.3/EntropyEncoding.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.3/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       60 2023-08-04 19:41:22.000000 EntropyEncoding-0.0.3/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     3394 2023-08-05 08:03:52.511734 EntropyEncoding-0.0.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1998 2023-08-04 20:54:46.000000 EntropyEncoding-0.0.3/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     1778 2023-08-04 20:39:24.000000 EntropyEncoding-0.0.3/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)     1444 2023-08-05 08:03:52.511734 EntropyEncoding-0.0.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1838 2023-08-05 07:43:08.000000 EntropyEncoding-0.0.3/setup.py
```

### Comparing `EntropyEncoding-0.0.2/EntropyEncoding.egg-info/PKG-INFO` & `EntropyEncoding-0.0.3/EntropyEncoding.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EntropyEncoding
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package implements an encoding to bypass entropy antivirus check.
 Home-page: https://github.com/mauricelambert/EntropyEncoding
 Author: Maurice Lambert
 Author-email: Maurice Lambert <mauricelambert434@gmail.com>
 Maintainer: Maurice Lambert
 Maintainer-email: Maurice Lambert <mauricelambert434@gmail.com>
 License: GPL-3.0 License
@@ -29,20 +29,28 @@
 Classifier: Topic :: System :: Systems Administration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+![EntropyEncoding logo](https://mauricelambert.github.io/info/python/security/EntropyEncoding.gif "EntropyEncoding logo")
+
 # EntropyEncoding
 
 ## Description
 
 This package implements an encoding to bypass entropy antivirus check.
 
+I have researched about entropy bypass techniques and found people who use adding low-entropy data to bypass entropy check. I think adding data can be optimized and more efficient with a simple entropy encoding to reduce entropy score.
+
+Adding low-entropy data:
+ 1. you get a larger file
+ 2. you do not change payload entropy (if the antivirus software splits the file for entropy calculation, it will probably have high entropy on a payload chunk)
+
 ## Requirements
 
 This package require:
  - python3
  - python3 Standard Library
 
 ## Installation
@@ -58,20 +66,34 @@
 ```
 
 ## Usages
 
 ```python
 from EntropyEncoding import *
 
+print(shannon_entropy(b"shellcode_payload"))
 encoded_shellcode = entropy_encode(b"shellcode_payload")
 print(encoded_shellcode)
 
 entropy_decode(encoded_shellcode) == b"shellcode_payload"
 
-print(shannon_entropy)
+print(shannon_entropy(encoded_shellcode))
+```
+
+Tests results:
+
+```
+~# python3 EntropyEncoding.py
+Entropy for non-encoded secrets: 4.521591372417719
+Entropy for non-encoded encrypted secrets: 7.951320327821406
+Entropy for entropy-encoded encrypted secrets: 5.774096152750044
+Entropy for non-encoded exe: 5.22055339277441
+Entropy for non-encoded encrypted exe: 7.914685739354301
+Entropy for entropy-encoded encrypted exe: 5.759477906043907
+~# 
 ```
 
 ## Links
 
  - [Pypi](https://pypi.org/project/EntropyEncoding)
  - [Github](https://github.com/mauricelambert/EntropyEncoding)
  - [Documentation](https://user.github.io/info/python/security/EntropyEncoding.html)
```

### Comparing `EntropyEncoding-0.0.2/EntropyEncoding.py` & `EntropyEncoding-0.0.3/EntropyEncoding.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,37 +23,45 @@
 This package implements an encoding to bypass entropy antivirus check.
 
 https://www.schellman.com/blog/cybersecurity/penetration-testing-methods-entropy
 https://vanmieghem.io/blueprint-for-evading-edr-in-2022/
 https://pentest.blog/art-of-anti-detection-1-introduction-to-av-detection-techniques/
 
 Information based on a blog (red teamer test a not named EDR):
-    - antivirus detect potentially malicious entropy when entropy greater than 7.2
+    - antivirus detect potentially malicious entropy when the entropy score is greater than 7.2
 
 ~# python3 EntropyEncoding.py
 Entropy for non-encoded secrets: 4.521591372417719
-Entropy for non-encoded encrypted secrets: 7.951320327821406
-Entropy for entropy-encoded encrypted secrets: 5.774096152750044
+Entropy for non-encoded encrypted secrets: 7.945422222752084
+Entropy for entropy-encoded encrypted secrets: 5.762166896848745
+Entropy for entropy-encoded2 encrypted secrets: 5.748670434218312
 Entropy for non-encoded exe: 5.22055339277441
-Entropy for non-encoded encrypted exe: 7.914685739354301
-Entropy for entropy-encoded encrypted exe: 5.759477906043907
+Entropy for non-encoded encrypted exe: 7.923900258907012
+Entropy for entropy-encoded encrypted exe: 5.756072685391074
+Entropy for entropy-encoded2 encrypted exe: 5.799741821347019
 ~# 
 """
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements an encoding to bypass entropy antivirus check.
 """
 __url__ = "https://github.com/mauricelambert/EntropyEncoding"
 
-__all__ = ["entropy_encode", "entropy_decode", "shannon_entropy"]
+__all__ = [
+    "entropy_encode2",
+    "entropy_decode2",
+    "entropy_encode",
+    "entropy_decode",
+    "shannon_entropy",
+]
 
 __license__ = "GPL-3.0 License"
 __copyright__ = """
 EntropyEncoding  Copyright (C) 2023  Maurice Lambert
 This program comes with ABSOLUTELY NO WARRANTY.
 This is free software, and you are welcome to redistribute it
 under certain conditions.
@@ -221,75 +229,175 @@
 
     encoding = defaultdict(bytearray)
 
     while base32_characters:
         character = choice(base32_characters)
         base32_characters.remove(character)
         data.append(character)
+        encoding[character].append(character)
+
         choice_ = choice(random_characters)
         random_characters.remove(choice_)
-        order = randint(0, 1)
-        if order:
-            encoding[character].append(character)
+
         for _ in range(randint(2, 5)):
             data.append(choice_)
             encoding[character].append(choice_)
-        if not order:
-            encoding[character].append(character)
 
     return data + random_characters, encoding
 
 
+def generate_entropy_encoding2() -> Tuple[bytearray, Dict[int, bytearray]]:
+    """
+    This function generates an encoding to bypass entropy checks.
+
+     + Very difficult to identify
+     - Entropy score is higher
+     - Longer to encode/decode
+    """
+
+    base32_characters = bytearray(b"01234567ABCDEFGHIJKLMNOPQRSTUVWXYZ=")
+    random_characters = bytearray(
+        b"89abcdefghijklmnopqrstuvwxyz!\"#$%&'()*+,-./:;<>?@[\\]^_`{|}~ \t\n\r"
+    )
+
+    data = bytearray()
+
+    encoding = defaultdict(bytearray)
+
+    while base32_characters:
+        character = choice(base32_characters)
+        base32_characters.remove(character)
+        data.append(character)
+
+        choice1 = choice(random_characters)
+        random_characters.remove(choice1)
+        encoding[character].append(choice1)
+
+        choice2 = choice(random_characters)
+        random_characters.remove(choice2)
+
+        order = randint(0, 1)
+        if order:
+            data.append(choice1)
+        for _ in range(randint(2, 5)):
+            data.append(choice2)
+            encoding[character].append(choice2)
+        if not order:
+            data.append(choice1)
+
+        random_characters.append(character)
+
+    return data, encoding
+
+
 def get_entropy_encoding(data: bytes) -> bytes:
     """
     This function returns the encoding to decode entropy-encoding.
     """
 
     encoding = {}
     while len(encoding) < 70:
         character1 = data[0]
         character2 = data[1]
+
         encoding[character1] = character1
         encoding[character2] = character1
+
         index = 2
         for character in data[2:]:
             if character != character2:
                 data = data[index:]
                 break
             index += 1
 
     return data[28:], encoding
 
 
-def entropy_encode(data: bytes) -> bytes:
+def get_entropy_encoding2(data: bytes) -> bytes:
+    """
+    This function returns the encoding to decode entropy-encoding.
+    """
+
+    encoding = {}
+    while len(encoding) < 70:
+        character_base = data[0]
+        character1 = data[1]
+        character2 = data[2]
+        index = 3
+
+        while character1 == character2:
+            character2 = data[index]
+            index += 1
+
+        encoding[character1] = character_base
+        encoding[character2] = character_base
+
+        for character in data[index:]:
+            if character != character2:
+                data = data[index:]
+                break
+            index += 1
+
+    return data, encoding
+
+
+def entropy_encode(data: bytes, version: int = 1) -> bytes:
     """
     This function encodes data to bypass entropy checks.
+
+    version should be 1 or 2.
     """
 
-    data_encoded, encoding = generate_entropy_encoding()
+    data_encoded, encoding = (
+        generate_entropy_encoding()
+        if version == 1
+        else generate_entropy_encoding2()
+    )
     for character in b32encode(data):
         data_encoded.append(choice(encoding[character]))
 
     return data_encoded
 
 
-def entropy_decode(data: bytes) -> bytes:
+def entropy_encode2(data: bytes) -> bytes:
+    """
+    Call entropy_encode with version 2.
+    """
+
+    return entropy_encode(data, version=2)
+
+
+def entropy_decode(data: bytes, version: int = 1) -> bytes:
     """
     This function decodes entropy-encoding to retrieve
     data from entropy-encoded data.
+
+    version should be 1 or 2.
     """
 
-    data, encoding = get_entropy_encoding(data)
+    data, encoding = (
+        get_entropy_encoding(data)
+        if version == 1
+        else get_entropy_encoding2(data)
+    )
     data_decoded = bytearray()
     for character in data:
         data_decoded.append(encoding[character])
 
     return b32decode(data_decoded)
 
 
+def entropy_decode2(data: bytes) -> bytes:
+    """
+    Call entropy_decode with version 2.
+    """
+
+    return entropy_decode(data, version=2)
+
+
 def shannon_entropy(data: bytes) -> float:
     """
     This function returns the shannon entropy for bytes.
 
     Greater entropy = more randomness
     Max entropy: 8
     Min entropy: 0
@@ -305,31 +413,46 @@
         p = frequency[key] / data_length
         entropy -= p * log(p, 2)
 
     return entropy
 
 
 def test():
-    # For test i use:
+    # For test i use librc4 to encrypt data to get higher entropy:
     #     - https://github.com/mauricelambert/FastRC4/releases/download/v0.0.1/librc4.dll
     #     - https://github.com/mauricelambert/FastRC4/releases/download/v0.0.1/librc4.so
     #     - https://raw.githubusercontent.com/mauricelambert/FastRC4/main/librc4.py
 
     from urllib.request import urlopen
     from shutil import copyfileobj
     from os import remove, name
 
     with open("librc4.dll", "wb") as file:
-        copyfileobj(urlopen("https://github.com/mauricelambert/FastRC4/releases/download/v0.0.1/librc4.dll"), file)
+        copyfileobj(
+            urlopen(
+                "https://github.com/mauricelambert/FastRC4/releases/download/v0.0.1/librc4.dll"
+            ),
+            file,
+        )
 
     with open("librc4.so", "wb") as file:
-        copyfileobj(urlopen("https://github.com/mauricelambert/FastRC4/releases/download/v0.0.1/librc4.so"), file)
+        copyfileobj(
+            urlopen(
+                "https://github.com/mauricelambert/FastRC4/releases/download/v0.0.1/librc4.so"
+            ),
+            file,
+        )
 
     with open("librc4.py", "wb") as file:
-        copyfileobj(urlopen("https://raw.githubusercontent.com/mauricelambert/FastRC4/main/librc4.py"), file)
+        copyfileobj(
+            urlopen(
+                "https://raw.githubusercontent.com/mauricelambert/FastRC4/main/librc4.py"
+            ),
+            file,
+        )
 
     from librc4 import RC4
 
     rc4 = RC4(b"my secret key")
     print("Entropy for non-encoded secrets:", shannon_entropy(secrets))
     encrypted_data = rc4.encrypt(secrets)
     print(
@@ -337,28 +460,38 @@
         shannon_entropy(encrypted_data),
     )
     data = entropy_encode(encrypted_data)
     print(
         "Entropy for entropy-encoded encrypted secrets:", shannon_entropy(data)
     )
     assert encrypted_data == entropy_decode(data)
+    data = entropy_encode2(encrypted_data)
+    print(
+        "Entropy for entropy-encoded2 encrypted secrets:",
+        shannon_entropy(data),
+    )
+    assert encrypted_data == entropy_decode2(data)
 
     rc4 = RC4(b"my secret key")
     print("Entropy for non-encoded exe:", shannon_entropy(dll))
     encrypted_data = rc4.encrypt(dll)
     print(
         "Entropy for non-encoded encrypted exe:",
         shannon_entropy(encrypted_data),
     )
     data = entropy_encode(encrypted_data)
     print("Entropy for entropy-encoded encrypted exe:", shannon_entropy(data))
     assert encrypted_data == entropy_decode(data)
+    data = entropy_encode2(encrypted_data)
+    print("Entropy for entropy-encoded2 encrypted exe:", shannon_entropy(data))
+    assert encrypted_data == entropy_decode2(data)
 
     if name == "nt":
         from ctypes import windll
+
         windll.kernel32.FreeLibrary(".\\librc4.dll")
 
     remove("librc4.py")
     remove("librc4.so")
     remove("librc4.dll")
```

### Comparing `EntropyEncoding-0.0.2/LICENSE.txt` & `EntropyEncoding-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EntropyEncoding-0.0.2/PKG-INFO` & `EntropyEncoding-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EntropyEncoding
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package implements an encoding to bypass entropy antivirus check.
 Home-page: https://github.com/mauricelambert/EntropyEncoding
 Author: Maurice Lambert
 Author-email: Maurice Lambert <mauricelambert434@gmail.com>
 Maintainer: Maurice Lambert
 Maintainer-email: Maurice Lambert <mauricelambert434@gmail.com>
 License: GPL-3.0 License
@@ -29,20 +29,28 @@
 Classifier: Topic :: System :: Systems Administration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+![EntropyEncoding logo](https://mauricelambert.github.io/info/python/security/EntropyEncoding.gif "EntropyEncoding logo")
+
 # EntropyEncoding
 
 ## Description
 
 This package implements an encoding to bypass entropy antivirus check.
 
+I have researched about entropy bypass techniques and found people who use adding low-entropy data to bypass entropy check. I think adding data can be optimized and more efficient with a simple entropy encoding to reduce entropy score.
+
+Adding low-entropy data:
+ 1. you get a larger file
+ 2. you do not change payload entropy (if the antivirus software splits the file for entropy calculation, it will probably have high entropy on a payload chunk)
+
 ## Requirements
 
 This package require:
  - python3
  - python3 Standard Library
 
 ## Installation
@@ -58,20 +66,34 @@
 ```
 
 ## Usages
 
 ```python
 from EntropyEncoding import *
 
+print(shannon_entropy(b"shellcode_payload"))
 encoded_shellcode = entropy_encode(b"shellcode_payload")
 print(encoded_shellcode)
 
 entropy_decode(encoded_shellcode) == b"shellcode_payload"
 
-print(shannon_entropy)
+print(shannon_entropy(encoded_shellcode))
+```
+
+Tests results:
+
+```
+~# python3 EntropyEncoding.py
+Entropy for non-encoded secrets: 4.521591372417719
+Entropy for non-encoded encrypted secrets: 7.951320327821406
+Entropy for entropy-encoded encrypted secrets: 5.774096152750044
+Entropy for non-encoded exe: 5.22055339277441
+Entropy for non-encoded encrypted exe: 7.914685739354301
+Entropy for entropy-encoded encrypted exe: 5.759477906043907
+~# 
 ```
 
 ## Links
 
  - [Pypi](https://pypi.org/project/EntropyEncoding)
  - [Github](https://github.com/mauricelambert/EntropyEncoding)
  - [Documentation](https://user.github.io/info/python/security/EntropyEncoding.html)
```

### Comparing `EntropyEncoding-0.0.2/pyproject.toml` & `EntropyEncoding-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EntropyEncoding"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = []
 authors = [
     {name = "Maurice Lambert", email = "mauricelambert434@gmail.com"},
 ]
 maintainers = [
     {name = "Maurice Lambert", email = "mauricelambert434@gmail.com"},
 ]
```

### Comparing `EntropyEncoding-0.0.2/setup.cfg` & `EntropyEncoding-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EntropyEncoding
-version = 0.0.2
+version = 0.0.3
 author = Maurice Lambert
 author_email = mauricelambert434@gmail.com
 maintainer = Maurice Lambert
 maintainer_email = mauricelambert434@gmail.com
 description = This package implements an encoding to bypass entropy antivirus check.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `EntropyEncoding-0.0.2/setup.py` & `EntropyEncoding-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 from setuptools import setup, find_packages
 import EntropyEncoding as package
 
 setup(
-    name='EntropyEncoding',
+    name="EntropyEncoding",
     version=package.__version__,
-    py_modules=['EntropyEncoding'],
+    py_modules=["EntropyEncoding"],
     packages=find_packages(include=[]),
     install_requires=[],
     scripts=[],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
-    description='This package implements an encoding to bypass entropy antivirus check.',
-    long_description=open('README.md').read(),
+    description="This package implements an encoding to bypass entropy antivirus check.",
+    long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mauricelambert/EntropyEncoding",
     project_urls={
         "Github": "https://github.com/mauricelambert/EntropyEncoding",
         "Documentation": "https://user.github.io/info/python/security/EntropyEncoding.html",
     },
     include_package_data=True,
     classifiers=[
         "Topic :: System",
         "Topic :: Security",
         "Environment :: Console",
         "Topic :: System :: Shells",
-        'Operating System :: POSIX',
+        "Operating System :: POSIX",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Intended Audience :: Developers",
         "Topic :: System :: System Shells",
-        'Operating System :: MacOS :: MacOS X',
+        "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3.8",
-        'Operating System :: Microsoft :: Windows',
+        "Operating System :: Microsoft :: Windows",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     ],
-    keywords=['entropy', 'antivirus-bypass', 'payload-encoding', 'encoding', 'malware'],
-    platforms=['Windows', 'Linux', "MacOS"],
+    keywords=[
+        "entropy",
+        "antivirus-bypass",
+        "payload-encoding",
+        "encoding",
+        "malware",
+    ],
+    platforms=["Windows", "Linux", "MacOS"],
     license="GPL-3.0 License",
-    python_requires='>=3.8',
-)
+    python_requires=">=3.8",
+)
```

