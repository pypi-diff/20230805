# Comparing `tmp/sqlite_lines-0.2.1a1-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_lines-0.2.1a2-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9307 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15792 b- defN 23-Aug-05 03:54 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      531 b- defN 23-Aug-05 03:54 sqlite_lines/__init__.py
--rw-r--r--  2.0 unx    21784 b- defN 23-Aug-05 03:54 sqlite_lines/lines0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:54 sqlite_lines/version.py
--rw-r--r--  2.0 unx      506 b- defN 23-Aug-05 03:54 sqlite_lines-0.2.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Aug-05 03:54 sqlite_lines-0.2.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Aug-05 03:54 sqlite_lines-0.2.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      658 b- defN 23-Aug-05 03:54 sqlite_lines-0.2.1a1.dist-info/RECORD
-8 files, 39473 bytes uncompressed, 8155 bytes compressed:  79.3%
+Zip file size: 9314 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15792 b- defN 23-Aug-05 03:57 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      531 b- defN 23-Aug-05 03:57 sqlite_lines/__init__.py
+-rw-r--r--  2.0 unx    21784 b- defN 23-Aug-05 03:57 sqlite_lines/lines0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:57 sqlite_lines/version.py
+-rw-r--r--  2.0 unx      506 b- defN 23-Aug-05 03:57 sqlite_lines-0.2.1a2.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Aug-05 03:57 sqlite_lines-0.2.1a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Aug-05 03:57 sqlite_lines-0.2.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-Aug-05 03:57 sqlite_lines-0.2.1a2.dist-info/RECORD
+8 files, 39473 bytes uncompressed, 8162 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_lines/lines0.so
 Comment: 
 
 Filename: sqlite_lines/version.py
 Comment: 
 
-Filename: sqlite_lines-0.2.1a1.dist-info/METADATA
+Filename: sqlite_lines-0.2.1a2.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_lines-0.2.1a1.dist-info/WHEEL
+Filename: sqlite_lines-0.2.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_lines-0.2.1a1.dist-info/top_level.txt
+Filename: sqlite_lines-0.2.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_lines-0.2.1a1.dist-info/RECORD
+Filename: sqlite_lines-0.2.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_lines/lines0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 186c2d2f85ecb46c0102d4ef971da57622016439
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 3196ee37aea28c8a743d490c318e3b80226a04cd
```

### strings --all --bytes=8 {}

```diff
@@ -17,17 +17,17 @@
 unable to allocate memory for idxStr
 path argument is required
 Error reading document, size=%d: %s
 Delimiter must be 1 character long, got %d characters
 path is null
 Error reading %s: %s
 CREATE TABLE x(line text,path hidden, delimiter hidden)
-d057655e4e5a0fa1f00df9bee01d8c73ace40ef6
-2023-08-05T03:53:59Z+0000
-v0.2.1-alpha.1
+b11e91b4a2d0bb2e7011bd554398c775d8e5c471
+2023-08-05T03:57:10Z+0000
+v0.2.1-alpha.2
 Version: %s
 Date: %s
 Source: %s
 lines_version
 lines_debug
 lines_read
 Version: %s
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -21,20 +21,20 @@
   0x00003120 25642063 68617261 63746572 73000070 %d characters..p
   0x00003130 61746820 6973206e 756c6c00 4572726f ath is null.Erro
   0x00003140 72207265 6164696e 67202573 3a202573 r reading %s: %s
   0x00003150 00000000 00000000 43524541 54452054 ........CREATE T
   0x00003160 41424c45 2078286c 696e6520 74657874 ABLE x(line text
   0x00003170 2c706174 68206869 6464656e 2c206465 ,path hidden, de
   0x00003180 6c696d69 74657220 68696464 656e2900 limiter hidden).
-  0x00003190 64303537 36353565 34653561 30666131 d057655e4e5a0fa1
-  0x000031a0 66303064 66396265 65303164 38633733 f00df9bee01d8c73
-  0x000031b0 61636534 30656636 00323032 332d3038 ace40ef6.2023-08
-  0x000031c0 2d303554 30333a35 333a3539 5a2b3030 -05T03:53:59Z+00
+  0x00003190 62313165 39316234 61326430 62623265 b11e91b4a2d0bb2e
+  0x000031a0 37303131 62643535 34333938 63373735 7011bd554398c775
+  0x000031b0 64386535 63343731 00323032 332d3038 d8e5c471.2023-08
+  0x000031c0 2d303554 30333a35 373a3130 5a2b3030 -05T03:57:10Z+00
   0x000031d0 30300076 302e322e 312d616c 7068612e 00.v0.2.1-alpha.
-  0x000031e0 31000000 00000000 56657273 696f6e3a 1.......Version:
+  0x000031e0 32000000 00000000 56657273 696f6e3a 2.......Version:
   0x000031f0 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003200 7263653a 20257300 6c696e65 735f7665 rce: %s.lines_ve
   0x00003210 7273696f 6e006c69 6e65735f 64656275 rsion.lines_debu
   0x00003220 67006c69 6e657300 6c696e65 735f7265 g.lines.lines_re
   0x00003230 61640000 00000000 56657273 696f6e3a ad......Version:
   0x00003240 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003250 7263653a 2025730a 4e4f2046 494c4553 rce: %s.NO FILES
```

## sqlite_lines/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1-alpha.1"
+__version__ = "0.2.1-alpha.2"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_lines-0.2.1a1.dist-info/RECORD` & `sqlite_lines-0.2.1a2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noop.cpython-311-x86_64-linux-gnu.so,sha256=SEA9CON0Bl_hsbOLmnG_Fooq8GKSZ2LBe9Dg4u9LAcM,15792
 sqlite_lines/__init__.py,sha256=ksBSpzg9sQ2ztMY47JwEqDTXUkbDrftFwG7FlCjzimc,531
-sqlite_lines/lines0.so,sha256=BEr6KGuRmF_9AzRNvtDPZkpXLjVnG2pSX5hnTYXCuLk,21784
-sqlite_lines/version.py,sha256=WppcRjRLLKcT4AjiCVj6y2WUrCw5t7pNt9rpyOwDZmE,79
-sqlite_lines-0.2.1a1.dist-info/METADATA,sha256=Rdewkq_P7kXss4f898j8tw-ZBYSLbaVomAZzw6luCXM,506
-sqlite_lines-0.2.1a1.dist-info/WHEEL,sha256=bc9AIvLXnt_uk1DFAs9A9G48iq3HERrVzvuB4WpotO8,105
-sqlite_lines-0.2.1a1.dist-info/top_level.txt,sha256=ytsboFBVlsDCFmrrB0YXRhB-r7n9Sb6f8fvKH2ePxrg,18
-sqlite_lines-0.2.1a1.dist-info/RECORD,,
+sqlite_lines/lines0.so,sha256=hShZO9oManquJnNFicJjOpcm9bRo7NAKZ_lqwySW4RI,21784
+sqlite_lines/version.py,sha256=CRIJcMUAZwueE6kdN1m2vVoRLn2LpHt0nta4aK_kq0I,79
+sqlite_lines-0.2.1a2.dist-info/METADATA,sha256=JA_65TZ4RRermfRdy0gCjj9EldFBW9PHIY0uWbs-CPQ,506
+sqlite_lines-0.2.1a2.dist-info/WHEEL,sha256=bc9AIvLXnt_uk1DFAs9A9G48iq3HERrVzvuB4WpotO8,105
+sqlite_lines-0.2.1a2.dist-info/top_level.txt,sha256=ytsboFBVlsDCFmrrB0YXRhB-r7n9Sb6f8fvKH2ePxrg,18
+sqlite_lines-0.2.1a2.dist-info/RECORD,,
```

