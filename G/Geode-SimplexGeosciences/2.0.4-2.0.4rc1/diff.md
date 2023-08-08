# Comparing `tmp/Geode_SimplexGeosciences-2.0.4-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_SimplexGeosciences-2.0.4rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 2963992 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      212 b- defN 23-Aug-08 01:16 geode_simplexgeosciences/__init__.py
--rw-rw-rw-  2.0 fat      261 b- defN 23-Aug-08 01:16 geode_simplexgeosciences/cross_section.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-Aug-08 01:16 geode_simplexgeosciences/structural_model.py
--rw-rw-rw-  2.0 fat  3667968 b- defN 23-Aug-08 01:16 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll
--rw-rw-rw-  2.0 fat  3667968 b- defN 23-Aug-08 01:16 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll
--rw-rw-rw-  2.0 fat   137216 b- defN 23-Aug-08 01:16 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   137216 b- defN 23-Aug-08 01:16 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3368 b- defN 23-Aug-08 01:16 Geode_SimplexGeosciences-2.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-08 01:16 Geode_SimplexGeosciences-2.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Aug-08 01:16 Geode_SimplexGeosciences-2.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1220 b- defN 23-Aug-08 01:16 Geode_SimplexGeosciences-2.0.4.dist-info/RECORD
-11 files, 7615821 bytes uncompressed, 2961848 bytes compressed:  61.1%
+Zip file size: 2964017 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      212 b- defN 23-Aug-07 10:32 geode_simplexgeosciences/__init__.py
+-rw-rw-rw-  2.0 fat      261 b- defN 23-Aug-07 10:32 geode_simplexgeosciences/cross_section.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Aug-07 10:32 geode_simplexgeosciences/structural_model.py
+-rw-rw-rw-  2.0 fat  3667968 b- defN 23-Aug-07 10:32 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll
+-rw-rw-rw-  2.0 fat  3667968 b- defN 23-Aug-07 10:32 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-Aug-07 10:32 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-Aug-07 10:32 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3389 b- defN 23-Aug-07 10:32 Geode_SimplexGeosciences-2.0.4rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-07 10:32 Geode_SimplexGeosciences-2.0.4rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Aug-07 10:32 Geode_SimplexGeosciences-2.0.4rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1232 b- defN 23-Aug-07 10:32 Geode_SimplexGeosciences-2.0.4rc1.dist-info/RECORD
+11 files, 7615854 bytes uncompressed, 2961849 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.4.dist-info/METADATA
+Filename: Geode_SimplexGeosciences-2.0.4rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.4.dist-info/WHEEL
+Filename: Geode_SimplexGeosciences-2.0.4rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.4.dist-info/top_level.txt
+Filename: Geode_SimplexGeosciences-2.0.4rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.4.dist-info/RECORD
+Filename: Geode_SimplexGeosciences-2.0.4rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802a230c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Aug  8 01:16:18 2023
+Time/Date		Mon Aug  7 10:32:23 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002a3c00
 SizeOfInitializedData	00000000000de000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002a230c
@@ -994609,18 +994609,17 @@
    180340bcd:	insb   (%dx),%es:(%rdi)
    180340bce:	insb   (%dx),%es:(%rdi)
    180340bcf:	outsl  %ds:(%rsi),(%dx)
    180340bd0:	movsxd 0x74(%rcx),%esp
    180340bd3:	imul   $0x0,0x6e(%rdi),%ebp
    180340bda:	add    %al,(%rax)
    180340bdc:	(bad)
-   180340bdd:	xchg   %eax,%edi
-   180340bde:	shll   0x0(%rax,%rax,1)
-   180340be2:	add    %al,(%rax)
-   180340be4:	or     $0x88000000,%eax
+   180340bdd:	enter  $0x64d0,$0x0
+   180340be1:	add    %al,(%rax)
+   180340be3:	add    %cl,-0x78000000(%rip)        # 0x108340be9
    180340be9:	add    (%rax),%eax
    180340beb:	add    %dl,%al
    180340bed:	(bad)
    180340bee:	xor    $0x0,%al
    180340bf0:	rclb   (%rdi)
    180340bf2:	xor    $0x0,%al
 	...
```

## geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802a230c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Aug  8 01:16:18 2023
+Time/Date		Mon Aug  7 10:32:23 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002a3c00
 SizeOfInitializedData	00000000000de000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002a230c
@@ -994614,18 +994614,17 @@
    180340bcd:	insb   (%dx),%es:(%rdi)
    180340bce:	insb   (%dx),%es:(%rdi)
    180340bcf:	outsl  %ds:(%rsi),(%dx)
    180340bd0:	movsxd 0x74(%rcx),%esp
    180340bd3:	imul   $0x0,0x6e(%rdi),%ebp
    180340bda:	add    %al,(%rax)
    180340bdc:	(bad)
-   180340bdd:	xchg   %eax,%edi
-   180340bde:	shll   0x0(%rax,%rax,1)
-   180340be2:	add    %al,(%rax)
-   180340be4:	or     $0x88000000,%eax
+   180340bdd:	enter  $0x64d0,$0x0
+   180340be1:	add    %al,(%rax)
+   180340be3:	add    %cl,-0x78000000(%rip)        # 0x108340be9
    180340be9:	add    (%rax),%eax
    180340beb:	add    %dl,%al
    180340bed:	(bad)
    180340bee:	xor    $0x0,%al
    180340bf0:	rclb   (%rdi)
    180340bf2:	xor    $0x0,%al
 	...
```

## Comparing `Geode_SimplexGeosciences-2.0.4.dist-info/METADATA` & `Geode_SimplexGeosciences-2.0.4rc1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Geode-SimplexGeosciences
-Version: 2.0.4
+Version: 2.0.4rc1
 Summary: Geosciences simplex remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-SimplexGeosciences
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
-Requires-Dist: opengeode-geosciences ==7.*,>=7.1.5
+Requires-Dist: geode-background ==7.*,>=7.3.4rc1
+Requires-Dist: geode-common ==26.*,>=26.1.6rc1
+Requires-Dist: geode-numerics ==3.*,>=3.0.10rc1
+Requires-Dist: geode-simplex ==6.*,>=6.1.3rc1
+Requires-Dist: opengeode-core ==14.*,>=14.4.7rc1
+Requires-Dist: opengeode-geosciences ==7.*,>=7.1.5rc1
 
 <h1 align="center">Geode-SimplexGeosciences_private<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Template for creating your own OpenGeode modules</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: Geode-SimplexGeosciences Version: 2.0.4 Summary:
+Metadata-Version: 2.1 Name: Geode-SimplexGeosciences Version: 2.0.4rc1 Summary:
 Geosciences simplex remeshing Geode-solutions OpenGeode module Home-page:
 https://github.com/Geode-solutions/Geode-SimplexGeosciences Author: Geode-
 solutions Author-email: contact@geode-solutions.com License: Proprietary
 Platform: UNKNOWN Description-Content-Type: text/markdown Requires-Dist: geode-
-background ==7.*,>=7.3.4 Requires-Dist: geode-common ==26.*,>=26.1.6 Requires-
-Dist: geode-numerics ==3.*,>=3.0.10 Requires-Dist: geode-simplex ==6.*,>=6.1.3
-Requires-Dist: opengeode-core ==14.*,>=14.4.7 Requires-Dist: opengeode-
-geosciences ==7.*,>=7.1.5
+background ==7.*,>=7.3.4rc1 Requires-Dist: geode-common ==26.*,>=26.1.6rc1
+Requires-Dist: geode-numerics ==3.*,>=3.0.10rc1 Requires-Dist: geode-simplex
+==6.*,>=6.1.3rc1 Requires-Dist: opengeode-core ==14.*,>=14.4.7rc1 Requires-
+Dist: opengeode-geosciences ==7.*,>=7.1.5rc1
        ****** Geode-SimplexGeosciences_privateby Geode-solutions ******
           **** Template for creating your own OpenGeode modules ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
      [Windows support] [Ubuntu support] [Red Hat support] [macOS support]
       [Language] [License] [Semantic-release] [Slack_invite] [DOI] --- ##
   Introduction OpenGeode-ModuleTemplate provides a template for creating an
  [OpenGeode] module. [OpenGeode]: https://github.com/Geode-solutions/OpenGeode
```

## Comparing `Geode_SimplexGeosciences-2.0.4.dist-info/RECORD` & `Geode_SimplexGeosciences-2.0.4rc1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 geode_simplexgeosciences/__init__.py,sha256=9Xfy1rpJuIS2R_cfuk994vKEKycGjnMfO2gksAOUo00,212
 geode_simplexgeosciences/cross_section.py,sha256=iDB6FabUvuIeMb0Iz-MCZCIJ6kKumhhC88Man2GZ1SY,261
 geode_simplexgeosciences/structural_model.py,sha256=3BXiqsIwvfscpzxGP-Mi5oMzw15AcWoo_lwKC_hgwcE,267
-geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll,sha256=caSAnintXgYqAgnl8SLLbJnMIAKagpFIb-Fyq-yL3Nk,3667968
-geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll,sha256=URbaWKj06B4XQvBfwh0BG9wWR-pCsngnwzova68E2BM,3667968
-geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd,sha256=VwLMcojrkzdIzf6WUCwm1v9qXDGZd66FS-81i8fq9hw,137216
-geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd,sha256=32ngW9poBlk5cQsL3YbtKm20Jffy6MLRO6UxCDnx0aI,137216
-Geode_SimplexGeosciences-2.0.4.dist-info/METADATA,sha256=JTdOBFK07YZvfL3k5qEHEsnIKxnHNWEDK0TTEOwVjT8,3368
-Geode_SimplexGeosciences-2.0.4.dist-info/WHEEL,sha256=6LUvBh8thwnyqgVgCADtj3fTB0_JYWDpaYISzieo71U,100
-Geode_SimplexGeosciences-2.0.4.dist-info/top_level.txt,sha256=2n7r8_YGfMeW_LYPqU_ijrPfdfp4XwWFxWWYhLvzJDU,25
-Geode_SimplexGeosciences-2.0.4.dist-info/RECORD,,
+geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll,sha256=yvQlfW2-SwgoV9EtAb42l8ALBl9gAL6BHWN7EVkQnvI,3667968
+geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll,sha256=sI2blWwXHYypM7eGaxqyVUWQmWWIhGGK3cfe6VVRQzU,3667968
+geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd,sha256=67GVhD696Mhs91WbFGaW6cakRcToNuNy-KSE1gGgJsk,137216
+geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd,sha256=wffAPUXvIr0MdRAiidGERVWGQl3mTU1gLEjH83t3nkE,137216
+Geode_SimplexGeosciences-2.0.4rc1.dist-info/METADATA,sha256=8_0-cGXyQPq1EDLMmsvlCsikppU7hkFHZzpvEUHwd90,3389
+Geode_SimplexGeosciences-2.0.4rc1.dist-info/WHEEL,sha256=6LUvBh8thwnyqgVgCADtj3fTB0_JYWDpaYISzieo71U,100
+Geode_SimplexGeosciences-2.0.4rc1.dist-info/top_level.txt,sha256=2n7r8_YGfMeW_LYPqU_ijrPfdfp4XwWFxWWYhLvzJDU,25
+Geode_SimplexGeosciences-2.0.4rc1.dist-info/RECORD,,
```

