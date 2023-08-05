# Comparing `tmp/pypomes_crypto-0.1.4.tar.gz` & `tmp/pypomes_crypto-0.1.5.tar.gz`

## Comparing `pypomes_crypto-0.1.4.tar` & `pypomes_crypto-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/src/pypomes_crypto/__init__.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pkcs7.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pomes.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/README.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/src/pypomes_crypto/__init__.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/src/pypomes_crypto/crypto_pkcs7.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/src/pypomes_crypto/crypto_pomes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/README.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.5/PKG-INFO
```

### Comparing `pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pkcs7.py` & `pypomes_crypto-0.1.5/src/pypomes_crypto/crypto_pkcs7.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from asn1crypto import cms
 from datetime import datetime
-from cryptography import x509
 from cryptography.hazmat.primitives.serialization import pkcs7, Encoding, PublicFormat
+from pathlib import Path
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from cryptography import x509
 
 
 class Pkcs7Data:
     """Python code to extract relevant data from a PKCS#7 signature file."""
 
     # class attributes
     payload: bytes                       # the original payload
@@ -22,25 +26,23 @@
         Instantiate the PKCS#7 crypto class, and extract the relevant data.
 
         :param p7s_file: a p7s file path or the p7s file bytes
         """
         # is the input argument a file path ?
         if isinstance(p7s_file, str):
             # yes, load pkcs#7 data from file
-            with open(p7s_file, "rb") as f:
+            with Path.open(Path(p7s_file), "rb") as f:
                 p7s_bytes: bytes = f.read()
         else:
             # no, it holds the pkcs#7 data
             p7s_bytes = p7s_file
 
         # extract the certificate chain and serialize it in PEM format
-        self.cert_chain = []
         certs: list[x509.Certificate] = pkcs7.load_der_pkcs7_certificates(p7s_bytes)
-        for cert in certs:
-            self.cert_chain.append(cert.public_bytes(Encoding.PEM))
+        self.cert_chain = [cert.public_bytes(Encoding.PEM) for cert in certs]
 
         #  extract the public key and serialize it in PEM format
         cert: x509.Certificate = certs[-1]
         self.public_key = cert.public_key().public_bytes(Encoding.PEM, PublicFormat.SubjectPublicKeyInfo)
 
         # extract the needed structures
         content_info: cms.ContentInfo = cms.ContentInfo.load(p7s_bytes)
```

### Comparing `pypomes_crypto-0.1.4/src/pypomes_crypto/crypto_pomes.py` & `pypomes_crypto-0.1.5/src/pypomes_crypto/crypto_pomes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import hashlib
-import os
+from pathlib import Path
 from typing import Final
 from pypomes_core import APP_PREFIX, env_get_str
 
 CRYPTO_HASH_ALGORITHM: Final[str] = env_get_str(f"{APP_PREFIX}_DEFAULT_HASH_ALGORITHM", "sha256")
 
 
-def crypto_hash(msg: str | bytes, alg: str = CRYPTO_HASH_ALGORITHM) -> bytes:
+def crypto_hash(msg: Path | str | bytes, alg: str = CRYPTO_HASH_ALGORITHM) -> bytes:
     """
     Compute the hash of *msg*, using the algorithm specified in *alg*.
 
     Return *None* if computing the hash not possible.
     Supported algorithms: md5, blake2b, blake2s, sha1, sha224, sha256, sha384 sha512,
     sha3_224, sha3_256, sha3_384, sha3_512, shake_128, shake_256.
 
@@ -21,18 +21,18 @@
     hasher = hashlib.new(alg.lower())
 
     # what is the type of the argument ?
     if isinstance(msg, bytes):
         # argument is type 'bytes'
         hasher.update(msg)
 
-    elif os.path.isfile(msg):
+    elif Path.is_file(Path(msg)):
         # argument is the path to a file
         buf_size: int = 128 * 1024
-        with open(msg, "rb") as f:
+        with Path.open(Path(msg), "rb") as f:
             while True:
                 file_bytes: bytes = f.read(buf_size)
                 if not file_bytes:
                     break
                 hasher.update(file_bytes)
 
     return hasher.digest()
```

### Comparing `pypomes_crypto-0.1.4/LICENSE` & `pypomes_crypto-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_crypto-0.1.4/pyproject.toml` & `pypomes_crypto-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_crypto"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (cryptography modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,15 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "asn1crypto>=1.5.1",
     "cryptography>=41.0.2",
     "pip>=23.3.1",
-    "pypomes_core>=0.2.1",
+    "pypomes_core>=0.2.3",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Crypto"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Crypto/issues"
```

### Comparing `pypomes_crypto-0.1.4/PKG-INFO` & `pypomes_crypto-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pypomes_crypto
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of Python pomes, pennyeach (cryptography modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Crypto
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Crypto/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: asn1crypto>=1.5.1
 Requires-Dist: cryptography>=41.0.2
 Requires-Dist: pip>=23.3.1
-Requires-Dist: pypomes-core>=0.2.1
+Requires-Dist: pypomes-core>=0.2.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

