# Comparing `tmp/Geode_Hybrid-2.0.5-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Hybrid-2.0.5rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1533899 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      170 b- defN 23-Aug-08 01:16 geode_hybrid/__init__.py
--rw-rw-rw-  2.0 fat      234 b- defN 23-Aug-08 01:16 geode_hybrid/brep.py
--rw-rw-rw-  2.0 fat  3794944 b- defN 23-Aug-08 01:16 geode_hybrid/bin/Geode-Hybrid_brep.dll
--rw-rw-rw-  2.0 fat   137216 b- defN 23-Aug-08 01:16 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2223 b- defN 23-Aug-08 01:16 Geode_Hybrid-2.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-08 01:16 Geode_Hybrid-2.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-08 01:16 Geode_Hybrid-2.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      688 b- defN 23-Aug-08 01:16 Geode_Hybrid-2.0.5.dist-info/RECORD
-8 files, 3935588 bytes uncompressed, 1532697 bytes compressed:  61.1%
+Zip file size: 1533930 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      170 b- defN 23-Aug-07 10:32 geode_hybrid/__init__.py
+-rw-rw-rw-  2.0 fat      234 b- defN 23-Aug-07 10:32 geode_hybrid/brep.py
+-rw-rw-rw-  2.0 fat  3794944 b- defN 23-Aug-07 10:32 geode_hybrid/bin/Geode-Hybrid_brep.dll
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-Aug-07 10:32 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2241 b- defN 23-Aug-07 10:32 Geode_Hybrid-2.0.5rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-07 10:32 Geode_Hybrid-2.0.5rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-07 10:32 Geode_Hybrid-2.0.5rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      700 b- defN 23-Aug-07 10:32 Geode_Hybrid-2.0.5rc1.dist-info/RECORD
+8 files, 3935618 bytes uncompressed, 1532704 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: geode_hybrid/bin/Geode-Hybrid_brep.dll
 Comment: 
 
 Filename: geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Hybrid-2.0.5.dist-info/METADATA
+Filename: Geode_Hybrid-2.0.5rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Hybrid-2.0.5.dist-info/WHEEL
+Filename: Geode_Hybrid-2.0.5rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Hybrid-2.0.5.dist-info/top_level.txt
+Filename: Geode_Hybrid-2.0.5rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Hybrid-2.0.5.dist-info/RECORD
+Filename: Geode_Hybrid-2.0.5rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_hybrid/bin/Geode-Hybrid_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802b628c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Aug  8 01:16:35 2023
+Time/Date		Mon Aug  7 10:32:37 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002b8600
 SizeOfInitializedData	00000000000e8800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002b628c
@@ -1022050,18 +1022050,17 @@
    180356b88:	(bad)
    180356b8d:	insb   (%dx),%es:(%rdi)
    180356b8e:	insb   (%dx),%es:(%rdi)
    180356b8f:	outsl  %ds:(%rsi),(%dx)
    180356b90:	movsxd 0x74(%rcx),%esp
    180356b93:	imul   $0x0,0x6e(%rdi),%ebp
    180356b9a:	add    %al,(%rax)
-   180356b9c:	jae    0x180356b35
-   180356b9e:	shll   0x0(%rax,%rax,1)
-   180356ba2:	add    %al,(%rax)
-   180356ba4:	or     $0x88000000,%eax
+   180356b9c:	rex.RB enter $0x64d0,$0x0
+   180356ba1:	add    %al,(%rax)
+   180356ba3:	add    %cl,-0x78000000(%rip)        # 0x108356ba9
    180356ba9:	add    (%rax),%eax
    180356bab:	add    %al,-0x7fffca73(%rax)
    180356bb1:	ja     0x180356be8
 	...
    180356bbf:	add    %bh,(%rax)
    180356bc1:	add    %eax,(%rax)
 	...
@@ -1084622,18 +1084621,18 @@
    18037e33b:	(bad)
    18037e33c:	addr32 rex
    18037e33e:	rex.W
    18037e33f:	gs js  0x18037e38f
    18037e342:	gs jae 0x18037e3ad
    18037e345:	gs jb  0x18037e388
    18037e348:	(bad)
-   18037e349:	xor    %dil,0x66(%r8)
-   18037e34d:	ss xor 0x30(%rcx),%ah
-   18037e351:	xor    %bh,(%rcx)
-   18037e353:	gs rex
+   18037e349:	xor    %dil,0x64(%r8)
+   18037e34d:	xor    0x64(%rsi),%ah
+   18037e350:	cmp    %esp,%gs:0x33(%rdx)
+   18037e354:	rex
    18037e355:	rex
    18037e356:	rex
    18037e357:	outsl  %gs:(%esi),(%dx)
    18037e35a:	fs gs rex
    18037e35d:	rex add %al,(%rax)
    18037e360:	shrb   $0x80,0x35(%rdx)
    18037e364:	add    %eax,(%rax)
@@ -1084645,18 +1084644,18 @@
    18037e376:	(bad)
    18037e377:	addr32 rex
    18037e379:	rex.W
    18037e37a:	gs js  0x18037e3ca
    18037e37d:	gs jae 0x18037e3e8
    18037e380:	gs jb  0x18037e3c3
    18037e383:	(bad)
-   18037e384:	xor    %dil,0x66(%r8)
-   18037e388:	ss xor 0x30(%rcx),%ah
-   18037e38c:	xor    %bh,(%rcx)
-   18037e38e:	gs rex
+   18037e384:	xor    %dil,0x64(%r8)
+   18037e388:	xor    0x64(%rsi),%ah
+   18037e38b:	cmp    %esp,%gs:0x33(%rdx)
+   18037e38f:	rex
    18037e390:	rex add %al,(%rax)
    18037e393:	add    %al,(%rax)
    18037e395:	add    %al,(%rax)
    18037e397:	add    %al,%al
    18037e399:	push   $0x35
    18037e39b:	addb   $0x0,(%rcx)
 	...
@@ -1084806,18 +1084805,18 @@
    18037e538:	cs (bad)
    18037e53a:	push   %r14
    18037e53c:	rex.W
    18037e53d:	gs js  0x18037e58d
    18037e540:	gs jae 0x18037e5ab
    18037e543:	gs jb  0x18037e586
    18037e546:	(bad)
-   18037e547:	xor    %dil,0x66(%r8)
-   18037e54b:	ss xor 0x30(%rcx),%ah
-   18037e54f:	xor    %bh,(%rcx)
-   18037e551:	gs rex
+   18037e547:	xor    %dil,0x64(%r8)
+   18037e54b:	xor    0x64(%rsi),%ah
+   18037e54e:	cmp    %esp,%gs:0x33(%rdx)
+   18037e552:	rex
    18037e553:	rex add %al,(%rax)
 	...
    18037e55e:	add    %al,(%rax)
    18037e560:	shrb   $0x80,0x35(%rdx)
    18037e564:	add    %eax,(%rax)
 	...
    18037e56e:	add    %al,(%rax)
@@ -1084874,18 +1084873,18 @@
    18037e5eb:	(bad)
    18037e5ec:	addr32 rex
    18037e5ee:	rex.W
    18037e5ef:	gs js  0x18037e63f
    18037e5f2:	gs jae 0x18037e65d
    18037e5f5:	gs jb  0x18037e638
    18037e5f8:	(bad)
-   18037e5f9:	xor    %dil,0x66(%r8)
-   18037e5fd:	ss xor 0x30(%rcx),%ah
-   18037e601:	xor    %bh,(%rcx)
-   18037e603:	gs rex
+   18037e5f9:	xor    %dil,0x64(%r8)
+   18037e5fd:	xor    0x64(%rsi),%ah
+   18037e600:	cmp    %esp,%gs:0x33(%rdx)
+   18037e604:	rex
    18037e605:	rex
    18037e606:	rex
    18037e607:	outsl  %gs:(%esi),(%dx)
    18037e60a:	fs gs rex
    18037e60d:	rex add %al,(%rax)
    18037e610:	shrb   $0x80,0x35(%rdx)
    18037e614:	add    %eax,(%rax)
@@ -1084916,18 +1084915,18 @@
    18037e649:	(bad)
    18037e64a:	addr32 rex
    18037e64c:	rex.W
    18037e64d:	gs js  0x18037e69d
    18037e650:	gs jae 0x18037e6bb
    18037e653:	gs jb  0x18037e696
    18037e656:	(bad)
-   18037e657:	xor    %dil,0x66(%r8)
-   18037e65b:	ss xor 0x30(%rcx),%ah
-   18037e65f:	xor    %bh,(%rcx)
-   18037e661:	gs rex
+   18037e657:	xor    %dil,0x64(%r8)
+   18037e65b:	xor    0x64(%rsi),%ah
+   18037e65e:	cmp    %esp,%gs:0x33(%rdx)
+   18037e662:	rex
    18037e663:	rex
    18037e664:	rex
    18037e665:	outsl  %gs:(%esi),(%dx)
    18037e668:	fs gs rex
    18037e66b:	rex
    18037e66c:	rex jae 0x18037e6e3
    18037e66f:	fs rex
```

## Comparing `Geode_Hybrid-2.0.5.dist-info/METADATA` & `Geode_Hybrid-2.0.5rc1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Geode-Hybrid
-Version: 2.0.5
+Version: 2.0.5rc1
 Summary: Hybrid remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-Hybrid
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.3.4
-Requires-Dist: geode-common ==26.*,>=26.1.6
-Requires-Dist: geode-numerics ==3.*,>=3.0.10
-Requires-Dist: geode-simplex ==6.*,>=6.1.3
-Requires-Dist: opengeode-core ==14.*,>=14.4.7
+Requires-Dist: geode-background ==7.*,>=7.3.4rc1
+Requires-Dist: geode-common ==26.*,>=26.1.6rc1
+Requires-Dist: geode-numerics ==3.*,>=3.0.10rc1
+Requires-Dist: geode-simplex ==6.*,>=6.1.3rc1
+Requires-Dist: opengeode-core ==14.*,>=14.4.7rc1
 
 <h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Template for creating your own OpenGeode private module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.5 Summary: Hybrid
+Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.5rc1 Summary: Hybrid
 remeshing Geode-solutions OpenGeode module Home-page: https://github.com/Geode-
 solutions/Geode-Hybrid Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
-text/markdown Requires-Dist: geode-background ==7.*,>=7.3.4 Requires-Dist:
-geode-common ==26.*,>=26.1.6 Requires-Dist: geode-numerics ==3.*,>=3.0.10
-Requires-Dist: geode-simplex ==6.*,>=6.1.3 Requires-Dist: opengeode-core
-==14.*,>=14.4.7
+text/markdown Requires-Dist: geode-background ==7.*,>=7.3.4rc1 Requires-Dist:
+geode-common ==26.*,>=26.1.6rc1 Requires-Dist: geode-numerics ==3.*,>=3.0.10rc1
+Requires-Dist: geode-simplex ==6.*,>=6.1.3rc1 Requires-Dist: opengeode-core
+==14.*,>=14.4.7rc1
          ****** Geode-ModuleTemplate_privateby Geode-solutions ******
        **** Template for creating your own OpenGeode private module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

