# Comparing `tmp/extype-1.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/extype-1.1.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 94805 bytes, number of entries: 15
-?rw-rw-r--  2.0 fat     8766 b- stor 23-Mar-23 20:19 extype-1.0.0.dist-info/METADATA
-?rw-rw-r--  2.0 fat       83 b- stor 23-Mar-23 20:19 extype-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat    73493 b- stor 23-Mar-23 20:19 extype/core.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1500 b- stor 23-Mar-23 20:19 extype/core.cp39-win_amd64.dll.a
--rw-rw-rw-  2.0 fat       58 b- stor 23-Mar-23 20:19 extype/__init__.py
--rw-rw-rw-  2.0 fat     1767 b- stor 23-Mar-23 20:19 extype/extension_utils.py
--rw-rw-rw-  2.0 fat        0 b- stor 23-Mar-23 20:19 extype/builtin_extensions/__init__.py
--rw-rw-rw-  2.0 fat      244 b- stor 23-Mar-23 20:19 extype/builtin_extensions/extend_all.py
--rw-rw-rw-  2.0 fat      647 b- stor 23-Mar-23 20:19 extype/builtin_extensions/dict_ext.py
--rw-rw-rw-  2.0 fat      598 b- stor 23-Mar-23 20:19 extype/builtin_extensions/float_ext.py
--rw-rw-rw-  2.0 fat      954 b- stor 23-Mar-23 20:19 extype/builtin_extensions/function_ext.py
--rw-rw-rw-  2.0 fat      514 b- stor 23-Mar-23 20:19 extype/builtin_extensions/int_ext.py
--rw-rw-rw-  2.0 fat     1822 b- stor 23-Mar-23 20:19 extype/builtin_extensions/list_ext.py
--rw-rw-rw-  2.0 fat      926 b- stor 23-Mar-23 20:19 extype/builtin_extensions/seq_ext.py
-?rw-rw-r--  2.0 fat     1283 b- stor 23-Mar-23 20:19 extype-1.0.0.dist-info/RECORD
-15 files, 92655 bytes uncompressed, 92655 bytes compressed:  0.0%
+Zip file size: 96806 bytes, number of entries: 16
+?rw-rw-r--  2.0 fat     9266 b- stor 23-Aug-05 20:34 extype-1.1.0.dist-info/METADATA
+?rw-rw-r--  2.0 fat       83 b- stor 23-Aug-05 20:34 extype-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat    73493 b- stor 23-Aug-05 20:34 extype/core.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1500 b- stor 23-Aug-05 20:34 extype/core.cp39-win_amd64.dll.a
+-rw-rw-rw-  2.0 fat       58 b- stor 23-Aug-05 20:34 extype/__init__.py
+-rw-rw-rw-  2.0 fat     1767 b- stor 23-Aug-05 20:34 extype/extension_utils.py
+-rw-rw-rw-  2.0 fat        0 b- stor 23-Aug-05 20:34 extype/builtin_extensions/__init__.py
+-rw-rw-rw-  2.0 fat      272 b- stor 23-Aug-05 20:34 extype/builtin_extensions/extend_all.py
+-rw-rw-rw-  2.0 fat      647 b- stor 23-Aug-05 20:34 extype/builtin_extensions/dict_ext.py
+-rw-rw-rw-  2.0 fat      598 b- stor 23-Aug-05 20:34 extype/builtin_extensions/float_ext.py
+-rw-rw-rw-  2.0 fat      954 b- stor 23-Aug-05 20:34 extype/builtin_extensions/function_ext.py
+-rw-rw-rw-  2.0 fat      514 b- stor 23-Aug-05 20:34 extype/builtin_extensions/int_ext.py
+-rw-rw-rw-  2.0 fat     1822 b- stor 23-Aug-05 20:34 extype/builtin_extensions/list_ext.py
+-rw-rw-rw-  2.0 fat      926 b- stor 23-Aug-05 20:34 extype/builtin_extensions/seq_ext.py
+-rw-rw-rw-  2.0 fat     1232 b- stor 23-Aug-05 20:34 extype/builtin_extensions/str_ext.py
+?rw-rw-r--  2.0 fat     1376 b- stor 23-Aug-05 20:34 extype-1.1.0.dist-info/RECORD
+16 files, 94508 bytes uncompressed, 94508 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: extype-1.0.0.dist-info/METADATA
+Filename: extype-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: extype-1.0.0.dist-info/WHEEL
+Filename: extype-1.1.0.dist-info/WHEEL
 Comment: 
 
 Filename: extype/core.cp39-win_amd64.pyd
 Comment: 
 
 Filename: extype/core.cp39-win_amd64.dll.a
 Comment: 
@@ -36,11 +36,14 @@
 
 Filename: extype/builtin_extensions/list_ext.py
 Comment: 
 
 Filename: extype/builtin_extensions/seq_ext.py
 Comment: 
 
-Filename: extype-1.0.0.dist-info/RECORD
+Filename: extype/builtin_extensions/str_ext.py
+Comment: 
+
+Filename: extype-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extype/core.cp39-win_amd64.dll.a

### file list

```diff
@@ -1,4 +1,4 @@
-----------   0        0        0      110 2023-03-23 20:19:32.000000 /
-?rw-r--r--   0        0        0      286 2023-03-23 20:19:32.000000 d000024.o
-?rw-r--r--   0        0        0      344 2023-03-23 20:19:32.000000 d000022.o
-?rw-r--r--   0        0        0      512 2023-03-23 20:19:32.000000 d000023.o
+----------   0        0        0      110 2023-08-05 20:34:40.000000 /
+?rw-r--r--   0        0        0      286 2023-08-05 20:34:40.000000 d000024.o
+?rw-r--r--   0        0        0      344 2023-08-05 20:34:40.000000 d000022.o
+?rw-r--r--   0        0        0      512 2023-08-05 20:34:40.000000 d000023.o
```

## extype/builtin_extensions/extend_all.py

```diff
@@ -1,18 +1,20 @@
 from . import (
     list_ext,
     int_ext,
     float_ext,
     seq_ext,
     function_ext,
     dict_ext,
+    str_ext,
 )
 
 for ext in [
     list_ext,
     int_ext,
     float_ext,
     seq_ext,
     function_ext,
     dict_ext,
+    str_ext,
 ]:
     ext.extend()
```

## Comparing `extype-1.0.0.dist-info/METADATA` & `extype-1.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: extype
-Version: 1.0.0
+Version: 1.1.0
 Summary: ExType is a Python package that allows you to externally extend types.
-Author-Email: Xpo Development <biny@xpo.dev>, Elazar Cohen <elazarcoh@gmail.com>
+Author-Email: Xpo Development <dev@xpo.dev>, Elazar Cohen <elazarcoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ExType
 Extype stands for extensible types, a Python package that enables extending types.
 
 [![PyPI version](https://badge.fury.io/py/extype.svg)](https://badge.fury.io/py/extype)
@@ -59,14 +59,16 @@
 |:---------------:|:----------------------------------:|
 |   dict_ext.py   | dict_keys, dict_values, dict_items |
 |   float_ext.py  |                float               |
 | function_ext.py |      FunctionType, LambdaType      |
 |    int_ext.py   |                 int                |
 |   list_ext.py   |                list                |
 |    seq_ext.py   |       map, filter, range, zip      |
+|    str_ext.py   |          to_int, to_float          |
+
 
 
 Then you can use these extensions. Here's an example of using the `list.map` extension:
 ```py
 print([1, 2, 3].map(lambda x: x + 1))  # [2, 3, 4]
 ```
 
@@ -247,14 +249,28 @@
 Returns the octal representation of the integer.
 
 ```py
 int.bin(self: int) -> str
 ```
 Returns the binary representation of the integer.
 
+```py
+str.to_int(self: str, base: int = 10, default: T = ...) -> int | T
+```
+Converts the given string to an int with the given base. If it can't be
+converted and `default` is given, it is returned. Otherwise, a `ValueError`
+is thrown.
+
+```py
+str.to_float(self: str, default: T = ...) -> float | T
+```
+Converts the given string to a float. If it can't be
+converted and `default` is given, it is returned. Otherwise, a `ValueError`
+is thrown.
+
 * The following extensions are valid for `map`, `filter`, `range` and `zip`
 ```py
 .tolist(self: Iterable[T]) -> List[T]
 ```
 Exhausts the iterble and creates a list from it.
 
 ```py
```

## Comparing `extype-1.0.0.dist-info/RECORD` & `extype-1.1.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-extype-1.0.0.dist-info/METADATA,sha256=zfS8Ab2eOTofKL3JH0uPEIuMU3KrdUbZnRRIuC1gMzg,8766
-extype-1.0.0.dist-info/WHEEL,sha256=8AdrFzOtKQ6LLJ-VyqCU3y1iN8N--fMXYqrdkeTKDn0,83
-extype/core.cp39-win_amd64.pyd,sha256=iIOroj4viSowF64betCiPDCKlPSlN7JssHRbOt8ZXvU,73493
-extype/core.cp39-win_amd64.dll.a,sha256=CjnBZMBfFlNAqKIE7eDk9pOT2rA2kZ7itBlPVyBIK98,1500
+extype-1.1.0.dist-info/METADATA,sha256=gXMe5zrunm2e577fnJJzbcAkn9N0r2RA376HL0NU_SI,9266
+extype-1.1.0.dist-info/WHEEL,sha256=8AdrFzOtKQ6LLJ-VyqCU3y1iN8N--fMXYqrdkeTKDn0,83
+extype/core.cp39-win_amd64.pyd,sha256=X2uNvPrVAnJCH5s2TBaMgDyWWAb4RLL06yDxAZ1RVPI,73493
+extype/core.cp39-win_amd64.dll.a,sha256=eNRIfdLVCxzYj7gQpXvzoswTIUq-VVW1wjcF4tG9ATI,1500
 extype/__init__.py,sha256=1dYHhwdCgVDa5miQQygzjkXO7j-npq07aWbzNnQtdvM,58
 extype/extension_utils.py,sha256=WP8toOvOV8ANnjnUwMsNbMrn1JJOJER4ANB7IztCALg,1767
 extype/builtin_extensions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-extype/builtin_extensions/extend_all.py,sha256=ZiEZho3t9Gxohk_ChAGX5ueP7qt9GZRFOqUksuQ8NKw,244
+extype/builtin_extensions/extend_all.py,sha256=uEcmieRTbAh_K-_cZ7rGAM7BE8i-gSFJqywn11i7JvQ,272
 extype/builtin_extensions/dict_ext.py,sha256=ANes_fjKHkCZiprJnMFxHit4VbvJpx2uCll5VN8HcNA,647
 extype/builtin_extensions/float_ext.py,sha256=s4xsz_X0yLmn3rZqXEkV-DsGl8tJQepKBjSC3TC0J7M,598
 extype/builtin_extensions/function_ext.py,sha256=EStG40f_X-adpRHc8zGJBcwYPxO2TwKIR0RFK6kWBJE,954
 extype/builtin_extensions/int_ext.py,sha256=jjrwibZoqKIigj2PnhCyZHsOnGRvXGn-TFqtPIr73c8,514
 extype/builtin_extensions/list_ext.py,sha256=4CeMH9nDke86FdxEQrKBSr642f6H7VKz4Pj5AWy9LGw,1822
 extype/builtin_extensions/seq_ext.py,sha256=qTeM2-Pv10jwGjFHvtrpmCvAzttOVk8gerzRLWcjJB8,926
-extype-1.0.0.dist-info/RECORD,,
+extype/builtin_extensions/str_ext.py,sha256=oJfV9NKq6el214FQlII-5v-h8CSL5JOsRnUEPgS3dMQ,1232
+extype-1.1.0.dist-info/RECORD,,
```

