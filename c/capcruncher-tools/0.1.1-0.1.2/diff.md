# Comparing `tmp/capcruncher_tools-0.1.1.tar.gz` & `tmp/capcruncher_tools-0.1.2.tar.gz`

## Comparing `capcruncher_tools-0.1.1.tar` & `capcruncher_tools-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 capcruncher_tools-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2313 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/.github/workflows/cd_workflow.yml
--rw-r--r--   0     1001      123     2435 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/.github/workflows/ci_workflow.yml
--rw-r--r--   0     1001      123       19 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/.gitignore
--rw-r--r--   0     1001      123    35149 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/LICENSE
--rw-r--r--   0     1001      123     1089 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/README.md
--rw-r--r--   0     1001      123       10 2023-06-26 13:34:33.000000 capcruncher_tools-0.1.1/dist/capcruncher_tools-0.1.1.tar.gz
--rw-r--r--   0     1001      123      962 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123      151 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/python/capcruncher_tools/__init__.py
--rw-r--r--   0     1001      123    10406 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/python/capcruncher_tools/cli.py
--rw-r--r--   0     1001      123      767 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/python/capcruncher_tools/count.py
--rw-r--r--   0     1001      123    11528 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/src/fastq_deduplication.rs
--rw-r--r--   0     1001      123     8167 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/src/genome_digest.rs
--rw-r--r--   0     1001      123     2127 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/src/interactions_count.rs
--rw-r--r--   0     1001      123     2995 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123     1549 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/src/utils.rs
--rw-r--r--   0     1001      123    99395 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/tests/fastq_deduplicate/duplicated_1.fastq.gz
--rw-r--r--   0     1001      123    99395 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/tests/fastq_deduplicate/duplicated_2.fastq.gz
--rw-r--r--   0     1001      123     1523 2023-06-26 13:34:17.000000 capcruncher_tools-0.1.1/tests/test_deduplicate.py
--rw-r--r--   0     1001      123    72872 2023-06-26 13:34:28.000000 capcruncher_tools-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 capcruncher_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 capcruncher_tools-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     2313 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/.github/workflows/cd_workflow.yml
+-rw-r--r--   0     1001      123     2435 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/.github/workflows/ci_workflow.yml
+-rw-r--r--   0     1001      123       19 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/.gitignore
+-rw-r--r--   0     1001      123    35149 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/LICENSE
+-rw-r--r--   0     1001      123     1089 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/README.md
+-rw-r--r--   0     1001      123       10 2023-06-29 16:05:31.000000 capcruncher_tools-0.1.2/dist/capcruncher_tools-0.1.2.tar.gz
+-rw-r--r--   0     1001      123      972 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123      151 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/python/capcruncher_tools/__init__.py
+-rw-r--r--   0     1001      123    10406 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/python/capcruncher_tools/cli.py
+-rw-r--r--   0     1001      123      767 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/python/capcruncher_tools/count.py
+-rw-r--r--   0     1001      123    11528 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/src/fastq_deduplication.rs
+-rw-r--r--   0     1001      123     8167 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/src/genome_digest.rs
+-rw-r--r--   0     1001      123     2127 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/src/interactions_count.rs
+-rw-r--r--   0     1001      123     2995 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123     1549 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/src/utils.rs
+-rw-r--r--   0     1001      123    99395 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/tests/fastq_deduplicate/duplicated_1.fastq.gz
+-rw-r--r--   0     1001      123    99395 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/tests/fastq_deduplicate/duplicated_2.fastq.gz
+-rw-r--r--   0     1001      123     1523 2023-06-29 16:05:16.000000 capcruncher_tools-0.1.2/tests/test_deduplicate.py
+-rw-r--r--   0     1001      123    74021 2023-06-29 16:05:27.000000 capcruncher_tools-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1654 1970-01-01 00:00:00.000000 capcruncher_tools-0.1.2/PKG-INFO
```

### Comparing `capcruncher_tools-0.1.1/Cargo.toml` & `capcruncher_tools-0.1.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/.github/workflows/cd_workflow.yml` & `capcruncher_tools-0.1.2/.github/workflows/cd_workflow.yml`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/.github/workflows/ci_workflow.yml` & `capcruncher_tools-0.1.2/.github/workflows/ci_workflow.yml`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/LICENSE` & `capcruncher_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/README.md` & `capcruncher_tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/pyproject.toml` & `capcruncher_tools-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 authors = [{ name = "asmith" }, { email = "alastair.smith@ndcls.ox.ac.uk" }]
-dependencies = ["click", "toml>=0.10.0", "pandas", "tabulate", "loguru", "capcruncher", "ray", "pyranges"]
+dependencies = ["click", "toml>=0.10.0", "pandas", "tabulate", "loguru", "capcruncher", "ray", "pyranges", "polars"]
 name = "capcruncher-tools"
-version = "0.1.1"
+version = "0.1.2"
 description = "Extra utilities to enhance CapCruncher"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 # dynamic = ["version", "dependencies"]
```

### Comparing `capcruncher_tools-0.1.1/python/capcruncher_tools/cli.py` & `capcruncher_tools-0.1.2/python/capcruncher_tools/cli.py`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/python/capcruncher_tools/count.py` & `capcruncher_tools-0.1.2/python/capcruncher_tools/count.py`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/src/fastq_deduplication.rs` & `capcruncher_tools-0.1.2/src/fastq_deduplication.rs`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/src/genome_digest.rs` & `capcruncher_tools-0.1.2/src/genome_digest.rs`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/src/interactions_count.rs` & `capcruncher_tools-0.1.2/src/interactions_count.rs`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/src/lib.rs` & `capcruncher_tools-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/src/utils.rs` & `capcruncher_tools-0.1.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/tests/fastq_deduplicate/duplicated_1.fastq.gz` & `capcruncher_tools-0.1.2/tests/fastq_deduplicate/duplicated_1.fastq.gz`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/tests/fastq_deduplicate/duplicated_2.fastq.gz` & `capcruncher_tools-0.1.2/tests/fastq_deduplicate/duplicated_2.fastq.gz`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/tests/test_deduplicate.py` & `capcruncher_tools-0.1.2/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `capcruncher_tools-0.1.1/Cargo.lock` & `capcruncher_tools-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a76fd60b23679b7d19bd066031410fb7e458ccc5e958eb5c325888ce4baedc97"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
@@ -189,14 +198,29 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "backtrace"
+version = "0.3.67"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide 0.6.2",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bgzip"
@@ -744,15 +768,15 @@
 name = "flate2"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "libz-sys",
- "miniz_oxide",
+ "miniz_oxide 0.7.1",
 ]
 
 [[package]]
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
@@ -877,14 +901,20 @@
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "hash_hasher"
@@ -923,23 +953,14 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "home"
 version = "0.5.5"
@@ -1013,15 +1034,15 @@
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
- "hermit-abi 0.3.1",
+ "hermit-abi",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
@@ -1260,14 +1281,23 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+dependencies = [
+ "adler",
+]
+
+[[package]]
+name = "miniz_oxide"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
@@ -1500,29 +1530,38 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
+name = "object"
+version = "0.30.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "03b4680b86d9cfafba8fc491dc9b6df26b68cf40e9e6cd73909194759a63c385"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "ordered-float"
@@ -1574,15 +1613,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.3.5",
  "smallvec",
- "windows-targets 0.48.0",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "parquet-format-safe"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
@@ -2030,17 +2069,17 @@
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -2147,14 +2186,20 @@
 [[package]]
 name = "regex-syntax"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustc_version"
@@ -2522,19 +2567,20 @@
  "proc-macro2",
  "quote",
  "syn 2.0.22",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "374442f06ee49c3a28a8fc9f01a2596fed7559c6b99b31279c3261778e77d84f"
 dependencies = [
  "autocfg",
+ "backtrace",
  "libc",
  "mio",
  "pin-project-lite",
  "socket2",
  "windows-sys 0.48.0",
 ]
 
@@ -2731,15 +2777,15 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
@@ -2749,15 +2795,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -2769,17 +2815,17 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.0",
  "windows_aarch64_msvc 0.48.0",
  "windows_i686_gnu 0.48.0",
  "windows_i686_msvc 0.48.0",
  "windows_x86_64_gnu 0.48.0",
  "windows_x86_64_gnullvm 0.48.0",
```

### Comparing `capcruncher_tools-0.1.1/PKG-INFO` & `capcruncher_tools-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: capcruncher-tools
-Version: 0.1.1
+Version: 0.1.2
 Requires-Dist: click
 Requires-Dist: toml >=0.10.0
 Requires-Dist: pandas
 Requires-Dist: tabulate
 Requires-Dist: loguru
 Requires-Dist: capcruncher
 Requires-Dist: ray
 Requires-Dist: pyranges
+Requires-Dist: polars
 License-File: LICENSE
 Summary: Extra utilities to enhance CapCruncher
 Author: asmith
 Author-email: alastair.smith@ndcls.ox.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/alsmith151/CapCruncherTools
```

