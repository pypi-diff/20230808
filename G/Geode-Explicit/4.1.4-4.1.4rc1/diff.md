# Comparing `tmp/Geode_Explicit-4.1.4-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.1.4rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3113362 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-Aug-08 01:17 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-Aug-08 01:17 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Aug-08 01:17 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  3947008 b- defN 23-Aug-08 01:18 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33280 b- defN 23-Aug-08 01:18 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  3704832 b- defN 23-Aug-08 01:18 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   153600 b- defN 23-Aug-08 01:18 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-Aug-08 01:18 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2365 b- defN 23-Aug-08 01:18 Geode_Explicit-4.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-08 01:18 Geode_Explicit-4.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Aug-08 01:18 Geode_Explicit-4.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1118 b- defN 23-Aug-08 01:18 Geode_Explicit-4.1.4.dist-info/RECORD
-12 files, 7984856 bytes uncompressed, 3111462 bytes compressed:  61.0%
+Zip file size: 3113389 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 23-Aug-07 10:32 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-Aug-07 10:32 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Aug-07 10:32 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  3947008 b- defN 23-Aug-07 10:33 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    33280 b- defN 23-Aug-07 10:33 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  3704832 b- defN 23-Aug-07 10:33 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-Aug-07 10:33 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   141824 b- defN 23-Aug-07 10:33 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-Aug-07 10:33 Geode_Explicit-4.1.4rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-07 10:33 Geode_Explicit-4.1.4rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Aug-07 10:33 Geode_Explicit-4.1.4rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 23-Aug-07 10:33 Geode_Explicit-4.1.4rc1.dist-info/RECORD
+12 files, 7984895 bytes uncompressed, 3111465 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-4.1.4.dist-info/METADATA
+Filename: Geode_Explicit-4.1.4rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.1.4.dist-info/WHEEL
+Filename: Geode_Explicit-4.1.4rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.1.4.dist-info/top_level.txt
+Filename: Geode_Explicit-4.1.4rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.1.4.dist-info/RECORD
+Filename: Geode_Explicit-4.1.4rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802d576c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Aug  8 01:17:54 2023
+Time/Date		Mon Aug  7 10:33:19 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002d8a00
 SizeOfInitializedData	00000000000ed400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002d576c
@@ -1067274,18 +1067274,18 @@
    180376dc8:	(bad)
    180376dcd:	insb   (%dx),%es:(%rdi)
    180376dce:	insb   (%dx),%es:(%rdi)
    180376dcf:	outsl  %ds:(%rsi),(%dx)
    180376dd0:	movsxd 0x74(%rcx),%esp
    180376dd3:	imul   $0x0,0x6e(%rdi),%ebp
    180376dda:	add    %al,(%rax)
-   180376ddc:	ret    $0xd197
-   180376ddf:	add    %al,%fs:(%rax)
-   180376de2:	add    %al,(%rax)
-   180376de4:	or     $0x88000000,%eax
+   180376ddc:	outsl  %ds:(%rsi),(%dx)
+   180376ddd:	enter  $0x64d0,$0x0
+   180376de1:	add    %al,(%rax)
+   180376de3:	add    %cl,-0x78000000(%rip)        # 0x108376de9
    180376de9:	add    (%rax),%eax
    180376deb:	add    %al,(%rax)
    180376ded:	xchg   %eax,%esp
    180376dee:	(bad)
    180376def:	add    %al,(%rax)
    180376df1:	(bad)
    180376df2:	(bad)
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800040e0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Aug  8 01:17:34 2023
+Time/Date		Mon Aug  7 10:32:55 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000004000
 SizeOfInitializedData	0000000000004400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000040e0
@@ -6732,17 +6732,18 @@
    18000552a:	(bad)
    18000552b:	(bad)
    18000552c:	(bad)
    18000552d:	(bad)
    18000552e:	(bad)
    18000552f:	incl   (%rax)
    180005531:	add    %al,(%rax)
-   180005533:	add    %ch,0x64d197(%rsi)
-   180005539:	add    %al,(%rax)
-   18000553b:	add    %cl,-0x5c000000(%rip)        # 0x124005541
+   180005533:	add    %dl,-0x38(%rdi)
+   180005536:	shlb   0x0(%rax,%rax,1)
+   18000553a:	add    %al,(%rax)
+   18000553c:	or     $0xa4000000,%eax
    180005541:	add    (%rax),%al
    180005543:	add    %ah,0x5b(%rax)
    180005546:	add    %al,(%rax)
    180005548:	(bad)
    180005549:	rex.WRXB add %r8b,(%r8)
    18000554c:	add    %al,(%rax)
    18000554e:	add    %al,(%rax)
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802a8790
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Aug  8 01:17:37 2023
+Time/Date		Mon Aug  7 10:32:59 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002aa200
 SizeOfInitializedData	00000000000e0a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002a8790
@@ -1001029,18 +1001029,18 @@
    180347f08:	(bad)
    180347f0d:	insb   (%dx),%es:(%rdi)
    180347f0e:	insb   (%dx),%es:(%rdi)
    180347f0f:	outsl  %ds:(%rsi),(%dx)
    180347f10:	movsxd 0x74(%rcx),%esp
    180347f13:	imul   $0x0,0x6e(%rdi),%ebp
    180347f1a:	add    %al,(%rax)
-   180347f1c:	mov    $0x97,%cl
-   180347f1e:	shll   0x0(%rax,%rax,1)
-   180347f22:	add    %al,(%rax)
-   180347f24:	or     $0x88000000,%eax
+   180347f1c:	pop    %rbx
+   180347f1d:	enter  $0x64d0,$0x0
+   180347f21:	add    %al,(%rax)
+   180347f23:	add    %cl,-0x78000000(%rip)        # 0x108347f29
    180347f29:	add    (%rax),%eax
    180347f2b:	add    %dl,0x34(%rbx,%rbx,4)
    180347f2f:	add    %dl,0x34(%rcx,%rax,4)
 	...
    180347f3f:	add    %bh,(%rax)
    180347f41:	add    %eax,(%rax)
 	...
```

## Comparing `Geode_Explicit-4.1.4.dist-info/METADATA` & `Geode_Explicit-4.1.4rc1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 4.1.4
+Version: 4.1.4rc1
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.3.4
-Requires-Dist: geode-common ==26.*,>=26.1.6
-Requires-Dist: geode-conversion ==5.*,>=5.0.10
-Requires-Dist: opengeode-core ==14.*,>=14.4.7
-Requires-Dist: opengeode-geosciences ==7.*,>=7.1.5
-Requires-Dist: opengeode-geosciencesio ==4.*,>=4.2.2
-Requires-Dist: opengeode-inspector ==3.*,>=3.0.9
-Requires-Dist: opengeode-io ==6.*,>=6.0.11
+Requires-Dist: geode-background ==7.*,>=7.3.4rc1
+Requires-Dist: geode-common ==26.*,>=26.1.6rc1
+Requires-Dist: geode-conversion ==5.*,>=5.0.10rc1
+Requires-Dist: opengeode-core ==14.*,>=14.4.7rc1
+Requires-Dist: opengeode-geosciences ==7.*,>=7.1.5rc1
+Requires-Dist: opengeode-geosciencesio ==4.*,>=4.2.2rc1
+Requires-Dist: opengeode-inspector ==3.*,>=3.0.9rc1
+Requires-Dist: opengeode-io ==6.*,>=6.0.11rc1
 
 <h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.1.4 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.1.4rc1 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background ==7.*,>=7.3.4
-Requires-Dist: geode-common ==26.*,>=26.1.6 Requires-Dist: geode-conversion
-==5.*,>=5.0.10 Requires-Dist: opengeode-core ==14.*,>=14.4.7 Requires-Dist:
-opengeode-geosciences ==7.*,>=7.1.5 Requires-Dist: opengeode-geosciencesio
-==4.*,>=4.2.2 Requires-Dist: opengeode-inspector ==3.*,>=3.0.9 Requires-Dist:
-opengeode-io ==6.*,>=6.0.11
+Content-Type: text/markdown Requires-Dist: geode-background ==7.*,>=7.3.4rc1
+Requires-Dist: geode-common ==26.*,>=26.1.6rc1 Requires-Dist: geode-conversion
+==5.*,>=5.0.10rc1 Requires-Dist: opengeode-core ==14.*,>=14.4.7rc1 Requires-
+Dist: opengeode-geosciences ==7.*,>=7.1.5rc1 Requires-Dist: opengeode-
+geosciencesio ==4.*,>=4.2.2rc1 Requires-Dist: opengeode-inspector
+==3.*,>=3.0.9rc1 Requires-Dist: opengeode-io ==6.*,>=6.0.11rc1
                 ****** Geode-Explicitby Geode-solutions ******
     **** Geode-solutions OpenGeode module for building explicit models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

## Comparing `Geode_Explicit-4.1.4.dist-info/RECORD` & `Geode_Explicit-4.1.4rc1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 geode_explicit/__init__.py,sha256=-1Ma-Q_qKho5-HJywdEjGH_v91Dp0h8zchFCzKp7ADk,194
 geode_explicit/brep.py,sha256=5gXUGyujJVK7W7i2Zoqb5_9Mb5jPPZLiYZX9piVVUGY,271
 geode_explicit/section.py,sha256=diHY0-G0OXfICdOX3HSTnwrdrW3WOsct7GAT4rECQb4,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=TIACW7HZtmpQ-jX8JZEQZaOjxdvuIa7bdKGO4--Cfu0,3947008
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=4e6gUIoywmTmZk-9f3tydmgf_81Pd102903tvSXR39c,33280
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=QS4A_XShIGe-UjQYk-6gWdzOr4hAWV6B9Gu5vhm5R5s,3704832
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=WbiDlMwyeJ_Qt6kRXeA88qPYg7V_Y-BjoOSsvb71Eog,153600
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=9f9nGB65tKbEoj4p1dOF7dCC3Yh8UceSKHDQsnCeQBI,141824
-Geode_Explicit-4.1.4.dist-info/METADATA,sha256=HXy0KlPh5M4b2X6sN_pQURlGAskBh1AldByQXO2_2UY,2365
-Geode_Explicit-4.1.4.dist-info/WHEEL,sha256=6LUvBh8thwnyqgVgCADtj3fTB0_JYWDpaYISzieo71U,100
-Geode_Explicit-4.1.4.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.1.4.dist-info/RECORD,,
+geode_explicit/bin/Geode-Explicit_brep.dll,sha256=baHrNry7yRxLmqu_IVNQJvTFu1XYZaof4rF9PnLRax8,3947008
+geode_explicit/bin/Geode-Explicit_common.dll,sha256=y8xLjU4xZBZZb6NUGTCOSgOFgakNW4PQvkBfdUuUSJg,33280
+geode_explicit/bin/Geode-Explicit_section.dll,sha256=UgTCYoXDxYE_fkVXrxDcymSoRIQC0pg7o4qntcqH6kg,3704832
+geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=sCqBCOIc_wjTa7A_NHkzJdxaTly9_LmOdwu5s61BoxQ,153600
+geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=ALZYRNPR5CFuYEQpdVQl1CC_CGc_dYv_F3BT_8GGsOI,141824
+Geode_Explicit-4.1.4rc1.dist-info/METADATA,sha256=KpCdOTcT--MQBymSAW8HwmfGLdZF94C3oMeegkLchuU,2392
+Geode_Explicit-4.1.4rc1.dist-info/WHEEL,sha256=6LUvBh8thwnyqgVgCADtj3fTB0_JYWDpaYISzieo71U,100
+Geode_Explicit-4.1.4rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.1.4rc1.dist-info/RECORD,,
```

