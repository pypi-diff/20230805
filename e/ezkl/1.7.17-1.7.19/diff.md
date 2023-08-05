# Comparing `tmp/ezkl-1.7.17-cp37-abi3-win_amd64.whl.zip` & `tmp/ezkl-1.7.19-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10115962 bytes, number of entries: 6
--rw-r--r--  4.6 unx     5930 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/WHEEL
--rw-r--r--  4.6 unx    11558 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       99 b- defN 23-Aug-01 13:49 ezkl/__init__.py
--rwxr-xr-x  4.6 unx 29475328 b- defN 23-Aug-01 13:49 ezkl/ezkl.pyd
--rw-r--r--  4.6 unx      446 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/RECORD
-6 files, 29493457 bytes uncompressed, 10115170 bytes compressed:  65.7%
+Zip file size: 9965539 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     5932 b- defN 23-Aug-05 16:07 ezkl-1.7.19.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Aug-05 16:07 ezkl-1.7.19.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11558 b- defN 23-Aug-05 16:07 ezkl-1.7.19.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       99 b- defN 23-Aug-05 16:07 ezkl/__init__.py
+-rwxr-xr-x  4.6 unx 28678144 b- defN 23-Aug-05 16:07 ezkl/ezkl.pyd
+-rw-r--r--  4.6 unx      446 b- defN 23-Aug-05 16:07 ezkl-1.7.19.dist-info/RECORD
+6 files, 28696275 bytes uncompressed, 9964747 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: ezkl-1.7.17.dist-info/METADATA
+Filename: ezkl-1.7.19.dist-info/METADATA
 Comment: 
 
-Filename: ezkl-1.7.17.dist-info/WHEEL
+Filename: ezkl-1.7.19.dist-info/WHEEL
 Comment: 
 
-Filename: ezkl-1.7.17.dist-info/license_files/LICENSE
+Filename: ezkl-1.7.19.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: ezkl/__init__.py
 Comment: 
 
 Filename: ezkl/ezkl.pyd
 Comment: 
 
-Filename: ezkl-1.7.17.dist-info/RECORD
+Filename: ezkl-1.7.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ezkl-1.7.17.dist-info/METADATA` & `ezkl-1.7.19.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezkl
-Version: 1.7.17
+Version: 1.7.19
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
@@ -45,20 +45,17 @@
 
 ### resources 📖
 
 |  |  |
 | --- | --- |
 | [docs](https://docs.ezkl.xyz ) | the official ezkl docs page |
 | `cargo doc --open` | compile and open the docs in your default browser locally |
-| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zkonduit/ezkl/blob/master/examples/notebooks/simple_demo.ipynb)| a simple demo of the python bindings in action on Colab |
+| [![Simple Example](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zkonduit/ezkl/blob/master/examples/notebooks/simple_demo.ipynb)| a simple demo of the python bindings in action on Colab |
 
-
-
-
-#### tutorials 
+----------------------
 
 You can find a range of python based tutorials in the `examples/notebooks` section. These all assume you have the `ezkl` python library installed. If you want the bleeding edge version of the library, you can install it from the `main` branch with:
 
 ```bash
 python -m venv .env
 source .env/bin/activate
 pip install -r requirements.txt
```

## Comparing `ezkl-1.7.17.dist-info/license_files/LICENSE` & `ezkl-1.7.19.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

