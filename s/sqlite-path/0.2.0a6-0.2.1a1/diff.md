# Comparing `tmp/sqlite_path-0.2.0a6-py3-none-win_amd64.whl.zip` & `tmp/sqlite_path-0.2.1a1-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21073 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-24 04:24 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      315 b- defN 23-Jul-24 04:23 sqlite_path/__init__.py
--rw-rw-rw-  2.0 fat    63330 b- defN 23-Jul-24 04:23 sqlite_path/path0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jul-24 04:23 sqlite_path/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jul-24 04:24 sqlite_path-0.2.0a6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jul-24 04:24 sqlite_path-0.2.0a6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-24 04:24 sqlite_path-0.2.0a6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      635 b- defN 23-Jul-24 04:24 sqlite_path-0.2.0a6.dist-info/RECORD
-8 files, 64995 bytes uncompressed, 19959 bytes compressed:  69.3%
+Zip file size: 21068 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 03:02 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Aug-05 03:01 sqlite_path/__init__.py
+-rw-rw-rw-  2.0 fat    63330 b- defN 23-Aug-05 03:02 sqlite_path/path0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-05 03:01 sqlite_path/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Aug-05 03:02 sqlite_path-0.2.1a1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-05 03:02 sqlite_path-0.2.1a1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-05 03:02 sqlite_path-0.2.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      635 b- defN 23-Aug-05 03:02 sqlite_path-0.2.1a1.dist-info/RECORD
+8 files, 64995 bytes uncompressed, 19954 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_path/path0.dll
 Comment: 
 
 Filename: sqlite_path/version.py
 Comment: 
 
-Filename: sqlite_path-0.2.0a6.dist-info/METADATA
+Filename: sqlite_path-0.2.1a1.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_path-0.2.0a6.dist-info/WHEEL
+Filename: sqlite_path-0.2.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_path-0.2.0a6.dist-info/top_level.txt
+Filename: sqlite_path-0.2.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_path-0.2.0a6.dist-info/RECORD
+Filename: sqlite_path-0.2.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_path/path0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Mon Jul 24 04:23:02 2023
+Time/Date		Sat Aug  5 03:01:26 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	37
 SizeOfCode		0000000000005400
 SizeOfInitializedData	0000000000007e00
 SizeOfUninitializedData	0000000000000200
 AddressOfEntryPoint	0000000000001290
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00018000
 SizeOfHeaders		00000600
-CheckSum		00011191
+CheckSum		00018431
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
@@ -111,15 +111,15 @@
  0000e028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x2e05fd000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		64bdfca6
+Time/Date stamp 		64cdbb86
 Major/Minor 			0/0
 Name 				000000000000d032 path0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -8150,35 +8150,39 @@
    2e05f803a:	gs pop %rdi
    2e05f803c:	imul   $0x6f,0x66(%rsi),%ebp
 	...
 
 00000002e05f8050 <.rdata>:
    2e05f8050:	jbe    2e05f8082 <.rdata+0x32>
    2e05f8052:	cs xor (%rsi),%ch
-   2e05f8055:	xor    %ch,0x68706c61(%rip)        # 348cfecbc <.debug_line_str+0x686f7c72>
+   2e05f8055:	xor    %ebp,0x68706c61(%rip)        # 348cfecbc <.debug_line_str+0x686f7c72>
    2e05f805b:	(bad)
-   2e05f805c:	cs ss add %al,(%rax)
-   2e05f8060:	(bad)
-   2e05f8061:	(bad)
-   2e05f8062:	cmp    %esi,0x63623365(%rip)        # 343c1b3cd <.debug_line_str+0x63614383>
-   2e05f8068:	xor    $0x39,%al
-   2e05f806a:	(bad)
-   2e05f806f:	ss gs fs (bad)
-   2e05f8073:	xor    %esi,(%rbx)
-   2e05f8075:	(bad)
-   2e05f8076:	cmp    %dh,0x64643037(%rip)        # 344c3b0b3 <.debug_line_str+0x64634069>
-   2e05f807c:	xor    %dh,(%rbx)
-   2e05f807e:	xor    %dh,0x64613837(%rip)        # 344c0b8bb <.debug_line_str+0x64604871>
-   2e05f8084:	fs xor $0x32006363,%eax
+   2e05f805c:	cs xor %eax,(%rax)
+   2e05f805f:	add    %ah,0x36(%rax,%rsi,1)
+   2e05f8063:	xor    %esp,0x37(%rsi)
+   2e05f8066:	xor    0x35(%rbp),%ah
+   2e05f8069:	xor    $0x31373261,%eax
+   2e05f806e:	ss movsxd (%rbx),%esi
+   2e05f8071:	(bad)
+   2e05f8072:	(bad)
+   2e05f8073:	movsxd %fs:(%rdx),%esi
+   2e05f8076:	gs xor %fs:0x33(%rsi),%esp
+   2e05f807b:	xor    %esi,(%rax)
+   2e05f807d:	cmp    %dh,(%rdx)
+   2e05f807f:	(bad)
+   2e05f8080:	cmp    %ah,%gs:0x62(%rbx)
+   2e05f8084:	(bad)
+   2e05f8085:	xor    $0x32,%al
+   2e05f8087:	add    %dh,%fs:(%rdx)
    2e05f808a:	xor    %dh,(%rdx)
-   2e05f808c:	xor    0x322d3730(%rip),%ebp        # 3128cb7c2 <.debug_line_str+0x322c4778>
-   2e05f8092:	xor    $0x54,%al
-   2e05f8094:	xor    %dh,(%rdx,%rdi,1)
-   2e05f8097:	xor    (%rdx),%dh
-   2e05f8099:	cmp    (%rax,%rdi,1),%dh
+   2e05f808c:	xor    0x302d3830(%rip),%ebp        # 3108cb8c2 <.debug_line_str+0x302c4878>
+   2e05f8092:	xor    $0x3a333054,%eax
+   2e05f8097:	xor    %dh,(%rcx)
+   2e05f8099:	cmp    (%rcx),%dh
+   2e05f809b:	(bad)
    2e05f809c:	pop    %rdx
    2e05f809d:	sub    (%rax),%esi
    2e05f809f:	xor    %dh,(%rax)
    2e05f80a1:	xor    %al,(%rax)
    2e05f80a3:	add    %al,(%rax)
    2e05f80a5:	add    %al,(%rax)
    2e05f80a7:	add    %dl,0x65(%rsi)
@@ -10364,28 +10368,27 @@
 	...
 
 Disassembly of section .edata:
 
 00000002e05fd000 <.edata>:
    2e05fd000:	add    %al,(%rax)
    2e05fd002:	add    %al,(%rax)
-   2e05fd004:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   2e05fd005:	cld
-   2e05fd006:	mov    $0x64,%ebp
-   2e05fd00b:	add    %dh,(%rdx)
-   2e05fd00d:	rolb   (%rax)
-   2e05fd00f:	add    %al,(%rcx)
-   2e05fd011:	add    %al,(%rax)
-   2e05fd013:	add    %al,(%rcx)
-   2e05fd015:	add    %al,(%rax)
-   2e05fd017:	add    %al,(%rcx)
-   2e05fd019:	add    %al,(%rax)
-   2e05fd01b:	add    %ch,(%rax)
-   2e05fd01d:	rolb   (%rax)
-   2e05fd01f:	add    %ch,(%rax,%rdx,8)
+   2e05fd004:	xchg   %bh,0x64cd(%rbx)
+   2e05fd00a:	add    %al,(%rax)
+   2e05fd00c:	xor    %al,%dl
+   2e05fd00e:	add    %al,(%rax)
+   2e05fd010:	add    %eax,(%rax)
+   2e05fd012:	add    %al,(%rax)
+   2e05fd014:	add    %eax,(%rax)
+   2e05fd016:	add    %al,(%rax)
+   2e05fd018:	add    %eax,(%rax)
+   2e05fd01a:	add    %al,(%rax)
+   2e05fd01c:	sub    %dl,%al
+   2e05fd01e:	add    %al,(%rax)
+   2e05fd020:	sub    $0xd0,%al
    2e05fd022:	add    %al,(%rax)
    2e05fd024:	xor    %dl,%al
    2e05fd026:	add    %al,(%rax)
    2e05fd028:	popf
    2e05fd029:	(bad)
    2e05fd02a:	add    %al,(%rax)
    2e05fd02c:	cmp    $0xd0,%al
```

## sqlite_path/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.6"
+__version__ = "0.2.1-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_path-0.2.0a6.dist-info/METADATA` & `sqlite_path-0.2.1a1.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-path
-Version: 0.2.0a6
+Version: 0.2.1a1
 Home-page: https://github.com/asg017/sqlite-path
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-path/issues
 Project-URL: CI, https://github.com/asg017/sqlite-path/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-path/releases
 Requires-Python: >=3.7
```

