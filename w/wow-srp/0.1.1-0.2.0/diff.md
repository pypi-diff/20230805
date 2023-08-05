# Comparing `tmp/wow_srp-0.1.1.tar.gz` & `tmp/wow_srp-0.2.0.tar.gz`

## Comparing `wow_srp-0.1.1.tar` & `wow_srp-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 wow_srp-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-07-21 19:52:59.000000 wow_srp-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-21 19:52:59.000000 wow_srp-0.1.1/.gitignore
--rw-r--r--   0     1001      123      649 2023-07-21 19:52:59.000000 wow_srp-0.1.1/CHANGELOG.md
--rw-r--r--   0     1001      123    11336 2023-07-21 19:52:59.000000 wow_srp-0.1.1/LICENSE-APACHE
--rw-r--r--   0     1001      123     1045 2023-07-21 19:52:59.000000 wow_srp-0.1.1/LICENSE-MIT
--rw-r--r--   0     1001      123     4318 2023-07-21 19:52:59.000000 wow_srp-0.1.1/README.md
--rw-r--r--   0     1001      123      598 2023-07-21 19:52:59.000000 wow_srp-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123     3241 2023-07-21 19:52:59.000000 wow_srp-0.1.1/src/client.rs
--rw-r--r--   0     1001      123     4758 2023-07-21 19:52:59.000000 wow_srp-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123     4238 2023-07-21 19:52:59.000000 wow_srp-0.1.1/src/server.rs
--rwxr-xr-x   0     1001      123     1145 2023-07-21 19:52:59.000000 wow_srp-0.1.1/test.py
--rw-r--r--   0     1001      123    12720 2023-07-21 19:52:59.000000 wow_srp-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     4974 1970-01-01 00:00:00.000000 wow_srp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 wow_srp-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-08-05 11:54:01.000000 wow_srp-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-08-05 11:54:01.000000 wow_srp-0.2.0/.gitignore
+-rw-r--r--   0     1001      123      813 2023-08-05 11:54:01.000000 wow_srp-0.2.0/CHANGELOG.md
+-rw-r--r--   0     1001      123    11336 2023-08-05 11:54:01.000000 wow_srp-0.2.0/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1045 2023-08-05 11:54:01.000000 wow_srp-0.2.0/LICENSE-MIT
+-rw-r--r--   0     1001      123     6069 2023-08-05 11:54:01.000000 wow_srp-0.2.0/README.md
+-rw-r--r--   0     1001      123      580 2023-08-05 11:54:01.000000 wow_srp-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     3241 2023-08-05 11:54:01.000000 wow_srp-0.2.0/src/client.rs
+-rw-r--r--   0     1001      123     7268 2023-08-05 11:54:01.000000 wow_srp-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     4238 2023-08-05 11:54:01.000000 wow_srp-0.2.0/src/server.rs
+-rw-r--r--   0     1001      123     2754 2023-08-05 11:54:01.000000 wow_srp-0.2.0/src/tbc_header.rs
+-rw-r--r--   0     1001      123     2766 2023-08-05 11:54:01.000000 wow_srp-0.2.0/src/vanilla_header.rs
+-rw-r--r--   0     1001      123     3548 2023-08-05 11:54:01.000000 wow_srp-0.2.0/src/wrath_header.rs
+-rwxr-xr-x   0     1001      123     3352 2023-08-05 11:54:01.000000 wow_srp-0.2.0/test.py
+-rw-r--r--   0     1001      123    12720 2023-08-05 11:54:01.000000 wow_srp-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 wow_srp-0.2.0/PKG-INFO
```

### Comparing `wow_srp-0.1.1/Cargo.toml` & `wow_srp-0.2.0/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "wow_srp_python"
-version = "0.1.0"
+version = "0.2.0"
 edition = "2021"
 repository = "https://www.github.com/gtker/wow_srp_python"
 authors = ["Gtker <github@gtker.com>"]
 description = "Server and client library for the World of Warcraft flavor of SRP6 with support for reconnection."
 license = "MIT OR Apache-2.0"
 readme = "README.md"
```

### Comparing `wow_srp-0.1.1/.github/workflows/CI.yml` & `wow_srp-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `wow_srp-0.1.1/.gitignore` & `wow_srp-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wow_srp-0.1.1/LICENSE-APACHE` & `wow_srp-0.2.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `wow_srp-0.1.1/LICENSE-MIT` & `wow_srp-0.2.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `wow_srp-0.1.1/pyproject.toml` & `wow_srp-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "wow_srp"
-version = "0.1.1"
 description = "Cryptography library for authenticating with World of Warcraft 1.2-3.3.5 clients."
 authors = [{name = "Gtker", email = "pip@gtker.com"}]
 requires-python = ">=3.7"
 license = { file = "LICENSE-MIT" }
 keywords = ["wow", "srp"]
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `wow_srp-0.1.1/src/client.rs` & `wow_srp-0.2.0/src/client.rs`

 * *Files identical despite different names*

### Comparing `wow_srp-0.1.1/src/server.rs` & `wow_srp-0.2.0/src/server.rs`

 * *Files identical despite different names*

### Comparing `wow_srp-0.1.1/Cargo.lock` & `wow_srp-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -474,12 +474,12 @@
  "rand",
  "rc4",
  "sha-1",
 ]
 
 [[package]]
 name = "wow_srp_python"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "wow_srp",
 ]
```

### Comparing `wow_srp-0.1.1/PKG-INFO` & `wow_srp-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow_srp
-Version: 0.1.1
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE-MIT
 License-File: LICENSE-APACHE
 Summary: Cryptography library for authenticating with World of Warcraft 1.2-3.3.5 clients.
 Keywords: wow,srp
@@ -17,19 +17,29 @@
 
 # `wow_srp` for Python
 
 SRP6 library for Python that supports WoW version 1.2 through to 3.3.5.
 
 This is just a Python wrapper [around the original `wow_srp` library](https://github.com/gtker/wow_srp).
 
+# Installation
+
+Install from [PyPI](https://pypi.org/project/wow-srp/) with pip:
+
+```bash
+pip install wow-srp
+```
+
 # Usage
 
+## Authentication
+
 The module is split into functionality used by a server implementation and a client implementation.
 
-## Server
+### Server
 
 ```text
 SrpVerifier -> SrpProof -> SrpServer
 ```
 
 You will only want to save the username, salt, and password verifier for an account.
 Do not save the raw passwords on the server.
@@ -89,15 +99,15 @@
 
 ```python
 >>> client_challenge_data = [0] * 16 # Arbitrary data to show usage
 >>> client_proof = [0] * 20 # Arbitrary data to show usage
 >>> # reconnect_valid = server.verify_reconnection_attempt(client_challenge_data, client_proof)
 ```
 
-## Client
+### Client
 
 ```text
 SrpClientUser -> SrpClientChallenge -> SrpClient | -> SrpClientReconnection
 ```
 The `SrpClientReconnection` is just a data struct that contains reconnection values.
 
 The client does not have to save any values except for the username and password.
@@ -140,22 +150,78 @@
 And then access the reconnect values from `reconnect_data`:
 
 ```python
 >>> # challenge_data = reconnect_data.challenge_data()
 >>> # client_proof = reconnect_data.client_proof()
 ```
 
-## Development
+## Header Encryption
+
+### Server
+
+First, create a `ProofSeed` from for the version that you need:
+
+```python
+>>> server_seed = vanilla_header.ProofSeed()
+>>> server_seed_value = server_seed.seed()
+```
+
+Then send the value to the client in
+[SMSG_AUTH_CHALLENGE](https://gtker.com/wow_messages/docs/smsg_auth_challenge.html).
+
+After receiving [CMSG_AUTH_SESSION](https://gtker.com/wow_messages/docs/cmsg_auth_session.html)
+from the client, convert the proof to a `HeaderCrypto`.
+
+```python
+>>> # server_crypto = server_seed.into_server_header_crypto(username, session_key, client_proof, client_seed)
+```
+
+You can then encrypt and decrypt message headers with
+
+```python
+>>> # data = server_crypto.encrypt_server_header(size, opcode)
+>>> # size, opcode = server_crypto.decrypt_client_header(data)
+```
+
+### Client
+
+First, create a `ProofSeed` from for the version that you need:
+
+```python
+>>> client_seed = vanilla_header.ProofSeed()
+>>> client_seed_value = client_seed.seed()
+```
+
+Then convert the seed to a `HeaderCrypto` using the seed received from
+[SMSG_AUTH_CHALLENGE](https://gtker.com/wow_messages/docs/smsg_auth_challenge.html).
+
+```python
+>>> # client_proof, client_crypto = client_seed.into_client_header_crypto(username, session_key, server_seed)
+```
+
+Then send the `client_proof` and `client_seed_value` to the server through
+[CMSG_AUTH_SESSION](https://gtker.com/wow_messages/docs/cmsg_auth_session.html).
+
+You can then encrypt and decrypt message headers with
+
+```python
+>>> # data = client_crypto.encrypt_client_header(size, opcode)
+>>> # size, opcode = client_crypto.decrypt_server_header(data)
+```
+
+# Development
 
 ```bash
 pip install maturin
 curl https://pyenv.run | bash
+
 # For fish
 set -U PYENV_ROOT "$HOME/.pyenv"
 fish_add_path "$PYENV_ROOT/bin"
+
 pyenv init - | source
 pyenv install 3.10
 pyenv virtualenv 3.10 pyo3
 pyenv activate pyo3
 maturin develop
 ```
```

