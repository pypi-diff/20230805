# Comparing `tmp/sqlite_http-0.1.0a8-py3-none-win_amd64.whl.zip` & `tmp/sqlite_http-0.1.0a9-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5033567 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 01:30 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      556 b- defN 23-Aug-05 01:29 sqlite_http/__init__.py
--rw-rw-rw-  2.0 fat 15831410 b- defN 23-Aug-05 01:29 sqlite_http/http0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-05 01:29 sqlite_http/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Aug-05 01:30 sqlite_http-0.1.0a8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-05 01:30 sqlite_http-0.1.0a8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-05 01:30 sqlite_http-0.1.0a8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      638 b- defN 23-Aug-05 01:30 sqlite_http-0.1.0a8.dist-info/RECORD
-8 files, 15833319 bytes uncompressed, 5032453 bytes compressed:  68.2%
+Zip file size: 5033566 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 01:39 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      556 b- defN 23-Aug-05 01:38 sqlite_http/__init__.py
+-rw-rw-rw-  2.0 fat 15831410 b- defN 23-Aug-05 01:39 sqlite_http/http0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-05 01:38 sqlite_http/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      638 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/RECORD
+8 files, 15833319 bytes uncompressed, 5032452 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_http/http0.dll
 Comment: 
 
 Filename: sqlite_http/version.py
 Comment: 
 
-Filename: sqlite_http-0.1.0a8.dist-info/METADATA
+Filename: sqlite_http-0.1.0a9.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_http-0.1.0a8.dist-info/WHEEL
+Filename: sqlite_http-0.1.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_http-0.1.0a8.dist-info/top_level.txt
+Filename: sqlite_http-0.1.0a9.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_http-0.1.0a8.dist-info/RECORD
+Filename: sqlite_http-0.1.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_http/http0.dll

### objdump

```diff
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	1
 Win32Version		00000000
 SizeOfImage		00ef4000
 SizeOfHeaders		00000600
-CheckSum		00f27bc2
+CheckSum		00f23b04
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00008160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					TERMINAL_SERVICE_AWARE
 SizeOfStackReserve	0000000000200000
@@ -75026,52 +75026,53 @@
    377b6159a:	nopw   0x0(%rax,%rax,1)
 
 0000000377b615a0 <go:buildid>:
    377b615a0:	jmp    *(%rax)
    377b615a2:	rex.RXB outsl %ds:(%rsi),(%dx)
    377b615a4:	and    %ah,0x75(%rdx)
    377b615a7:	imul   $0x203a4449,0x20(%rsp,%riz,2),%ebp
-   377b615af:	and    0x78(%rax,%rdi,1),%dl
-   377b615b3:	pop    %rax
-   377b615b4:	ss js  377b61624 <internal/abi.(*RegArgs).Dump+0x4>
-   377b615b7:	push   $0x77
-   377b615b9:	imul   $0x756f6967,0x5a(%rbp),%ebp
-   377b615c0:	xor    %dl,0x6b(%rbx,%rsi,1)
+   377b615af:	and    0x72(%rdi),%bl
+   377b615b2:	rex.WRB jo 377b6161e <go:buildid+0x7e>
+   377b615b5:	push   %rsi
+   377b615b6:	data16 rex.RXB
+   377b615b8:	rex.WRXB push %r9
+   377b615ba:	cmp    %edx,0x34(%rbx)
+   377b615bd:	outsl  %ds:(%rsi),(%dx)
+   377b615be:	rex.RX pop %rdi
+   377b615c0:	jns    377b615f8 <go:buildid+0x58>
+   377b615c2:	pop    %rdi
+   377b615c3:	push   %rbx
    377b615c4:	(bad)
-   377b615c5:	rex.R
-   377b615c6:	rex.RB
-   377b615c7:	rex.WRX (bad)
-   377b615c9:	pop    %rdx
-   377b615ca:	imul   $0x36,0x76(%rbp),%edx
-   377b615ce:	fs jns 377b61633 <internal/abi.(*RegArgs).Dump+0x13>
-   377b615d1:	rex.WX pop %rdi
-   377b615d3:	rex.RB insl (%dx),%es:(%rdi)
-   377b615d5:	rex.WXB
-   377b615d6:	pop    %r10
-   377b615d8:	rex.RX (bad)
+   377b615c5:	rex.WXB xor %rbx,0x44(%r10)
+   377b615c9:	rex.RX push $0x42
+   377b615cc:	jae    377b61604 <go:buildid+0x64>
+   377b615ce:	imul   $0x4e,0x31(%rbx),%ebp
+   377b615d2:	rex.RB
+   377b615d3:	rex.RXB outsl %ds:(%rsi),(%dx)
+   377b615d5:	rex.WB
+   377b615d6:	data16 rex.W
+   377b615d8:	data16 (bad)
    377b615da:	xor    0x64(%rsi),%dh
    377b615dd:	rex.X sub $0x6a4a6243,%eax
    377b615e3:	push   %rcx
    377b615e4:	je     377b6165b <internal/abi.(*RegArgs).Dump+0x3b>
    377b615e6:	rex.WRX push %rsi
    377b615e8:	rex.WR
    377b615e9:	rex.WRX outsl %ds:(%rsi),(%dx)
    377b615eb:	push   %dx
    377b615ed:	gs (bad)
-   377b615ef:	rex.XB (bad)
-   377b615f2:	push   %rdx
-   377b615f3:	jo     377b61628 <internal/abi.(*RegArgs).Dump+0x8>
-   377b615f5:	movsxd 0x62(%rax),%esi
-   377b615f8:	(bad)
-   377b615f9:	push   %rsp
-   377b615fa:	jns    377b6162e <internal/abi.(*RegArgs).Dump+0xe>
-   377b615fc:	jno    377b61666 <internal/abi.(*RegArgs).Dump+0x46>
-   377b615fe:	push   %rdi
-   377b615ff:	jb     377b61649 <internal/abi.(*RegArgs).Dump+0x29>
-   377b61601:	rex.W push %rdx
+   377b615ef:	js     377b61665 <internal/abi.(*RegArgs).Dump+0x45>
+   377b615f1:	rex.WB jno 377b61669 <internal/abi.(*RegArgs).Dump+0x49>
+   377b615f4:	insb   (%dx),%es:(%rdi)
+   377b615f5:	xor    %eax,0x76(%rcx)
+   377b615f8:	push   %rsp
+   377b615f9:	push   $0x6a537366
+   377b615fe:	rex.WR insl (%dx),%es:(%rdi)
+   377b61600:	rex.X
+   377b61601:	fs insl (%dx),%es:(%rdi)
    377b61603:	and    (%rdx),%cl
    377b61605:	and    %bh,%bh
    377b61607:	int3
    377b61608:	int3
    377b61609:	int3
    377b6160a:	int3
    377b6160b:	int3
@@ -1130213,41 +1130214,43 @@
    377e5125d:	addr32 jae 377e5129d <go:buildinfo+0x27d>
    377e51260:	and    0x616d2058(%rip),%ch        # 3d95232be <.debug_line_str+0x60ad0274>
    377e51266:	imul   $0x73726556,0x2e(%rsi),%ebp
    377e5126d:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377e51274:	xor    %ebp,(%rsi)
    377e51276:	xor    %ch,0x68706c61(%rip)        # 3e0557edd <.debug_line_str+0x67b04e93>
    377e5127c:	(bad)
-   377e5127d:	cs cmp %ah,(%rax)
+   377e5127d:	cs cmp %esp,(%rax)
    377e51280:	sub    $0x616d2058,%eax
    377e51285:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377e5128c:	imul   $0x63633532,0x39(%rbp,%rdi,1),%esi
-   377e51294:	data16 gs xor %bh,%fs:(%rcx)
-   377e51299:	(bad)
-   377e5129a:	ss (bad)
-   377e5129c:	fs (bad)
-   377e5129f:	xor    0x64(%rsi),%ah
-   377e512a2:	xor    0x37(%rsp,%rsi,1),%ah
-   377e512a6:	xor    %esi,(%rbx)
-   377e512a8:	(bad)
-   377e512ad:	cmp    %ah,%gs:0x66(%rbp)
-   377e512b1:	xor    %edi,(%rcx)
-   377e512b3:	fs xor %esp,%fs:0x20(%rdx)
-   377e512b8:	sub    $0x616d2058,%eax
+   377e5128c:	imul   $0x35623631,0x32(%rbp,%rdi,1),%esi
+   377e51294:	xor    $0x31,%al
+   377e51296:	(bad)
+   377e51298:	xor    (%rsi),%esi
+   377e5129a:	cmp    %bh,(%rcx)
+   377e5129c:	xor    $0x38,%al
+   377e5129e:	gs xor $0x33,%al
+   377e512a1:	gs xor $0x31626130,%eax
+   377e512a7:	xor    0x30(%rbx),%esp
+   377e512aa:	xor    %esp,0x34(%rsi)
+   377e512ad:	(bad)
+   377e512ae:	cmp    %esp,0x66(%rbp)
+   377e512b1:	xor    $0x34,%al
+   377e512b3:	ss ss xor $0x582d2039,%eax
+   377e512ba:	and    %ch,0x61(%rbp)
    377e512bd:	imul   $0x65746144,0x2e(%rsi),%ebp
    377e512c4:	cmp    $0x33323032,%eax
    377e512c9:	sub    $0x302d3830,%eax
    377e512ce:	xor    $0x3a313054,%eax
-   377e512d3:	xor    (%rax),%bh
-   377e512d5:	cmp    (%rax),%dh
-   377e512d7:	ss pop %rdx
-   377e512d9:	sub    (%rax),%esi
-   377e512db:	xor    %dh,(%rax)
-   377e512dd:	xor    %ah,(%rdx)
-   377e512df:	or     0x75(%rdx),%ah
+   377e512d3:	xor    (%rdi),%esi
+   377e512d5:	cmp    (%rdx),%dh
+   377e512d7:	xor    %ebx,0x2b(%rdx)
+   377e512da:	xor    %dh,(%rax)
+   377e512dc:	xor    %dh,(%rax)
+   377e512de:	and    (%rdx),%cl
+   377e512e0:	(bad)
    377e512e2:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377e512ea:	jae    377e51329 <go:buildinfo+0x309>
    377e512ec:	jae    377e51356 <go:buildinfo+0x336>
    377e512ee:	(bad)
    377e512ef:	jb     377e51356 <go:buildinfo+0x336>
    377e512f1:	or     %fs:0x75(%rdx),%ah
    377e512f5:	imul   $0x61666544,0x9(%rsp,%riz,2),%ebp
@@ -1130335,37 +1130338,34 @@
    377e513ce:	or     %esi,0x63(%rsi)
    377e513d1:	jae    377e51401 <go:buildinfo+0x3e1>
    377e513d3:	jb     377e5143a <go:buildinfo+0x41a>
    377e513d5:	jbe    377e51440 <go:buildinfo+0x420>
    377e513d7:	jae    377e51442 <go:buildinfo+0x422>
    377e513d9:	outsl  %ds:(%rsi),(%dx)
    377e513da:	outsb  %ds:(%rsi),(%dx)
-   377e513db:	cmp    $0x63353239,%eax
-   377e513e0:	movsxd 0x65(%rsi),%esp
-   377e513e3:	xor    %bh,%fs:(%rcx)
-   377e513e6:	(bad)
-   377e513e7:	ss (bad)
-   377e513e9:	fs (bad)
-   377e513ec:	xor    0x64(%rsi),%ah
-   377e513ef:	xor    0x37(%rsp,%rsi,1),%ah
-   377e513f3:	xor    %esi,(%rbx)
-   377e513f5:	(bad)
-   377e513fa:	cmp    %ah,%gs:0x66(%rbp)
-   377e513fe:	xor    %edi,(%rcx)
-   377e51400:	fs xor %esp,%fs:0xa(%rdx)
-   377e51405:	(bad)
+   377e513db:	cmp    $0x62363132,%eax
+   377e513e0:	xor    $0x36623134,%eax
+   377e513e5:	xor    (%rsi),%esi
+   377e513e7:	cmp    %bh,(%rcx)
+   377e513e9:	xor    $0x38,%al
+   377e513eb:	gs xor $0x33,%al
+   377e513ee:	gs xor $0x31626130,%eax
+   377e513f4:	xor    0x30(%rbx),%esp
+   377e513f7:	xor    %esp,0x34(%rsi)
+   377e513fa:	(bad)
+   377e513fb:	cmp    %esp,0x66(%rbp)
+   377e513fe:	xor    $0x34,%al
+   377e51400:	ss ss xor $0x75620a39,%eax
    377e51407:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377e5140f:	je     377e5147a <text/template..gobytes.6+0x2>
    377e51411:	insl   (%dx),%es:(%rdi)
    377e51412:	gs cmp $0x33323032,%eax
    377e51418:	sub    $0x302d3830,%eax
    377e5141d:	xor    $0x3a313054,%eax
-   377e51422:	xor    (%rsi),%dh
-   377e51424:	cmp    (%rsi,%rsi,1),%dh
-   377e51427:	pop    %rdx
+   377e51422:	xor    0x5a32353a(%rip),%esi        # 3d2174962 <.debug_line_str+0x59721918>
    377e51428:	or     0x75(%rdx),%ah
    377e5142b:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377e51433:	insl   (%dx),%es:(%rdi)
    377e51434:	outsl  %ds:(%rsi),(%dx)
    377e51435:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377e5143d:	(bad)
    377e5143e:	insb   (%dx),%es:(%rdi)
@@ -1681334,15 +1681334,15 @@
 	...
 
 0000000377fa8e40 <main.Version.str>:
    377fa8e40:	jbe    377fa8e72 <vendor/golang.org/x/crypto/chacha20poly1305.sseIncMask+0x2>
    377fa8e42:	cs xor %ebp,(%rsi)
    377fa8e45:	xor    %ch,0x68706c61(%rip)        # 3e06afaac <.debug_line_str+0x67c5ca62>
    377fa8e4b:	(bad)
-   377fa8e4c:	cs cmp %al,(%rax)
+   377fa8e4c:	cs cmp %eax,(%rax)
 	...
 
 0000000377fa8e50 <bswapMask>:
    377fa8e50:	femms
    377fa8e52:	or     $0x90a0b0c,%eax
    377fa8e57:	or     %al,(%rdi)
    377fa8e59:	(bad)
@@ -1684513,20 +1684513,19 @@
 	...
 
 0000000377faa390 <main.Date.str>:
    377faa390:	xor    (%rax),%dh
    377faa392:	xor    (%rbx),%dh
    377faa394:	sub    $0x302d3830,%eax
    377faa399:	xor    $0x3a313054,%eax
-   377faa39e:	xor    (%rax),%bh
-   377faa3a0:	cmp    (%rax),%dh
-   377faa3a2:	ss pop %rdx
-   377faa3a4:	sub    (%rax),%esi
-   377faa3a6:	xor    %dh,(%rax)
-   377faa3a8:	xor    %al,(%rax)
+   377faa39e:	xor    (%rdi),%esi
+   377faa3a0:	cmp    (%rdx),%dh
+   377faa3a2:	xor    %ebx,0x2b(%rdx)
+   377faa3a5:	xor    %dh,(%rax)
+   377faa3a7:	xor    %dh,(%rax)
 	...
 
 0000000377faa3c0 <BSWAP_SHUFB_CTL>:
    377faa3c0:	add    (%rdx),%eax
    377faa3c2:	add    %eax,(%rax)
    377faa3c4:	(bad)
    377faa3c5:	(bad)
@@ -1689053,27 +1689052,27 @@
    377fac7c2:	int1
    377fac7c3:	ja     377fac7c8 <vendor/golang.org/x/text/unicode/norm..stmp_12+0x8>
    377fac7c5:	add    %al,(%rax)
    377fac7c7:	add    %al,(%rdx)
 	...
 
 0000000377fac800 <main.Commit.str>:
-   377fac800:	cmp    %esi,(%rdx)
-   377fac802:	xor    $0x65666363,%eax
-   377fac807:	xor    %bh,%fs:(%rcx)
-   377fac80a:	(bad)
-   377fac80b:	ss (bad)
-   377fac80d:	fs (bad)
-   377fac810:	xor    0x64(%rsi),%ah
-   377fac813:	xor    0x37(%rsp,%rsi,1),%ah
-   377fac817:	xor    %esi,(%rbx)
-   377fac819:	(bad)
-   377fac81e:	cmp    %ah,%gs:0x66(%rbp)
-   377fac822:	xor    %edi,(%rcx)
-   377fac824:	fs xor %esp,%fs:0x0(%rdx)
+   377fac800:	xor    (%rcx),%dh
+   377fac802:	(bad)
+   377fac808:	ss xor (%rsi),%esi
+   377fac80b:	cmp    %bh,(%rcx)
+   377fac80d:	xor    $0x38,%al
+   377fac80f:	gs xor $0x33,%al
+   377fac812:	gs xor $0x31626130,%eax
+   377fac818:	xor    0x30(%rbx),%esp
+   377fac81b:	xor    %esp,0x34(%rsi)
+   377fac81e:	(bad)
+   377fac81f:	cmp    %esp,0x66(%rbp)
+   377fac822:	xor    $0x34,%al
+   377fac824:	ss ss xor $0x39,%eax
 	...
 
 0000000377fac840 <zeroTLS>:
 	...
 
 0000000377fac870 <go:itab.encoding/json.byIndex,sort.Interface>:
    377fac870:	add    %bh,(%rdx)
@@ -1698341,41 +1698340,43 @@
    377fb2991:	addr32 jae 377fb29d1 <runtime.modinfo.str+0x251>
    377fb2994:	and    0x616d2058(%rip),%ch        # 3d96849f2 <.debug_line_str+0x60c319a8>
    377fb299a:	imul   $0x73726556,0x2e(%rsi),%ebp
    377fb29a1:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377fb29a8:	xor    %ebp,(%rsi)
    377fb29aa:	xor    %ch,0x68706c61(%rip)        # 3e06b9611 <.debug_line_str+0x67c665c7>
    377fb29b0:	(bad)
-   377fb29b1:	cs cmp %ah,(%rax)
+   377fb29b1:	cs cmp %esp,(%rax)
    377fb29b4:	sub    $0x616d2058,%eax
    377fb29b9:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377fb29c0:	imul   $0x63633532,0x39(%rbp,%rdi,1),%esi
-   377fb29c8:	data16 gs xor %bh,%fs:(%rcx)
-   377fb29cd:	(bad)
-   377fb29ce:	ss (bad)
-   377fb29d0:	fs (bad)
-   377fb29d3:	xor    0x64(%rsi),%ah
-   377fb29d6:	xor    0x37(%rsp,%rsi,1),%ah
-   377fb29da:	xor    %esi,(%rbx)
-   377fb29dc:	(bad)
-   377fb29e1:	cmp    %ah,%gs:0x66(%rbp)
-   377fb29e5:	xor    %edi,(%rcx)
-   377fb29e7:	fs xor %esp,%fs:0x20(%rdx)
-   377fb29ec:	sub    $0x616d2058,%eax
+   377fb29c0:	imul   $0x35623631,0x32(%rbp,%rdi,1),%esi
+   377fb29c8:	xor    $0x31,%al
+   377fb29ca:	(bad)
+   377fb29cc:	xor    (%rsi),%esi
+   377fb29ce:	cmp    %bh,(%rcx)
+   377fb29d0:	xor    $0x38,%al
+   377fb29d2:	gs xor $0x33,%al
+   377fb29d5:	gs xor $0x31626130,%eax
+   377fb29db:	xor    0x30(%rbx),%esp
+   377fb29de:	xor    %esp,0x34(%rsi)
+   377fb29e1:	(bad)
+   377fb29e2:	cmp    %esp,0x66(%rbp)
+   377fb29e5:	xor    $0x34,%al
+   377fb29e7:	ss ss xor $0x582d2039,%eax
+   377fb29ee:	and    %ch,0x61(%rbp)
    377fb29f1:	imul   $0x65746144,0x2e(%rsi),%ebp
    377fb29f8:	cmp    $0x33323032,%eax
    377fb29fd:	sub    $0x302d3830,%eax
    377fb2a02:	xor    $0x3a313054,%eax
-   377fb2a07:	xor    (%rax),%bh
-   377fb2a09:	cmp    (%rax),%dh
-   377fb2a0b:	ss pop %rdx
-   377fb2a0d:	sub    (%rax),%esi
-   377fb2a0f:	xor    %dh,(%rax)
-   377fb2a11:	xor    %ah,(%rdx)
-   377fb2a13:	or     0x75(%rdx),%ah
+   377fb2a07:	xor    (%rdi),%esi
+   377fb2a09:	cmp    (%rdx),%dh
+   377fb2a0b:	xor    %ebx,0x2b(%rdx)
+   377fb2a0e:	xor    %dh,(%rax)
+   377fb2a10:	xor    %dh,(%rax)
+   377fb2a12:	and    (%rdx),%cl
+   377fb2a14:	(bad)
    377fb2a16:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377fb2a1e:	jae    377fb2a5d <runtime.modinfo.str+0x2dd>
    377fb2a20:	jae    377fb2a8a <runtime.modinfo.str+0x30a>
    377fb2a22:	(bad)
    377fb2a23:	jb     377fb2a8a <runtime.modinfo.str+0x30a>
    377fb2a25:	or     %fs:0x75(%rdx),%ah
    377fb2a29:	imul   $0x61666544,0x9(%rsp,%riz,2),%ebp
@@ -1698463,37 +1698464,34 @@
    377fb2b02:	or     %esi,0x63(%rsi)
    377fb2b05:	jae    377fb2b35 <runtime.modinfo.str+0x3b5>
    377fb2b07:	jb     377fb2b6e <runtime.modinfo.str+0x3ee>
    377fb2b09:	jbe    377fb2b74 <runtime.modinfo.str+0x3f4>
    377fb2b0b:	jae    377fb2b76 <runtime.modinfo.str+0x3f6>
    377fb2b0d:	outsl  %ds:(%rsi),(%dx)
    377fb2b0e:	outsb  %ds:(%rsi),(%dx)
-   377fb2b0f:	cmp    $0x63353239,%eax
-   377fb2b14:	movsxd 0x65(%rsi),%esp
-   377fb2b17:	xor    %bh,%fs:(%rcx)
-   377fb2b1a:	(bad)
-   377fb2b1b:	ss (bad)
-   377fb2b1d:	fs (bad)
-   377fb2b20:	xor    0x64(%rsi),%ah
-   377fb2b23:	xor    0x37(%rsp,%rsi,1),%ah
-   377fb2b27:	xor    %esi,(%rbx)
-   377fb2b29:	(bad)
-   377fb2b2e:	cmp    %ah,%gs:0x66(%rbp)
-   377fb2b32:	xor    %edi,(%rcx)
-   377fb2b34:	fs xor %esp,%fs:0xa(%rdx)
-   377fb2b39:	(bad)
+   377fb2b0f:	cmp    $0x62363132,%eax
+   377fb2b14:	xor    $0x36623134,%eax
+   377fb2b19:	xor    (%rsi),%esi
+   377fb2b1b:	cmp    %bh,(%rcx)
+   377fb2b1d:	xor    $0x38,%al
+   377fb2b1f:	gs xor $0x33,%al
+   377fb2b22:	gs xor $0x31626130,%eax
+   377fb2b28:	xor    0x30(%rbx),%esp
+   377fb2b2b:	xor    %esp,0x34(%rsi)
+   377fb2b2e:	(bad)
+   377fb2b2f:	cmp    %esp,0x66(%rbp)
+   377fb2b32:	xor    $0x34,%al
+   377fb2b34:	ss ss xor $0x75620a39,%eax
    377fb2b3b:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377fb2b43:	je     377fb2bae <vendor/golang.org/x/sys/cpu..stmp_1+0x26>
    377fb2b45:	insl   (%dx),%es:(%rdi)
    377fb2b46:	gs cmp $0x33323032,%eax
    377fb2b4c:	sub    $0x302d3830,%eax
    377fb2b51:	xor    $0x3a313054,%eax
-   377fb2b56:	xor    (%rsi),%dh
-   377fb2b58:	cmp    (%rsi,%rsi,1),%dh
-   377fb2b5b:	pop    %rdx
+   377fb2b56:	xor    0x5a32353a(%rip),%esi        # 3d22d6096 <.debug_line_str+0x5988304c>
    377fb2b5c:	or     0x75(%rdx),%ah
    377fb2b5f:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377fb2b67:	insl   (%dx),%es:(%rdi)
    377fb2b68:	outsl  %ds:(%rsi),(%dx)
    377fb2b69:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377fb2b71:	(bad)
    377fb2b72:	insb   (%dx),%es:(%rdi)
@@ -4194295,8 +4194293,10 @@
    3785f8154:	or     %dl,%ch
    3785f8156:	add    %eax,(%rax)
    3785f8158:	add    %al,(%rax)
    3785f815a:	add    %al,(%rax)
    3785f815c:	add    %bl,%cl
    3785f815e:	add    %eax,(%rax)
    3785f8160:	add    %al,(%rax)
-[ Too much input for diff (SHA256: 277fe01f4e3a9fb4875ea9dcaaf6ecba5ed1f9e39ac716384a000ea0e34b5375) ]
+   3785f8162:	add    %al,(%rax)
+   3785f8164:	add    %cl,(%rax)
+[ Too much input for diff (SHA256: 5f24e43ac3605c3a8de321df0ee034a2ca0bf02a4c7b8bc45ae399e17a524e3f) ]
```

## sqlite_http/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.8"
+__version__ = "0.1.0-alpha.9"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_http-0.1.0a8.dist-info/METADATA` & `sqlite_http-0.1.0a9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-http
-Version: 0.1.0a8
+Version: 0.1.0a9
 Home-page: https://github.com/asg017/sqlite-http
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-http/issues
 Project-URL: CI, https://github.com/asg017/sqlite-http/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-http/releases
 Requires-Python: >=3.7
```

