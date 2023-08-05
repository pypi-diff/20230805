# Comparing `tmp/lazrs-0.5.1.tar.gz` & `tmp/lazrs-0.5.2.tar.gz`

## Comparing `lazrs-0.5.1.tar` & `lazrs-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 lazrs-0.5.1/Cargo.toml
--rw-r--r--   0     1001      123     4823 2023-07-16 17:29:45.000000 lazrs-0.5.1/.github/workflows/build.yml
--rw-r--r--   0     1001      123       54 2023-07-16 17:29:45.000000 lazrs-0.5.1/.gitignore
--rw-r--r--   0     1001      123     1077 2023-07-16 17:29:45.000000 lazrs-0.5.1/LICENSE.txt
--rw-r--r--   0     1001      123      305 2023-07-16 17:29:45.000000 lazrs-0.5.1/README.md
--rw-r--r--   0     1001      123      715 2023-07-16 17:29:45.000000 lazrs-0.5.1/noxfile.py
--rw-r--r--   0     1001      123      233 2023-07-16 17:29:45.000000 lazrs-0.5.1/pyproject.toml
--rw-r--r--   0     1001      123     5522 2023-07-16 17:29:45.000000 lazrs-0.5.1/src/adapters.rs
--rw-r--r--   0     1001      123    17058 2023-07-16 17:29:45.000000 lazrs-0.5.1/src/lib.rs
--rw-r--r--   0     1001      123    10511 2023-07-16 17:29:54.000000 lazrs-0.5.1/Cargo.lock
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 lazrs-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 lazrs-0.5.2/Cargo.toml
+-rw-r--r--   0     1001      123     4823 2023-08-05 12:21:55.000000 lazrs-0.5.2/.github/workflows/build.yml
+-rw-r--r--   0     1001      123       54 2023-08-05 12:21:55.000000 lazrs-0.5.2/.gitignore
+-rw-r--r--   0     1001      123     1077 2023-08-05 12:21:55.000000 lazrs-0.5.2/LICENSE.txt
+-rw-r--r--   0     1001      123      305 2023-08-05 12:21:55.000000 lazrs-0.5.2/README.md
+-rw-r--r--   0     1001      123      715 2023-08-05 12:21:55.000000 lazrs-0.5.2/noxfile.py
+-rw-r--r--   0     1001      123      235 2023-08-05 12:21:55.000000 lazrs-0.5.2/pyproject.toml
+-rw-r--r--   0     1001      123     5523 2023-08-05 12:21:55.000000 lazrs-0.5.2/src/adapters.rs
+-rw-r--r--   0     1001      123    17254 2023-08-05 12:21:55.000000 lazrs-0.5.2/src/lib.rs
+-rw-r--r--   0     1001      123    10276 2023-08-05 12:22:01.000000 lazrs-0.5.2/Cargo.lock
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 lazrs-0.5.2/PKG-INFO
```

### Comparing `lazrs-0.5.1/.github/workflows/build.yml` & `lazrs-0.5.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lazrs-0.5.1/LICENSE.txt` & `lazrs-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lazrs-0.5.1/noxfile.py` & `lazrs-0.5.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `lazrs-0.5.1/src/adapters.rs` & `lazrs-0.5.2/src/adapters.rs`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                     .map_err(|_err| {
                         std::io::Error::new(
                             std::io::ErrorKind::Other,
                             format!("Failed to call read"),
                         )
                     })?;
 
-                match object.cast_as::<pyo3::types::PyBytes>(py) {
+                match object.downcast::<pyo3::types::PyBytes>(py) {
                     Ok(py_bytes) => {
                         let read_bytes = py_bytes.as_bytes();
                         let shortest = std::cmp::min(buf.len(), read_bytes.len());
                         buf[..shortest].copy_from_slice(read_bytes);
                         Ok(read_bytes.len())
                     }
                     Err(_) => Err(std::io::Error::new(
```

### Comparing `lazrs-0.5.1/src/lib.rs` & `lazrs-0.5.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 struct ParLasZipDecompressor {
     decompressor: laz::ParLasZipDecompressor<BufReader<PyReadableFileObject>>,
 }
 
 #[pymethods]
 impl ParLasZipDecompressor {
     #[new]
-    #[args(selection = "None")]
+    #[pyo3(signature=(source, vlr_record_data, selection = None))]
     fn new(
         source: PyObject,
         vlr_record_data: &PyAny,
         selection: Option<DecompressionSelection>,
     ) -> PyResult<Self> {
         Python::with_gil(|py| {
             let source = BufReader::new(PyReadableFileObject::new(py, source)?);
@@ -209,15 +209,15 @@
 struct LasZipDecompressor {
     decompressor: laz::LasZipDecompressor<'static, BufReader<PyReadableFileObject>>,
 }
 
 #[pymethods]
 impl LasZipDecompressor {
     #[new]
-    #[args(selection = "None")]
+    #[pyo3(signature = (source, record_data, selection = None))]
     pub fn new(
         source: PyObject,
         record_data: &PyAny,
         selection: Option<DecompressionSelection>,
     ) -> PyResult<Self> {
         Python::with_gil(|py| {
             let source = BufReader::new(PyReadableFileObject::new(py, source)?);
@@ -345,15 +345,22 @@
                 laz::par_decompress_buffer(data_slc, output, &vlr)
             }
         })
         .map_err(into_py_err)?;
     Ok(())
 }
 
-#[pyfunction(selection = "None")]
+#[pyfunction]
+#[pyo3(signature = (
+    compressed_points_data,
+    laszip_vlr_record_data,
+    decompression_output,
+    py_chunk_table,
+    selection = None
+))]
 fn decompress_points_with_chunk_table(
     compressed_points_data: &PyAny,
     laszip_vlr_record_data: &PyAny,
     decompression_output: &PyAny,
     py_chunk_table: &PyList,
     selection: Option<DecompressionSelection>,
 ) -> PyResult<()> {
```

### Comparing `lazrs-0.5.1/Cargo.lock` & `lazrs-0.5.2/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -52,32 +52,32 @@
 version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.9.0",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "hermit-abi"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
@@ -85,26 +85,26 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "laz"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78438fec528e9c26c15001f3d64ecfe1daef73a41a20a268037f748248c0c51e"
+checksum = "3d1dfc0faf3b57f11d2ada8e704640fa593688216aacbf8e92f5c0ee6187b05a"
 dependencies = [
  "byteorder",
  "num-traits",
  "rayon",
 ]
 
 [[package]]
 name = "lazrs"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "laz",
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
@@ -120,35 +120,26 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -186,86 +177,86 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.65"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92de25114670a878b1261c79c9f8f729fb97e95bac93f6312f583c60dd6a1dfe"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.30"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5907a1b7c277254a8b15170f6e7c97cfa60ee7872a3217663bb81151e48184bb"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rayon"
 version = "1.7.0"
@@ -295,17 +286,17 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
@@ -318,17 +309,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.9"
+version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
+checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
```

### Comparing `lazrs-0.5.1/PKG-INFO` & `lazrs-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazrs
-Version: 0.5.1
+Version: 0.5.2
 License-File: LICENSE.txt
 Summary: Python bindings for laz-rs
 Author: tmontaigu <thomas.montaigu@laposte.net>
 Author-email: tmontaigu <thomas.montaigu@laposte.net>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

