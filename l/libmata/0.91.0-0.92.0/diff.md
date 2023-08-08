# Comparing `tmp/libmata-0.91.0.tar.gz` & `tmp/libmata-0.92.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-0.91.0.tar", last modified: Fri Aug  4 05:50:35 2023, max compression
+gzip compressed data, was "libmata-0.92.0.tar", last modified: Tue Aug  8 05:32:18 2023, max compression
```

## Comparing `libmata-0.91.0.tar` & `libmata-0.92.0.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.269998 libmata-0.91.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-08-04 05:50:35.269998 libmata-0.91.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.241998 libmata-0.91.0/libmata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   525998 2023-08-04 05:46:34.930143 libmata-0.91.0/libmata/alphabets.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/alphabets.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/alphabets.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.241998 libmata-0.91.0/libmata/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/nfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1690493 2023-08-04 05:46:35.934164 libmata-0.91.0/libmata/nfa/nfa.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/nfa/nfa.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    43671 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/nfa/nfa.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   434179 2023-08-04 05:46:36.674180 libmata-0.91.0/libmata/nfa/strings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/nfa/strings.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/nfa/strings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   249287 2023-08-04 05:46:37.122189 libmata-0.91.0/libmata/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   696495 2023-08-04 05:46:37.806203 libmata-0.91.0/libmata/plotting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/plotting.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   458228 2023-08-04 05:46:38.094209 libmata-0.91.0/libmata/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-08-04 05:45:46.217114 libmata-0.91.0/libmata/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.245998 libmata-0.91.0/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.245998 libmata-0.91.0/mata/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-08-04 05:45:46.177113 libmata-0.91.0/mata/3rdparty/args.hxx
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-08-04 05:45:46.181113 libmata-0.91.0/mata/3rdparty/catch.hpp.1.9.3
--rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/catch.hpp.2.0.1
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/catch.hpp.2.13.9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.245998 libmata-0.91.0/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.245998 libmata-0.91.0/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.249998 libmata-0.91.0/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-08-04 05:45:46.185113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-08-04 05:45:46.189113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-08-04 05:45:46.197113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-08-04 05:45:46.201113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.249998 libmata-0.91.0/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.249998 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 05:45:46.205113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/composeids.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.229998 libmata-0.91.0/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.229998 libmata-0.91.0/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-08-04 05:45:46.209113 libmata-0.91.0/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.233998 libmata-0.91.0/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.233998 libmata-0.91.0/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-04 05:45:46.213113 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.253998 libmata-0.91.0/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-08-04 05:50:35.121997 libmata-0.91.0/mata/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101164 2023-08-04 05:50:35.121997 libmata-0.91.0/mata/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-04 05:50:35.121997 libmata-0.91.0/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-04 05:50:35.121997 libmata-0.91.0/mata/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-04 05:50:35.121997 libmata-0.91.0/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 05:50:35.121997 libmata-0.91.0/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.237998 libmata-0.91.0/mata/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.257998 libmata-0.91.0/mata/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/cmake/Modules/Catch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/cmake/Modules/CatchAddTests.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/cmake/Modules/CodeCoverage.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/cmake/Modules/FindValgrind.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/cmake/Modules/GetGitRevisionDescription.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-04 05:45:46.217114 libmata-0.91.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.237998 libmata-0.91.0/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.257998 libmata-0.91.0/mata/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.257998 libmata-0.91.0/mata/include/mata/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/afa/afa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/alphabet.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.257998 libmata-0.91.0/mata/include/mata/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/nfa/algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/nfa/builder.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/nfa/delta.hh
--rw-r--r--   0 runner    (1001) docker     (123)    32186 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/nfa/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/nfa/plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/nfa/strings.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/nfa/types.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.257998 libmata-0.91.0/mata/include/mata/parser/
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/parser/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/parser/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/parser/parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/parser/re2parser.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.261998 libmata-0.91.0/mata/include/mata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/utils/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/utils/number-predicate.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/utils/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/utils/sparse-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/utils/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/include/mata/utils/util.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.261998 libmata-0.91.0/mata/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/scripts/merge_static_libraries.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.261998 libmata-0.91.0/mata/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.261998 libmata-0.91.0/mata/src/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    38800 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.265998 libmata-0.91.0/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/complement.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/delta.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)    35558 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32836 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/operations.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/nfa/universal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-04 05:45:46.221114 libmata-0.91.0/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-08-04 05:45:46.225114 libmata-0.91.0/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.265998 libmata-0.91.0/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-08-04 05:45:46.225114 libmata-0.91.0/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-08-04 05:45:46.225114 libmata-0.91.0/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-04 05:45:46.225114 libmata-0.91.0/mata/src/strings/nfa-strings.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.269998 libmata-0.91.0/mata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.269998 libmata-0.91.0/mata/tests/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    27575 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)    42818 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.269998 libmata-0.91.0/mata/tests/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/nfa/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32066 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/nfa/nfa-concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/nfa/nfa-intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/nfa/nfa-profiling.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/nfa/nfa-util.hh
--rw-r--r--   0 runner    (1001) docker     (123)    86124 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/ord-vector.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/re2parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/sparse-set.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:50:35.269998 libmata-0.91.0/mata/tests/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    18138 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/strings/nfa-string-solving.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-04 05:45:46.237114 libmata-0.91.0/mata/tests/synchronized-iterator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 05:45:46.217114 libmata-0.91.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-04 05:45:46.217114 libmata-0.91.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-08-08 05:32:18.176341 libmata-0.92.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/libmata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:27:23.922237 libmata-0.92.0/libmata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   526340 2023-08-08 05:28:11.155266 libmata-0.92.0/libmata/alphabets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-08 05:27:23.922237 libmata-0.92.0/libmata/alphabets.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-08-08 05:27:23.922237 libmata-0.92.0/libmata/alphabets.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/libmata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:27:23.922237 libmata-0.92.0/libmata/nfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1680473 2023-08-08 05:28:12.175288 libmata-0.92.0/libmata/nfa/nfa.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/nfa/nfa.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    43696 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/nfa/nfa.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   434195 2023-08-08 05:28:12.923304 libmata-0.92.0/libmata/nfa/strings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/nfa/strings.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/nfa/strings.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   249287 2023-08-08 05:28:13.403314 libmata-0.92.0/libmata/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   696495 2023-08-08 05:28:14.135330 libmata-0.92.0/libmata/plotting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/plotting.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   458228 2023-08-08 05:28:14.259333 libmata-0.92.0/libmata/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-08-08 05:27:23.926236 libmata-0.92.0/libmata/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-08-08 05:27:23.890236 libmata-0.92.0/mata/3rdparty/args.hxx
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-08-08 05:27:23.898236 libmata-0.92.0/mata/3rdparty/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-08-08 05:27:23.894236 libmata-0.92.0/mata/3rdparty/catch.hpp.1.9.3
+-rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-08-08 05:27:23.898236 libmata-0.92.0/mata/3rdparty/catch.hpp.2.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-08-08 05:27:23.898236 libmata-0.92.0/mata/3rdparty/catch.hpp.2.13.9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-08-08 05:27:23.898236 libmata-0.92.0/mata/3rdparty/cudd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-08-08 05:27:23.898236 libmata-0.92.0/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.168340 libmata-0.92.0/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-08-08 05:27:23.902236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-08-08 05:27:23.906236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.168340 libmata-0.92.0/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-08-08 05:27:23.910236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.168340 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/composeids.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-08-08 05:27:23.914236 libmata-0.92.0/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.160340 libmata-0.92.0/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.160340 libmata-0.92.0/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-08-08 05:27:23.918236 libmata-0.92.0/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-08-08 05:27:23.922237 libmata-0.92.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-08-08 05:32:18.076339 libmata-0.92.0/mata/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   101164 2023-08-08 05:32:18.076339 libmata-0.92.0/mata/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-08 05:32:18.076339 libmata-0.92.0/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-08 05:32:18.076339 libmata-0.92.0/mata/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-08 05:32:18.076339 libmata-0.92.0/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 05:32:18.076339 libmata-0.92.0/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/cmake/Modules/Catch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/cmake/Modules/CatchAddTests.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/cmake/Modules/CodeCoverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/cmake/Modules/FindValgrind.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/cmake/Modules/GetGitRevisionDescription.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.164340 libmata-0.92.0/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.172340 libmata-0.92.0/mata/include/mata/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/afa/afa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/alphabet.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/include/mata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/nfa/algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/nfa/builder.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/nfa/delta.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    32333 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/nfa/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/nfa/plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/nfa/strings.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/nfa/types.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/include/mata/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/parser/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/parser/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/parser/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/parser/re2parser.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/include/mata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/utils/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/utils/number-predicate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15389 2023-08-08 05:27:23.926236 libmata-0.92.0/mata/include/mata/utils/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/include/mata/utils/sparse-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/include/mata/utils/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/include/mata/utils/util.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/scripts/merge_static_libraries.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/src/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    38724 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/complement.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/delta.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    35569 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31253 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/operations.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/nfa/universal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-08 05:27:23.930237 libmata-0.92.0/mata/src/strings/nfa-strings.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/tests/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    42818 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/tests/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32084 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/nfa/nfa-concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/nfa/nfa-intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/nfa/nfa-profiling.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/nfa/nfa-util.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    86684 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/ord-vector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/re2parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/sparse-set.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:18.176341 libmata-0.92.0/mata/tests/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/strings/nfa-string-solving.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-08 05:27:23.946237 libmata-0.92.0/mata/tests/synchronized-iterator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 05:27:23.926236 libmata-0.92.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-08 05:27:23.926236 libmata-0.92.0/setup.py
```

### Comparing `libmata-0.91.0/PKG-INFO` & `libmata-0.92.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 0.91.0
+Version: 0.92.0
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
```

### Comparing `libmata-0.91.0/libmata/alphabets.cpp` & `libmata-0.92.0/libmata/alphabets.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1460,43 +1460,43 @@
  */
 struct __pyx_obj_7libmata_5utils_BinaryRelation {
   PyObject_HEAD
   Simlib::Util::BinaryRelation *thisptr;
 };
 
 
-/* "libmata/nfa/nfa.pxd":211
+/* "libmata/nfa/nfa.pxd":210
  * #
  * # This is needed in order for these classes to be used in other packages.
  * cdef class Nfa:             # <<<<<<<<<<<<<<
  *     # TODO: Shared pointers are not ideal as they bring some overhead which could be substantial in theory. We are not
  *     #  sure whether the shared pointers will be a problem in this case, but it would be good to pay attention to this and
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Nfa {
   PyObject_HEAD
   std::shared_ptr<Mata::Nfa::Nfa>  thisptr;
   PyObject *label;
 };
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Trans {
   PyObject_HEAD
   struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans *__pyx_vtab;
   Mata::Nfa::Trans *thisptr;
 };
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 struct __pyx_obj_7libmata_9alphabets_Alphabet {
@@ -1528,15 +1528,15 @@
 struct __pyx_obj_7libmata_9alphabets_IntAlphabet {
   struct __pyx_obj_7libmata_9alphabets_Alphabet __pyx_base;
   Mata::IntAlphabet *thisptr;
 };
 
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 
@@ -4474,15 +4474,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_9alphabets_16OnTheFlyAlphabet_6add_symbols_from_symbol_map(struct __pyx_obj_7libmata_9alphabets_OnTheFlyAlphabet *__pyx_v_self, PyObject *__pyx_v_symbol_map) {
-  Mata::StringToSymbolMap __pyx_v_c_symbol_map;
+  Mata::OnTheFlyAlphabet::StringToSymbolMap __pyx_v_c_symbol_map;
   PyObject *__pyx_v_symbol = NULL;
   PyObject *__pyx_v_value = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
@@ -4496,18 +4496,18 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_symbols_from_symbol_map", 0);
 
   /* "libmata/alphabets.pyx":60
  *         """
- *         cdef StringToSymbolMap c_symbol_map
+ *         cdef COnTheFlyAlphabet.StringToSymbolMap c_symbol_map
  *         for symbol, value in symbol_map.items():             # <<<<<<<<<<<<<<
  *             c_symbol_map[symbol.encode('utf-8')] = value
- *         self.thisptr.add_symbols_from(c_symbol_map)
+ *         self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)
  */
   __pyx_t_2 = 0;
   __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_symbol_map, 1, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_5;
   __pyx_t_5 = 0;
@@ -4519,18 +4519,18 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XDECREF_SET(__pyx_v_symbol, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_6);
     __pyx_t_6 = 0;
 
     /* "libmata/alphabets.pyx":61
- *         cdef StringToSymbolMap c_symbol_map
+ *         cdef COnTheFlyAlphabet.StringToSymbolMap c_symbol_map
  *         for symbol, value in symbol_map.items():
  *             c_symbol_map[symbol.encode('utf-8')] = value             # <<<<<<<<<<<<<<
- *         self.thisptr.add_symbols_from(c_symbol_map)
+ *         self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)
  * 
  */
     __pyx_t_8 = __Pyx_PyInt_As_size_t(__pyx_v_value); if (unlikely((__pyx_t_8 == ((Mata::Symbol)-1)) && PyErr_Occurred())) __PYX_ERR(1, 61, __pyx_L1_error)
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_symbol, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_9 = NULL;
     __pyx_t_7 = 0;
@@ -4557,19 +4557,19 @@
     (__pyx_v_c_symbol_map[__pyx_t_10]) = __pyx_t_8;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "libmata/alphabets.pyx":62
  *         for symbol, value in symbol_map.items():
  *             c_symbol_map[symbol.encode('utf-8')] = value
- *         self.thisptr.add_symbols_from(c_symbol_map)             # <<<<<<<<<<<<<<
+ *         self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)             # <<<<<<<<<<<<<<
  * 
  *     def add_symbols_for_names(self, symbol_names: list[str]) -> None:
  */
-  (void)(__pyx_v_self->thisptr->add_symbols_from(__pyx_v_c_symbol_map));
+  __pyx_v_self->thisptr->add_symbols_from(((Mata::OnTheFlyAlphabet::StringToSymbolMap)__pyx_v_c_symbol_map));
 
   /* "libmata/alphabets.pyx":54
  *         return alphabet
  * 
  *     def add_symbols_from_symbol_map(self, symbol_map: dict[str, int]) -> None:             # <<<<<<<<<<<<<<
  *         """Add symbols from symbol_map to the current alphabet.
  * 
@@ -4590,15 +4590,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "libmata/alphabets.pyx":64
- *         self.thisptr.add_symbols_from(c_symbol_map)
+ *         self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)
  * 
  *     def add_symbols_for_names(self, symbol_names: list[str]) -> None:             # <<<<<<<<<<<<<<
  *         """Add symbols for symbol names to the current alphabet.
  * 
  */
 
 /* Python wrapper */
@@ -4765,18 +4765,18 @@
   /* "libmata/alphabets.pyx":72
  *         for symbol_name in symbol_names:
  *             c_symbol_names.push_back(symbol_name.encode('utf-8'))
  *         self.thisptr.add_symbols_from(c_symbol_names)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  (void)(__pyx_v_self->thisptr->add_symbols_from(__pyx_v_c_symbol_names));
+  __pyx_v_self->thisptr->add_symbols_from(__pyx_v_c_symbol_names);
 
   /* "libmata/alphabets.pyx":64
- *         self.thisptr.add_symbols_from(c_symbol_map)
+ *         self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)
  * 
  *     def add_symbols_for_names(self, symbol_names: list[str]) -> None:             # <<<<<<<<<<<<<<
  *         """Add symbols for symbol names to the current alphabet.
  * 
  */
 
   /* function exit code */
@@ -6947,15 +6947,15 @@
  */
   __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_symbol_map, __pyx_n_s_c_symbol_map, __pyx_n_s_symbol, __pyx_n_s_value); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
   __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_alphabets_pyx, __pyx_n_s_add_symbols_from_symbol_map, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 54, __pyx_L1_error)
 
   /* "libmata/alphabets.pyx":64
- *         self.thisptr.add_symbols_from(c_symbol_map)
+ *         self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)
  * 
  *     def add_symbols_for_names(self, symbol_names: list[str]) -> None:             # <<<<<<<<<<<<<<
  *         """Add symbols for symbol names to the current alphabet.
  * 
  */
   __pyx_tuple__13 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_symbol_names, __pyx_n_s_c_symbol_names, __pyx_n_s_symbol_name); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
@@ -7226,19 +7226,19 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 211, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 211, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(3, 219, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(3, 219, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 210, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(3, 218, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(3, 218, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7658,15 +7658,15 @@
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_7libmata_9alphabets_OnTheFlyAlphabet->tp_dict, __pyx_n_s_add_symbols_from_symbol_map, __pyx_t_3) < 0) __PYX_ERR(1, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_7libmata_9alphabets_OnTheFlyAlphabet);
 
   /* "libmata/alphabets.pyx":64
- *         self.thisptr.add_symbols_from(c_symbol_map)
+ *         self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)
  * 
  *     def add_symbols_for_names(self, symbol_names: list[str]) -> None:             # <<<<<<<<<<<<<<
  *         """Add symbols for symbol names to the current alphabet.
  * 
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
```

### Comparing `libmata-0.91.0/libmata/alphabets.pyx` & `libmata-0.92.0/libmata/alphabets.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,18 @@
         return alphabet
 
     def add_symbols_from_symbol_map(self, symbol_map: dict[str, int]) -> None:
         """Add symbols from symbol_map to the current alphabet.
 
         :param symbol_map: Map mapping strings to symbols.
         """
-        cdef StringToSymbolMap c_symbol_map
+        cdef COnTheFlyAlphabet.StringToSymbolMap c_symbol_map
         for symbol, value in symbol_map.items():
             c_symbol_map[symbol.encode('utf-8')] = value
-        self.thisptr.add_symbols_from(c_symbol_map)
+        self.thisptr.add_symbols_from(<COnTheFlyAlphabet.StringToSymbolMap>c_symbol_map)
 
     def add_symbols_for_names(self, symbol_names: list[str]) -> None:
         """Add symbols for symbol names to the current alphabet.
 
         :param symbol_names: Vector of symbol names.
         """
         cdef vector[string] c_symbol_names
```

### Comparing `libmata-0.91.0/libmata/nfa/nfa.cpp` & `libmata-0.92.0/libmata/nfa/nfa.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1466,42 +1466,42 @@
  */
 struct __pyx_obj_7libmata_5utils_BinaryRelation {
   PyObject_HEAD
   Simlib::Util::BinaryRelation *thisptr;
 };
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 struct __pyx_obj_7libmata_9alphabets_Alphabet {
   PyObject_HEAD
   struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *__pyx_vtab;
 };
 
 
-/* "libmata/nfa/nfa.pxd":211
+/* "libmata/nfa/nfa.pxd":210
  * #
  * # This is needed in order for these classes to be used in other packages.
  * cdef class Nfa:             # <<<<<<<<<<<<<<
  *     # TODO: Shared pointers are not ideal as they bring some overhead which could be substantial in theory. We are not
  *     #  sure whether the shared pointers will be a problem in this case, but it would be good to pay attention to this and
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Nfa {
   PyObject_HEAD
   std::shared_ptr<Mata::Nfa::Nfa>  thisptr;
   PyObject *label;
 };
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Trans {
@@ -1550,15 +1550,15 @@
   Mata::Nfa::Trans __pyx_v_lhs;
   struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_self;
   struct __pyx_obj_7libmata_3nfa_3nfa_Trans *__pyx_v_trans;
 };
 
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 
@@ -2592,15 +2592,14 @@
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 static PyObject *__pyx_convert_pair_to_py_std_3a__3a_pair_3c_Mata_3a__3a_Nfa_3a__3a_State_2c_Mata_3a__3a_Nfa_3a__3a_State_3e_______Mata_3a__3a_Nfa_3a__3a_State(std::pair<std::pair<Mata::Nfa::State,Mata::Nfa::State> ,Mata::Nfa::State>  const &); /*proto*/
 static std::unordered_map<std::string,std::string>  __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_std_3a__3a_string(PyObject *); /*proto*/
-static std::unordered_map<std::string,Mata::Symbol>  __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol(PyObject *); /*proto*/
 static std::vector<std::string>  __pyx_convert_vector_from_py_std_3a__3a_string(PyObject *); /*proto*/
 static std::vector<uint8_t>  __pyx_convert_vector_from_py_uint8_t(PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "libmata.nfa.nfa"
 extern int __pyx_module_is_main_libmata__nfa__nfa;
 int __pyx_module_is_main_libmata__nfa__nfa = 0;
@@ -2890,15 +2889,14 @@
 static const char __pyx_k_get_num_of_trans[] = "get_num_of_trans";
 static const char __pyx_k_graphviz_command[] = "graphviz_command";
 static const char __pyx_k_is_deterministic[] = "is_deterministic";
 static const char __pyx_k_make_final_state[] = "make_final_state";
 static const char __pyx_k_pandas_DataFrame[] = "pandas.DataFrame";
 static const char __pyx_k_preserve_epsilon[] = "preserve_epsilon";
 static const char __pyx_k_remove_trans_raw[] = "remove_trans_raw";
-static const char __pyx_k_string_to_symbol[] = "string_to_symbol";
 static const char __pyx_k_transitions_list[] = "transitions_list";
 static const char __pyx_k_translate_symbol[] = "translate_symbol";
 static const char __pyx_k_unpiped_commands[] = "unpiped_commands";
 static const char __pyx_k_Nfa_add_new_state[] = "Nfa.add_new_state";
 static const char __pyx_k_Nfa_clear_initial[] = "Nfa.clear_initial";
 static const char __pyx_k_Nfa_unify_initial[] = "Nfa.unify_initial";
 static const char __pyx_k_equivalence_check[] = "equivalence_check";
@@ -2970,15 +2968,15 @@
 static const char __pyx_k_determinize_with_subset_map[] = "determinize_with_subset_map";
 static const char __pyx_k_get_word_for_path_line_1096[] = "get_word_for_path (line 1096)";
 static const char __pyx_k_run_safely_external_command[] = "run_safely_external_command";
 static const char __pyx_k_Nfa_get_transitions_to_state[] = "Nfa.get_transitions_to_state";
 static const char __pyx_k_intersection_with_product_map[] = "intersection_with_product_map";
 static const char __pyx_k_Nfa_get_transitions_from_state[] = "Nfa.get_transitions_from_state";
 static const char __pyx_k_tuple_Nfa_dict_str_str_dict_str[] = "tuple[Nfa, dict[str, str], dict[str, str]]";
-static const char __pyx_k_Encodes_word_based_on_a_string_t[] = "Encodes word based on a string to symbol map\n\n    >>> mata_nfa.Nfa.encode_word({'a': 1, 'b': 2, \"c\": 0}, \"abca\")\n    [1, 2, 0, 1]\n\n    :param dict string_to_symbol: dictionary of strings to integers\n    :param word: list of strings representing a encoded word\n    :return:\n    ";
+static const char __pyx_k_Encodes_word_based_on_a_passed_a[] = "Encodes word based on a passed alphabet\n\n    >>> mata_nfa.Nfa.encode_word(OnTheFlyAlphabet.from_symbol_map({'a': 1, 'b': 2, \"c\": 0}), \"abca\")\n    [1, 2, 0, 1]\n\n    :param alph.Alphabet alphabet: Alphabet to encode the word with.\n    :param word: list of strings representing an encoded word.\n    :return: Encoded word.\n    ";
 static const char __pyx_k_For_a_given_path_set_of_states_r[] = "For a given path (set of states) returns a corresponding word\n\n    >>> mata_nfa.Nfa.get_word_for_path(lhs, [0, 1, 2])\n    ([1, 1], True)\n\n    :param Nfa lhs: source automaton\n    :param list path: list of states\n    :return: pair of word (list of symbols) and true or false, whether the search was successful\n    ";
 static const char __pyx_k_Nfa_get_trans_from_state_as_sequ[] = "Nfa.get_trans_from_state_as_sequence";
 static const char __pyx_k_concatenate_with_result_state_ma[] = "concatenate_with_result_state_maps";
 static const char __pyx_k_get_trans_from_state_as_sequence[] = "get_trans_from_state_as_sequence";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_epsilon(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
@@ -3095,15 +3093,15 @@
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_40is_included(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_rhs, struct __pyx_obj_7libmata_9alphabets_Alphabet *__pyx_v_alphabet, PyObject *__pyx_v_params); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_42equivalence_check(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_rhs, struct __pyx_obj_7libmata_9alphabets_Alphabet *__pyx_v_alphabet, PyObject *__pyx_v_params); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_44is_complete(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs, struct __pyx_obj_7libmata_9alphabets_Alphabet *__pyx_v_alphabet); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_46is_in_lang(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs, std::vector<Mata::Symbol>  __pyx_v_word); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_48is_prefix_in_lang(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs, std::vector<Mata::Symbol>  __pyx_v_word); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_50accepts_epsilon(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_52get_word_for_path(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs, PyObject *__pyx_v_path); /* proto */
-static PyObject *__pyx_pf_7libmata_3nfa_3nfa_54encode_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_string_to_symbol, PyObject *__pyx_v_word); /* proto */
+static PyObject *__pyx_pf_7libmata_3nfa_3nfa_54encode_word(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_9alphabets_Alphabet *__pyx_v_alphabet, PyObject *__pyx_v_word); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_56divisible_by(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_k); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_58run_safely_external_command(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_cmd, PyObject *__pyx_v_check_results, PyObject *__pyx_v_quiet, PyObject *__pyx_v_timeout, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_60get_elements_from_bool_vec(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_bool_vec); /* proto */
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_62store(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_tp_new_7libmata_3nfa_3nfa_Nfa(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_7libmata_3nfa_3nfa_Trans(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_7libmata_3nfa_3nfa_Run(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -3184,15 +3182,15 @@
   PyObject *__pyx_kp_u_1_5;
   PyObject *__pyx_n_s_AssertionError;
   PyObject *__pyx_n_s_CalledProcessError;
   PyObject *__pyx_kp_u_Cannot_translate_symbol;
   PyObject *__pyx_kp_u_Courier_Bold;
   PyObject *__pyx_n_s_DataFrame;
   PyObject *__pyx_n_s_DiGraph;
-  PyObject *__pyx_kp_u_Encodes_word_based_on_a_string_t;
+  PyObject *__pyx_kp_u_Encodes_word_based_on_a_passed_a;
   PyObject *__pyx_kp_u_For_a_given_path_set_of_states_r;
   PyObject *__pyx_n_s_G;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_n_s_Move;
   PyObject *__pyx_kp_s_Move_None;
   PyObject *__pyx_n_s_Move___neq;
   PyObject *__pyx_n_s_Move___reduce_cython;
@@ -3494,15 +3492,14 @@
   PyObject *__pyx_n_s_states;
   PyObject *__pyx_n_s_stderr;
   PyObject *__pyx_n_s_stdin;
   PyObject *__pyx_n_s_stdout;
   PyObject *__pyx_n_s_store;
   PyObject *__pyx_n_s_store_2;
   PyObject *__pyx_n_s_str;
-  PyObject *__pyx_n_s_string_to_symbol;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_strip;
   PyObject *__pyx_n_u_style;
   PyObject *__pyx_n_s_subprocess;
   PyObject *__pyx_n_s_subset_map;
   PyObject *__pyx_n_s_symb;
   PyObject *__pyx_n_s_symbol;
@@ -3765,15 +3762,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_1_5);
   Py_CLEAR(clear_module_state->__pyx_n_s_AssertionError);
   Py_CLEAR(clear_module_state->__pyx_n_s_CalledProcessError);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Cannot_translate_symbol);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Courier_Bold);
   Py_CLEAR(clear_module_state->__pyx_n_s_DataFrame);
   Py_CLEAR(clear_module_state->__pyx_n_s_DiGraph);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Encodes_word_based_on_a_string_t);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Encodes_word_based_on_a_passed_a);
   Py_CLEAR(clear_module_state->__pyx_kp_u_For_a_given_path_set_of_states_r);
   Py_CLEAR(clear_module_state->__pyx_n_s_G);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Move);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Move_None);
   Py_CLEAR(clear_module_state->__pyx_n_s_Move___neq);
   Py_CLEAR(clear_module_state->__pyx_n_s_Move___reduce_cython);
@@ -4075,15 +4072,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_states);
   Py_CLEAR(clear_module_state->__pyx_n_s_stderr);
   Py_CLEAR(clear_module_state->__pyx_n_s_stdin);
   Py_CLEAR(clear_module_state->__pyx_n_s_stdout);
   Py_CLEAR(clear_module_state->__pyx_n_s_store);
   Py_CLEAR(clear_module_state->__pyx_n_s_store_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_str);
-  Py_CLEAR(clear_module_state->__pyx_n_s_string_to_symbol);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_strip);
   Py_CLEAR(clear_module_state->__pyx_n_u_style);
   Py_CLEAR(clear_module_state->__pyx_n_s_subprocess);
   Py_CLEAR(clear_module_state->__pyx_n_s_subset_map);
   Py_CLEAR(clear_module_state->__pyx_n_s_symb);
   Py_CLEAR(clear_module_state->__pyx_n_s_symbol);
@@ -4322,15 +4318,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_1_5);
   Py_VISIT(traverse_module_state->__pyx_n_s_AssertionError);
   Py_VISIT(traverse_module_state->__pyx_n_s_CalledProcessError);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Cannot_translate_symbol);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Courier_Bold);
   Py_VISIT(traverse_module_state->__pyx_n_s_DataFrame);
   Py_VISIT(traverse_module_state->__pyx_n_s_DiGraph);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Encodes_word_based_on_a_string_t);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Encodes_word_based_on_a_passed_a);
   Py_VISIT(traverse_module_state->__pyx_kp_u_For_a_given_path_set_of_states_r);
   Py_VISIT(traverse_module_state->__pyx_n_s_G);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Move);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Move_None);
   Py_VISIT(traverse_module_state->__pyx_n_s_Move___neq);
   Py_VISIT(traverse_module_state->__pyx_n_s_Move___reduce_cython);
@@ -4632,15 +4628,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_states);
   Py_VISIT(traverse_module_state->__pyx_n_s_stderr);
   Py_VISIT(traverse_module_state->__pyx_n_s_stdin);
   Py_VISIT(traverse_module_state->__pyx_n_s_stdout);
   Py_VISIT(traverse_module_state->__pyx_n_s_store);
   Py_VISIT(traverse_module_state->__pyx_n_s_store_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_str);
-  Py_VISIT(traverse_module_state->__pyx_n_s_string_to_symbol);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_strip);
   Py_VISIT(traverse_module_state->__pyx_n_u_style);
   Py_VISIT(traverse_module_state->__pyx_n_s_subprocess);
   Py_VISIT(traverse_module_state->__pyx_n_s_subset_map);
   Py_VISIT(traverse_module_state->__pyx_n_s_symb);
   Py_VISIT(traverse_module_state->__pyx_n_s_symbol);
@@ -4917,15 +4912,15 @@
 #define __pyx_kp_u_1_5 __pyx_mstate_global->__pyx_kp_u_1_5
 #define __pyx_n_s_AssertionError __pyx_mstate_global->__pyx_n_s_AssertionError
 #define __pyx_n_s_CalledProcessError __pyx_mstate_global->__pyx_n_s_CalledProcessError
 #define __pyx_kp_u_Cannot_translate_symbol __pyx_mstate_global->__pyx_kp_u_Cannot_translate_symbol
 #define __pyx_kp_u_Courier_Bold __pyx_mstate_global->__pyx_kp_u_Courier_Bold
 #define __pyx_n_s_DataFrame __pyx_mstate_global->__pyx_n_s_DataFrame
 #define __pyx_n_s_DiGraph __pyx_mstate_global->__pyx_n_s_DiGraph
-#define __pyx_kp_u_Encodes_word_based_on_a_string_t __pyx_mstate_global->__pyx_kp_u_Encodes_word_based_on_a_string_t
+#define __pyx_kp_u_Encodes_word_based_on_a_passed_a __pyx_mstate_global->__pyx_kp_u_Encodes_word_based_on_a_passed_a
 #define __pyx_kp_u_For_a_given_path_set_of_states_r __pyx_mstate_global->__pyx_kp_u_For_a_given_path_set_of_states_r
 #define __pyx_n_s_G __pyx_mstate_global->__pyx_n_s_G
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_n_s_Move __pyx_mstate_global->__pyx_n_s_Move
 #define __pyx_kp_s_Move_None __pyx_mstate_global->__pyx_kp_s_Move_None
 #define __pyx_n_s_Move___neq __pyx_mstate_global->__pyx_n_s_Move___neq
 #define __pyx_n_s_Move___reduce_cython __pyx_mstate_global->__pyx_n_s_Move___reduce_cython
@@ -5227,15 +5222,14 @@
 #define __pyx_n_s_states __pyx_mstate_global->__pyx_n_s_states
 #define __pyx_n_s_stderr __pyx_mstate_global->__pyx_n_s_stderr
 #define __pyx_n_s_stdin __pyx_mstate_global->__pyx_n_s_stdin
 #define __pyx_n_s_stdout __pyx_mstate_global->__pyx_n_s_stdout
 #define __pyx_n_s_store __pyx_mstate_global->__pyx_n_s_store
 #define __pyx_n_s_store_2 __pyx_mstate_global->__pyx_n_s_store_2
 #define __pyx_n_s_str __pyx_mstate_global->__pyx_n_s_str
-#define __pyx_n_s_string_to_symbol __pyx_mstate_global->__pyx_n_s_string_to_symbol
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_strip __pyx_mstate_global->__pyx_n_s_strip
 #define __pyx_n_u_style __pyx_mstate_global->__pyx_n_u_style
 #define __pyx_n_s_subprocess __pyx_mstate_global->__pyx_n_s_subprocess
 #define __pyx_n_s_subset_map __pyx_mstate_global->__pyx_n_s_subset_map
 #define __pyx_n_s_symb __pyx_mstate_global->__pyx_n_s_symb
 #define __pyx_n_s_symbol __pyx_mstate_global->__pyx_n_s_symbol
@@ -6610,195 +6604,14 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static std::unordered_map<std::string,Mata::Symbol>  __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol(PyObject *__pyx_v_o) {
-  std::unordered_map<std::string,Mata::Symbol>  __pyx_v_m;
-  PyObject *__pyx_v_key = NULL;
-  PyObject *__pyx_v_value = NULL;
-  std::unordered_map<std::string,Mata::Symbol>  __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  std::string __pyx_t_9;
-  Mata::Symbol __pyx_t_10;
-  std::pair<std::string,Mata::Symbol>  __pyx_t_11;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol", 0);
-
-  /* "map.from_py":209
- * cdef map[X,Y] __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol(object o) except *:
- *     cdef map[X,Y] m
- *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
- *         for key, value in o.iteritems():
- *             m.insert(pair[X,Y](<X>key, <Y>value))
- */
-  __pyx_t_1 = (PY_MAJOR_VERSION < 3);
-  if (__pyx_t_1) {
-
-    /* "map.from_py":210
- *     cdef map[X,Y] m
- *     if PY_MAJOR_VERSION < 3:
- *         for key, value in o.iteritems():             # <<<<<<<<<<<<<<
- *             m.insert(pair[X,Y](<X>key, <Y>value))
- *     else:
- */
-    __pyx_t_3 = 0;
-    if (unlikely(__pyx_v_o == Py_None)) {
-      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "iteritems");
-      __PYX_ERR(0, 210, __pyx_L1_error)
-    }
-    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_iteritems, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_2);
-    __pyx_t_2 = __pyx_t_6;
-    __pyx_t_6 = 0;
-    while (1) {
-      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
-      if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 210, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_7);
-      __pyx_t_7 = 0;
-
-      /* "map.from_py":211
- *     if PY_MAJOR_VERSION < 3:
- *         for key, value in o.iteritems():
- *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
- *     else:
- *         for key, value in o.items():
- */
-      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L1_error)
-      __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((Mata::Symbol)-1)) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L1_error)
-      try {
-        __pyx_t_11 = std::pair<std::string,Mata::Symbol> (((std::string)__pyx_t_9), ((Mata::Symbol)__pyx_t_10));
-      } catch(...) {
-        __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 211, __pyx_L1_error)
-      }
-      try {
-        __pyx_v_m.insert(__pyx_t_11);
-      } catch(...) {
-        __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 211, __pyx_L1_error)
-      }
-    }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-    /* "map.from_py":209
- * cdef map[X,Y] __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol(object o) except *:
- *     cdef map[X,Y] m
- *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
- *         for key, value in o.iteritems():
- *             m.insert(pair[X,Y](<X>key, <Y>value))
- */
-    goto __pyx_L3;
-  }
-
-  /* "map.from_py":213
- *             m.insert(pair[X,Y](<X>key, <Y>value))
- *     else:
- *         for key, value in o.items():             # <<<<<<<<<<<<<<
- *             m.insert(pair[X,Y](<X>key, <Y>value))
- *     return m
- */
-  /*else*/ {
-    __pyx_t_4 = 0;
-    if (unlikely(__pyx_v_o == Py_None)) {
-      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 213, __pyx_L1_error)
-    }
-    __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_5)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 213, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_2);
-    __pyx_t_2 = __pyx_t_7;
-    __pyx_t_7 = 0;
-    while (1) {
-      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_3, &__pyx_t_4, &__pyx_t_7, &__pyx_t_6, NULL, __pyx_t_5);
-      if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 213, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_6);
-      __pyx_t_6 = 0;
-
-      /* "map.from_py":214
- *     else:
- *         for key, value in o.items():
- *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
- *     return m
- * 
- */
-      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L1_error)
-      __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((Mata::Symbol)-1)) && PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L1_error)
-      try {
-        __pyx_t_11 = std::pair<std::string,Mata::Symbol> (((std::string)__pyx_t_9), ((Mata::Symbol)__pyx_t_10));
-      } catch(...) {
-        __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 214, __pyx_L1_error)
-      }
-      try {
-        __pyx_v_m.insert(__pyx_t_11);
-      } catch(...) {
-        __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 214, __pyx_L1_error)
-      }
-    }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  }
-  __pyx_L3:;
-
-  /* "map.from_py":215
- *         for key, value in o.items():
- *             m.insert(pair[X,Y](<X>key, <Y>value))
- *     return m             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_m;
-  goto __pyx_L0;
-
-  /* "map.from_py":207
- * 
- * @cname("__pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol")
- * cdef map[X,Y] __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef map[X,Y] m
- *     if PY_MAJOR_VERSION < 3:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("map.from_py.__pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_key);
-  __Pyx_XDECREF(__pyx_v_value);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "vector.from_py":45
  * 
  * @cname("__pyx_convert_vector_from_py_std_3a__3a_string")
  * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_string(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef vector[X] v
  *     for item in o:
  */
@@ -15019,15 +14832,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_3Nfa_67trim_with_state_map(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_self) {
-  Mata::Nfa::StateToStateMap __pyx_v_state_map;
+  Mata::Nfa::StateRenaming __pyx_v_state_map;
   PyObject *__pyx_8genexpr6__pyx_v_k = NULL;
   PyObject *__pyx_8genexpr6__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   std::unordered_map<Mata::Nfa::State,Mata::Nfa::State> ::iterator __pyx_t_2;
   std::pair<Mata::Nfa::State,Mata::Nfa::State>  __pyx_t_3;
@@ -15039,23 +14852,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("trim_with_state_map", 0);
 
   /* "libmata/nfa/nfa.pyx":508
  *         """
- *         cdef StateToStateMap state_map
+ *         cdef StateRenaming state_map
  *         self.thisptr.get().trim(&state_map)             # <<<<<<<<<<<<<<
  *         return {k: v for k, v in state_map}
  * 
  */
   __pyx_v_self->thisptr.get()->trim((&__pyx_v_state_map));
 
   /* "libmata/nfa/nfa.pyx":509
- *         cdef StateToStateMap state_map
+ *         cdef StateRenaming state_map
  *         self.thisptr.get().trim(&state_map)
  *         return {k: v for k, v in state_map}             # <<<<<<<<<<<<<<
  * 
  *     def get_one_letter_aut(self) -> Nfa:
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
@@ -19244,16 +19057,16 @@
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_14concatenate_with_result_state_maps(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_lhs, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_rhs, bool __pyx_v_use_epsilon) {
   struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_result = NULL;
-  Mata::Nfa::StateToStateMap __pyx_v_c_lhs_map;
-  Mata::Nfa::StateToStateMap __pyx_v_c_rhs_map;
+  Mata::Nfa::StateRenaming __pyx_v_c_lhs_map;
+  Mata::Nfa::StateRenaming __pyx_v_c_rhs_map;
   PyObject *__pyx_v_lhs_map = NULL;
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_value = NULL;
   PyObject *__pyx_v_rhs_map = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -19268,25 +19081,25 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("concatenate_with_result_state_maps", 0);
 
   /* "libmata/nfa/nfa.pyx":784
  *     :return: Nfa: Concatenated automaton.
  *     """
  *     result = Nfa()             # <<<<<<<<<<<<<<
- *     cdef StateToStateMap c_lhs_map
- *     cdef StateToStateMap c_rhs_map
+ *     cdef StateRenaming c_lhs_map
+ *     cdef StateRenaming c_rhs_map
  */
   __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7libmata_3nfa_3nfa_Nfa)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "libmata/nfa/nfa.pyx":787
- *     cdef StateToStateMap c_lhs_map
- *     cdef StateToStateMap c_rhs_map
+ *     cdef StateRenaming c_lhs_map
+ *     cdef StateRenaming c_rhs_map
  *     mata_nfa.c_concatenate(result.thisptr.get(), dereference(lhs.thisptr.get()), dereference(rhs.thisptr.get()),             # <<<<<<<<<<<<<<
  *                          use_epsilon, &c_lhs_map, &c_rhs_map)
  *     lhs_map = {}
  */
   Mata::Nfa::Plumbing::concatenate(__pyx_v_result->thisptr.get(), (*__pyx_v_lhs->thisptr.get()), (*__pyx_v_rhs->thisptr.get()), __pyx_v_use_epsilon, (&__pyx_v_c_lhs_map), (&__pyx_v_c_rhs_map));
 
   /* "libmata/nfa/nfa.pyx":789
@@ -19658,15 +19471,15 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  Mata::Nfa::StringMap __pyx_t_14;
+  Mata::Nfa::ParameterMap __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("complement", 0);
   __Pyx_INCREF(__pyx_v_params);
 
   /* "libmata/nfa/nfa.pyx":809
@@ -20733,15 +20546,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_26reduce_with_state_map(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_aut, bool __pyx_v_trim_input, PyObject *__pyx_v_params) {
-  Mata::Nfa::StateToStateMap __pyx_v_state_map;
+  Mata::Nfa::StateRenaming __pyx_v_state_map;
   struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_result = NULL;
   PyObject *__pyx_9genexpr14__pyx_v_k = NULL;
   PyObject *__pyx_9genexpr14__pyx_v_v = NULL;
   PyObject *__pyx_9genexpr15__pyx_v_k = NULL;
   PyObject *__pyx_9genexpr15__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -20752,29 +20565,29 @@
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
-  Mata::Nfa::StringMap __pyx_t_12;
+  Mata::Nfa::ParameterMap __pyx_t_12;
   std::unordered_map<Mata::Nfa::State,Mata::Nfa::State> ::iterator __pyx_t_13;
   std::pair<Mata::Nfa::State,Mata::Nfa::State>  __pyx_t_14;
   PyObject *(*__pyx_t_15)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reduce_with_state_map", 0);
   __Pyx_INCREF(__pyx_v_params);
 
   /* "libmata/nfa/nfa.pyx":873
  *     :return: (Reduced automaton, state map of original to new states)
  *     """
  *     params = params or {"algorithm": "simulation"}             # <<<<<<<<<<<<<<
- *     cdef StateToStateMap state_map
+ *     cdef StateRenaming state_map
  *     result = Nfa()
  */
   __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_params); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 873, __pyx_L1_error)
   if (!__pyx_t_2) {
   } else {
     __Pyx_INCREF(__pyx_v_params);
     __pyx_t_1 = __pyx_v_params;
@@ -20788,26 +20601,26 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __Pyx_DECREF_SET(__pyx_v_params, __pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "libmata/nfa/nfa.pyx":875
  *     params = params or {"algorithm": "simulation"}
- *     cdef StateToStateMap state_map
+ *     cdef StateRenaming state_map
  *     result = Nfa()             # <<<<<<<<<<<<<<
  *     mata_nfa.c_reduce(result.thisptr.get(), dereference(aut.thisptr.get()), trim_input, &state_map,
  *                     {
  */
   __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7libmata_3nfa_3nfa_Nfa)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 875, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "libmata/nfa/nfa.pyx":876
- *     cdef StateToStateMap state_map
+ *     cdef StateRenaming state_map
  *     result = Nfa()
  *     mata_nfa.c_reduce(result.thisptr.get(), dereference(aut.thisptr.get()), trim_input, &state_map,             # <<<<<<<<<<<<<<
  *                     {
  *                         k.encode('utf-8'): v.encode('utf-8') for k, v in params.items()
  */
   { /* enter inner scope */
 
@@ -20914,15 +20727,15 @@
  *                         k.encode('utf-8'): v.encode('utf-8') for k, v in params.items()
  *                     }
  */
   __pyx_t_12 = __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_std_3a__3a_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 877, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "libmata/nfa/nfa.pyx":876
- *     cdef StateToStateMap state_map
+ *     cdef StateRenaming state_map
  *     result = Nfa()
  *     mata_nfa.c_reduce(result.thisptr.get(), dereference(aut.thisptr.get()), trim_input, &state_map,             # <<<<<<<<<<<<<<
  *                     {
  *                         k.encode('utf-8'): v.encode('utf-8') for k, v in params.items()
  */
   Mata::Nfa::Plumbing::reduce(__pyx_v_result->thisptr.get(), (*__pyx_v_aut->thisptr.get()), __pyx_v_trim_input, (&__pyx_v_state_map), __pyx_t_12);
 
@@ -21178,15 +20991,15 @@
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
-  Mata::Nfa::StringMap __pyx_t_12;
+  Mata::Nfa::ParameterMap __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reduce", 0);
   __Pyx_INCREF(__pyx_v_params);
 
   /* "libmata/nfa/nfa.pyx":893
@@ -21509,15 +21322,15 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
-  Mata::Nfa::StringMap __pyx_t_13;
+  Mata::Nfa::ParameterMap __pyx_t_13;
   size_t __pyx_t_14;
   size_t __pyx_t_15;
   size_t __pyx_t_16;
   size_t __pyx_t_17;
   size_t __pyx_t_18;
   size_t __pyx_t_19;
   int __pyx_lineno = 0;
@@ -22297,15 +22110,15 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  Mata::Nfa::StringMap __pyx_t_14;
+  Mata::Nfa::ParameterMap __pyx_t_14;
   bool __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_universal", 0);
   __Pyx_INCREF(__pyx_v_params);
 
@@ -22667,15 +22480,15 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  Mata::Nfa::StringMap __pyx_t_14;
+  Mata::Nfa::ParameterMap __pyx_t_14;
   bool __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_included_with_cex", 0);
   __Pyx_INCREF(__pyx_v_params);
 
@@ -23095,15 +22908,15 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  Mata::Nfa::StringMap __pyx_t_14;
+  Mata::Nfa::ParameterMap __pyx_t_14;
   bool __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_included", 0);
   __Pyx_INCREF(__pyx_v_params);
 
@@ -23503,15 +23316,15 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  Mata::Nfa::StringMap __pyx_t_14;
+  Mata::Nfa::ParameterMap __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("equivalence_check", 0);
   __Pyx_INCREF(__pyx_v_params);
 
   /* "libmata/nfa/nfa.pyx":1027
@@ -24762,15 +24575,15 @@
   __pyx_v_result = Mata::Nfa::get_word_for_path((*__pyx_v_lhs->thisptr.get()), (*__pyx_v_input->thisptr));
 
   /* "libmata/nfa/nfa.pyx":1110
  *     input.path = path
  *     result = mata_nfa.c_get_word_for_path(dereference(lhs.thisptr.get()), dereference(input.thisptr))
  *     return result.first.word, result.second             # <<<<<<<<<<<<<<
  * 
- * def encode_word(string_to_symbol, word):
+ * def encode_word(alph.Alphabet alphabet, word):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_convert_vector_to_py_Mata_3a__3a_Symbol(__pyx_v_result.first.word); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_result.second); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1110, __pyx_L1_error)
@@ -24806,65 +24619,65 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "libmata/nfa/nfa.pyx":1112
  *     return result.first.word, result.second
  * 
- * def encode_word(string_to_symbol, word):             # <<<<<<<<<<<<<<
- *     """Encodes word based on a string to symbol map
+ * def encode_word(alph.Alphabet alphabet, word):             # <<<<<<<<<<<<<<
+ *     """Encodes word based on a passed alphabet
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7libmata_3nfa_3nfa_55encode_word(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7libmata_3nfa_3nfa_54encode_word, "Encodes word based on a string to symbol map\n\n    >>> mata_nfa.Nfa.encode_word({'a': 1, 'b': 2, \"c\": 0}, \"abca\")\n    [1, 2, 0, 1]\n\n    :param dict string_to_symbol: dictionary of strings to integers\n    :param word: list of strings representing a encoded word\n    :return:\n    ");
+PyDoc_STRVAR(__pyx_doc_7libmata_3nfa_3nfa_54encode_word, "Encodes word based on a passed alphabet\n\n    >>> mata_nfa.Nfa.encode_word(OnTheFlyAlphabet.from_symbol_map({'a': 1, 'b': 2, \"c\": 0}), \"abca\")\n    [1, 2, 0, 1]\n\n    :param alph.Alphabet alphabet: Alphabet to encode the word with.\n    :param word: list of strings representing an encoded word.\n    :return: Encoded word.\n    ");
 static PyMethodDef __pyx_mdef_7libmata_3nfa_3nfa_55encode_word = {"encode_word", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7libmata_3nfa_3nfa_55encode_word, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7libmata_3nfa_3nfa_54encode_word};
 static PyObject *__pyx_pw_7libmata_3nfa_3nfa_55encode_word(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
-  PyObject *__pyx_v_string_to_symbol = 0;
+  struct __pyx_obj_7libmata_9alphabets_Alphabet *__pyx_v_alphabet = 0;
   PyObject *__pyx_v_word = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("encode_word (wrapper)", 0);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_string_to_symbol,&__pyx_n_s_word,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_alphabet,&__pyx_n_s_word,0};
     PyObject* values[2] = {0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_string_to_symbol)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_alphabet)) != 0)) kw_args--;
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1112, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_word)) != 0)) kw_args--;
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1112, __pyx_L3_error)
         else {
@@ -24877,269 +24690,211 @@
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_string_to_symbol = values[0];
+    __pyx_v_alphabet = ((struct __pyx_obj_7libmata_9alphabets_Alphabet *)values[0]);
     __pyx_v_word = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("encode_word", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 1112, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("libmata.nfa.nfa.encode_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7libmata_3nfa_3nfa_54encode_word(__pyx_self, __pyx_v_string_to_symbol, __pyx_v_word);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_alphabet), __pyx_ptype_7libmata_9alphabets_Alphabet, 1, "alphabet", 0))) __PYX_ERR(1, 1112, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7libmata_3nfa_3nfa_54encode_word(__pyx_self, __pyx_v_alphabet, __pyx_v_word);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7libmata_3nfa_3nfa_54encode_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_string_to_symbol, PyObject *__pyx_v_word) {
+static PyObject *__pyx_pf_7libmata_3nfa_3nfa_54encode_word(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7libmata_9alphabets_Alphabet *__pyx_v_alphabet, PyObject *__pyx_v_word) {
+  Mata::Alphabet *__pyx_v_c_alphabet;
   Mata::Nfa::Run __pyx_v_result;
-  PyObject *__pyx_9genexpr23__pyx_v_k = NULL;
-  PyObject *__pyx_9genexpr23__pyx_v_v = NULL;
-  PyObject *__pyx_9genexpr24__pyx_v_s = NULL;
+  PyObject *__pyx_9genexpr23__pyx_v_s = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  Mata::Alphabet *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
+  PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
-  int __pyx_t_5;
+  PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
-  Mata::StringToSymbolMap __pyx_t_10;
-  PyObject *(*__pyx_t_11)(PyObject *);
-  std::vector<std::string>  __pyx_t_12;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
+  std::vector<std::string>  __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_word", 0);
 
   /* "libmata/nfa/nfa.pyx":1122
- *     :return:
+ *     :return: Encoded word.
  *     """
- *     result = mata_nfa.c_encode_word(             # <<<<<<<<<<<<<<
- *         {k.encode('utf-8'): v for (k, v) in string_to_symbol.items()},
- *         [s.encode('utf-8') for s in word]
+ *     cdef CAlphabet* c_alphabet = alphabet.as_base()             # <<<<<<<<<<<<<<
+ *     result = mata_nfa.c_encode_word(
+ *         c_alphabet,
  */
-  { /* enter inner scope */
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *)__pyx_v_alphabet->__pyx_vtab)->as_base(__pyx_v_alphabet); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1122, __pyx_L1_error)
+  __pyx_v_c_alphabet = __pyx_t_1;
 
-    /* "libmata/nfa/nfa.pyx":1123
- *     """
+  /* "libmata/nfa/nfa.pyx":1124
+ *     cdef CAlphabet* c_alphabet = alphabet.as_base()
  *     result = mata_nfa.c_encode_word(
- *         {k.encode('utf-8'): v for (k, v) in string_to_symbol.items()},             # <<<<<<<<<<<<<<
+ *         c_alphabet,             # <<<<<<<<<<<<<<
  *         [s.encode('utf-8') for s in word]
  *     )
  */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1123, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = 0;
-    if (unlikely(__pyx_v_string_to_symbol == Py_None)) {
-      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(1, 1123, __pyx_L5_error)
-    }
-    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_string_to_symbol, 0, __pyx_n_s_items, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1123, __pyx_L5_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_2);
-    __pyx_t_2 = __pyx_t_6;
-    __pyx_t_6 = 0;
-    while (1) {
-      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
-      if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 1123, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_XDECREF_SET(__pyx_9genexpr23__pyx_v_k, __pyx_t_6);
-      __pyx_t_6 = 0;
-      __Pyx_XDECREF_SET(__pyx_9genexpr23__pyx_v_v, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_9genexpr23__pyx_v_k, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1123, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_9 = NULL;
-      __pyx_t_8 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_9)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_9);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_6, function);
-          __pyx_t_8 = 1;
-        }
-      }
-      {
-        PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
-        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1123, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      }
-      if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_t_7, (PyObject*)__pyx_9genexpr23__pyx_v_v))) __PYX_ERR(1, 1123, __pyx_L5_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_k); __pyx_9genexpr23__pyx_v_k = 0;
-    __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_v); __pyx_9genexpr23__pyx_v_v = 0;
-    goto __pyx_L8_exit_scope;
-    __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_k); __pyx_9genexpr23__pyx_v_k = 0;
-    __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_v); __pyx_9genexpr23__pyx_v_v = 0;
-    goto __pyx_L1_error;
-    __pyx_L8_exit_scope:;
-  } /* exit inner scope */
-  __pyx_t_10 = __pyx_convert_unordered_map_from_py_std_3a__3a_string__and_Mata_3a__3a_Symbol(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1123, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   { /* enter inner scope */
 
-    /* "libmata/nfa/nfa.pyx":1124
+    /* "libmata/nfa/nfa.pyx":1125
  *     result = mata_nfa.c_encode_word(
- *         {k.encode('utf-8'): v for (k, v) in string_to_symbol.items()},
+ *         c_alphabet,
  *         [s.encode('utf-8') for s in word]             # <<<<<<<<<<<<<<
  *     )
  *     return result.word
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1124, __pyx_L11_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1125, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_v_word)) || PyTuple_CheckExact(__pyx_v_word)) {
-      __pyx_t_2 = __pyx_v_word; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
-      __pyx_t_11 = NULL;
+      __pyx_t_3 = __pyx_v_word; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
+      __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_word); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1124, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 1124, __pyx_L11_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_word); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1125, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1125, __pyx_L5_error)
     }
     for (;;) {
-      if (likely(!__pyx_t_11)) {
-        if (likely(PyList_CheckExact(__pyx_t_2))) {
-          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
+      if (likely(!__pyx_t_5)) {
+        if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1124, __pyx_L11_error)
+          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_6); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1125, __pyx_L5_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1124, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_7);
+          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1125, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_6);
           #endif
         } else {
-          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1124, __pyx_L11_error)
+          __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_6); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1125, __pyx_L5_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1124, __pyx_L11_error)
-          __Pyx_GOTREF(__pyx_t_7);
+          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1125, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_6);
           #endif
         }
       } else {
-        __pyx_t_7 = __pyx_t_11(__pyx_t_2);
-        if (unlikely(!__pyx_t_7)) {
+        __pyx_t_6 = __pyx_t_5(__pyx_t_3);
+        if (unlikely(!__pyx_t_6)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 1124, __pyx_L11_error)
+            else __PYX_ERR(1, 1125, __pyx_L5_error)
           }
           break;
         }
-        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_GOTREF(__pyx_t_6);
       }
-      __Pyx_XDECREF_SET(__pyx_9genexpr24__pyx_v_s, __pyx_t_7);
-      __pyx_t_7 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_9genexpr24__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1124, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_9 = NULL;
-      __pyx_t_5 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_9)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_9);
+      __Pyx_XDECREF_SET(__pyx_9genexpr23__pyx_v_s, __pyx_t_6);
+      __pyx_t_6 = 0;
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_9genexpr23__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1125, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_8 = NULL;
+      __pyx_t_9 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+        if (likely(__pyx_t_8)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+          __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_6, function);
-          __pyx_t_5 = 1;
+          __Pyx_DECREF_SET(__pyx_t_7, function);
+          __pyx_t_9 = 1;
         }
       }
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
-        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1124, __pyx_L11_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_kp_u_utf_8};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1125, __pyx_L5_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(1, 1124, __pyx_L11_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 1125, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_9genexpr24__pyx_v_s); __pyx_9genexpr24__pyx_v_s = 0;
-    goto __pyx_L15_exit_scope;
-    __pyx_L11_error:;
-    __Pyx_XDECREF(__pyx_9genexpr24__pyx_v_s); __pyx_9genexpr24__pyx_v_s = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_s); __pyx_9genexpr23__pyx_v_s = 0;
+    goto __pyx_L9_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_s); __pyx_9genexpr23__pyx_v_s = 0;
     goto __pyx_L1_error;
-    __pyx_L15_exit_scope:;
+    __pyx_L9_exit_scope:;
   } /* exit inner scope */
-  __pyx_t_12 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1124, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_10 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1125, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1122
- *     :return:
+  /* "libmata/nfa/nfa.pyx":1123
  *     """
+ *     cdef CAlphabet* c_alphabet = alphabet.as_base()
  *     result = mata_nfa.c_encode_word(             # <<<<<<<<<<<<<<
- *         {k.encode('utf-8'): v for (k, v) in string_to_symbol.items()},
+ *         c_alphabet,
  *         [s.encode('utf-8') for s in word]
  */
-  __pyx_v_result = Mata::Nfa::encode_word(__pyx_t_10, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_12));
+  __pyx_v_result = Mata::Nfa::encode_word(__pyx_v_c_alphabet, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_10));
 
-  /* "libmata/nfa/nfa.pyx":1126
+  /* "libmata/nfa/nfa.pyx":1127
  *         [s.encode('utf-8') for s in word]
  *     )
  *     return result.word             # <<<<<<<<<<<<<<
  * 
  * cdef subset_map_to_dictionary(umap[StateSet, State] subset_map):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_Mata_3a__3a_Symbol(__pyx_v_result.word); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __pyx_convert_vector_to_py_Mata_3a__3a_Symbol(__pyx_v_result.word); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "libmata/nfa/nfa.pyx":1112
  *     return result.first.word, result.second
  * 
- * def encode_word(string_to_symbol, word):             # <<<<<<<<<<<<<<
- *     """Encodes word based on a string to symbol map
+ * def encode_word(alph.Alphabet alphabet, word):             # <<<<<<<<<<<<<<
+ *     """Encodes word based on a passed alphabet
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("libmata.nfa.nfa.encode_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_k);
-  __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_v);
-  __Pyx_XDECREF(__pyx_9genexpr24__pyx_v_s);
+  __Pyx_XDECREF(__pyx_9genexpr23__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libmata/nfa/nfa.pyx":1128
+/* "libmata/nfa/nfa.pyx":1129
  *     return result.word
  * 
  * cdef subset_map_to_dictionary(umap[StateSet, State] subset_map):             # <<<<<<<<<<<<<<
  *     """Helper function that translates the unordered map to dictionary
  * 
  */
 
@@ -25158,112 +24913,112 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("subset_map_to_dictionary", 0);
 
-  /* "libmata/nfa/nfa.pyx":1134
+  /* "libmata/nfa/nfa.pyx":1135
  *     :return: subset_map as dictionary
  *     """
  *     result = {}             # <<<<<<<<<<<<<<
  *     cdef umap[StateSet, State].iterator it = subset_map.begin()
  *     while it != subset_map.end():
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1134, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1135
+  /* "libmata/nfa/nfa.pyx":1136
  *     """
  *     result = {}
  *     cdef umap[StateSet, State].iterator it = subset_map.begin()             # <<<<<<<<<<<<<<
  *     while it != subset_map.end():
  *         key = dereference(it).first.ToVector()
  */
   __pyx_v_it = __pyx_v_subset_map.begin();
 
-  /* "libmata/nfa/nfa.pyx":1136
+  /* "libmata/nfa/nfa.pyx":1137
  *     result = {}
  *     cdef umap[StateSet, State].iterator it = subset_map.begin()
  *     while it != subset_map.end():             # <<<<<<<<<<<<<<
  *         key = dereference(it).first.ToVector()
  *         value = dereference(it).second
  */
   while (1) {
     __pyx_t_2 = (__pyx_v_it != __pyx_v_subset_map.end());
     if (!__pyx_t_2) break;
 
-    /* "libmata/nfa/nfa.pyx":1137
+    /* "libmata/nfa/nfa.pyx":1138
  *     cdef umap[StateSet, State].iterator it = subset_map.begin()
  *     while it != subset_map.end():
  *         key = dereference(it).first.ToVector()             # <<<<<<<<<<<<<<
  *         value = dereference(it).second
  *         result[tuple(sorted(key))] = value
  */
     __pyx_v_key = (*__pyx_v_it).first.ToVector();
 
-    /* "libmata/nfa/nfa.pyx":1138
+    /* "libmata/nfa/nfa.pyx":1139
  *     while it != subset_map.end():
  *         key = dereference(it).first.ToVector()
  *         value = dereference(it).second             # <<<<<<<<<<<<<<
  *         result[tuple(sorted(key))] = value
  *         postinc(it)
  */
     __pyx_t_3 = (*__pyx_v_it).second;
     __pyx_v_value = __pyx_t_3;
 
-    /* "libmata/nfa/nfa.pyx":1139
+    /* "libmata/nfa/nfa.pyx":1140
  *         key = dereference(it).first.ToVector()
  *         value = dereference(it).second
  *         result[tuple(sorted(key))] = value             # <<<<<<<<<<<<<<
  *         postinc(it)
  *     return result
  */
-    __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1139, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __pyx_convert_vector_to_py_Mata_3a__3a_Nfa_3a__3a_State(__pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1139, __pyx_L1_error)
+    __pyx_t_5 = __pyx_convert_vector_to_py_Mata_3a__3a_Nfa_3a__3a_State(__pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PySequence_List(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1139, __pyx_L1_error)
+    __pyx_t_6 = PySequence_List(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_4 = ((PyObject*)__pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_7 = PyList_Sort(__pyx_t_4); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 1139, __pyx_L1_error)
-    __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_4)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1139, __pyx_L1_error)
+    __pyx_t_7 = PyList_Sort(__pyx_t_4); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 1140, __pyx_L1_error)
+    __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_4)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_t_6, __pyx_t_1) < 0))) __PYX_ERR(1, 1139, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_t_6, __pyx_t_1) < 0))) __PYX_ERR(1, 1140, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1140
+    /* "libmata/nfa/nfa.pyx":1141
  *         value = dereference(it).second
  *         result[tuple(sorted(key))] = value
  *         postinc(it)             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
     (void)((__pyx_v_it++));
   }
 
-  /* "libmata/nfa/nfa.pyx":1141
+  /* "libmata/nfa/nfa.pyx":1142
  *         result[tuple(sorted(key))] = value
  *         postinc(it)
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "libmata/nfa/nfa.pyx":1128
+  /* "libmata/nfa/nfa.pyx":1129
  *     return result.word
  * 
  * cdef subset_map_to_dictionary(umap[StateSet, State] subset_map):             # <<<<<<<<<<<<<<
  *     """Helper function that translates the unordered map to dictionary
  * 
  */
 
@@ -25278,15 +25033,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libmata/nfa/nfa.pyx":1145
+/* "libmata/nfa/nfa.pyx":1146
  * 
  * # Temporary for testing
  * def divisible_by(k: int):             # <<<<<<<<<<<<<<
  *     """Constructs automaton accepting strings containing ones divisible by "k"."""
  *     assert k > 1
  */
 
@@ -25329,37 +25084,37 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_k)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1145, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1146, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "divisible_by") < 0)) __PYX_ERR(1, 1145, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "divisible_by") < 0)) __PYX_ERR(1, 1146, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_k = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("divisible_by", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 1145, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("divisible_by", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 1146, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("libmata.nfa.nfa.divisible_by", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_k), (&PyInt_Type), 0, "k", 1))) __PYX_ERR(1, 1145, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_k), (&PyInt_Type), 0, "k", 1))) __PYX_ERR(1, 1146, __pyx_L1_error)
   __pyx_r = __pyx_pf_7libmata_3nfa_3nfa_56divisible_by(__pyx_self, __pyx_v_k);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -25382,58 +25137,58 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("divisible_by", 0);
 
-  /* "libmata/nfa/nfa.pyx":1147
+  /* "libmata/nfa/nfa.pyx":1148
  * def divisible_by(k: int):
  *     """Constructs automaton accepting strings containing ones divisible by "k"."""
  *     assert k > 1             # <<<<<<<<<<<<<<
  *     lhs = Nfa(k+1)
  *     lhs.make_initial_state(0)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_k, __pyx_int_1, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1147, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 1147, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_k, __pyx_int_1, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1148, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 1148, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_2)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(1, 1147, __pyx_L1_error)
+      __PYX_ERR(1, 1148, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(1, 1147, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(1, 1148, __pyx_L1_error)
   #endif
 
-  /* "libmata/nfa/nfa.pyx":1148
+  /* "libmata/nfa/nfa.pyx":1149
  *     """Constructs automaton accepting strings containing ones divisible by "k"."""
  *     assert k > 1
  *     lhs = Nfa(k+1)             # <<<<<<<<<<<<<<
  *     lhs.make_initial_state(0)
  *     lhs.add_transition(0, 0, 0)
  */
-  __pyx_t_1 = PyNumber_Add(__pyx_v_k, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1148, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_k, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7libmata_3nfa_3nfa_Nfa), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1148, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7libmata_3nfa_3nfa_Nfa), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_lhs = ((struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1149
+  /* "libmata/nfa/nfa.pyx":1150
  *     assert k > 1
  *     lhs = Nfa(k+1)
  *     lhs.make_initial_state(0)             # <<<<<<<<<<<<<<
  *     lhs.add_transition(0, 0, 0)
  *     for i in range(1, k + 1):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_make_initial_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1149, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_make_initial_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -25443,107 +25198,107 @@
       __pyx_t_5 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_int_0};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1149, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1150
+  /* "libmata/nfa/nfa.pyx":1151
  *     lhs = Nfa(k+1)
  *     lhs.make_initial_state(0)
  *     lhs.add_transition(0, 0, 0)             # <<<<<<<<<<<<<<
  *     for i in range(1, k + 1):
  *         lhs.add_transition(i - 1, 1, i)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1150, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1150, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1151
+  /* "libmata/nfa/nfa.pyx":1152
  *     lhs.make_initial_state(0)
  *     lhs.add_transition(0, 0, 0)
  *     for i in range(1, k + 1):             # <<<<<<<<<<<<<<
  *         lhs.add_transition(i - 1, 1, i)
  *         lhs.add_transition(i, 0, i)
  */
-  __pyx_t_1 = PyNumber_Add(__pyx_v_k, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1151, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_k, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1151, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_int_1);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1151, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_3 = __pyx_t_1; __Pyx_INCREF(__pyx_t_3); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1151, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1151, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1152, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 1151, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 1152, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1151, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1152, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 1151, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 1152, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1151, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1152, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_7(__pyx_t_3);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 1151, __pyx_L1_error)
+          else __PYX_ERR(1, 1152, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1152
+    /* "libmata/nfa/nfa.pyx":1153
  *     lhs.add_transition(0, 0, 0)
  *     for i in range(1, k + 1):
  *         lhs.add_transition(i - 1, 1, i)             # <<<<<<<<<<<<<<
  *         lhs.add_transition(i, 0, i)
  *     lhs.add_transition(k, 1, 1)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1152, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1152, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -25554,28 +25309,28 @@
       }
     }
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_9, __pyx_t_8, __pyx_int_1, __pyx_v_i};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 3+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1152, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1153
+    /* "libmata/nfa/nfa.pyx":1154
  *     for i in range(1, k + 1):
  *         lhs.add_transition(i - 1, 1, i)
  *         lhs.add_transition(i, 0, i)             # <<<<<<<<<<<<<<
  *     lhs.add_transition(k, 1, 1)
  *     lhs.make_final_state(k)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1153, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_8 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -25585,38 +25340,38 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_8, __pyx_v_i, __pyx_int_0, __pyx_v_i};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 3+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1153, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1151
+    /* "libmata/nfa/nfa.pyx":1152
  *     lhs.make_initial_state(0)
  *     lhs.add_transition(0, 0, 0)
  *     for i in range(1, k + 1):             # <<<<<<<<<<<<<<
  *         lhs.add_transition(i - 1, 1, i)
  *         lhs.add_transition(i, 0, i)
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1154
+  /* "libmata/nfa/nfa.pyx":1155
  *         lhs.add_transition(i - 1, 1, i)
  *         lhs.add_transition(i, 0, i)
  *     lhs.add_transition(k, 1, 1)             # <<<<<<<<<<<<<<
  *     lhs.make_final_state(k)
  *     return lhs
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1154, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_add_transition); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -25626,28 +25381,28 @@
       __pyx_t_5 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[4] = {__pyx_t_4, __pyx_v_k, __pyx_int_1, __pyx_int_1};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 3+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1154, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1155, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1155
+  /* "libmata/nfa/nfa.pyx":1156
  *         lhs.add_transition(i, 0, i)
  *     lhs.add_transition(k, 1, 1)
  *     lhs.make_final_state(k)             # <<<<<<<<<<<<<<
  *     return lhs
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_make_final_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1155, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lhs), __pyx_n_s_make_final_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -25657,33 +25412,33 @@
       __pyx_t_5 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_k};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1155, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1156, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1156
+  /* "libmata/nfa/nfa.pyx":1157
  *     lhs.add_transition(k, 1, 1)
  *     lhs.make_final_state(k)
  *     return lhs             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_lhs);
   __pyx_r = ((PyObject *)__pyx_v_lhs);
   goto __pyx_L0;
 
-  /* "libmata/nfa/nfa.pyx":1145
+  /* "libmata/nfa/nfa.pyx":1146
  * 
  * # Temporary for testing
  * def divisible_by(k: int):             # <<<<<<<<<<<<<<
  *     """Constructs automaton accepting strings containing ones divisible by "k"."""
  *     assert k > 1
  */
 
@@ -25700,15 +25455,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_lhs);
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libmata/nfa/nfa.pyx":1159
+/* "libmata/nfa/nfa.pyx":1160
  * 
  * 
  * def run_safely_external_command(cmd: str, check_results=True, quiet=True, timeout=None, **kwargs):             # <<<<<<<<<<<<<<
  *     """Safely runs the piped command, without executing of the shell
  * 
  */
 
@@ -25766,41 +25521,41 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cmd)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1159, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1160, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_check_results);
           if (value) { values[1] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1159, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1160, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_quiet);
           if (value) { values[2] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1159, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1160, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_timeout);
           if (value) { values[3] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1159, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1160, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "run_safely_external_command") < 0)) __PYX_ERR(1, 1159, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "run_safely_external_command") < 0)) __PYX_ERR(1, 1160, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -25814,22 +25569,22 @@
     __pyx_v_cmd = ((PyObject*)values[0]);
     __pyx_v_check_results = values[1];
     __pyx_v_quiet = values[2];
     __pyx_v_timeout = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("run_safely_external_command", 0, 1, 4, __pyx_nargs); __PYX_ERR(1, 1159, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("run_safely_external_command", 0, 1, 4, __pyx_nargs); __PYX_ERR(1, 1160, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("libmata.nfa.nfa.run_safely_external_command", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cmd), (&PyUnicode_Type), 0, "cmd", 1))) __PYX_ERR(1, 1159, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cmd), (&PyUnicode_Type), 0, "cmd", 1))) __PYX_ERR(1, 1160, __pyx_L1_error)
   __pyx_r = __pyx_pf_7libmata_3nfa_3nfa_58run_safely_external_command(__pyx_self, __pyx_v_cmd, __pyx_v_check_results, __pyx_v_quiet, __pyx_v_timeout, __pyx_v_kwargs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -25871,132 +25626,132 @@
   int __pyx_t_17;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("run_safely_external_command", 0);
 
-  /* "libmata/nfa/nfa.pyx":1173
+  /* "libmata/nfa/nfa.pyx":1174
  *     """
  *     # Split
  *     unpiped_commands = list(map(str.strip, cmd.split(" | ")))             # <<<<<<<<<<<<<<
  *     cmd_no = len(unpiped_commands)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyUnicode_Type)), __pyx_n_s_strip); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1173, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyUnicode_Type)), __pyx_n_s_strip); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyUnicode_Split(__pyx_v_cmd, __Pyx_NoneAsNull(__pyx_kp_u__14), -1L); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1173, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_Split(__pyx_v_cmd, __Pyx_NoneAsNull(__pyx_kp_u__14), -1L); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1173, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1173, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PySequence_ListKeepNew(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1173, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PySequence_ListKeepNew(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_unpiped_commands = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1174
+  /* "libmata/nfa/nfa.pyx":1175
  *     # Split
  *     unpiped_commands = list(map(str.strip, cmd.split(" | ")))
  *     cmd_no = len(unpiped_commands)             # <<<<<<<<<<<<<<
  * 
  *     # Run the command through pipes
  */
-  __pyx_t_4 = PyList_GET_SIZE(__pyx_v_unpiped_commands); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 1174, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1174, __pyx_L1_error)
+  __pyx_t_4 = PyList_GET_SIZE(__pyx_v_unpiped_commands); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 1175, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_cmd_no = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1177
+  /* "libmata/nfa/nfa.pyx":1178
  * 
  *     # Run the command through pipes
  *     objects: List[subprocess.Popen] = []             # <<<<<<<<<<<<<<
  *     for i in range(cmd_no):
  *         executed_command = shlex.split(unpiped_commands[i])
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1177, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_objects = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1178
+  /* "libmata/nfa/nfa.pyx":1179
  *     # Run the command through pipes
  *     objects: List[subprocess.Popen] = []
  *     for i in range(cmd_no):             # <<<<<<<<<<<<<<
  *         executed_command = shlex.split(unpiped_commands[i])
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_cmd_no); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1178, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_cmd_no); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
     __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1178, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1178, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1179, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1178, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1179, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1178, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1179, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1178, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1179, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1178, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1179, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_5(__pyx_t_2);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 1178, __pyx_L1_error)
+          else __PYX_ERR(1, 1179, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1179
+    /* "libmata/nfa/nfa.pyx":1180
  *     objects: List[subprocess.Popen] = []
  *     for i in range(cmd_no):
  *         executed_command = shlex.split(unpiped_commands[i])             # <<<<<<<<<<<<<<
  * 
  *         # set streams
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_shlex); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1179, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_shlex); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1180, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_split); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1179, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_split); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1180, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_unpiped_commands, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1179, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_unpiped_commands, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1180, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -26007,170 +25762,170 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_1};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1179, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1180, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_executed_command, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1182
+    /* "libmata/nfa/nfa.pyx":1183
  * 
  *         # set streams
  *         stdin = None if i == 0 else objects[i-1].stdout             # <<<<<<<<<<<<<<
  *         stderr = subprocess.STDOUT if i < (cmd_no - 1) else subprocess.PIPE
  * 
  */
-    __pyx_t_9 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_i, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1182, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_i, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1183, __pyx_L1_error)
     if (__pyx_t_9) {
       __Pyx_INCREF(Py_None);
       __pyx_t_3 = Py_None;
     } else {
-      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1182, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1183, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1182, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1183, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_stdout); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1182, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_stdout); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1183, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_3 = __pyx_t_6;
       __pyx_t_6 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_stdin, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1183
+    /* "libmata/nfa/nfa.pyx":1184
  *         # set streams
  *         stdin = None if i == 0 else objects[i-1].stdout
  *         stderr = subprocess.STDOUT if i < (cmd_no - 1) else subprocess.PIPE             # <<<<<<<<<<<<<<
  * 
  *         # run the piped command and close the previous one
  */
-    __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_cmd_no, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1183, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_cmd_no, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_i, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1183, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_i, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1184, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1183, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1184, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_9) {
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1183, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_STDOUT); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1183, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_STDOUT); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_3 = __pyx_t_6;
       __pyx_t_6 = 0;
     } else {
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1183, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_PIPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1183, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_PIPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_3 = __pyx_t_1;
       __pyx_t_1 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_stderr, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1186
+    /* "libmata/nfa/nfa.pyx":1187
  * 
  *         # run the piped command and close the previous one
  *         piped_command = subprocess.Popen(             # <<<<<<<<<<<<<<
  *             executed_command,
  *             shell=False, stdin=stdin, stdout=subprocess.PIPE, stderr=stderr, **kwargs
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1186, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Popen); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1186, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Popen); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1187
+    /* "libmata/nfa/nfa.pyx":1188
  *         # run the piped command and close the previous one
  *         piped_command = subprocess.Popen(
  *             executed_command,             # <<<<<<<<<<<<<<
  *             shell=False, stdin=stdin, stdout=subprocess.PIPE, stderr=stderr, **kwargs
  *         )
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1186, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_executed_command);
     __Pyx_GIVEREF(__pyx_v_executed_command);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_executed_command);
 
-    /* "libmata/nfa/nfa.pyx":1188
+    /* "libmata/nfa/nfa.pyx":1189
  *         piped_command = subprocess.Popen(
  *             executed_command,
  *             shell=False, stdin=stdin, stdout=subprocess.PIPE, stderr=stderr, **kwargs             # <<<<<<<<<<<<<<
  *         )
  *         if i != 0:
  */
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1188, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shell, Py_False) < 0) __PYX_ERR(1, 1188, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_stdin, __pyx_v_stdin) < 0) __PYX_ERR(1, 1188, __pyx_L1_error)
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 1188, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shell, Py_False) < 0) __PYX_ERR(1, 1189, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_stdin, __pyx_v_stdin) < 0) __PYX_ERR(1, 1189, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 1189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_PIPE); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 1188, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_PIPE); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 1189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_stdout, __pyx_t_11) < 0) __PYX_ERR(1, 1188, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_stdout, __pyx_t_11) < 0) __PYX_ERR(1, 1189, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_stderr, __pyx_v_stderr) < 0) __PYX_ERR(1, 1188, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_stderr, __pyx_v_stderr) < 0) __PYX_ERR(1, 1189, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_7;
     __pyx_t_7 = 0;
-    if (__Pyx_MergeKeywords(__pyx_t_6, __pyx_v_kwargs) < 0) __PYX_ERR(1, 1188, __pyx_L1_error)
+    if (__Pyx_MergeKeywords(__pyx_t_6, __pyx_v_kwargs) < 0) __PYX_ERR(1, 1189, __pyx_L1_error)
 
-    /* "libmata/nfa/nfa.pyx":1186
+    /* "libmata/nfa/nfa.pyx":1187
  * 
  *         # run the piped command and close the previous one
  *         piped_command = subprocess.Popen(             # <<<<<<<<<<<<<<
  *             executed_command,
  *             shell=False, stdin=stdin, stdout=subprocess.PIPE, stderr=stderr, **kwargs
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1186, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_piped_command, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1190
+    /* "libmata/nfa/nfa.pyx":1191
  *             shell=False, stdin=stdin, stdout=subprocess.PIPE, stderr=stderr, **kwargs
  *         )
  *         if i != 0:             # <<<<<<<<<<<<<<
  *             objects[i-1].stdout.close()  # type: ignore
  *         objects.append(piped_command)
  */
-    __pyx_t_9 = (__Pyx_PyInt_BoolNeObjC(__pyx_v_i, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1190, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyInt_BoolNeObjC(__pyx_v_i, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1191, __pyx_L1_error)
     if (__pyx_t_9) {
 
-      /* "libmata/nfa/nfa.pyx":1191
+      /* "libmata/nfa/nfa.pyx":1192
  *         )
  *         if i != 0:
  *             objects[i-1].stdout.close()  # type: ignore             # <<<<<<<<<<<<<<
  *         objects.append(piped_command)
  * 
  */
-      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1191, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1192, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1191, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1192, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stdout); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1191, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stdout); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1192, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1191, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1192, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_6)) {
@@ -26181,49 +25936,49 @@
           __pyx_t_8 = 1;
         }
       }
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_6, };
         __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1191, __pyx_L1_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1192, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "libmata/nfa/nfa.pyx":1190
+      /* "libmata/nfa/nfa.pyx":1191
  *             shell=False, stdin=stdin, stdout=subprocess.PIPE, stderr=stderr, **kwargs
  *         )
  *         if i != 0:             # <<<<<<<<<<<<<<
  *             objects[i-1].stdout.close()  # type: ignore
  *         objects.append(piped_command)
  */
     }
 
-    /* "libmata/nfa/nfa.pyx":1192
+    /* "libmata/nfa/nfa.pyx":1193
  *         if i != 0:
  *             objects[i-1].stdout.close()  # type: ignore
  *         objects.append(piped_command)             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_objects, __pyx_v_piped_command); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(1, 1192, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_objects, __pyx_v_piped_command); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(1, 1193, __pyx_L1_error)
 
-    /* "libmata/nfa/nfa.pyx":1178
+    /* "libmata/nfa/nfa.pyx":1179
  *     # Run the command through pipes
  *     objects: List[subprocess.Popen] = []
  *     for i in range(cmd_no):             # <<<<<<<<<<<<<<
  *         executed_command = shlex.split(unpiped_commands[i])
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1194
+  /* "libmata/nfa/nfa.pyx":1195
  *         objects.append(piped_command)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         # communicate with the last piped object
  *         cmdout, cmderr = objects[-1].communicate(timeout=timeout)
  */
   {
@@ -26231,172 +25986,172 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
     __Pyx_XGOTREF(__pyx_t_13);
     __Pyx_XGOTREF(__pyx_t_14);
     __Pyx_XGOTREF(__pyx_t_15);
     /*try:*/ {
 
-      /* "libmata/nfa/nfa.pyx":1196
+      /* "libmata/nfa/nfa.pyx":1197
  *     try:
  *         # communicate with the last piped object
  *         cmdout, cmderr = objects[-1].communicate(timeout=timeout)             # <<<<<<<<<<<<<<
  * 
  *         for i in range(len(objects) - 1):
  */
-      __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_objects, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1196, __pyx_L7_error)
+      __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_objects, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1197, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_communicate); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1196, __pyx_L7_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_communicate); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1197, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1196, __pyx_L7_error)
+      __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1197, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_timeout, __pyx_v_timeout) < 0) __PYX_ERR(1, 1196, __pyx_L7_error)
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1196, __pyx_L7_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_timeout, __pyx_v_timeout) < 0) __PYX_ERR(1, 1197, __pyx_L7_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1197, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
         PyObject* sequence = __pyx_t_3;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(1, 1196, __pyx_L7_error)
+          __PYX_ERR(1, 1197, __pyx_L7_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_7);
         #else
-        __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1196, __pyx_L7_error)
+        __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1197, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1196, __pyx_L7_error)
+        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1197, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1196, __pyx_L7_error)
+        __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1197, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_16 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6);
         index = 0; __pyx_t_2 = __pyx_t_16(__pyx_t_6); if (unlikely(!__pyx_t_2)) goto __pyx_L13_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_2);
         index = 1; __pyx_t_7 = __pyx_t_16(__pyx_t_6); if (unlikely(!__pyx_t_7)) goto __pyx_L13_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_16(__pyx_t_6), 2) < 0) __PYX_ERR(1, 1196, __pyx_L7_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_16(__pyx_t_6), 2) < 0) __PYX_ERR(1, 1197, __pyx_L7_error)
         __pyx_t_16 = NULL;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         goto __pyx_L14_unpacking_done;
         __pyx_L13_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_16 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(1, 1196, __pyx_L7_error)
+        __PYX_ERR(1, 1197, __pyx_L7_error)
         __pyx_L14_unpacking_done:;
       }
       __pyx_v_cmdout = __pyx_t_2;
       __pyx_t_2 = 0;
       __pyx_v_cmderr = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "libmata/nfa/nfa.pyx":1198
+      /* "libmata/nfa/nfa.pyx":1199
  *         cmdout, cmderr = objects[-1].communicate(timeout=timeout)
  * 
  *         for i in range(len(objects) - 1):             # <<<<<<<<<<<<<<
  *             objects[i].wait(timeout=timeout)
  * 
  */
-      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_objects); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 1198, __pyx_L7_error)
-      __pyx_t_3 = PyInt_FromSsize_t((__pyx_t_4 - 1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1198, __pyx_L7_error)
+      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_objects); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 1199, __pyx_L7_error)
+      __pyx_t_3 = PyInt_FromSsize_t((__pyx_t_4 - 1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1199, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1198, __pyx_L7_error)
+      __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1199, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (likely(PyList_CheckExact(__pyx_t_7)) || PyTuple_CheckExact(__pyx_t_7)) {
         __pyx_t_3 = __pyx_t_7; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
         __pyx_t_5 = NULL;
       } else {
-        __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1198, __pyx_L7_error)
+        __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1199, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1198, __pyx_L7_error)
+        __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1199, __pyx_L7_error)
       }
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       for (;;) {
         if (likely(!__pyx_t_5)) {
           if (likely(PyList_CheckExact(__pyx_t_3))) {
             if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_7 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1198, __pyx_L7_error)
+            __pyx_t_7 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1199, __pyx_L7_error)
             #else
-            __pyx_t_7 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1198, __pyx_L7_error)
+            __pyx_t_7 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1199, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_7);
             #endif
           } else {
             if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1198, __pyx_L7_error)
+            __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1199, __pyx_L7_error)
             #else
-            __pyx_t_7 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1198, __pyx_L7_error)
+            __pyx_t_7 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1199, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_7);
             #endif
           }
         } else {
           __pyx_t_7 = __pyx_t_5(__pyx_t_3);
           if (unlikely(!__pyx_t_7)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(1, 1198, __pyx_L7_error)
+              else __PYX_ERR(1, 1199, __pyx_L7_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_7);
         }
         __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "libmata/nfa/nfa.pyx":1199
+        /* "libmata/nfa/nfa.pyx":1200
  * 
  *         for i in range(len(objects) - 1):
  *             objects[i].wait(timeout=timeout)             # <<<<<<<<<<<<<<
  * 
  *     except subprocess.TimeoutExpired:
  */
-        __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_v_i); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1199, __pyx_L7_error)
+        __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_v_i); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1200, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1199, __pyx_L7_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1200, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1199, __pyx_L7_error)
+        __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1200, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_7);
-        if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_timeout, __pyx_v_timeout) < 0) __PYX_ERR(1, 1199, __pyx_L7_error)
-        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1199, __pyx_L7_error)
+        if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_timeout, __pyx_v_timeout) < 0) __PYX_ERR(1, 1200, __pyx_L7_error)
+        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1200, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-        /* "libmata/nfa/nfa.pyx":1198
+        /* "libmata/nfa/nfa.pyx":1199
  *         cmdout, cmderr = objects[-1].communicate(timeout=timeout)
  * 
  *         for i in range(len(objects) - 1):             # <<<<<<<<<<<<<<
  *             objects[i].wait(timeout=timeout)
  * 
  */
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "libmata/nfa/nfa.pyx":1194
+      /* "libmata/nfa/nfa.pyx":1195
  *         objects.append(piped_command)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         # communicate with the last piped object
  *         cmdout, cmderr = objects[-1].communicate(timeout=timeout)
  */
     }
@@ -26409,65 +26164,65 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1201
+    /* "libmata/nfa/nfa.pyx":1202
  *             objects[i].wait(timeout=timeout)
  * 
  *     except subprocess.TimeoutExpired:             # <<<<<<<<<<<<<<
  *         for process in objects:
  *             process.terminate()
  */
     __Pyx_ErrFetch(&__pyx_t_3, &__pyx_t_6, &__pyx_t_7);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1201, __pyx_L9_except_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1202, __pyx_L9_except_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_TimeoutExpired); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1201, __pyx_L9_except_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_TimeoutExpired); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1202, __pyx_L9_except_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_3, __pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_ErrRestore(__pyx_t_3, __pyx_t_6, __pyx_t_7);
     __pyx_t_3 = 0; __pyx_t_6 = 0; __pyx_t_7 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("libmata.nfa.nfa.run_safely_external_command", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_6, &__pyx_t_3) < 0) __PYX_ERR(1, 1201, __pyx_L9_except_error)
+      if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_6, &__pyx_t_3) < 0) __PYX_ERR(1, 1202, __pyx_L9_except_error)
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_3);
 
-      /* "libmata/nfa/nfa.pyx":1202
+      /* "libmata/nfa/nfa.pyx":1203
  * 
  *     except subprocess.TimeoutExpired:
  *         for process in objects:             # <<<<<<<<<<<<<<
  *             process.terminate()
  *         raise
  */
       __pyx_t_1 = __pyx_v_objects; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
       for (;;) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1202, __pyx_L9_except_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1203, __pyx_L9_except_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1202, __pyx_L9_except_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1203, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_process, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "libmata/nfa/nfa.pyx":1203
+        /* "libmata/nfa/nfa.pyx":1204
  *     except subprocess.TimeoutExpired:
  *         for process in objects:
  *             process.terminate()             # <<<<<<<<<<<<<<
  *         raise
  * 
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_process, __pyx_n_s_terminate); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 1203, __pyx_L9_except_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_process, __pyx_n_s_terminate); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 1204, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_10 = NULL;
         __pyx_t_8 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_10)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -26477,47 +26232,47 @@
             __pyx_t_8 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_10, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1203, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1204, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "libmata/nfa/nfa.pyx":1202
+        /* "libmata/nfa/nfa.pyx":1203
  * 
  *     except subprocess.TimeoutExpired:
  *         for process in objects:             # <<<<<<<<<<<<<<
  *             process.terminate()
  *         raise
  */
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "libmata/nfa/nfa.pyx":1204
+      /* "libmata/nfa/nfa.pyx":1205
  *         for process in objects:
  *             process.terminate()
  *         raise             # <<<<<<<<<<<<<<
  * 
  *     # collect the return codes
  */
       __Pyx_GIVEREF(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_3);
       __Pyx_ErrRestoreWithState(__pyx_t_7, __pyx_t_6, __pyx_t_3);
       __pyx_t_7 = 0; __pyx_t_6 = 0; __pyx_t_3 = 0; 
-      __PYX_ERR(1, 1204, __pyx_L9_except_error)
+      __PYX_ERR(1, 1205, __pyx_L9_except_error)
     }
     goto __pyx_L9_except_error;
 
-    /* "libmata/nfa/nfa.pyx":1194
+    /* "libmata/nfa/nfa.pyx":1195
  *         objects.append(piped_command)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         # communicate with the last piped object
  *         cmdout, cmderr = objects[-1].communicate(timeout=timeout)
  */
     __pyx_L9_except_error:;
@@ -26525,125 +26280,125 @@
     __Pyx_XGIVEREF(__pyx_t_14);
     __Pyx_XGIVEREF(__pyx_t_15);
     __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
     goto __pyx_L1_error;
     __pyx_L12_try_end:;
   }
 
-  /* "libmata/nfa/nfa.pyx":1207
+  /* "libmata/nfa/nfa.pyx":1208
  * 
  *     # collect the return codes
  *     if check_results:             # <<<<<<<<<<<<<<
  *         for i in range(cmd_no):
  *             if objects[i].returncode:
  */
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_check_results); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1207, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_check_results); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1208, __pyx_L1_error)
   if (__pyx_t_9) {
 
-    /* "libmata/nfa/nfa.pyx":1208
+    /* "libmata/nfa/nfa.pyx":1209
  *     # collect the return codes
  *     if check_results:
  *         for i in range(cmd_no):             # <<<<<<<<<<<<<<
  *             if objects[i].returncode:
  *                 if not quiet and (cmdout or cmderr):
  */
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_cmd_no); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1208, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_cmd_no); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_6 = __pyx_t_3; __Pyx_INCREF(__pyx_t_6); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1208, __pyx_L1_error)
+      __pyx_t_4 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1208, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1209, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_6))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1208, __pyx_L1_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1209, __pyx_L1_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1208, __pyx_L1_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1209, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1208, __pyx_L1_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 1209, __pyx_L1_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1208, __pyx_L1_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1209, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_5(__pyx_t_6);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 1208, __pyx_L1_error)
+            else __PYX_ERR(1, 1209, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "libmata/nfa/nfa.pyx":1209
+      /* "libmata/nfa/nfa.pyx":1210
  *     if check_results:
  *         for i in range(cmd_no):
  *             if objects[i].returncode:             # <<<<<<<<<<<<<<
  *                 if not quiet and (cmdout or cmderr):
  *                     print(f"captured stdout: {cmdout.decode('utf-8')}", 'red')
  */
-      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1209, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1210, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_returncode); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1209, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_returncode); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1210, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1209, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(1, 1210, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       if (__pyx_t_9) {
 
-        /* "libmata/nfa/nfa.pyx":1210
+        /* "libmata/nfa/nfa.pyx":1211
  *         for i in range(cmd_no):
  *             if objects[i].returncode:
  *                 if not quiet and (cmdout or cmderr):             # <<<<<<<<<<<<<<
  *                     print(f"captured stdout: {cmdout.decode('utf-8')}", 'red')
  *                     print(f"captured stderr: {cmderr.decode('utf-8')}", 'red')
  */
-        __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_v_quiet); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(1, 1210, __pyx_L1_error)
+        __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_v_quiet); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(1, 1211, __pyx_L1_error)
         __pyx_t_18 = (!__pyx_t_17);
         if (__pyx_t_18) {
         } else {
           __pyx_t_9 = __pyx_t_18;
           goto __pyx_L28_bool_binop_done;
         }
-        __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_cmdout); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(1, 1210, __pyx_L1_error)
+        __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_cmdout); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(1, 1211, __pyx_L1_error)
         if (!__pyx_t_18) {
         } else {
           __pyx_t_9 = __pyx_t_18;
           goto __pyx_L28_bool_binop_done;
         }
-        __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_cmderr); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(1, 1210, __pyx_L1_error)
+        __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_cmderr); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(1, 1211, __pyx_L1_error)
         __pyx_t_9 = __pyx_t_18;
         __pyx_L28_bool_binop_done:;
         if (__pyx_t_9) {
 
-          /* "libmata/nfa/nfa.pyx":1211
+          /* "libmata/nfa/nfa.pyx":1212
  *             if objects[i].returncode:
  *                 if not quiet and (cmdout or cmderr):
  *                     print(f"captured stdout: {cmdout.decode('utf-8')}", 'red')             # <<<<<<<<<<<<<<
  *                     print(f"captured stderr: {cmderr.decode('utf-8')}", 'red')
  *                 raise subprocess.CalledProcessError(
  */
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cmdout, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1211, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cmdout, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1212, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_1 = NULL;
           __pyx_t_8 = 0;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
             __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
             if (likely(__pyx_t_1)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -26653,45 +26408,45 @@
               __pyx_t_8 = 1;
             }
           }
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_kp_u_utf_8};
             __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1211, __pyx_L1_error)
+            if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1212, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           }
-          __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1211, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1212, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_captured_stdout, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1211, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_captured_stdout, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1212, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1211, __pyx_L1_error)
+          __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1212, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_7);
           PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7);
           __Pyx_INCREF(__pyx_n_u_red);
           __Pyx_GIVEREF(__pyx_n_u_red);
           PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_n_u_red);
           __pyx_t_7 = 0;
-          __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_3, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1211, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_3, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1212, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-          /* "libmata/nfa/nfa.pyx":1212
+          /* "libmata/nfa/nfa.pyx":1213
  *                 if not quiet and (cmdout or cmderr):
  *                     print(f"captured stdout: {cmdout.decode('utf-8')}", 'red')
  *                     print(f"captured stderr: {cmderr.decode('utf-8')}", 'red')             # <<<<<<<<<<<<<<
  *                 raise subprocess.CalledProcessError(
  *                     objects[i].returncode, unpiped_commands[i]
  */
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cmderr, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1212, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cmderr, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1213, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_1 = NULL;
           __pyx_t_8 = 0;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
             __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
             if (likely(__pyx_t_1)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -26701,72 +26456,72 @@
               __pyx_t_8 = 1;
             }
           }
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_kp_u_utf_8};
             __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1212, __pyx_L1_error)
+            if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1213, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           }
-          __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1212, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1213, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_captured_stderr, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1212, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_captured_stderr, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1213, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1212, __pyx_L1_error)
+          __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1213, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_7);
           PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7);
           __Pyx_INCREF(__pyx_n_u_red);
           __Pyx_GIVEREF(__pyx_n_u_red);
           PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_n_u_red);
           __pyx_t_7 = 0;
-          __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_3, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1212, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_3, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1213, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-          /* "libmata/nfa/nfa.pyx":1210
+          /* "libmata/nfa/nfa.pyx":1211
  *         for i in range(cmd_no):
  *             if objects[i].returncode:
  *                 if not quiet and (cmdout or cmderr):             # <<<<<<<<<<<<<<
  *                     print(f"captured stdout: {cmdout.decode('utf-8')}", 'red')
  *                     print(f"captured stderr: {cmderr.decode('utf-8')}", 'red')
  */
         }
 
-        /* "libmata/nfa/nfa.pyx":1213
+        /* "libmata/nfa/nfa.pyx":1214
  *                     print(f"captured stdout: {cmdout.decode('utf-8')}", 'red')
  *                     print(f"captured stderr: {cmderr.decode('utf-8')}", 'red')
  *                 raise subprocess.CalledProcessError(             # <<<<<<<<<<<<<<
  *                     objects[i].returncode, unpiped_commands[i]
  *                 )
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1213, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_subprocess); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1214, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CalledProcessError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1213, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CalledProcessError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1214, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "libmata/nfa/nfa.pyx":1214
+        /* "libmata/nfa/nfa.pyx":1215
  *                     print(f"captured stderr: {cmderr.decode('utf-8')}", 'red')
  *                 raise subprocess.CalledProcessError(
  *                     objects[i].returncode, unpiped_commands[i]             # <<<<<<<<<<<<<<
  *                 )
  * 
  */
-        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1214, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_objects, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1215, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_returncode); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1214, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_returncode); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1215, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_unpiped_commands, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1214, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_unpiped_commands, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1215, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_11 = NULL;
         __pyx_t_8 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_11)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -26778,71 +26533,71 @@
         }
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_t_2, __pyx_t_3};
           __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_8, 2+__pyx_t_8);
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1213, __pyx_L1_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1214, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
         __Pyx_Raise(__pyx_t_7, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __PYX_ERR(1, 1213, __pyx_L1_error)
+        __PYX_ERR(1, 1214, __pyx_L1_error)
 
-        /* "libmata/nfa/nfa.pyx":1209
+        /* "libmata/nfa/nfa.pyx":1210
  *     if check_results:
  *         for i in range(cmd_no):
  *             if objects[i].returncode:             # <<<<<<<<<<<<<<
  *                 if not quiet and (cmdout or cmderr):
  *                     print(f"captured stdout: {cmdout.decode('utf-8')}", 'red')
  */
       }
 
-      /* "libmata/nfa/nfa.pyx":1208
+      /* "libmata/nfa/nfa.pyx":1209
  *     # collect the return codes
  *     if check_results:
  *         for i in range(cmd_no):             # <<<<<<<<<<<<<<
  *             if objects[i].returncode:
  *                 if not quiet and (cmdout or cmderr):
  */
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "libmata/nfa/nfa.pyx":1207
+    /* "libmata/nfa/nfa.pyx":1208
  * 
  *     # collect the return codes
  *     if check_results:             # <<<<<<<<<<<<<<
  *         for i in range(cmd_no):
  *             if objects[i].returncode:
  */
   }
 
-  /* "libmata/nfa/nfa.pyx":1217
+  /* "libmata/nfa/nfa.pyx":1218
  *                 )
  * 
  *     return cmdout, cmderr             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1217, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 1218, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_cmdout);
   __Pyx_GIVEREF(__pyx_v_cmdout);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_cmdout);
   __Pyx_INCREF(__pyx_v_cmderr);
   __Pyx_GIVEREF(__pyx_v_cmderr);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_cmderr);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "libmata/nfa/nfa.pyx":1159
+  /* "libmata/nfa/nfa.pyx":1160
  * 
  * 
  * def run_safely_external_command(cmd: str, check_results=True, quiet=True, timeout=None, **kwargs):             # <<<<<<<<<<<<<<
  *     """Safely runs the piped command, without executing of the shell
  * 
  */
 
@@ -26870,15 +26625,15 @@
   __Pyx_XDECREF(__pyx_v_cmderr);
   __Pyx_XDECREF(__pyx_v_process);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libmata/nfa/nfa.pyx":1220
+/* "libmata/nfa/nfa.pyx":1221
  * 
  * 
  * def get_elements_from_bool_vec(bool_vec: list[int]):             # <<<<<<<<<<<<<<
  *     cdef CBoolVector c_bool_vec = CBoolVector(bool_vec)
  *     cdef StateSet c_states
  */
 
@@ -26920,111 +26675,111 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_bool_vec)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1220, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1221, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_elements_from_bool_vec") < 0)) __PYX_ERR(1, 1220, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_elements_from_bool_vec") < 0)) __PYX_ERR(1, 1221, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_bool_vec = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_elements_from_bool_vec", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 1220, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_elements_from_bool_vec", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 1221, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("libmata.nfa.nfa.get_elements_from_bool_vec", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_bool_vec), (&PyList_Type), 0, "bool_vec", 1))) __PYX_ERR(1, 1220, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_bool_vec), (&PyList_Type), 0, "bool_vec", 1))) __PYX_ERR(1, 1221, __pyx_L1_error)
   __pyx_r = __pyx_pf_7libmata_3nfa_3nfa_60get_elements_from_bool_vec(__pyx_self, __pyx_v_bool_vec);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_3nfa_3nfa_60get_elements_from_bool_vec(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_bool_vec) {
   Mata::BoolVector __pyx_v_c_bool_vec;
   Mata::Nfa::StateSet __pyx_v_c_states;
-  Mata::Nfa::State __pyx_9genexpr25__pyx_v_state;
+  Mata::Nfa::State __pyx_9genexpr24__pyx_v_state;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   std::vector<uint8_t>  __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Mata::Util::OrdVector<Mata::Nfa::State> ::iterator __pyx_t_3;
   Mata::Nfa::State __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_elements_from_bool_vec", 0);
 
-  /* "libmata/nfa/nfa.pyx":1221
+  /* "libmata/nfa/nfa.pyx":1222
  * 
  * def get_elements_from_bool_vec(bool_vec: list[int]):
  *     cdef CBoolVector c_bool_vec = CBoolVector(bool_vec)             # <<<<<<<<<<<<<<
  *     cdef StateSet c_states
  *     mata_nfa.get_elements(&c_states, c_bool_vec)
  */
-  __pyx_t_1 = __pyx_convert_vector_from_py_uint8_t(__pyx_v_bool_vec); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1221, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_from_py_uint8_t(__pyx_v_bool_vec); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1222, __pyx_L1_error)
   __pyx_v_c_bool_vec = Mata::BoolVector(__pyx_t_1);
 
-  /* "libmata/nfa/nfa.pyx":1223
+  /* "libmata/nfa/nfa.pyx":1224
  *     cdef CBoolVector c_bool_vec = CBoolVector(bool_vec)
  *     cdef StateSet c_states
  *     mata_nfa.get_elements(&c_states, c_bool_vec)             # <<<<<<<<<<<<<<
  *     return { state for state in c_states }
  * 
  */
   Mata::Nfa::Plumbing::get_elements((&__pyx_v_c_states), __pyx_v_c_bool_vec);
 
-  /* "libmata/nfa/nfa.pyx":1224
+  /* "libmata/nfa/nfa.pyx":1225
  *     cdef StateSet c_states
  *     mata_nfa.get_elements(&c_states, c_bool_vec)
  *     return { state for state in c_states }             # <<<<<<<<<<<<<<
  * 
  * # On the fly configuration of the library
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_2 = PySet_New(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1224, __pyx_L1_error)
+    __pyx_t_2 = PySet_New(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_v_c_states.begin();
     for (;;) {
       if (!(__pyx_t_3 != __pyx_v_c_states.end())) break;
       __pyx_t_4 = *__pyx_t_3;
       ++__pyx_t_3;
-      __pyx_9genexpr25__pyx_v_state = __pyx_t_4;
-      __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_9genexpr25__pyx_v_state); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1224, __pyx_L1_error)
+      __pyx_9genexpr24__pyx_v_state = __pyx_t_4;
+      __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_9genexpr24__pyx_v_state); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1225, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(PySet_Add(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 1224, __pyx_L1_error)
+      if (unlikely(PySet_Add(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 1225, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
   } /* exit inner scope */
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "libmata/nfa/nfa.pyx":1220
+  /* "libmata/nfa/nfa.pyx":1221
  * 
  * 
  * def get_elements_from_bool_vec(bool_vec: list[int]):             # <<<<<<<<<<<<<<
  *     cdef CBoolVector c_bool_vec = CBoolVector(bool_vec)
  *     cdef StateSet c_states
  */
 
@@ -27036,15 +26791,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "libmata/nfa/nfa.pyx":1247
+/* "libmata/nfa/nfa.pyx":1248
  * 
  * 
  * def store():             # <<<<<<<<<<<<<<
  *     """
  *     Returns the configuration of the library
  */
 
@@ -27069,27 +26824,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("store", 0);
 
-  /* "libmata/nfa/nfa.pyx":1251
+  /* "libmata/nfa/nfa.pyx":1252
  *     Returns the configuration of the library
  *     """
  *     return _store             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_store_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1251, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_store_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "libmata/nfa/nfa.pyx":1247
+  /* "libmata/nfa/nfa.pyx":1248
  * 
  * 
  * def store():             # <<<<<<<<<<<<<<
  *     """
  *     Returns the configuration of the library
  */
 
@@ -28145,15 +27900,15 @@
     {&__pyx_kp_u_1_5, __pyx_k_1_5, sizeof(__pyx_k_1_5), 0, 1, 0, 0},
     {&__pyx_n_s_AssertionError, __pyx_k_AssertionError, sizeof(__pyx_k_AssertionError), 0, 0, 1, 1},
     {&__pyx_n_s_CalledProcessError, __pyx_k_CalledProcessError, sizeof(__pyx_k_CalledProcessError), 0, 0, 1, 1},
     {&__pyx_kp_u_Cannot_translate_symbol, __pyx_k_Cannot_translate_symbol, sizeof(__pyx_k_Cannot_translate_symbol), 0, 1, 0, 0},
     {&__pyx_kp_u_Courier_Bold, __pyx_k_Courier_Bold, sizeof(__pyx_k_Courier_Bold), 0, 1, 0, 0},
     {&__pyx_n_s_DataFrame, __pyx_k_DataFrame, sizeof(__pyx_k_DataFrame), 0, 0, 1, 1},
     {&__pyx_n_s_DiGraph, __pyx_k_DiGraph, sizeof(__pyx_k_DiGraph), 0, 0, 1, 1},
-    {&__pyx_kp_u_Encodes_word_based_on_a_string_t, __pyx_k_Encodes_word_based_on_a_string_t, sizeof(__pyx_k_Encodes_word_based_on_a_string_t), 0, 1, 0, 0},
+    {&__pyx_kp_u_Encodes_word_based_on_a_passed_a, __pyx_k_Encodes_word_based_on_a_passed_a, sizeof(__pyx_k_Encodes_word_based_on_a_passed_a), 0, 1, 0, 0},
     {&__pyx_kp_u_For_a_given_path_set_of_states_r, __pyx_k_For_a_given_path_set_of_states_r, sizeof(__pyx_k_For_a_given_path_set_of_states_r), 0, 1, 0, 0},
     {&__pyx_n_s_G, __pyx_k_G, sizeof(__pyx_k_G), 0, 0, 1, 1},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_n_s_Move, __pyx_k_Move, sizeof(__pyx_k_Move), 0, 0, 1, 1},
     {&__pyx_kp_s_Move_None, __pyx_k_Move_None, sizeof(__pyx_k_Move_None), 0, 0, 1, 0},
     {&__pyx_n_s_Move___neq, __pyx_k_Move___neq, sizeof(__pyx_k_Move___neq), 0, 0, 1, 1},
     {&__pyx_n_s_Move___reduce_cython, __pyx_k_Move___reduce_cython, sizeof(__pyx_k_Move___reduce_cython), 0, 0, 1, 1},
@@ -28455,15 +28210,14 @@
     {&__pyx_n_s_states, __pyx_k_states, sizeof(__pyx_k_states), 0, 0, 1, 1},
     {&__pyx_n_s_stderr, __pyx_k_stderr, sizeof(__pyx_k_stderr), 0, 0, 1, 1},
     {&__pyx_n_s_stdin, __pyx_k_stdin, sizeof(__pyx_k_stdin), 0, 0, 1, 1},
     {&__pyx_n_s_stdout, __pyx_k_stdout, sizeof(__pyx_k_stdout), 0, 0, 1, 1},
     {&__pyx_n_s_store, __pyx_k_store, sizeof(__pyx_k_store), 0, 0, 1, 1},
     {&__pyx_n_s_store_2, __pyx_k_store_2, sizeof(__pyx_k_store_2), 0, 0, 1, 1},
     {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
-    {&__pyx_n_s_string_to_symbol, __pyx_k_string_to_symbol, sizeof(__pyx_k_string_to_symbol), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_strip, __pyx_k_strip, sizeof(__pyx_k_strip), 0, 0, 1, 1},
     {&__pyx_n_u_style, __pyx_k_style, sizeof(__pyx_k_style), 0, 1, 0, 1},
     {&__pyx_n_s_subprocess, __pyx_k_subprocess, sizeof(__pyx_k_subprocess), 0, 0, 1, 1},
     {&__pyx_n_s_subset_map, __pyx_k_subset_map, sizeof(__pyx_k_subset_map), 0, 0, 1, 1},
     {&__pyx_n_s_symb, __pyx_k_symb, sizeof(__pyx_k_symb), 0, 0, 1, 1},
     {&__pyx_n_s_symbol, __pyx_k_symbol, sizeof(__pyx_k_symbol), 0, 0, 1, 1},
@@ -28515,34 +28269,34 @@
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(1, 176, __pyx_L1_error)
   __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(1, 566, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 920, __pyx_L1_error)
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 1147, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 1148, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 68, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "libmata/nfa/nfa.pyx":1150
+  /* "libmata/nfa/nfa.pyx":1151
  *     lhs = Nfa(k+1)
  *     lhs.make_initial_state(0)
  *     lhs.add_transition(0, 0, 0)             # <<<<<<<<<<<<<<
  *     for i in range(1, k + 1):
  *         lhs.add_transition(i - 1, 1, i)
  */
-  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_0, __pyx_int_0, __pyx_int_0); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 1150, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_0, __pyx_int_0, __pyx_int_0); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 1151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "libmata/nfa/nfa.pyx":30
  * cdef Symbol EPSILON = CEPSILON
  * 
  * def epsilon():             # <<<<<<<<<<<<<<
@@ -29441,70 +29195,70 @@
   __Pyx_GOTREF(__pyx_tuple__156);
   __Pyx_GIVEREF(__pyx_tuple__156);
   __pyx_codeobj__157 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__156, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_get_word_for_path, 1096, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__157)) __PYX_ERR(1, 1096, __pyx_L1_error)
 
   /* "libmata/nfa/nfa.pyx":1112
  *     return result.first.word, result.second
  * 
- * def encode_word(string_to_symbol, word):             # <<<<<<<<<<<<<<
- *     """Encodes word based on a string to symbol map
+ * def encode_word(alph.Alphabet alphabet, word):             # <<<<<<<<<<<<<<
+ *     """Encodes word based on a passed alphabet
  * 
  */
-  __pyx_tuple__158 = PyTuple_Pack(6, __pyx_n_s_string_to_symbol, __pyx_n_s_word, __pyx_n_s_result, __pyx_n_s_k, __pyx_n_s_v, __pyx_n_s_s); if (unlikely(!__pyx_tuple__158)) __PYX_ERR(1, 1112, __pyx_L1_error)
+  __pyx_tuple__158 = PyTuple_Pack(5, __pyx_n_s_alphabet, __pyx_n_s_word, __pyx_n_s_c_alphabet, __pyx_n_s_result, __pyx_n_s_s); if (unlikely(!__pyx_tuple__158)) __PYX_ERR(1, 1112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__158);
   __Pyx_GIVEREF(__pyx_tuple__158);
-  __pyx_codeobj__159 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__158, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_encode_word, 1112, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__159)) __PYX_ERR(1, 1112, __pyx_L1_error)
+  __pyx_codeobj__159 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__158, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_encode_word, 1112, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__159)) __PYX_ERR(1, 1112, __pyx_L1_error)
 
-  /* "libmata/nfa/nfa.pyx":1145
+  /* "libmata/nfa/nfa.pyx":1146
  * 
  * # Temporary for testing
  * def divisible_by(k: int):             # <<<<<<<<<<<<<<
  *     """Constructs automaton accepting strings containing ones divisible by "k"."""
  *     assert k > 1
  */
-  __pyx_tuple__160 = PyTuple_Pack(3, __pyx_n_s_k, __pyx_n_s_lhs, __pyx_n_s_i); if (unlikely(!__pyx_tuple__160)) __PYX_ERR(1, 1145, __pyx_L1_error)
+  __pyx_tuple__160 = PyTuple_Pack(3, __pyx_n_s_k, __pyx_n_s_lhs, __pyx_n_s_i); if (unlikely(!__pyx_tuple__160)) __PYX_ERR(1, 1146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__160);
   __Pyx_GIVEREF(__pyx_tuple__160);
-  __pyx_codeobj__161 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__160, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_divisible_by, 1145, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__161)) __PYX_ERR(1, 1145, __pyx_L1_error)
+  __pyx_codeobj__161 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__160, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_divisible_by, 1146, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__161)) __PYX_ERR(1, 1146, __pyx_L1_error)
 
-  /* "libmata/nfa/nfa.pyx":1159
+  /* "libmata/nfa/nfa.pyx":1160
  * 
  * 
  * def run_safely_external_command(cmd: str, check_results=True, quiet=True, timeout=None, **kwargs):             # <<<<<<<<<<<<<<
  *     """Safely runs the piped command, without executing of the shell
  * 
  */
-  __pyx_tuple__162 = PyTuple_Pack(16, __pyx_n_s_cmd, __pyx_n_s_check_results, __pyx_n_s_quiet, __pyx_n_s_timeout, __pyx_n_s_kwargs, __pyx_n_s_unpiped_commands, __pyx_n_s_cmd_no, __pyx_n_s_objects, __pyx_n_s_i, __pyx_n_s_executed_command, __pyx_n_s_stdin, __pyx_n_s_stderr, __pyx_n_s_piped_command, __pyx_n_s_cmdout, __pyx_n_s_cmderr, __pyx_n_s_process); if (unlikely(!__pyx_tuple__162)) __PYX_ERR(1, 1159, __pyx_L1_error)
+  __pyx_tuple__162 = PyTuple_Pack(16, __pyx_n_s_cmd, __pyx_n_s_check_results, __pyx_n_s_quiet, __pyx_n_s_timeout, __pyx_n_s_kwargs, __pyx_n_s_unpiped_commands, __pyx_n_s_cmd_no, __pyx_n_s_objects, __pyx_n_s_i, __pyx_n_s_executed_command, __pyx_n_s_stdin, __pyx_n_s_stderr, __pyx_n_s_piped_command, __pyx_n_s_cmdout, __pyx_n_s_cmderr, __pyx_n_s_process); if (unlikely(!__pyx_tuple__162)) __PYX_ERR(1, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__162);
   __Pyx_GIVEREF(__pyx_tuple__162);
-  __pyx_codeobj__163 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__162, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_run_safely_external_command, 1159, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__163)) __PYX_ERR(1, 1159, __pyx_L1_error)
-  __pyx_tuple__164 = PyTuple_Pack(3, ((PyObject *)Py_True), ((PyObject *)Py_True), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__164)) __PYX_ERR(1, 1159, __pyx_L1_error)
+  __pyx_codeobj__163 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__162, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_run_safely_external_command, 1160, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__163)) __PYX_ERR(1, 1160, __pyx_L1_error)
+  __pyx_tuple__164 = PyTuple_Pack(3, ((PyObject *)Py_True), ((PyObject *)Py_True), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__164)) __PYX_ERR(1, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__164);
   __Pyx_GIVEREF(__pyx_tuple__164);
 
-  /* "libmata/nfa/nfa.pyx":1220
+  /* "libmata/nfa/nfa.pyx":1221
  * 
  * 
  * def get_elements_from_bool_vec(bool_vec: list[int]):             # <<<<<<<<<<<<<<
  *     cdef CBoolVector c_bool_vec = CBoolVector(bool_vec)
  *     cdef StateSet c_states
  */
-  __pyx_tuple__165 = PyTuple_Pack(4, __pyx_n_s_bool_vec, __pyx_n_s_c_bool_vec, __pyx_n_s_c_states, __pyx_n_s_state); if (unlikely(!__pyx_tuple__165)) __PYX_ERR(1, 1220, __pyx_L1_error)
+  __pyx_tuple__165 = PyTuple_Pack(4, __pyx_n_s_bool_vec, __pyx_n_s_c_bool_vec, __pyx_n_s_c_states, __pyx_n_s_state); if (unlikely(!__pyx_tuple__165)) __PYX_ERR(1, 1221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__165);
   __Pyx_GIVEREF(__pyx_tuple__165);
-  __pyx_codeobj__166 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__165, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_get_elements_from_bool_vec, 1220, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__166)) __PYX_ERR(1, 1220, __pyx_L1_error)
+  __pyx_codeobj__166 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__165, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_get_elements_from_bool_vec, 1221, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__166)) __PYX_ERR(1, 1221, __pyx_L1_error)
 
-  /* "libmata/nfa/nfa.pyx":1247
+  /* "libmata/nfa/nfa.pyx":1248
  * 
  * 
  * def store():             # <<<<<<<<<<<<<<
  *     """
  *     Returns the configuration of the library
  */
-  __pyx_codeobj__167 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_store, 1247, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__167)) __PYX_ERR(1, 1247, __pyx_L1_error)
+  __pyx_codeobj__167 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_libmata_nfa_nfa_pyx, __pyx_n_s_store, 1248, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__167)) __PYX_ERR(1, 1248, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -29712,18 +29466,18 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 33, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -31236,152 +30990,152 @@
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_word_for_path, __pyx_t_4) < 0) __PYX_ERR(1, 1096, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "libmata/nfa/nfa.pyx":1112
  *     return result.first.word, result.second
  * 
- * def encode_word(string_to_symbol, word):             # <<<<<<<<<<<<<<
- *     """Encodes word based on a string to symbol map
+ * def encode_word(alph.Alphabet alphabet, word):             # <<<<<<<<<<<<<<
+ *     """Encodes word based on a passed alphabet
  * 
  */
   __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_55encode_word, 0, __pyx_n_s_encode_word, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__159)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_word, __pyx_t_4) < 0) __PYX_ERR(1, 1112, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1145
+  /* "libmata/nfa/nfa.pyx":1146
  * 
  * # Temporary for testing
  * def divisible_by(k: int):             # <<<<<<<<<<<<<<
  *     """Constructs automaton accepting strings containing ones divisible by "k"."""
  *     assert k > 1
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1145, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_k, __pyx_n_s_int) < 0) __PYX_ERR(1, 1145, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_57divisible_by, 0, __pyx_n_s_divisible_by, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__161)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_k, __pyx_n_s_int) < 0) __PYX_ERR(1, 1146, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_57divisible_by, 0, __pyx_n_s_divisible_by, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__161)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_divisible_by, __pyx_t_2) < 0) __PYX_ERR(1, 1145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_divisible_by, __pyx_t_2) < 0) __PYX_ERR(1, 1146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1159
+  /* "libmata/nfa/nfa.pyx":1160
  * 
  * 
  * def run_safely_external_command(cmd: str, check_results=True, quiet=True, timeout=None, **kwargs):             # <<<<<<<<<<<<<<
  *     """Safely runs the piped command, without executing of the shell
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1159, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_cmd, __pyx_n_s_str) < 0) __PYX_ERR(1, 1159, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_59run_safely_external_command, 0, __pyx_n_s_run_safely_external_command, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__163)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_cmd, __pyx_n_s_str) < 0) __PYX_ERR(1, 1160, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_59run_safely_external_command, 0, __pyx_n_s_run_safely_external_command, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__163)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__164);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_run_safely_external_command, __pyx_t_4) < 0) __PYX_ERR(1, 1159, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_run_safely_external_command, __pyx_t_4) < 0) __PYX_ERR(1, 1160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1220
+  /* "libmata/nfa/nfa.pyx":1221
  * 
  * 
  * def get_elements_from_bool_vec(bool_vec: list[int]):             # <<<<<<<<<<<<<<
  *     cdef CBoolVector c_bool_vec = CBoolVector(bool_vec)
  *     cdef StateSet c_states
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_bool_vec, __pyx_kp_s_list_int) < 0) __PYX_ERR(1, 1220, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_61get_elements_from_bool_vec, 0, __pyx_n_s_get_elements_from_bool_vec, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__166)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1220, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_bool_vec, __pyx_kp_s_list_int) < 0) __PYX_ERR(1, 1221, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_61get_elements_from_bool_vec, 0, __pyx_n_s_get_elements_from_bool_vec, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__166)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_elements_from_bool_vec, __pyx_t_2) < 0) __PYX_ERR(1, 1220, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_elements_from_bool_vec, __pyx_t_2) < 0) __PYX_ERR(1, 1221, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1228
+  /* "libmata/nfa/nfa.pyx":1229
  * # On the fly configuration of the library
  * _store = {
  *     'node_style': {             # <<<<<<<<<<<<<<
  *         "style": "filled",
  *         "color": "darkblue",
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1228, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "libmata/nfa/nfa.pyx":1229
+  /* "libmata/nfa/nfa.pyx":1230
  * _store = {
  *     'node_style': {
  *         "style": "filled",             # <<<<<<<<<<<<<<
  *         "color": "darkblue",
  *         "fillcolor": "lightsteelblue",
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1229, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(9); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_style, __pyx_n_u_filled) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_color, __pyx_n_u_darkblue) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fillcolor, __pyx_n_u_lightsteelblue) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fontname, __pyx_kp_u_Courier_Bold) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_width, __pyx_kp_u_0_3) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_height, __pyx_kp_u_0_3) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fontsize, __pyx_kp_u_12) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fixedsize, __pyx_n_u_true) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_penwidth, __pyx_kp_u_1_5) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_node_style, __pyx_t_4) < 0) __PYX_ERR(1, 1228, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_style, __pyx_n_u_filled) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_color, __pyx_n_u_darkblue) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fillcolor, __pyx_n_u_lightsteelblue) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fontname, __pyx_kp_u_Courier_Bold) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_width, __pyx_kp_u_0_3) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_height, __pyx_kp_u_0_3) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fontsize, __pyx_kp_u_12) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_fixedsize, __pyx_n_u_true) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_penwidth, __pyx_kp_u_1_5) < 0) __PYX_ERR(1, 1230, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_node_style, __pyx_t_4) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1240
+  /* "libmata/nfa/nfa.pyx":1241
  *     },
  *     'edge_style': {
  *         "penwidth": "1.5",             # <<<<<<<<<<<<<<
  *         "color": "midnightblue",
  *     },
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1240, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_penwidth, __pyx_kp_u_1_5) < 0) __PYX_ERR(1, 1240, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_color, __pyx_n_u_midnightblue) < 0) __PYX_ERR(1, 1240, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_edge_style, __pyx_t_4) < 0) __PYX_ERR(1, 1228, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_penwidth, __pyx_kp_u_1_5) < 0) __PYX_ERR(1, 1241, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_color, __pyx_n_u_midnightblue) < 0) __PYX_ERR(1, 1241, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_edge_style, __pyx_t_4) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1243
+  /* "libmata/nfa/nfa.pyx":1244
  *         "color": "midnightblue",
  *     },
  *     'alphabet': None,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_alphabet, Py_None) < 0) __PYX_ERR(1, 1228, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_store_2, __pyx_t_2) < 0) __PYX_ERR(1, 1227, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_alphabet, Py_None) < 0) __PYX_ERR(1, 1229, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_store_2, __pyx_t_2) < 0) __PYX_ERR(1, 1228, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "libmata/nfa/nfa.pyx":1247
+  /* "libmata/nfa/nfa.pyx":1248
  * 
  * 
  * def store():             # <<<<<<<<<<<<<<
  *     """
  *     Returns the configuration of the library
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_63store, 0, __pyx_n_s_store, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__167)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1247, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7libmata_3nfa_3nfa_63store, 0, __pyx_n_s_store, NULL, __pyx_n_s_libmata_nfa_nfa, __pyx_d, ((PyObject *)__pyx_codeobj__167)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_store, __pyx_t_2) < 0) __PYX_ERR(1, 1247, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_store, __pyx_t_2) < 0) __PYX_ERR(1, 1248, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "libmata/nfa/nfa.pyx":1
  * import shlex             # <<<<<<<<<<<<<<
  * import subprocess
  * import pandas
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_get_word_for_path_line_1096, __pyx_kp_u_For_a_given_path_set_of_states_r) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_encode_word_line_1112, __pyx_kp_u_Encodes_word_based_on_a_string_t) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_encode_word_line_1112, __pyx_kp_u_Encodes_word_based_on_a_passed_a) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
```

### Comparing `libmata-0.91.0/libmata/nfa/nfa.pxd` & `libmata-0.92.0/libmata/nfa/nfa.pxd`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from libcpp.memory cimport shared_ptr
 from libcpp.string cimport string
 from libcpp.list cimport list as clist
 from libcpp.pair cimport pair
 from libc.stdint cimport uintptr_t, uint8_t
 
 from libmata.utils cimport CSparseSet, COrdVector, CBoolVector, CBinaryRelation
-from libmata.alphabets cimport CAlphabet, StringToSymbolMap, Symbol
+from libmata.alphabets cimport CAlphabet, Symbol
 
 cdef extern from "<iostream>" namespace "std":
     cdef cppclass ostream:
         ostream& write(const char*, int) except +
 
 cdef extern from "<fstream>" namespace "std":
     cdef cppclass ofstream(ostream):
@@ -29,19 +29,18 @@
     # Typedefs
     ctypedef uintptr_t State
     ctypedef COrdVector[State] StateSet
     ctypedef uset[State] UnorderedStateSet
     ctypedef umap[Symbol, StateSet] PostSymb
     ctypedef umap[State, PostSymb] StateToPostMap
     ctypedef umap[string, State] StringSubsetMap
-    ctypedef umap[string, State] StringToStateMap
-    ctypedef umap[State, string] StateToStringMap
-    ctypedef umap[State, State] StateToStateMap
-    ctypedef umap[Symbol, string] SymbolToStringMap
-    ctypedef umap[string, string] StringMap
+    ctypedef umap[string, State] StateNameMap
+    ctypedef umap[State, string] StateNameMap
+    ctypedef umap[State, State] StateRenaming
+    ctypedef umap[string, string] ParameterMap
 
     cdef const Symbol CEPSILON "Mata::Nfa::EPSILON"
 
     cdef cppclass CPost "Mata::Nfa::Post":
         void insert(CMove&)
         CMove& operator[](Symbol)
         CMove& back()
@@ -152,60 +151,60 @@
         State add_state()
         State add_state(State)
         void print_to_DOT(ostream)
         CPost get_moves_from(State)
         vector[CTrans] get_transitions_to(State)
         vector[CTrans] get_trans_as_sequence()
         vector[CTrans] get_trans_from_as_sequence(State)
-        void trim(StateToStateMap*)
+        void trim(StateRenaming*)
         void get_one_letter_aut(CNfa&)
         bool is_epsilon(Symbol)
         CBoolVector get_useful_states()
         StateSet get_reachable_states()
         StateSet get_terminating_states()
         void remove_epsilon(Symbol) except +
         COrdVector[CMove].const_iterator get_epsilon_transitions(State state, Symbol epsilon)
         COrdVector[CMove].const_iterator get_epsilon_transitions(CPost& post, Symbol epsilon)
         void clear()
         size_t size()
 
     # Automata tests
     cdef bool c_is_deterministic "Mata::Nfa::is_deterministic" (CNfa&)
     cdef bool c_is_lang_empty "Mata::Nfa::is_lang_empty" (CNfa&, CRun*)
-    cdef bool c_is_universal "Mata::Nfa::is_universal" (CNfa&, CAlphabet&, StringMap&) except +
-    cdef bool c_is_included "Mata::Nfa::is_included" (CNfa&, CNfa&, CAlphabet*, StringMap&)
-    cdef bool c_is_included "Mata::Nfa::is_included" (CNfa&, CNfa&, CRun*, CAlphabet*, StringMap&) except +
-    cdef bool c_are_equivalent "Mata::Nfa::are_equivalent" (CNfa&, CNfa&, CAlphabet*, StringMap&)
-    cdef bool c_are_equivalent "Mata::Nfa::are_equivalent" (CNfa&, CNfa&, StringMap&)
+    cdef bool c_is_universal "Mata::Nfa::is_universal" (CNfa&, CAlphabet&, ParameterMap&) except +
+    cdef bool c_is_included "Mata::Nfa::is_included" (CNfa&, CNfa&, CAlphabet*, ParameterMap&)
+    cdef bool c_is_included "Mata::Nfa::is_included" (CNfa&, CNfa&, CRun*, CAlphabet*, ParameterMap&) except +
+    cdef bool c_are_equivalent "Mata::Nfa::are_equivalent" (CNfa&, CNfa&, CAlphabet*, ParameterMap&)
+    cdef bool c_are_equivalent "Mata::Nfa::are_equivalent" (CNfa&, CNfa&, ParameterMap&)
     cdef bool c_is_complete "Mata::Nfa::is_complete" (CNfa&, CAlphabet&) except +
     cdef bool c_is_in_lang "Mata::Nfa::is_in_lang" (CNfa&, CRun&)
     cdef bool c_is_prfx_in_lang "Mata::Nfa::is_prfx_in_lang" (CNfa&, CRun&)
 
     # Automata operations
     cdef void compute_fw_direct_simulation(const CNfa&)
 
     # Helper functions
     cdef pair[CRun, bool] c_get_word_for_path "Mata::Nfa::get_word_for_path" (CNfa&, CRun&)
-    cdef CRun c_encode_word "Mata::Nfa::encode_word" (StringToSymbolMap&, vector[string])
+    cdef CRun c_encode_word "Mata::Nfa::encode_word" (CAlphabet*, vector[string])
 
 cdef extern from "mata/nfa/algorithms.hh" namespace "Mata::Nfa::Algorithms":
-    cdef CBinaryRelation& c_compute_relation "Mata::Nfa::Algorithms::compute_relation" (CNfa&, StringMap&)
+    cdef CBinaryRelation& c_compute_relation "Mata::Nfa::Algorithms::compute_relation" (CNfa&, ParameterMap&)
 
 cdef extern from "mata/nfa/plumbing.hh" namespace "Mata::Nfa::Plumbing":
     cdef void get_elements(StateSet*, CBoolVector)
     cdef void c_determinize "Mata::Nfa::Plumbing::determinize" (CNfa*, CNfa&, umap[StateSet, State]*)
     cdef void c_uni "Mata::Nfa::Plumbing::uni" (CNfa*, CNfa&, CNfa&)
     cdef void c_intersection "Mata::Nfa::Plumbing::intersection" (CNfa*, CNfa&, CNfa&, bool, umap[pair[State, State], State]*)
-    cdef void c_concatenate "Mata::Nfa::Plumbing::concatenate" (CNfa*, CNfa&, CNfa&, bool, StateToStateMap*, StateToStateMap*)
-    cdef void c_complement "Mata::Nfa::Plumbing::complement" (CNfa*, CNfa&, CAlphabet&, StringMap&) except +
+    cdef void c_concatenate "Mata::Nfa::Plumbing::concatenate" (CNfa*, CNfa&, CNfa&, bool, StateRenaming*, StateRenaming*)
+    cdef void c_complement "Mata::Nfa::Plumbing::complement" (CNfa*, CNfa&, CAlphabet&, ParameterMap&) except +
     cdef void c_make_complete "Mata::Nfa::Plumbing::make_complete" (CNfa*, CAlphabet&, State) except +
     cdef void c_revert "Mata::Nfa::Plumbing::revert" (CNfa*, CNfa&)
     cdef void c_remove_epsilon "Mata::Nfa::Plumbing::remove_epsilon" (CNfa*, CNfa&, Symbol) except +
     cdef void c_minimize "Mata::Nfa::Plumbing::minimize" (CNfa*, CNfa&)
-    cdef void c_reduce "Mata::Nfa::Plumbing::reduce" (CNfa*, CNfa&, bool, StateToStateMap*, StringMap&)
+    cdef void c_reduce "Mata::Nfa::Plumbing::reduce" (CNfa*, CNfa&, bool, StateRenaming*, ParameterMap&)
 
 
 
 # Forward declarations of classes
 #
 # This is needed in order for these classes to be used in other packages.
 cdef class Nfa:
```

### Comparing `libmata-0.91.0/libmata/nfa/nfa.pyx` & `libmata-0.92.0/libmata/nfa/nfa.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from cython.operator import dereference, postincrement as postinc, preincrement as preinc
 
 cimport libmata.nfa.nfa as mata_nfa
 cimport libmata.alphabets as alph
 
 from libmata.nfa.nfa cimport \
-    Symbol, State, StateSet, StateToStateMap, StringToSymbolMap, \
+    Symbol, State, StateSet, StateRenaming, \
     CDelta, CRun, CTrans, CNfa, CMove, CEPSILON
 
 from libmata.alphabets cimport CAlphabet
 from libmata.utils cimport COrdVector, CBinaryRelation, BinaryRelation
 
 cdef Symbol EPSILON = CEPSILON
 
@@ -500,15 +500,15 @@
 
         Remove states which are not accessible (unreachable; state is accessible when the state is the endpoint of a path
          starting from an initial state) or not co-accessible (non-terminating; state is co-accessible when the state is
          the starting point of a path ending in a final state).
 
         :return: State map of original to new states.
         """
-        cdef StateToStateMap state_map
+        cdef StateRenaming state_map
         self.thisptr.get().trim(&state_map)
         return {k: v for k, v in state_map}
 
     def get_one_letter_aut(self) -> Nfa:
         """Unify transitions to create a directed graph with at most a single transition between two states (using only
          one letter for all transitions).
 
@@ -778,16 +778,16 @@
 
     :param Nfa lhs: First automaton to concatenate.
     :param Nfa rhs: Second automaton to concatenate.
     :param use_epsilon: Whether to concatenate over an epsilon symbol.
     :return: Nfa: Concatenated automaton.
     """
     result = Nfa()
-    cdef StateToStateMap c_lhs_map
-    cdef StateToStateMap c_rhs_map
+    cdef StateRenaming c_lhs_map
+    cdef StateRenaming c_rhs_map
     mata_nfa.c_concatenate(result.thisptr.get(), dereference(lhs.thisptr.get()), dereference(rhs.thisptr.get()),
                          use_epsilon, &c_lhs_map, &c_rhs_map)
     lhs_map = {}
     for key, value in c_lhs_map:
         lhs_map[key] = value
     rhs_map = {}
     for key, value in c_rhs_map:
@@ -867,15 +867,15 @@
     :param Nfa aut: Original automaton to reduce.
     :param bool trim_input: Whether to trim the input automaton first or not.
     :param Dict params: Additional parameters for the reduction algorithm:
         - "algorithm": "simulation"
     :return: (Reduced automaton, state map of original to new states)
     """
     params = params or {"algorithm": "simulation"}
-    cdef StateToStateMap state_map
+    cdef StateRenaming state_map
     result = Nfa()
     mata_nfa.c_reduce(result.thisptr.get(), dereference(aut.thisptr.get()), trim_input, &state_map,
                     {
                         k.encode('utf-8'): v.encode('utf-8') for k, v in params.items()
                     }
                     )
 
@@ -1105,26 +1105,27 @@
     """
     cdef pair[CRun, bool] result
     input = Run()
     input.path = path
     result = mata_nfa.c_get_word_for_path(dereference(lhs.thisptr.get()), dereference(input.thisptr))
     return result.first.word, result.second
 
-def encode_word(string_to_symbol, word):
-    """Encodes word based on a string to symbol map
+def encode_word(alph.Alphabet alphabet, word):
+    """Encodes word based on a passed alphabet
 
-    >>> mata_nfa.Nfa.encode_word({'a': 1, 'b': 2, "c": 0}, "abca")
+    >>> mata_nfa.Nfa.encode_word(OnTheFlyAlphabet.from_symbol_map({'a': 1, 'b': 2, "c": 0}), "abca")
     [1, 2, 0, 1]
 
-    :param dict string_to_symbol: dictionary of strings to integers
-    :param word: list of strings representing a encoded word
-    :return:
+    :param alph.Alphabet alphabet: Alphabet to encode the word with.
+    :param word: list of strings representing an encoded word.
+    :return: Encoded word.
     """
+    cdef CAlphabet* c_alphabet = alphabet.as_base()
     result = mata_nfa.c_encode_word(
-        {k.encode('utf-8'): v for (k, v) in string_to_symbol.items()},
+        c_alphabet,
         [s.encode('utf-8') for s in word]
     )
     return result.word
 
 cdef subset_map_to_dictionary(umap[StateSet, State] subset_map):
     """Helper function that translates the unordered map to dictionary
 
@@ -1244,8 +1245,8 @@
 }
 
 
 def store():
     """
     Returns the configuration of the library
     """
-    return _store
+    return _store
```

### Comparing `libmata-0.91.0/libmata/nfa/strings.cpp` & `libmata-0.92.0/libmata/nfa/strings.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1462,42 +1462,42 @@
  */
 struct __pyx_obj_7libmata_5utils_BinaryRelation {
   PyObject_HEAD
   Simlib::Util::BinaryRelation *thisptr;
 };
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 struct __pyx_obj_7libmata_9alphabets_Alphabet {
   PyObject_HEAD
   struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *__pyx_vtab;
 };
 
 
-/* "libmata/nfa/nfa.pxd":211
+/* "libmata/nfa/nfa.pxd":210
  * #
  * # This is needed in order for these classes to be used in other packages.
  * cdef class Nfa:             # <<<<<<<<<<<<<<
  *     # TODO: Shared pointers are not ideal as they bring some overhead which could be substantial in theory. We are not
  *     #  sure whether the shared pointers will be a problem in this case, but it would be good to pay attention to this and
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Nfa {
   PyObject_HEAD
   std::shared_ptr<Mata::Nfa::Nfa>  thisptr;
   PyObject *label;
 };
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Trans {
@@ -1517,30 +1517,30 @@
 struct __pyx_obj_7libmata_3nfa_7strings_Segmentation {
   PyObject_HEAD
   Mata::Strings::SegNfa::Segmentation *thisptr;
 };
 
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 
 struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet {
   Mata::Alphabet *(*as_base)(struct __pyx_obj_7libmata_9alphabets_Alphabet *);
   PyObject *(*get_symbols)(struct __pyx_obj_7libmata_9alphabets_Alphabet *);
 };
 static struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *__pyx_vtabptr_7libmata_9alphabets_Alphabet;
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 
@@ -3921,15 +3921,15 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_3nfa_7strings_12Segmentation_6get_segments(struct __pyx_obj_7libmata_3nfa_7strings_Segmentation *__pyx_v_self) {
   PyObject *__pyx_v_segments = NULL;
-  Mata::Nfa::AutSequence __pyx_v_c_segments;
+  std::vector<Mata::Nfa::Nfa>  __pyx_v_c_segments;
   Mata::Nfa::Nfa __pyx_v_c_segment;
   PyObject *__pyx_v_segment = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   std::vector<Mata::Nfa::Nfa> ::iterator __pyx_t_2;
   Mata::Nfa::Nfa __pyx_t_3;
@@ -3942,47 +3942,47 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_segments", 0);
 
   /* "libmata/nfa/strings.pyx":47
  *                  automaton) to the right (final states of segment automaton).
  *         """
  *         segments = []             # <<<<<<<<<<<<<<
- *         cdef AutSequence c_segments = self.thisptr.get_segments()
+ *         cdef vector[CNfa] c_segments = self.thisptr.get_segments()
  *         for c_segment in c_segments:
  */
   __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_segments = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "libmata/nfa/strings.pyx":48
  *         """
  *         segments = []
- *         cdef AutSequence c_segments = self.thisptr.get_segments()             # <<<<<<<<<<<<<<
+ *         cdef vector[CNfa] c_segments = self.thisptr.get_segments()             # <<<<<<<<<<<<<<
  *         for c_segment in c_segments:
  *             segment = mata_nfa.Nfa(c_segment.size())
  */
   __pyx_v_c_segments = __pyx_v_self->thisptr->get_segments();
 
   /* "libmata/nfa/strings.pyx":49
  *         segments = []
- *         cdef AutSequence c_segments = self.thisptr.get_segments()
+ *         cdef vector[CNfa] c_segments = self.thisptr.get_segments()
  *         for c_segment in c_segments:             # <<<<<<<<<<<<<<
  *             segment = mata_nfa.Nfa(c_segment.size())
  *             (<mata_nfa.Nfa>segment).thisptr.get().initial = c_segment.initial
  */
   __pyx_t_2 = __pyx_v_c_segments.begin();
   for (;;) {
     if (!(__pyx_t_2 != __pyx_v_c_segments.end())) break;
     __pyx_t_3 = *__pyx_t_2;
     ++__pyx_t_2;
     __pyx_v_c_segment = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3);
 
     /* "libmata/nfa/strings.pyx":50
- *         cdef AutSequence c_segments = self.thisptr.get_segments()
+ *         cdef vector[CNfa] c_segments = self.thisptr.get_segments()
  *         for c_segment in c_segments:
  *             segment = mata_nfa.Nfa(c_segment.size())             # <<<<<<<<<<<<<<
  *             (<mata_nfa.Nfa>segment).thisptr.get().initial = c_segment.initial
  *             (<mata_nfa.Nfa>segment).thisptr.get().final = c_segment.final
  */
     __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_c_segment.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
@@ -4029,15 +4029,15 @@
  * 
  *         return segments
  */
     __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_segments, __pyx_v_segment); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 55, __pyx_L1_error)
 
     /* "libmata/nfa/strings.pyx":49
  *         segments = []
- *         cdef AutSequence c_segments = self.thisptr.get_segments()
+ *         cdef vector[CNfa] c_segments = self.thisptr.get_segments()
  *         for c_segment in c_segments:             # <<<<<<<<<<<<<<
  *             segment = mata_nfa.Nfa(c_segment.size())
  *             (<mata_nfa.Nfa>segment).thisptr.get().initial = c_segment.initial
  */
   }
 
   /* "libmata/nfa/strings.pyx":57
@@ -4889,15 +4889,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_3nfa_7strings_4noodlify_for_equation(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_left_side_automata, struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *__pyx_v_right_side_automaton, PyObject *__pyx_v_include_empty, PyObject *__pyx_v_params) {
-  Mata::Nfa::AutPtrSequence __pyx_v_c_left_side_automata;
+  std::vector<Mata::Nfa::Nfa *>  __pyx_v_c_left_side_automata;
   PyObject *__pyx_v_lhs_aut = NULL;
   PyObject *__pyx_v_noodle_segments = NULL;
   Mata::Strings::SegNfa::NoodleSequence __pyx_v_c_noodle_segments;
   std::vector<std::shared_ptr<Mata::Nfa::Nfa> >  __pyx_v_c_noodle;
   PyObject *__pyx_v_noodle = NULL;
   std::shared_ptr<Mata::Nfa::Nfa>  __pyx_v_c_noodle_segment;
   PyObject *__pyx_v_noodle_segment = NULL;
@@ -4914,29 +4914,29 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  Mata::Nfa::StringMap __pyx_t_14;
+  Mata::Nfa::ParameterMap __pyx_t_14;
   std::vector<std::vector<std::shared_ptr<Mata::Nfa::Nfa> > > ::iterator __pyx_t_15;
   std::vector<std::shared_ptr<Mata::Nfa::Nfa> >  __pyx_t_16;
   std::vector<std::shared_ptr<Mata::Nfa::Nfa> > ::iterator __pyx_t_17;
   std::shared_ptr<Mata::Nfa::Nfa>  __pyx_t_18;
   int __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("noodlify_for_equation", 0);
   __Pyx_INCREF(__pyx_v_params);
 
   /* "libmata/nfa/strings.pyx":120
  *     """
- *     cdef AutPtrSequence c_left_side_automata
+ *     cdef vector[CNfa*] c_left_side_automata
  *     for lhs_aut in left_side_automata:             # <<<<<<<<<<<<<<
  *         c_left_side_automata.push_back((<mata_nfa.Nfa>lhs_aut).thisptr.get())
  *     noodle_segments = []
  */
   __pyx_t_1 = __pyx_v_left_side_automata; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
@@ -4946,30 +4946,30 @@
     __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_lhs_aut, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "libmata/nfa/strings.pyx":121
- *     cdef AutPtrSequence c_left_side_automata
+ *     cdef vector[CNfa*] c_left_side_automata
  *     for lhs_aut in left_side_automata:
  *         c_left_side_automata.push_back((<mata_nfa.Nfa>lhs_aut).thisptr.get())             # <<<<<<<<<<<<<<
  *     noodle_segments = []
  *     params = params or {}
  */
     try {
       __pyx_v_c_left_side_automata.push_back(((struct __pyx_obj_7libmata_3nfa_3nfa_Nfa *)__pyx_v_lhs_aut)->thisptr.get());
     } catch(...) {
       __Pyx_CppExn2PyErr();
       __PYX_ERR(1, 121, __pyx_L1_error)
     }
 
     /* "libmata/nfa/strings.pyx":120
  *     """
- *     cdef AutPtrSequence c_left_side_automata
+ *     cdef vector[CNfa*] c_left_side_automata
  *     for lhs_aut in left_side_automata:             # <<<<<<<<<<<<<<
  *         c_left_side_automata.push_back((<mata_nfa.Nfa>lhs_aut).thisptr.get())
  *     noodle_segments = []
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
@@ -5725,24 +5725,24 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 33, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 211, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 211, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(4, 219, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(4, 219, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 210, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(4, 218, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(4, 218, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `libmata-0.91.0/libmata/nfa/strings.pxd` & `libmata-0.92.0/libmata/nfa/strings.pxd`

 * *Files 22% similar despite different names*

```diff
@@ -6,31 +6,27 @@
 from libcpp.unordered_map cimport unordered_map as umap
 from libcpp.vector cimport vector
 
 from libmata.nfa.nfa cimport CNfa, CTrans
 from libmata.alphabets cimport Symbol
 
 cdef extern from "mata/nfa/nfa.hh" namespace "Mata::Nfa":
-    ctypedef vector[CTrans] TransitionSequence
-    ctypedef vector[CNfa] AutSequence
-    ctypedef vector[CNfa*] AutPtrSequence
-    ctypedef vector[const CNfa*] ConstAutPtrSequence
-    ctypedef umap[string, string] StringMap
+    ctypedef umap[string, string] ParameterMap
 
 cdef extern from "mata/nfa/strings.hh" namespace "Mata::Strings":
     cdef cset[vector[Symbol]] c_get_shortest_words "Mata::Strings::get_shortest_words" (CNfa&)
 
 cdef extern from "mata/nfa/strings.hh" namespace "Mata::Strings::SegNfa":
     cdef cppclass CSegmentation "Mata::Strings::SegNfa::Segmentation":
         CSegmentation(CNfa&, cset[Symbol]) except +
 
         ctypedef size_t EpsilonDepth
-        ctypedef umap[EpsilonDepth, TransitionSequence] EpsilonDepthTransitions
+        ctypedef umap[EpsilonDepth, vector[CTrans]] EpsilonDepthTransitions
 
         EpsilonDepthTransitions get_epsilon_depths()
-        AutSequence get_segments()
+        vector[CNfa] get_segments()
 
     ctypedef vector[vector[shared_ptr[CNfa]]] NoodleSequence
 
     cdef NoodleSequence c_noodlify "Mata::Strings::SegNfa::noodlify" (CNfa&, Symbol, bool)
-    cdef NoodleSequence c_noodlify_for_equation "Mata::Strings::SegNfa::noodlify_for_equation" (const AutPtrSequence&, CNfa&, bool, StringMap&)
-
+    cdef NoodleSequence c_noodlify_for_equation "Mata::Strings::SegNfa::noodlify_for_equation" \
+        (const vector[CNfa*]&, CNfa&, bool, ParameterMap&)
```

### Comparing `libmata-0.91.0/libmata/nfa/strings.pyx` & `libmata-0.92.0/libmata/nfa/strings.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cimport libmata.nfa.nfa as mata_nfa
 cimport libmata.nfa.strings as mata_strings
 
 from cython.operator import dereference, postincrement as postinc
 
-from libmata.nfa.strings cimport AutSequence, NoodleSequence, AutPtrSequence, CSegmentation
+from libmata.nfa.strings cimport NoodleSequence, CSegmentation
 from libmata.nfa.nfa cimport CTrans
 
 cdef class Segmentation:
     """Wrapper over Segmentation."""
 
     cdef CSegmentation* thisptr
 
@@ -41,15 +41,15 @@
     def get_segments(self):
         """Get segment automata.
 
         :return: A vector of segments for the segment automaton in the order from the left (initial state in segment
                  automaton) to the right (final states of segment automaton).
         """
         segments = []
-        cdef AutSequence c_segments = self.thisptr.get_segments()
+        cdef vector[CNfa] c_segments = self.thisptr.get_segments()
         for c_segment in c_segments:
             segment = mata_nfa.Nfa(c_segment.size())
             (<mata_nfa.Nfa>segment).thisptr.get().initial = c_segment.initial
             (<mata_nfa.Nfa>segment).thisptr.get().final = c_segment.final
             (<mata_nfa.Nfa>segment).thisptr.get().delta = c_segment.delta
 
             segments.append(segment)
@@ -112,15 +112,15 @@
     :param: mata_nfa.Nfa aut: Segment automaton representing the right side of the equation to noodlify.
     :param: bool include_empty: Whether to also include empty noodles.
     :param: dict params: Additional parameters for the noodlification:
         - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
                     minimization before noodlification.
     :return: List of automata: A list of all (non-empty) noodles.
     """
-    cdef AutPtrSequence c_left_side_automata
+    cdef vector[CNfa*] c_left_side_automata
     for lhs_aut in left_side_automata:
         c_left_side_automata.push_back((<mata_nfa.Nfa>lhs_aut).thisptr.get())
     noodle_segments = []
     params = params or {}
     cdef NoodleSequence c_noodle_segments = mata_strings.c_noodlify_for_equation(
         c_left_side_automata, dereference(right_side_automaton.thisptr.get()), include_empty,
         {
```

### Comparing `libmata-0.91.0/libmata/parser.cpp` & `libmata-0.92.0/libmata/parser.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1461,72 +1461,72 @@
  */
 struct __pyx_obj_7libmata_5utils_BinaryRelation {
   PyObject_HEAD
   Simlib::Util::BinaryRelation *thisptr;
 };
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 struct __pyx_obj_7libmata_9alphabets_Alphabet {
   PyObject_HEAD
   struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *__pyx_vtab;
 };
 
 
-/* "libmata/nfa/nfa.pxd":211
+/* "libmata/nfa/nfa.pxd":210
  * #
  * # This is needed in order for these classes to be used in other packages.
  * cdef class Nfa:             # <<<<<<<<<<<<<<
  *     # TODO: Shared pointers are not ideal as they bring some overhead which could be substantial in theory. We are not
  *     #  sure whether the shared pointers will be a problem in this case, but it would be good to pay attention to this and
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Nfa {
   PyObject_HEAD
   std::shared_ptr<Mata::Nfa::Nfa>  thisptr;
   PyObject *label;
 };
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Trans {
   PyObject_HEAD
   struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans *__pyx_vtab;
   Mata::Nfa::Trans *thisptr;
 };
 
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 
 struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet {
   Mata::Alphabet *(*as_base)(struct __pyx_obj_7libmata_9alphabets_Alphabet *);
   PyObject *(*get_symbols)(struct __pyx_obj_7libmata_9alphabets_Alphabet *);
 };
 static struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *__pyx_vtabptr_7libmata_9alphabets_Alphabet;
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 
@@ -2819,24 +2819,24 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(2, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 33, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(3, 35, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(3, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 211, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 211, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(4, 219, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(4, 219, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(4, 210, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(4, 218, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(4, 218, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `libmata-0.91.0/libmata/parser.pyx` & `libmata-0.92.0/libmata/parser.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/libmata/plotting.cpp` & `libmata-0.92.0/libmata/plotting.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1459,42 +1459,42 @@
  */
 struct __pyx_obj_7libmata_5utils_BinaryRelation {
   PyObject_HEAD
   Simlib::Util::BinaryRelation *thisptr;
 };
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 struct __pyx_obj_7libmata_9alphabets_Alphabet {
   PyObject_HEAD
   struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *__pyx_vtab;
 };
 
 
-/* "libmata/nfa/nfa.pxd":211
+/* "libmata/nfa/nfa.pxd":210
  * #
  * # This is needed in order for these classes to be used in other packages.
  * cdef class Nfa:             # <<<<<<<<<<<<<<
  *     # TODO: Shared pointers are not ideal as they bring some overhead which could be substantial in theory. We are not
  *     #  sure whether the shared pointers will be a problem in this case, but it would be good to pay attention to this and
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Nfa {
   PyObject_HEAD
   std::shared_ptr<Mata::Nfa::Nfa>  thisptr;
   PyObject *label;
 };
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 struct __pyx_obj_7libmata_3nfa_3nfa_Trans {
@@ -1515,30 +1515,30 @@
   PyObject_HEAD
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_t;
 };
 
 
 
-/* "libmata/alphabets.pxd":33
+/* "libmata/alphabets.pxd":35
  * 
  * 
  * cdef class Alphabet:             # <<<<<<<<<<<<<<
  *     cdef CAlphabet* as_base(self)
  *     cdef get_symbols(self)
  */
 
 struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet {
   Mata::Alphabet *(*as_base)(struct __pyx_obj_7libmata_9alphabets_Alphabet *);
   PyObject *(*get_symbols)(struct __pyx_obj_7libmata_9alphabets_Alphabet *);
 };
 static struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet *__pyx_vtabptr_7libmata_9alphabets_Alphabet;
 
 
-/* "libmata/nfa/nfa.pxd":219
+/* "libmata/nfa/nfa.pxd":218
  *     cdef label
  * 
  * cdef class Trans:             # <<<<<<<<<<<<<<
  *     cdef CTrans* thisptr
  *     cdef copy_from(self, CTrans trans)
  */
 
@@ -9642,24 +9642,24 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libmata.utils"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7libmata_5utils_BinaryRelation = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.utils", "BinaryRelation", sizeof(struct __pyx_obj_7libmata_5utils_BinaryRelation), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_5utils_BinaryRelation),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_5utils_BinaryRelation) __PYX_ERR(1, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 33, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.alphabets"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(2, 33, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(2, 33, __pyx_L1_error)
+  __pyx_ptype_7libmata_9alphabets_Alphabet = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.alphabets", "Alphabet", sizeof(struct __pyx_obj_7libmata_9alphabets_Alphabet), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_9alphabets_Alphabet),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_9alphabets_Alphabet) __PYX_ERR(2, 35, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_9alphabets_Alphabet = (struct __pyx_vtabstruct_7libmata_9alphabets_Alphabet*)__Pyx_GetVtable(__pyx_ptype_7libmata_9alphabets_Alphabet); if (unlikely(!__pyx_vtabptr_7libmata_9alphabets_Alphabet)) __PYX_ERR(2, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 211, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("libmata.nfa.nfa"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 211, __pyx_L1_error)
-  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(3, 219, __pyx_L1_error)
-  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(3, 219, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Nfa = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Nfa", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Nfa),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Nfa) __PYX_ERR(3, 210, __pyx_L1_error)
+  __pyx_ptype_7libmata_3nfa_3nfa_Trans = __Pyx_ImportType_3_0_0(__pyx_t_1, "libmata.nfa.nfa", "Trans", sizeof(struct __pyx_obj_7libmata_3nfa_3nfa_Trans), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_7libmata_3nfa_3nfa_Trans),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7libmata_3nfa_3nfa_Trans) __PYX_ERR(3, 218, __pyx_L1_error)
+  __pyx_vtabptr_7libmata_3nfa_3nfa_Trans = (struct __pyx_vtabstruct_7libmata_3nfa_3nfa_Trans*)__Pyx_GetVtable(__pyx_ptype_7libmata_3nfa_3nfa_Trans); if (unlikely(!__pyx_vtabptr_7libmata_3nfa_3nfa_Trans)) __PYX_ERR(3, 218, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `libmata-0.91.0/libmata/plotting.pyx` & `libmata-0.92.0/libmata/plotting.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/libmata/utils.cpp` & `libmata-0.92.0/libmata/utils.cpp`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/libmata/utils.pxd` & `libmata-0.92.0/libmata/utils.pxd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/libmata/utils.pyx` & `libmata-0.92.0/libmata/utils.pyx`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/args.hxx` & `libmata-0.92.0/mata/3rdparty/args.hxx`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/catch.hpp` & `libmata-0.92.0/mata/3rdparty/catch.hpp`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/catch.hpp.1.9.3` & `libmata-0.92.0/mata/3rdparty/catch.hpp.1.9.3`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/catch.hpp.2.0.1` & `libmata-0.92.0/mata/3rdparty/catch.hpp.2.0.1`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/catch.hpp.2.13.9` & `libmata-0.92.0/mata/3rdparty/catch.hpp.2.13.9`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/CMakeLists.txt` & `libmata-0.92.0/mata/3rdparty/cudd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/Doxyfile.in` & `libmata-0.92.0/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/LICENSE` & `libmata-0.92.0/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/README` & `libmata-0.92.0/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-0.92.0/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-0.92.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-0.92.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-0.92.0/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-0.92.0/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-0.92.0/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-0.92.0/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpDoc.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-0.92.0/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-0.92.0/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-0.92.0/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/epd/epd.c` & `libmata-0.92.0/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/epd/epd.h` & `libmata-0.92.0/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-0.92.0/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/groups.dox` & `libmata-0.92.0/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-0.92.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-0.92.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-0.92.0/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-0.92.0/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-0.92.0/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-0.92.0/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-0.92.0/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-0.92.0/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/st/st.c` & `libmata-0.92.0/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/st/st.h` & `libmata-0.92.0/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/st/testst.c` & `libmata-0.92.0/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-0.92.0/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/datalimit.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/pipefork.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/prtime.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/strsav.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/texpand.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-0.92.0/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/cudd/util/util.h` & `libmata-0.92.0/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/CMakeLists.txt` & `libmata-0.92.0/mata/3rdparty/re2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-0.92.0/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/LICENSE` & `libmata-0.92.0/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/compile.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/parse.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/pod_array.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/prog.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/prog.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/re2.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/re2.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/regexp.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/regexp.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/simplify.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/tostring.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-0.92.0/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-0.92.0/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/util/logging.h` & `libmata-0.92.0/mata/3rdparty/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/util/mutex.h` & `libmata-0.92.0/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/util/rune.cc` & `libmata-0.92.0/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/util/strutil.cc` & `libmata-0.92.0/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/util/utf.h` & `libmata-0.92.0/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/re2/util/util.h` & `libmata-0.92.0/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-0.92.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-0.92.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/CMakeLists.txt` & `libmata-0.92.0/mata/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/Doxyfile.in` & `libmata-0.92.0/mata/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/LICENSE` & `libmata-0.92.0/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/Makefile` & `libmata-0.92.0/mata/Makefile`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/README.md` & `libmata-0.92.0/mata/README.md`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/cmake/Modules/Catch.cmake` & `libmata-0.92.0/mata/cmake/Modules/Catch.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/cmake/Modules/CatchAddTests.cmake` & `libmata-0.92.0/mata/cmake/Modules/CatchAddTests.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/cmake/Modules/CodeCoverage.cmake` & `libmata-0.92.0/mata/cmake/Modules/CodeCoverage.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/cmake/Modules/FindValgrind.cmake` & `libmata-0.92.0/mata/cmake/Modules/FindValgrind.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/cmake/Modules/GetGitRevisionDescription.cmake` & `libmata-0.92.0/mata/cmake/Modules/GetGitRevisionDescription.cmake`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in` & `libmata-0.92.0/mata/cmake/Modules/GetGitRevisionDescription.cmake.in`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/afa/afa.hh` & `libmata-0.92.0/mata/include/mata/afa/afa.hh`

 * *Files 3% similar despite different names*

```diff
@@ -30,41 +30,43 @@
 
 #include "mata/alphabet.hh"
 #include "mata/nfa/nfa.hh"
 #include "mata/parser/parser.hh"
 #include "mata/utils/util.hh"
 #include "mata/utils/ord-vector.hh"
 #include "mata/utils/closed-set.hh"
+#include "mata/nfa/builder.hh"
 
 /**
  * Alternating Finite Automata including structures, transitions and algorithms.
  *
  * In particular, this includes:
  *   1. Structures (Automaton, Transitions, Results),
  *   2. Algorithms (operations, checks, tests),
  *   3. Constructions.
  */
 namespace Mata::Afa {
 extern const std::string TYPE_AFA;
 
 using State = Mata::Nfa::State;
 
+using SymbolToStringMap = std::unordered_map<Symbol, std::string>;
+
 template<typename T> using OrdVec = Mata::Util::OrdVector<T>;
 
 using Node = OrdVec<State>;
 using Nodes = OrdVec<Node>;
 
-using SymbolToStringMap = Mata::Nfa::SymbolToStringMap;
-using StateToStringMap = Mata::Nfa::StateToStringMap;
-using StringToStateMap = Mata::Nfa::StringToStateMap;
+using StateNameMap = std::unordered_map<State, std::string>;
+using NameStateMap = Nfa::Builder::NameStateMap;
 
-using Path = Util::OrdVector<State>;
-using Word = Util::OrdVector<Symbol>;
+using Path = std::vector<State>;
+using Word = std::vector<Symbol>;
 
-using StringDict = Mata::Nfa::StringMap;
+using StringDict = Mata::Nfa::ParameterMap;
 
 using StateSet = OrdVec<State>;
 using StateClosedSet = Mata::ClosedSet<Mata::Afa::State>;
 
 /*
 * A node is an ordered vector of states of the automaton.
 * A transition consists of a source state, a symbol on the transition
@@ -152,15 +154,15 @@
 
 struct Afa;
 
 /// serializes Afa into a ParsedSection
 Mata::Parser::ParsedSection serialize(
     const Afa&                aut,
     const SymbolToStringMap*  symbol_map = nullptr,
-    const StateToStringMap*   state_map = nullptr);
+    const StateNameMap*   state_map = nullptr);
 
 
 ///  An AFA
 struct Afa
 { // {{{
 private:
     TransRelation transitionrelation{};
@@ -297,15 +299,15 @@
     /// the AFA
     Afa afa;
 
     /// the alphabet
     Alphabet* alphabet;
 
     /// mapping of state names (as strings) to their numerical values
-    StringToStateMap state_dict;
+    NameStateMap state_dict;
 }; // AfaWrapper }}}
 
 /// Do the automata have disjoint sets of states?
 bool are_state_disjoint(const Afa& lhs, const Afa& rhs);
 /// Is the language of the automaton empty?
 bool is_lang_empty(const Afa& aut, Path* cex = nullptr);
 bool is_lang_empty_cex(const Afa& aut, Word* cex);
@@ -426,43 +428,40 @@
 
 /// Test for automaton completeness wrt an alphabet.  An automaton is complete
 /// if every reachable state has at least one outgoing transition over every
 /// symbol.
 bool is_complete(const Afa& aut, const Alphabet& alphabet);
 
 /** Loads an automaton from Parsed object */
-Afa construct(const Mata::Parser::ParsedSection& parsec, Alphabet* alphabet, StringToStateMap* state_map = nullptr);
+Afa construct(const Mata::Parser::ParsedSection& parsec, Alphabet* alphabet, NameStateMap* state_map = nullptr);
 /** Loads automaton from intermediate automaton */
-Afa construct(const Mata::IntermediateAut& inter_aut, Alphabet* alphabet, StringToStateMap* state_map = nullptr);
+Afa construct(const Mata::IntermediateAut& inter_aut, Alphabet* alphabet, NameStateMap* state_map = nullptr);
 
 /**
  * @brief Loads automaton from parsed object (either ParsedSection or Intermediate automaton.
  *
  * If user does not provide symbol map or state map, it allocates its own ones.
  */
 template <class ParsedObject>
-Afa construct(const ParsedObject& parsed, StringToSymbolMap* symbol_map = nullptr, StringToStateMap* state_map = nullptr) {
-    StringToSymbolMap tmp_symbol_map;
-    if (symbol_map) {
-        tmp_symbol_map = *symbol_map;
+Afa construct(const ParsedObject& parsed, Alphabet* alphabet = nullptr, NameStateMap* state_map = nullptr) {
+    Mata::OnTheFlyAlphabet tmp_alphabet{};
+    if (!alphabet) {
+        alphabet = &tmp_alphabet;
     }
-    Mata::OnTheFlyAlphabet alphabet(tmp_symbol_map);
-
-    Afa aut = construct(parsed, &alphabet, state_map);
-
-    if (symbol_map) {
-        *symbol_map = alphabet.get_symbol_map();
-    }
-    return aut;
+    return construct(parsed, alphabet, state_map);;
 }
 
 /** Loads an automaton from Parsed object */
 template <class ParsedObject> void construct(Afa* result, const ParsedObject& parsed,
-    StringToSymbolMap* symbol_map = nullptr, StringToStateMap* state_map = nullptr) {
-    *result = construct(parsed, symbol_map, state_map);
+                                             Alphabet* alphabet = nullptr, NameStateMap* state_map = nullptr) {
+    Mata::OnTheFlyAlphabet tmp_alphabet{};
+    if (!alphabet) {
+        alphabet = &tmp_alphabet;
+    }
+    *result = construct(parsed, alphabet, state_map);
 }
 
 /**
  * @brief  Obtains a word corresponding to a path in an automaton (or sets a flag)
  *
  * Returns a word that is consistent with @p path of states in automaton @p
  * aut, or sets a flag to @p false if such a word does not exist.  Note that
@@ -481,15 +480,15 @@
 /// Checks whether a string is in the language of an automaton
 bool is_in_lang(const Afa& aut, const Word& word);
 
 /// Checks whether the prefix of a string is in the language of an automaton
 bool is_prfx_in_lang(const Afa& aut, const Word& word);
 
 /** Encodes a vector of strings (each corresponding to one symbol) into a @c Word instance. */
-inline Word encode_word(const StringToSymbolMap& symbol_map, const std::vector<std::string>& input);
+inline Word encode_word(const Alphabet& alphabet, const std::vector<std::string>& input);
 
 std::ostream& operator<<(std::ostream& os, const Afa& afa);
 
 /// global constructor to be called at program startup (from vm-dispatch)
 void init();
 
 } // namespace Mata::Afa.
```

### Comparing `libmata-0.91.0/mata/include/mata/alphabet.hh` & `libmata-0.92.0/mata/include/mata/alphabet.hh`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 #include "utils/util.hh"
 #include "utils/ord-vector.hh"
 
 namespace Mata {
 
 using Symbol = unsigned;
-using StringToSymbolMap = std::unordered_map<std::string, Symbol>;
 
  /**
   * The abstract interface for NFA alphabets.
   */
 class Alphabet {
 public:
     /// translates a string into a symbol
@@ -262,28 +261,42 @@
 
 /**
  * An alphabet constructed 'on the fly'.
  * Should be use anytime the automata have a specific names for the symbols.
  */
 class OnTheFlyAlphabet : public Alphabet {
 public:
+    using StringToSymbolMap = std::unordered_map<std::string, Symbol>;
+
     /// Result of the insertion of a new symbol.
     using InsertionResult = std::pair<StringToSymbolMap::const_iterator, bool>;
 
     explicit OnTheFlyAlphabet(Symbol init_symbol = 0) : next_symbol_value(init_symbol) {};
     OnTheFlyAlphabet(const OnTheFlyAlphabet& rhs) : symbol_map(rhs.symbol_map), next_symbol_value(rhs.next_symbol_value) {}
     explicit OnTheFlyAlphabet(StringToSymbolMap str_sym_map) : symbol_map(std::move(str_sym_map)) {}
+
     /**
      * Create alphabet from a list of symbol names.
      * @param symbol_names Names for symbols on transitions.
      * @param init_symbol Start of a sequence of values to use for new symbols.
      */
     explicit OnTheFlyAlphabet(const std::vector<std::string>& symbol_names, Symbol init_symbol = 0)
             : symbol_map(), next_symbol_value(init_symbol) { add_symbols_from(symbol_names); }
 
+    template <class InputIt> OnTheFlyAlphabet(InputIt first, InputIt last) {
+        for (; first != last; ++first) {
+            add_new_symbol(*first, next_symbol_value);
+        }
+    }
+    OnTheFlyAlphabet(std::initializer_list<std::pair<std::string, Symbol>> name_symbol_map) : symbol_map{} {
+        for (auto&& [name, symbol]: name_symbol_map) {
+            add_new_symbol(name, symbol);
+        }
+    }
+
     Util::OrdVector<Symbol> get_alphabet_symbols() const override;
     Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override;
 
     std::string reverse_translate_symbol(Symbol symbol) const override;
 
 private:
     OnTheFlyAlphabet& operator=(const OnTheFlyAlphabet& rhs);
@@ -301,21 +314,14 @@
      * @brief Expand alphabet by symbols from the passed @p symbol_map.
      *
      * The value of the already existing symbols will NOT be overwritten.
      * @param[in] new_symbol_map Map of strings to symbols.
      */
     void add_symbols_from(const StringToSymbolMap& new_symbol_map);
 
-    template <class InputIt> OnTheFlyAlphabet(InputIt first, InputIt last) {
-        for (; first != last; ++first) {
-            add_new_symbol(*first, next_symbol_value);
-        }
-    }
-    OnTheFlyAlphabet(std::initializer_list<std::string> l) : OnTheFlyAlphabet(l.begin(), l.end()) {}
-
     Symbol translate_symb(const std::string& str) override;
 
     virtual std::vector<Symbol> translate_word(const std::vector<std::string>& word) const override;
 
     /**
      * @brief Add new symbol to the alphabet with the value of @c next_symbol_value.
      *
```

### Comparing `libmata-0.91.0/mata/include/mata/nfa/algorithms.hh` & `libmata-0.92.0/mata/include/mata/nfa/algorithms.hh`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
  * @param[out] cex Counterexample word which eventually breaks the universality
  * @return True if the automaton is universal, otherwise false.
  */
 bool is_universal_antichains(const Nfa& aut, const Alphabet& alphabet, Run* cex);
 
 Simlib::Util::BinaryRelation compute_relation(
         const Nfa& aut,
-        const StringMap&  params = {{"relation", "simulation"}, {"direction", "forward"}});
+        const ParameterMap&  params = {{ "relation", "simulation"}, { "direction", "forward"}});
 
 /**
  * @brief Compute intersection of two NFAs with a possibility of using multiple epsilons.
  *
  * @param[in] lhs First NFA to compute intersection for.
  * @param[in] rhs Second NFA to compute intersection for.
  * @param[in] preserve_epsilon Whether to compute intersection preserving epsilon transitions.
@@ -119,17 +119,17 @@
  * @brief Concatenate two NFAs.
  *
  * Supports epsilon symbols when @p use_epsilon is set to true.
  * @param[in] lhs First automaton to concatenate.
  * @param[in] rhs Second automaton to concatenate.
  * @param[in] epsilon Epsilon to be used co concatenation (provided @p use_epsilon is true)
  * @param[in] use_epsilon Whether to concatenate over epsilon symbol.
- * @param[out] lhs_result_states_map Map mapping lhs states to result states.
- * @param[out] rhs_result_states_map Map mapping rhs states to result states.
+ * @param[out] lhs_state_renaming Map mapping lhs states to result states.
+ * @param[out] rhs_state_renaming Map mapping rhs states to result states.
  * @return Concatenated automaton.
  */
 Nfa concatenate_eps(const Nfa& lhs, const Nfa& rhs, const Symbol& epsilon, bool use_epsilon = false,
-    StateToStateMap* lhs_result_states_map = nullptr, StateToStateMap* rhs_result_states_map = nullptr);
+                    StateRenaming* lhs_state_renaming = nullptr, StateRenaming* rhs_state_renaming = nullptr);
 
 } // Namespace Mata::Nfa::Algorithms.
 
 #endif // MATA_NFA_INTERNALS_HH_
```

### Comparing `libmata-0.91.0/mata/include/mata/nfa/builder.hh` & `libmata-0.92.0/mata/include/mata/nfa/builder.hh`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 #ifndef LIBMATA_BUILDER_HH
 #define LIBMATA_BUILDER_HH
 
 #include "nfa.hh"
 
 #include <filesystem>
 
-using namespace Mata::Nfa;
 
 /**
  * Namespace providing options to build NFAs.
  */
 namespace Mata::Nfa::Builder {
 
+using namespace Mata::Nfa;
+
+using NameStateMap = std::unordered_map<std::string, State>;
+
 /**
  * Create an automaton accepting only a single @p word.
  */
 Nfa create_single_word_nfa(const std::vector<Symbol>& word);
 
 /**
  * Create an automaton accepting only a single @p word.
@@ -40,34 +43,27 @@
  * @param[in] alphabet Alphabet to construct sigma star automaton with. When alphabet is left empty, the default empty
  *  alphabet is used, creating an automaton accepting only the empty string.
  */
 Nfa create_sigma_star_nfa(Alphabet* alphabet = new OnTheFlyAlphabet{});
 
 /** Loads an automaton from Parsed object */
 // TODO this function should the same thing as the one taking IntermediateAut or be deleted
-Nfa construct(const Mata::Parser::ParsedSection& parsec, Alphabet* alphabet, StringToStateMap* state_map = nullptr);
+Nfa construct(const Mata::Parser::ParsedSection& parsec, Alphabet* alphabet, NameStateMap* state_map = nullptr);
 
 /** Loads an automaton from Parsed object */
-Nfa construct(const Mata::IntermediateAut& inter_aut, Alphabet* alphabet, StringToStateMap* state_map = nullptr);
+Nfa construct(const Mata::IntermediateAut& inter_aut, Alphabet* alphabet, NameStateMap* state_map = nullptr);
 
 template<class ParsedObject>
-Nfa construct(const ParsedObject& parsed, Mata::StringToSymbolMap* symbol_map = nullptr,
-              StringToStateMap* state_map = nullptr) {
-    Mata::StringToSymbolMap tmp_symbol_map;
-    if (symbol_map) {
-        tmp_symbol_map = *symbol_map;
-    }
-    Mata::OnTheFlyAlphabet alphabet(tmp_symbol_map);
-
-    Nfa aut = construct(parsed, &alphabet, state_map);
-
-    if (symbol_map) {
-        *symbol_map = alphabet.get_symbol_map();
+Nfa construct(const ParsedObject& parsed, Alphabet* alphabet = nullptr,
+              NameStateMap* state_map = nullptr) {
+    OnTheFlyAlphabet tmp_alphabet{};
+    if (!alphabet) {
+        alphabet = &tmp_alphabet;
     }
-    return aut;
+    return construct(parsed, alphabet, state_map);
 } // construct().
 
 /**
  * Parse NFA from the mata format in an input stream.
  *
  * @param nfa_stream Input stream containing NFA in mata format.
  * @throws std::runtime_error Parsing of NFA fails.
```

### Comparing `libmata-0.91.0/mata/include/mata/nfa/delta.hh` & `libmata-0.92.0/mata/include/mata/nfa/delta.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/nfa/nfa.hh` & `libmata-0.92.0/mata/include/mata/nfa/nfa.hh`

 * *Files 5% similar despite different names*

```diff
@@ -214,32 +214,32 @@
     /**
      * @brief Remove inaccessible (unreachable) and not co-accessible (non-terminating) states.
      *
      * Remove states which are not accessible (unreachable; state is accessible when the state is the endpoint of a path
      * starting from an initial state) or not co-accessible (non-terminating; state is co-accessible when the state is
      * the starting point of a path ending in a final state).
      *
-     * @param[out] state_map Mapping of trimmed states to new states.
+     * @param[out] state_renaming Mapping of trimmed states to new states.
      * TODO: we can probably keep just trim_reverting, much faster. But the speed difference and how it is achieved is interesting. Keeping as a demonstration for now.
      */
-    void trim_inplace(StateToStateMap* state_map = nullptr);
-    void trim_reverting(StateToStateMap* state_map = nullptr);
-    void trim(StateToStateMap* state_map = nullptr) { trim_inplace(state_map); }
+    void trim_inplace(StateRenaming* state_renaming = nullptr);
+    void trim_reverting(StateRenaming* state_renaming = nullptr);
+    void trim(StateRenaming* state_renaming = nullptr) { trim_inplace(state_renaming); }
 
     /**
      * @brief Remove inaccessible (unreachable) and not co-accessible (non-terminating) states.
      *
      * Remove states which are not accessible (unreachable; state is accessible when the state is the endpoint of a path
      * starting from an initial state) or not co-accessible (non-terminating; state is co-accessible when the state is
      * the starting point of a path ending in a final state).
      *
-     * @param[out] state_map Mapping of trimmed states to new states.
+     * @param[out] state_renaming Mapping of trimmed states to new states.
      * @return Trimmed automaton.
      */
-    Nfa get_trimmed_automaton(StateToStateMap* state_map = nullptr) const;
+    Nfa get_trimmed_automaton(StateRenaming* state_renaming = nullptr) const;
 
     /**
      * Remove epsilon transitions from the automaton.
      */
     void remove_epsilon(Symbol epsilon = EPSILON);
 
     /**
@@ -254,43 +254,48 @@
      */
     size_t get_num_of_trans() const { return static_cast<size_t>(std::distance(delta.begin(), delta.end())); }
 
     /**
      * Get transitions as a sequence of @c Trans.
      * @return Sequence of transitions as @c Trans.
      */
-    TransSequence get_trans_as_sequence() const;
+    std::vector<Trans> get_trans_as_sequence() const;
 
     /**
      * Get transitions from @p state_from as a sequence of @c Trans.
      * @param state_from[in] Source state_from of transitions to get.
      * @return Sequence of transitions as @c Trans from @p state_from.
      */
-    TransSequence get_trans_from_as_sequence(State state_from) const;
+    std::vector<Trans> get_trans_from_as_sequence(State state_from) const;
 
     /**
      * Get transitions leading from @p state_from.
      *
      * If we try to access a state which is present in the delta as a target state, yet does not have allocated space
      *  for itself in @c post, @c post is resized to include @p state_from.
      * @param state_from[in] Source state for transitions to get.
      * @return List of transitions leading from @p state_from.
      */
     const Post& get_moves_from(const State state_from) const {
-        assert(state_from < size());
+        const size_t post_size{ size() };
+        if (state_from >= post_size) {
+            throw std::runtime_error(
+                    "Cannot get moves from nonexistent state '" + std::to_string(state_from)
+                    + "' for Post of size '" + std::to_string(post_size) + "'.");
+        }
         return delta[state_from];
     }
 
     /**
      * Get transitions leading to @p state_to.
      * @param state_to[in] Target state for transitions to get.
      * @return Sequence of @c Trans transitions leading to @p state_to.
      * (!slow!, traverses the entire delta)
      */
-    TransSequence get_transitions_to(State state_to) const;
+    std::vector<Trans> get_transitions_to(State state_to) const;
 
     /**
      * Unify transitions to create a directed graph with at most a single transition between two states.
      * @param[in] abstract_symbol Abstract symbol to use for transitions in digraph.
      * @return An automaton representing a directed graph.
      */
     Nfa get_one_letter_aut(Symbol abstract_symbol = 'x') const;
@@ -430,39 +435,36 @@
 }
 
 /**
  * Create alphabet from a vector of NFAs.
  * @param[in] nfas Vector of NFAs to create alphabet from.
  * @return Created alphabet.
  */
-OnTheFlyAlphabet create_alphabet(const ConstAutRefSequence& nfas);
+OnTheFlyAlphabet create_alphabet(const std::vector<std::reference_wrapper<const Nfa>>& nfas);
 
 /**
  * Create alphabet from a vector of NFAs.
  * @param[in] nfas Vector of NFAs to create alphabet from.
  * @return Created alphabet.
  */
-OnTheFlyAlphabet create_alphabet(const AutRefSequence& nfas);
+OnTheFlyAlphabet create_alphabet(const std::vector<std::reference_wrapper<Nfa>>& nfas);
 
 /**
  * Create alphabet from a vector of NFAs.
  * @param[in] nfas Vector of pointers to NFAs to create alphabet from.
  * @return Created alphabet.
  */
-OnTheFlyAlphabet create_alphabet(const ConstAutPtrSequence& nfas);
+OnTheFlyAlphabet create_alphabet(const std::vector<Nfa*>& nfas);
 
 /**
  * Create alphabet from a vector of NFAs.
  * @param[in] nfas Vector of pointers to NFAs to create alphabet from.
  * @return Created alphabet.
  */
-OnTheFlyAlphabet create_alphabet(const AutPtrSequence& nfas);
-
-/// Do the automata have disjoint sets of states?
-bool are_state_disjoint(const Nfa& lhs, const Nfa& rhs);
+OnTheFlyAlphabet create_alphabet(const std::vector<const Nfa*>& nfas);
 
 /**
  * Check whether is the language of the automaton empty.
  * @param[in] aut Automaton to check.
  * @param[out] cex Counter-example path for a case the language is not empty.
  * @return True if the language is empty, false otherwise.
  */
@@ -494,21 +496,21 @@
 /**
  * @brief Concatenate two NFAs.
  *
  * Supports epsilon symbols when @p use_epsilon is set to true.
  * @param[in] lhs First automaton to concatenate.
  * @param[in] rhs Second automaton to concatenate.
  * @param[in] use_epsilon Whether to concatenate over epsilon symbol.
- * @param[out] lhs_result_states_map Map mapping lhs states to result states.
- * @param[out] rhs_result_states_map Map mapping rhs states to result states.
+ * @param[out] lhs_state_renaming Map mapping lhs states to result states.
+ * @param[out] rhs_state_renaming Map mapping rhs states to result states.
  * @return Concatenated automaton.
  */
 // TODO: check how fast is using just concatenate over epsilon and then call remove_epsilon().
 Nfa concatenate(const Nfa& lhs, const Nfa& rhs, bool use_epsilon = false,
-                StateToStateMap* lhs_result_states_map = nullptr, StateToStateMap* rhs_result_states_map = nullptr);
+                StateRenaming* lhs_state_renaming = nullptr, StateRenaming* rhs_state_renaming = nullptr);
 
 /**
  * Make @c aut complete in place.
  *
  * For each state 0,...,aut.size()-1, add transitions with "missing" symbols from @p alphabet (symbols that do not occur
  *  on transitions from given state) to @p sink_state. If @p sink_state does not belong to the automaton, it is added to
  *  it, but only in the case that some transition to @p sink_state was added.
@@ -558,15 +560,15 @@
  * @param[in] alphabet Alphabet used for complementation.
  * @param[in] params Optional parameters to control the complementation algorithm:
  * - "algorithm": "classical" (classical algorithm determinizes the automaton, makes it complete and swaps final and non-final states);
  * - "minimize": "true"/"false" (whether to compute minimal deterministic automaton for classical algorithm);
  * @return Complemented automaton.
  */
 Nfa complement(const Nfa& aut, const Alphabet& alphabet,
-   const StringMap& params = {{"algorithm", "classical"}, {"minimize", "false"}});
+               const ParameterMap& params = {{ "algorithm", "classical" }, { "minimize", "false" }});
 
 /**
  * @brief Compute automaton accepting complement of @p aut.
  *
  * This overloaded version complements over an already created ordered set of @p symbols instead of an alphabet.
  * This is a more efficient solution in case you already have @p symbols precomputed or want to complement multiple
  *  automata over the same set of @c symbols: the function does not need to compute the ordered set of symbols from
@@ -576,110 +578,97 @@
  * @param[in] symbols Symbols to complement over.
  * @param[in] params Optional parameters to control the complementation algorithm:
  * - "algorithm": "classical" (classical algorithm determinizes the automaton, makes it complete and swaps final and non-final states);
  * - "minimize": "true"/"false" (whether to compute minimal deterministic automaton for classical algorithm);
  * @return Complemented automaton.
  */
 Nfa complement(const Nfa& aut, const Util::OrdVector<Symbol>& symbols,
-   const StringMap& params = {{"algorithm", "classical"}, {"minimize", "false"}});
+               const ParameterMap& params = {{ "algorithm", "classical" }, { "minimize", "false" }});
 
 /**
  * @brief Compute minimal deterministic automaton.
  *
  * @param[in] aut Automaton whose minimal version to compute.
  * @param[in] params Optional parameters to control the minimization algorithm:
  * - "algorithm": "brzozowski"
  * @return Minimal deterministic automaton.
  */
-Nfa minimize(const Nfa &aut, const StringMap& params = {{"algorithm", "brzozowski"}});
+Nfa minimize(const Nfa &aut, const ParameterMap& params = {{ "algorithm", "brzozowski" }});
 
 /**
  * @brief Determinize automaton.
  *
  * @param[in] aut Automaton to determinize.
  * @param[out] subset_map Map that maps sets of states of input automaton to states of determinized automaton.
  * @return Determinized automaton.
  */
-Nfa determinize(const Nfa&  aut, std::unordered_map<StateSet, State> *subset_map = nullptr);
+Nfa determinize(const Nfa& aut, std::unordered_map<StateSet, State> *subset_map = nullptr);
 
 /**
  * Reduce the size of the automaton.
  *
  * @param[in] aut Automaton to reduce.
  * @param[in] trim_input Whether to trim the input automaton first or not.
- * @param[out] state_map Mapping of trimmed states to new states.
+ * @param[out] state_renaming Mapping of trimmed states to new states.
  * @param[in] params Optional parameters to control the reduction algorithm:
  * - "algorithm": "simulation".
  * @return Reduced automaton.
  */
-Nfa reduce(const Nfa &aut, bool trim_input = true, StateToStateMap *state_map = nullptr,
-    const StringMap&  params = {{"algorithm", "simulation"}});
+Nfa reduce(const Nfa &aut, bool trim_input = true, StateRenaming *state_renaming = nullptr,
+           const ParameterMap& params = {{ "algorithm", "simulation" } });
 
 /// Is the language of the automaton universal?
-bool is_universal(
-        const Nfa&         aut,
-        const Alphabet&    alphabet,
-        Run*              cex = nullptr,
-        const StringMap&  params = {{"algorithm", "antichains"}});
-
-inline bool is_universal(
-        const Nfa&         aut,
-        const Alphabet&    alphabet,
-        const StringMap&  params) {
+bool is_universal(const Nfa& aut, const Alphabet& alphabet, Run* cex = nullptr,
+                  const ParameterMap& params = {{ "algorithm", "antichains" }});
+
+inline bool is_universal(const Nfa& aut, const Alphabet& alphabet, const ParameterMap& params) {
     return is_universal(aut, alphabet, nullptr, params);
 }
 
 /**
  * @brief Checks inclusion of languages of two NFAs: @p smaller and @p bigger (smaller <= bigger).
  *
  * @param[in] smaller First automaton to concatenate.
  * @param[in] bigger Second automaton to concatenate.
  * @param[out] cex Counterexample for the inclusion.
  * @param[in] alphabet Alphabet of both NFAs to compute with.
  * @param[in] params Optional parameters to control the equivalence check algorithm:
  * - "algorithm": "naive", "antichains" (Default: "antichains")
  * @return True if @p smaller is included in @p bigger, false otherwise.
  */
-bool is_included(
-        const Nfa&         smaller,
-        const Nfa&         bigger,
-        Run*               cex,
-        const Alphabet*    alphabet = nullptr,
-        const StringMap&   params = {{"algorithm", "antichains"}});
+bool is_included(const Nfa& smaller, const Nfa& bigger, Run* cex, const Alphabet* alphabet = nullptr,
+                 const ParameterMap& params = {{ "algorithm", "antichains" }});
 
 /**
  * @brief Checks inclusion of languages of two NFAs: @p smaller and @p bigger (smaller <= bigger).
  *
  * @param[in] smaller First automaton to concatenate.
  * @param[in] bigger Second automaton to concatenate.
  * @param[in] alphabet Alphabet of both NFAs to compute with.
  * @param[in] params Optional parameters to control the equivalence check algorithm:
  * - "algorithm": "naive", "antichains" (Default: "antichains")
  * @return True if @p smaller is included in @p bigger, false otherwise.
  */
-inline bool is_included(
-        const Nfa&             smaller,
-        const Nfa&             bigger,
-        const Alphabet* const  alphabet = nullptr,
-        const StringMap&      params = {{"algorithm", "antichains"}}) {
+inline bool is_included(const Nfa& smaller, const Nfa& bigger, const Alphabet* const alphabet = nullptr,
+                        const ParameterMap& params = {{ "algorithm", "antichains" }}) {
     return is_included(smaller, bigger, nullptr, alphabet, params);
 }
 
 /**
  * @brief Perform equivalence check of two NFAs: @p lhs and @p rhs.
  *
  * @param[in] lhs First automaton to concatenate.
  * @param[in] rhs Second automaton to concatenate.
  * @param[in] alphabet Alphabet of both NFAs to compute with.
  * @param[in] params[ Optional parameters to control the equivalence check algorithm:
  * - "algorithm": "naive", "antichains" (Default: "antichains")
  * @return True if @p lhs and @p rhs are equivalent, false otherwise.
  */
 bool are_equivalent(const Nfa& lhs, const Nfa& rhs, const Alphabet* alphabet,
-                    const StringMap& params = {{"algorithm", "antichains"}});
+                    const ParameterMap& params = {{ "algorithm", "antichains"}});
 
 /**
  * @brief Perform equivalence check of two NFAs: @p lhs and @p rhs.
  *
  * The current implementation of 'Mata::Nfa::Nfa' does not accept input alphabet. For this reason, an alphabet
  * has to be created from all transitions each time an operation on alphabet is called. When calling this function,
  * the alphabet has to be computed first.
@@ -690,15 +679,15 @@
  *
  * @param[in] lhs First automaton to concatenate.
  * @param[in] rhs Second automaton to concatenate.
  * @param[in] params Optional parameters to control the equivalence check algorithm:
  * - "algorithm": "naive", "antichains" (Default: "antichains")
  * @return True if @p lhs and @p rhs are equivalent, false otherwise.
  */
-bool are_equivalent(const Nfa& lhs, const Nfa& rhs, const StringMap& params = {{"algorithm", "antichains"}});
+bool are_equivalent(const Nfa& lhs, const Nfa& rhs, const ParameterMap& params = {{ "algorithm", "antichains"}});
 
 // Reverting the automaton by one of the three functions below,
 // currently simple_revert seems best (however, not tested enough).
 Nfa revert(const Nfa& aut);
 
 // This revert algorithm is fragile, uses low level accesses to Nfa and static data structures,
 // and it is potentially dangerous when there are used symbols with large numbers (allocates an array indexed by symbols)
@@ -738,15 +727,15 @@
 
 /** Encodes a vector of strings (each corresponding to one symbol) into a
  *  @c Word instance
  */
  // TODO: rename to something, but no idea to what.
  // Maybe we need some terminology - Symbols and Words are made of numbers.
  // What are the symbol names and their sequences?
-Run encode_word(const StringToSymbolMap& symbol_map, const std::vector<std::string>& input);
+Run encode_word(const Alphabet* alphabet, const std::vector<std::string>& input);
 
 } // namespace Mata::Nfa.
 
 namespace std {
 template <>
 struct hash<Mata::Nfa::Trans> {
 	inline size_t operator()(const Mata::Nfa::Trans& trans) const {
```

### Comparing `libmata-0.91.0/mata/include/mata/nfa/plumbing.hh` & `libmata-0.92.0/mata/include/mata/nfa/plumbing.hh`

 * *Files 9% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 
 #ifndef MATA_NFA_PLUMBING_HH_
 #define MATA_NFA_PLUMBING_HH_
 
 #include "nfa.hh"
 #include "builder.hh"
 
+using namespace Mata::Nfa::Builder;
+
 /**
  * Simplified NFA API, used in binding to call NFA algorithms.
  *
  * In particular, this mostly includes operations and checks, that do not return Automaton,
  * but instead take resulting automaton as pointer (e.g. `void f(Nfa* result, const Nfa& lhs, const Nfa& rhs)`).
  */
 namespace Mata::Nfa::Plumbing {
 
-void get_elements(StateSet* element_set, const BoolVector& bool_vec) {
+inline void get_elements(StateSet* element_set, const BoolVector& bool_vec) {
     element_set->clear();
     element_set->reserve(bool_vec.count());
     for (size_t i{ 0 }; i < bool_vec.size(); ++i) {
         if (bool_vec[i] == 1) {
             element_set->push_back(i);
         }
     }
@@ -40,39 +42,40 @@
 /// Make the transition relation complete.
 inline void make_complete(Nfa* aut, const Alphabet& alphabet, State sink_state) { make_complete(*aut, alphabet, sink_state); }
 
 inline void complement(
         Nfa*               result,
         const Nfa&         aut,
         const Alphabet&    alphabet,
-        const StringMap&  params = {{"algorithm", "classical"},
-                                    {"minimize", "false"}}) { *result = complement(aut, alphabet, params);
+        const ParameterMap&  params = {{ "algorithm", "classical"},
+                                       { "minimize",  "false"}}) { *result = complement(aut, alphabet, params);
 }
 
 inline void minimize(Nfa* res, const Nfa &aut) { *res = minimize(aut); }
 
 inline void determinize(Nfa* result, const Nfa& aut, std::unordered_map<StateSet, State> *subset_map = nullptr) {
     *result = determinize(aut, subset_map);
 }
 
-inline void reduce(Nfa* result, const Nfa &aut, bool trim_result = true, StateToStateMap *state_map = nullptr,
-    const StringMap&  params = {{"algorithm", "simulation"}}) { *result = reduce(aut, trim_result, state_map, params); }
+inline void reduce(Nfa* result, const Nfa &aut, bool trim_result = true, StateRenaming *state_renaming = nullptr,
+                   const ParameterMap& params = {{ "algorithm", "simulation"}}) {
+    *result = reduce(aut, trim_result, state_renaming, params);
+}
 
 inline void revert(Nfa* result, const Nfa& aut) { *result = revert(aut); }
 
 inline void remove_epsilon(Nfa* result, const Nfa& aut, Symbol epsilon = EPSILON) { *result = remove_epsilon(aut, epsilon); }
 
 /** Loads an automaton from Parsed object */
 template <class ParsedObject>
-void construct(
-        Nfa*                                 result,
-        const ParsedObject&                  parsed,
-        StringToSymbolMap*                   symbol_map = nullptr,
-        StringToStateMap*                    state_map = nullptr) {
-    *result = Builder::construct(parsed, symbol_map, state_map);
+void construct(Nfa* result, const ParsedObject& parsed, Alphabet* alphabet = nullptr,
+               NameStateMap* state_map = nullptr) {
+    OnTheFlyAlphabet tmp_alphabet{};
+    if (!alphabet) { alphabet = &tmp_alphabet; }
+    *result = Builder::construct(parsed, alphabet, state_map);
 }
 
 inline void uni(Nfa *unionAutomaton, const Nfa &lhs, const Nfa &rhs) { *unionAutomaton = uni(lhs, rhs); }
 
 /**
  * @brief Compute intersection of two NFAs.
  *
@@ -81,26 +84,26 @@
  *  contain ε-transitions. The product preserves the ε-transitions
  *  of both automata. This means that for each ε-transition of the form `s -ε-> p` and each product state `(s, a)`,
  *  an ε-transition `(s, a) -ε-> (p, a)` is created. Furthermore, for each ε-transition `s -ε-> p` and `a -ε-> b`,
  *  a product state `(s, a) -ε-> (p, b)` is created.
  *
  * Automata must share alphabets.
  */
-void intersection(Nfa* res, const Nfa& lhs, const Nfa& rhs,
+inline void intersection(Nfa* res, const Nfa& lhs, const Nfa& rhs,
                   bool preserve_epsilon = false,
                   std::unordered_map<std::pair<State, State>, State> *prod_map = nullptr) {
     *res = intersection(lhs, rhs, preserve_epsilon, prod_map);
 }
 
 /**
  * @brief Concatenate two NFAs.
- * @param[out] lhs_result_states_map Map mapping lhs states to result states.
- * @param[out] rhs_result_states_map Map mapping rhs states to result states.
+ * @param[out] lhs_result_state_renaming Map mapping lhs states to result states.
+ * @param[out] rhs_result_state_renaming Map mapping rhs states to result states.
  */
-void concatenate(Nfa* res, const Nfa& lhs, const Nfa& rhs, bool use_epsilon = false,
-                 StateToStateMap* lhs_result_states_map = nullptr, StateToStateMap* rhs_result_states_map = nullptr) {
-    *res = concatenate(lhs, rhs, use_epsilon, lhs_result_states_map, rhs_result_states_map);
+inline void concatenate(Nfa* res, const Nfa& lhs, const Nfa& rhs, bool use_epsilon = false,
+                 StateRenaming* lhs_result_state_renaming = nullptr, StateRenaming* rhs_result_state_renaming = nullptr) {
+    *res = concatenate(lhs, rhs, use_epsilon, lhs_result_state_renaming, rhs_result_state_renaming);
 }
 
 } // namespace Mata::Nfa::Plumbing.
 
 #endif // MATA_NFA_PLUMBING_HH_
```

### Comparing `libmata-0.91.0/mata/include/mata/nfa/strings.hh` & `libmata-0.92.0/mata/include/mata/nfa/strings.hh`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,14 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #ifndef MATA_NFA_STRING_SOLVING_HH_
 #define MATA_NFA_STRING_SOLVING_HH_
 
-#include <memory>
-#include <optional>
-
 #include "nfa.hh"
 
 namespace {
     using namespace Mata::Nfa;
 }
 
 /**
@@ -35,15 +32,15 @@
  */
 class ShortestWordsMap {
 public:
     /**
      * Maps states in the automaton @p aut to shortest words accepted by languages of the states.
      * @param aut Automaton to compute shortest words for.
      */
-    explicit ShortestWordsMap(const Nfa::Nfa& aut) : reversed_automaton(revert(aut)) {
+    explicit ShortestWordsMap(const Mata::Nfa::Nfa& aut) : reversed_automaton(revert(aut)) {
         insert_initial_lengths();
         compute();
     }
 
     /**
      * Gets shortest words for the given @p states.
      * @param[in] states States to map shortest words for.
@@ -62,15 +59,15 @@
     using WordLength = int; ///< A length of a word.
     /// Pair binding the length of all words in the word set and word set with words of the given length.
     using LengthWordsPair = std::pair<WordLength, WordSet>;
     /// Map mapping states to the shortest words accepted by the automaton from the mapped state.
     std::unordered_map<State, LengthWordsPair> shortest_words_map{};
     std::set<State> processed{}; ///< Set of already processed states.
     std::deque<State> fifo_queue{}; ///< FIFO queue for states to process.
-    const Nfa::Nfa reversed_automaton; ///< Reversed input automaton.
+    const Mata::Nfa::Nfa reversed_automaton; ///< Reversed input automaton.
 
     /**
      * @brief Inserts initial lengths into the shortest words map.
      *
      * Inserts initial length of length 0 for final state in the automaton (initial states in the reversed automaton).
      */
     void insert_initial_lengths();
@@ -104,61 +101,61 @@
     static void update_current_words(LengthWordsPair& act, const LengthWordsPair& dst, Symbol symbol);
 }; // Class ShortestWordsMap.
 
 /**
  * Get shortest words (regarding their length) of the automaton using BFS.
  * @return Set of shortest words.
  */
-WordSet get_shortest_words(const Nfa::Nfa& nfa);
+WordSet get_shortest_words(const Mata::Nfa::Nfa& nfa);
 
 /**
  * @brief Get the lengths of all words in the automaton @p aut. The function returns a set of pairs <u,v> where for each
  * such a pair there is a word with length u+k*v for all ks. The disjunction of such formulae of all pairs hence precisely
  * describe lengths of all words in the automaton.
  *
  * @param aut Input automaton
  * @return Set of pairs describing lengths
  */
-std::set<std::pair<int, int>> get_word_lengths(const Nfa::Nfa& aut);
+std::set<std::pair<int, int>> get_word_lengths(const Mata::Nfa::Nfa& aut);
 
 /**
  * @brief Checks if the automaton @p nfa accepts only a single word \eps.
  *
  * @param nfa Input automaton
  * @return true iff L(nfa) = {\eps}
  */
-bool is_lang_eps(const Nfa::Nfa& nfa);
+bool is_lang_eps(const Mata::Nfa::Nfa& nfa);
 
 /**
  * Segment Automata including structs and algorithms.
  *
  * These are automata whose state space can be split into several segments connected by ε-transitions in a chain.
  * No other ε-transitions are allowed. As a consequence, no ε-transitions can appear in a cycle.
  * Segment automaton can have initial states only in the first segment and final states only in the last segment.
  */
 namespace SegNfa {
 
-using SegNfa = Nfa::Nfa;
+using SegNfa = Mata::Nfa::Nfa;
 using VisitedEpsMap = std::map<State, std::map<Symbol, unsigned>>;
 
-/// Number of visited epsilons
-using EpsCntMap = std::map<Symbol, unsigned>;
-/// Projection of EpsCntMap to sorted keys (desc)
-using EpsCntVector = std::vector<unsigned>;
+/// Number of visited epsilons.
+using VisitedEpsilonsCounterMap = std::map<Symbol, unsigned>;
+/// Projection of VisitedEpsilonsNumberMap to sorted keys (in descending order).
+using VisitedEpsilonsCounterVector = std::vector<unsigned>;
 
 /**
 * Class executing segmentation operations for a given segment automaton. Works only with segment automata.
 */
 class Segmentation {
 public:
     using EpsilonDepth = size_t; ///< Depth of ε-transitions.
     /// Dictionary of lists of ε-transitions grouped by their depth.
     /// For each depth 'i' we have 'depths[i]' which contains a list of ε-transitions of depth 'i'.
-    using EpsilonDepthTransitions = std::unordered_map<EpsilonDepth, TransSequence>;
-    using EpsilonDepthTransitionMap = std::unordered_map<EpsilonDepth, std::unordered_map<State,TransSequence>>;
+    using EpsilonDepthTransitions = std::unordered_map<EpsilonDepth, std::vector<Trans>>;
+    using EpsilonDepthTransitionMap = std::unordered_map<EpsilonDepth, std::unordered_map<State, std::vector<Trans>>>;
 
     /**
      * Prepare automaton @p aut for segmentation.
      * @param[in] aut Segment automaton to make segments for.
      * @param[in] epsilon Symbol to execute segmentation for.
      */
     explicit Segmentation(const SegNfa& aut, const std::set<Symbol>& epsilons) : epsilons(epsilons), automaton(aut) {
@@ -179,42 +176,42 @@
     const EpsilonDepthTransitionMap& get_epsilon_depth_trans_map() const { return this->eps_depth_trans_map; }
 
     /**
      * Get segment automata.
      * @return A vector of segments for the segment automaton in the order from the left (initial state in segment automaton)
      * to the right (final states of segment automaton).
      */
-    const AutSequence& get_segments();
+    const std::vector<Mata::Nfa::Nfa>& get_segments();
 
     /**
      * Get raw segment automata.
      * @return A vector of segments for the segment automaton in the order from the left (initial state in segment automaton)
      * to the right (final states of segment automaton) without trimming (the states are same as in the original automaton).
      */
-    const AutSequence& get_untrimmed_segments();
+    const std::vector<Mata::Nfa::Nfa>& get_untrimmed_segments();
 
     const VisitedEpsMap& get_visited_eps() const { return this->visited_eps; }
 
 private:
     const std::set<Symbol> epsilons; ///< Symbol for which to execute segmentation.
     /// Automaton to execute segmentation for. Must be a segment automaton (can be split into @p segments).
     const SegNfa& automaton;
     EpsilonDepthTransitions epsilon_depth_transitions{}; ///< Epsilon depths.
     EpsilonDepthTransitionMap eps_depth_trans_map{}; /// Epsilon depths with mapping of states to epsilon transitions
-    AutSequence segments{}; ///< Segments for @p automaton.
-    AutSequence segments_raw{}; ///< Raw segments for @p automaton.
+    std::vector<Mata::Nfa::Nfa> segments{}; ///< Segments for @p automaton.
+    std::vector<Mata::Nfa::Nfa> segments_raw{}; ///< Raw segments for @p automaton.
     VisitedEpsMap visited_eps{}; /// number of visited eps for each state
 
     /**
      * Pair of state and its depth.
      */
     struct StateDepthTuple {
         State state; ///< State with a depth.
         EpsilonDepth depth; ///< Depth of a state.
-        EpsCntMap eps; /// visited epsilons and their numbers
+        VisitedEpsilonsCounterMap eps; /// visited epsilons and their numbers
     };
 
     /**
      * Compute epsilon depths with their transitions.
      */
     void compute_epsilon_depths();
 
@@ -281,34 +278,34 @@
      *  last one.
      */
     void remove_inner_initial_and_final_states();
 }; // Class Segmentation.
 
 /// A noodle is represented as a sequence of segments (a copy of the segment automata) created as if there was exactly
 ///  one ε-transition between each two consecutive segments.
-using Noodle = std::vector<SharedPtrAut>;
+using Noodle = std::vector<std::shared_ptr<Mata::Nfa::Nfa>>;
 using NoodleSequence = std::vector<Noodle>; ///< A sequence of noodles.
 
 /// Noodles as segments enriched with EpsCntMap
-using NoodleSubst = std::vector<std::pair<SharedPtrAut, EpsCntVector>>;
+using NoodleSubst = std::vector<std::pair<std::shared_ptr<Mata::Nfa::Nfa>, VisitedEpsilonsCounterVector>>;
 using NoodleSubstSequence = std::vector<NoodleSubst>;
 
 /**
  * @brief segs_one_initial_final
  *
  * segments_one_initial_final[init, final] is the pointer to automaton created from one of
  * the segments such that init and final are one of the initial and final states of the segment
  * and the created automaton takes this segment, sets initial={init}, final={final}
  * and trims it; also segments_one_initial_final[unused_state, final] is used for the first
  * segment (where we always want all initial states, only final state changes) and
  * segments_one_initial_final[init, unused_state] is similarly for the last segment
  * TODO: should we use unordered_map? then we need hash
  */
-void segs_one_initial_final(const Mata::Nfa::AutSequence& segments, bool include_empty,
-    const State& unused_state, std::map<std::pair<State, State>, std::shared_ptr<Nfa::Nfa>>& out);
+void segs_one_initial_final(const std::vector<Mata::Nfa::Nfa>& segments, bool include_empty,
+    const State& unused_state, std::map<std::pair<State, State>, std::shared_ptr<Mata::Nfa::Nfa>>& out);
 
 /**
  * @brief Create noodles from segment automaton @p aut.
  *
  * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
  * A noodle is a vector of pointers to copy of the segments automata created as if there was exactly one ε-transition
  *  between each two consecutive segments.
@@ -342,68 +339,71 @@
  *
  * Mata cannot work with equations, queries etc. Hence, we compute the noodles for the equation, but represent
  *  the equation in a way that libMata understands. The left side automata represent the left side of the equation
  *  and the right automaton represents the right side of the equation. To create noodles, we need a segment automaton
  *  representing the intersection. That can be achieved by computing a product of both sides. First, the left side
  *  has to be concatenated over an epsilon transitions into a single automaton to compute the intersection on, though.
  *
- * @param[in] left_automata Sequence of segment automata for left side of an equation to noodlify.
- * @param[in] right_automaton Segment automaton for right side of an equation to noodlify.
+ * @param[in] lhs_automata Sequence of segment automata for left side of an equation to noodlify.
+ * @param[in] rhs_automaton Segment automaton for right side of an equation to noodlify.
  * @param[in] include_empty Whether to also include empty noodles.
  * @param[in] params Additional parameters for the noodlification:
  *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
  *                 minimization before noodlification.
  * @return A list of all (non-empty) noodles.
  */
-NoodleSequence noodlify_for_equation(const AutRefSequence& left_automata, const Nfa::Nfa& right_automaton,
-                                     bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+NoodleSequence noodlify_for_equation(const std::vector<std::reference_wrapper<Mata::Nfa::Nfa>>& lhs_automata,
+                                     const Mata::Nfa::Nfa& rhs_automaton,
+                                     bool include_empty = false, const ParameterMap& params = {{ "reduce", "false"}});
 
 /**
  * @brief Create noodles for left and right side of equation.
  *
  * Segment automaton is a chain of finite automata (segments) connected via ε-transitions.
  * A noodle is a copy of the segment automaton with exactly one ε-transition between each two consecutive segments.
  *
  * Mata cannot work with equations, queries etc. Hence, we compute the noodles for the equation, but represent
  *  the equation in a way that libMata understands. The left side automata represent the left side of the equation
  *  and the right automaton represents the right side of the equation. To create noodles, we need a segment automaton
  *  representing the intersection. That can be achieved by computing a product of both sides. First, the left side
  *  has to be concatenated over an epsilon transitions into a single automaton to compute the intersection on, though.
  *
- * @param[in] left_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
- * @param[in] right_automaton Segment automaton for right side of an equation to noodlify.
+ * @param[in] lhs_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
+ * @param[in] rhs_automaton Segment automaton for right side of an equation to noodlify.
  * @param[in] include_empty Whether to also include empty noodles.
  * @param[in] params Additional parameters for the noodlification:
  *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
  *                 minimization before noodlification.
  * @return A list of all (non-empty) noodles.
  */
-NoodleSequence noodlify_for_equation(const AutPtrSequence& left_automata, const Nfa::Nfa& right_automaton,
-                                     bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+NoodleSequence noodlify_for_equation(const std::vector<Mata::Nfa::Nfa*>& lhs_automata, const Mata::Nfa::Nfa& rhs_automaton,
+                                     bool include_empty = false, const ParameterMap& params = {{ "reduce", "false"}});
 
 /**
  * @brief Create noodles for left and right side of equation (both sides are given as a sequence of automata).
  *
- * @param[in] left_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
- * @param[in] right_automaton Sequence of pointers to segment automata for right side of an equation to noodlify.
+ * @param[in] lhs_automata Sequence of pointers to segment automata for left side of an equation to noodlify.
+ * @param[in] rhs_automaton Sequence of pointers to segment automata for right side of an equation to noodlify.
  * @param[in] include_empty Whether to also include empty noodles.
  * @param[in] params Additional parameters for the noodlification:
  *     - "reduce": "false", "forward", "backward", "bidirectional"; Execute forward, backward or bidirectional simulation
  *                 minimization before noodlification.
  * @return A list of all (non-empty) noodles together with the positions reached from the beginning of left/right side.
  */
-NoodleSubstSequence noodlify_for_equation(const std::vector<std::shared_ptr<Nfa::Nfa>>& left_automata, const std::vector<std::shared_ptr<Nfa::Nfa>>& right_automata,
-                                                 bool include_empty = false, const StringMap& params = {{"reduce", "false"}});
+NoodleSubstSequence noodlify_for_equation(
+   const std::vector<std::shared_ptr<Mata::Nfa::Nfa>>& lhs_automata,
+   const std::vector<std::shared_ptr<Mata::Nfa::Nfa>>& rhs_automata,
+   bool include_empty = false, const ParameterMap& params = {{ "reduce", "false"}});
 
 /**
  * @brief Process epsilon map to a sequence of values (sorted according to key desc)
  *
  * @param eps_cnt Epsilon count
  * @return Vector of keys (count of epsilons)
  */
-EpsCntVector process_eps_map(const EpsCntMap& eps_cnt);
+VisitedEpsilonsCounterVector process_eps_map(const VisitedEpsilonsCounterMap& eps_cnt);
 
 } // namespace SegNfa.
 
 } // namespace Mata::Strings.
 
 #endif // MATA_NFA_STRING_SOLVING_HH_.
```

### Comparing `libmata-0.91.0/mata/include/mata/parser/inter-aut.hh` & `libmata-0.92.0/mata/include/mata/parser/inter-aut.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/parser/mintermization.hh` & `libmata-0.92.0/mata/include/mata/parser/mintermization.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/parser/parser.hh` & `libmata-0.92.0/mata/include/mata/parser/parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/parser/re2parser.hh` & `libmata-0.92.0/mata/include/mata/parser/re2parser.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/utils/closed-set.hh` & `libmata-0.92.0/mata/include/mata/utils/closed-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/utils/number-predicate.hh` & `libmata-0.92.0/mata/include/mata/utils/number-predicate.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/utils/ord-vector.hh` & `libmata-0.92.0/mata/include/mata/utils/ord-vector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     }
 
     /**
      * @brief Remove @p k from sorted vector.
      *
      * This function expects the vector to be sorted.
      */
-    inline void remove(Key k) {
+    inline void remove(const Key& k) {
         assert(vectorIsSorted());
         auto found_value_it = std::lower_bound(vec_.begin(), vec_.end(), k);
         if (found_value_it != vec_.end()) {
             if (*found_value_it == k) {
                 vec_.erase(found_value_it);
                 assert(vectorIsSorted());
                 return;
```

### Comparing `libmata-0.91.0/mata/include/mata/utils/sparse-set.hh` & `libmata-0.92.0/mata/include/mata/utils/sparse-set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/utils/synchronized-iterator.hh` & `libmata-0.92.0/mata/include/mata/utils/synchronized-iterator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/include/mata/utils/util.hh` & `libmata-0.92.0/mata/include/mata/utils/util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/CMakeLists.txt` & `libmata-0.92.0/mata/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/afa/afa.cc` & `libmata-0.92.0/mata/src/afa/afa.cc`

 * *Files 2% similar despite different names*

```diff
@@ -796,15 +796,15 @@
   assert(false);
 } // make_complete }}}
 
 
 Mata::Parser::ParsedSection Mata::Afa::serialize(
 	const Afa&                aut,
 	const SymbolToStringMap*  symbol_map,
-	const StateToStringMap*   state_map)
+	const StateNameMap*   state_map)
 { // {{{
 	Mata::Parser::ParsedSection parsec;
 	parsec.type = Mata::Afa::TYPE_AFA;
 
 	using bool_str_pair = std::pair<bool, std::string>;
 
 	std::function<bool_str_pair(State)> state_namer = nullptr;
@@ -903,29 +903,29 @@
 
   // TODO
   assert(false);
 } // minimize }}}
 
 // TODO this function should the same thing as the one taking IntermediateAut or be deleted
 Afa Mata::Afa::construct(
-	const Mata::Parser::ParsedSection&  parsec,
-	Alphabet*                            alphabet,
-	StringToStateMap*                    state_map)
+        const Mata::Parser::ParsedSection&  parsec,
+        Alphabet*                            alphabet,
+        NameStateMap*                    state_map)
 { // {{{
 	assert(nullptr != alphabet);
 	Afa aut;
 
 	if (parsec.type != Mata::Afa::TYPE_AFA) {
 		throw std::runtime_error(std::string(__FUNCTION__) + ": expecting type \"" +
                                  Mata::Afa::TYPE_AFA + "\"");
 	}
 
 	bool remove_state_map = false;
 	if (nullptr == state_map) {
-		state_map = new StringToStateMap();
+		state_map = new NameStateMap();
 		remove_state_map = true;
 	}
 
 	State cnt_state = 0;
 
 	// a lambda for translating state names to identifiers
 	auto get_state_name = [state_map, &cnt_state](const std::string& str) {
@@ -982,25 +982,25 @@
 
     return aut;
 } // construct }}}
 
 Afa Mata::Afa::construct(
         const Mata::IntermediateAut&         inter_aut,
         Alphabet*                            alphabet,
-        StringToStateMap*                    state_map)
+        NameStateMap*                    state_map)
 { // {{{
     Afa aut;
     assert(nullptr != alphabet);
 
     if (!inter_aut.is_afa()) {
         throw std::runtime_error(std::string(__FUNCTION__) + ": expecting type \"" +
                                  Mata::Afa::TYPE_AFA + "\"");
     }
 
-    StringToStateMap tmp_state_map;
+    NameStateMap tmp_state_map;
     if (nullptr == state_map) {
         state_map = &tmp_state_map;
     }
 
     // a lambda for translating state names to identifiers
     auto get_state_name = [&state_map, &aut](const std::string& str) {
         if (!state_map->count(str)) {
@@ -1173,18 +1173,16 @@
 } // is_complete }}}
 
 bool Mata::Afa::accepts_epsilon(const Afa& aut) {
     return std::any_of(aut.initialstates.cbegin(), aut.initialstates.cend(),
         [&aut](const Node& node) { return node.IsSubsetOf(aut.finalstates); });
 }
 
-Word encode_word(const Mata::StringToSymbolMap &symbol_map, const std::vector<std::string> &input) {
-    Word result;
-    for (const auto& str : input) { result.insert(symbol_map.at(str)); }
-    return result;
+Word encode_word(const Mata::Alphabet& alphabet, const std::vector<std::string> &input) {
+    return alphabet.translate_word(input);
 }
 
 std::ostream& std::operator<<(std::ostream& os, const Mata::Afa::AfaWrapper& afa_wrap)
 { // {{{
 	os << "{AFA wrapper|AFA: " << afa_wrap.afa << "|alphabet: " << afa_wrap.alphabet <<
 		"|state_dict: " << std::to_string(afa_wrap.state_dict) << "}";
 	return os;
```

### Comparing `libmata-0.91.0/mata/src/alphabet.cc` & `libmata-0.92.0/mata/src/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/inter-aut.cc` & `libmata-0.92.0/mata/src/inter-aut.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/mintermization.cc` & `libmata-0.92.0/mata/src/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/nfa/builder.cc` & `libmata-0.92.0/mata/src/nfa/builder.cc`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 #include <fstream>
 
 using namespace Mata::Nfa;
 using Mata::Nfa::Nfa;
 using Mata::Symbol;
 
-Nfa Builder::construct(const Mata::Parser::ParsedSection& parsec, Mata::Alphabet* alphabet, StringToStateMap* state_map) {
+Nfa Builder::construct(const Mata::Parser::ParsedSection& parsec, Mata::Alphabet* alphabet, NameStateMap* state_map) {
     Nfa aut;
     assert(nullptr != alphabet);
 
     if (parsec.type != TYPE_NFA) {
         throw std::runtime_error(std::string(__FUNCTION__) + ": expecting type \"" +
                                  TYPE_NFA + "\"");
     }
 
     bool remove_state_map = false;
     if (nullptr == state_map) {
-        state_map = new StringToStateMap();
+        state_map = new NameStateMap();
         remove_state_map = true;
     }
 
     // a lambda for translating state names to identifiers
     auto get_state_name = [&state_map, &aut](const std::string& str) {
         if (!state_map->count(str)) {
             State state = aut.add_state();
@@ -90,24 +90,24 @@
 
     // do the dishes and take out garbage
     clean_up();
 
     return aut;
 } // construct().
 
-Nfa Builder::construct(const Mata::IntermediateAut& inter_aut, Mata::Alphabet* alphabet, StringToStateMap* state_map) {
+Nfa Builder::construct(const Mata::IntermediateAut& inter_aut, Mata::Alphabet* alphabet, NameStateMap* state_map) {
     Nfa aut;
     assert(nullptr != alphabet);
 
     if (!inter_aut.is_nfa()) {
         throw std::runtime_error(std::string(__FUNCTION__) + ": expecting type \"" +
                                  TYPE_NFA + "\"");
     }
 
-    StringToStateMap tmp_state_map;
+    NameStateMap tmp_state_map;
     if (nullptr == state_map) {
         state_map = &tmp_state_map;
     }
 
     // a lambda for translating state names to identifiers
     auto get_state_name = [&state_map, &aut](const std::string& str) {
         if (!state_map->count(str)) {
```

### Comparing `libmata-0.91.0/mata/src/nfa/complement.cc` & `libmata-0.92.0/mata/src/nfa/complement.cc`

 * *Files 5% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     }
 
     make_complete(result, symbols, sink_state);
     result.final.complement(result.size());
     return result;
 }
 
-Nfa Mata::Nfa::complement(const Nfa& aut, const Alphabet& alphabet, const StringMap& params) {
+Nfa Mata::Nfa::complement(const Nfa& aut, const Alphabet& alphabet, const ParameterMap& params) {
     return Mata::Nfa::complement(aut, alphabet.get_alphabet_symbols(), params);
 }
 
-Nfa Mata::Nfa::complement(const Nfa& aut, const Mata::Util::OrdVector<Mata::Symbol>& symbols, const StringMap& params) {
+Nfa Mata::Nfa::complement(const Nfa& aut, const Mata::Util::OrdVector<Mata::Symbol>& symbols, const ParameterMap& params) {
     Nfa result;
     // Setting the requested algorithm.
     decltype(Algorithms::complement_classical)* algo = Algorithms::complement_classical;
     if (!haskey(params, "algorithm")) {
         throw std::runtime_error(std::to_string(__func__) +
                                  " requires setting the \"algo\" key in the \"params\" argument; "
                                  "received: " + std::to_string(params));
```

### Comparing `libmata-0.91.0/mata/src/nfa/concatenation.cc` & `libmata-0.92.0/mata/src/nfa/concatenation.cc`

 * *Files 20% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 #include "mata/nfa/algorithms.hh"
 
 using namespace Mata::Nfa;
 
 namespace Mata::Nfa {
 
 Nfa concatenate(const Nfa& lhs, const Nfa& rhs, bool use_epsilon,
-                StateToStateMap* lhs_result_states_map, StateToStateMap* rhs_result_states_map) {
-    return Algorithms::concatenate_eps(lhs, rhs, EPSILON, use_epsilon, lhs_result_states_map, rhs_result_states_map);
+                StateRenaming* lhs_state_renaming, StateRenaming* rhs_state_renaming) {
+    return Algorithms::concatenate_eps(lhs, rhs, EPSILON, use_epsilon, lhs_state_renaming, rhs_state_renaming);
 }
 
 Nfa& Nfa::concatenate(const Nfa& aut) {
     size_t n = this->size();
     auto upd_fnc = [&](State st) {
         return st + n;
     };
@@ -60,81 +60,81 @@
         }
     }
     this->final = new_fin;
     return *this;
 }
 
 Nfa Algorithms::concatenate_eps(const Nfa& lhs, const Nfa& rhs, const Symbol& epsilon, bool use_epsilon,
-                StateToStateMap* lhs_result_states_map, StateToStateMap* rhs_result_states_map) {
+                                StateRenaming* lhs_state_renaming, StateRenaming* rhs_state_renaming) {
     // Compute concatenation of given automata.
     // Concatenation will proceed in the order of the passed automata: Result is 'lhs . rhs'.
 
     if (lhs.size() == 0 || rhs.size() == 0 || lhs.initial.empty() || lhs.final.empty() ||
         rhs.initial.empty() || rhs.final.empty()) {
         return Nfa{};
     }
 
     const unsigned long lhs_states_num{lhs.size() };
     const unsigned long rhs_states_num{rhs.size() };
     Nfa result{}; // Concatenated automaton.
-    StateToStateMap lhs_result_states_map_internal{}; // Map mapping rhs states to result states.
-    StateToStateMap rhs_result_states_map_internal{}; // Map mapping rhs states to result states.
+    StateRenaming _lhs_states_renaming{}; // Map mapping rhs states to result states.
+    StateRenaming _rhs_states_renaming{}; // Map mapping rhs states to result states.
 
     const size_t result_num_of_states{lhs_states_num + rhs_states_num};
     if (result_num_of_states == 0) { return Nfa{}; }
 
     // Map lhs states to result states.
-    lhs_result_states_map_internal.reserve(lhs_states_num);
+    _lhs_states_renaming.reserve(lhs_states_num);
     Symbol result_state_index{ 0 };
     for (State lhs_state{ 0 }; lhs_state < lhs_states_num; ++lhs_state) {
-        lhs_result_states_map_internal.insert(std::make_pair(lhs_state, result_state_index));
+        _lhs_states_renaming.insert(std::make_pair(lhs_state, result_state_index));
         ++result_state_index;
     }
     // Map rhs states to result states.
-    rhs_result_states_map_internal.reserve(rhs_states_num);
+    _rhs_states_renaming.reserve(rhs_states_num);
     for (State rhs_state{ 0 }; rhs_state < rhs_states_num; ++rhs_state) {
-        rhs_result_states_map_internal.insert(std::make_pair(rhs_state, result_state_index));
+        _rhs_states_renaming.insert(std::make_pair(rhs_state, result_state_index));
         ++result_state_index;
     }
 
     result = Nfa();
     result.delta = lhs.delta;
     result.initial = lhs.initial;
     result.add_state(result_num_of_states-1);
 
     // Add epsilon transitions connecting lhs and rhs automata.
     // The epsilon transitions lead from lhs original final states to rhs original initial states.
     for (const auto& lhs_final_state: lhs.final) {
         for (const auto& rhs_initial_state: rhs.initial) {
             result.delta.add(lhs_final_state, epsilon,
-                             rhs_result_states_map_internal[rhs_initial_state]);
+                             _rhs_states_renaming[rhs_initial_state]);
         }
     }
 
     // Make result final states.
     for (const auto& rhs_final_state: rhs.final)
     {
-        result.final.insert(rhs_result_states_map_internal[rhs_final_state]);
+        result.final.insert(_rhs_states_renaming[rhs_final_state]);
     }
 
     // Add rhs transitions to the result.
     for (State rhs_state{ 0 }; rhs_state < rhs_states_num; ++rhs_state)
     {
         for (const Move& rhs_move: rhs.get_moves_from(rhs_state))
         {
             for (const State& rhs_state_to: rhs_move.targets)
             {
-                result.delta.add(rhs_result_states_map_internal[rhs_state],
+                result.delta.add(_rhs_states_renaming[rhs_state],
                                  rhs_move.symbol,
-                                 rhs_result_states_map_internal[rhs_state_to]);
+                                 _rhs_states_renaming[rhs_state_to]);
             }
         }
     }
 
     if (!use_epsilon) {
         result.remove_epsilon();
     }
-    if (lhs_result_states_map != nullptr) { *lhs_result_states_map = lhs_result_states_map_internal; }
-    if (rhs_result_states_map != nullptr) { *rhs_result_states_map = rhs_result_states_map_internal; }
+    if (lhs_state_renaming != nullptr) { *lhs_state_renaming = _lhs_states_renaming; }
+    if (rhs_state_renaming != nullptr) { *rhs_state_renaming = _rhs_states_renaming; }
     return result;
 } // concatenate_eps().
 } // Namespace Mata::Nfa.
```

### Comparing `libmata-0.91.0/mata/src/nfa/delta.cc` & `libmata-0.92.0/mata/src/nfa/delta.cc`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 "Transition [" + std::to_string(src) + ", " + std::to_string(symb) + ", " +
                 std::to_string(tgt) + "] does not exist.");
     } else if (state_transitions.back().symbol < symb) {
         throw std::invalid_argument(
                 "Transition [" + std::to_string(src) + ", " + std::to_string(symb) + ", " +
                 std::to_string(tgt) + "] does not exist.");
     } else {
-        const auto symbol_transitions{ state_transitions.find(Move{symb }) };
+        const auto symbol_transitions{ state_transitions.find(symb) };
         if (symbol_transitions == state_transitions.end()) {
             throw std::invalid_argument(
                     "Transition [" + std::to_string(src) + ", " + std::to_string(symb) + ", " +
                     std::to_string(tgt) + "] does not exist.");
         } else {
             symbol_transitions->remove(tgt);
             if (symbol_transitions->empty()) {
```

### Comparing `libmata-0.91.0/mata/src/nfa/inclusion.cc` & `libmata-0.92.0/mata/src/nfa/inclusion.cc`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
                 return true;
             }
         }
 
         return false;
     }
 
-    AlgoType set_algorithm(const std::string &function_name, const StringMap &params) {
+    AlgoType set_algorithm(const std::string &function_name, const ParameterMap &params) {
         if (!haskey(params, "algorithm")) {
             throw std::runtime_error(function_name +
                                      " requires setting the \"algo\" key in the \"params\" argument; "
                                      "received: " + std::to_string(params));
         }
 
         decltype(Algorithms::is_included_naive) *algo;
@@ -249,30 +249,30 @@
 
 // The dispatching method that calls the correct one based on parameters
 bool Mata::Nfa::is_included(
         const Nfa &smaller,
         const Nfa &bigger,
         Run *cex,
         const Alphabet *const alphabet,
-        const StringMap &params) { // {{{
+        const ParameterMap &params) { // {{{
     AlgoType algo{set_algorithm(std::to_string(__func__), params)};
     return algo(smaller, bigger, alphabet, cex);
 } // is_included }}}
 
-bool Mata::Nfa::are_equivalent(const Nfa& lhs, const Nfa& rhs, const Alphabet *alphabet, const StringMap& params)
+bool Mata::Nfa::are_equivalent(const Nfa& lhs, const Nfa& rhs, const Alphabet *alphabet, const ParameterMap& params)
 {
     //TODO: add comment on what this is doing, what is __func__ ...
     AlgoType algo{ set_algorithm(std::to_string(__func__), params) };
 
     if (params.at("algorithm") == "naive") {
         if (alphabet == nullptr) {
             const auto computed_alphabet{create_alphabet(lhs, rhs) };
             return compute_equivalence(lhs, rhs, &computed_alphabet, algo);
         }
     }
 
     return compute_equivalence(lhs, rhs, alphabet, algo);
 }
 
-bool Mata::Nfa::are_equivalent(const Nfa& lhs, const Nfa& rhs, const StringMap& params) {
+bool Mata::Nfa::are_equivalent(const Nfa& lhs, const Nfa& rhs, const ParameterMap& params) {
     return are_equivalent(lhs, rhs, nullptr, params);
 }
```

### Comparing `libmata-0.91.0/mata/src/nfa/intersection.cc` & `libmata-0.92.0/mata/src/nfa/intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/nfa/nfa.cc` & `libmata-0.92.0/mata/src/nfa/nfa.cc`

 * *Files 16% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 
 // MATA headers
 #include "mata/utils/sparse-set.hh"
 #include "mata/nfa/nfa.hh"
 #include "mata/nfa/algorithms.hh"
 #include <mata/simlib/explicit_lts.hh>
 
-using std::tie;
-
 using namespace Mata::Util;
 using namespace Mata::Nfa;
 using Mata::Symbol;
 using Mata::BoolVector;
 
 using StateBoolArray = std::vector<bool>; ///< Bool array for states in the automaton.
 
@@ -114,29 +112,29 @@
 
         return reachable;
     }
 
     /**
      * Add transitions to the trimmed automaton.
      * @param[in] nfa NFA to add transitions from.
-     * @param[in] original_to_new_states_map Map of old states to new trimmed automaton states.
+     * @param[in] state_renaming Map of old states to new trimmed automaton states.
      * @param[out] trimmed_aut The new trimmed automaton.
      */
-    void add_trimmed_transitions(const Nfa& nfa, const StateToStateMap& original_to_new_states_map, Nfa& trimmed_aut) {
+    void add_trimmed_transitions(const Nfa& nfa, const StateRenaming& state_renaming, Nfa& trimmed_aut) {
         // For each reachable original state 's' (which means it is mapped to the state of trimmed automaton)...
-        for (const auto& original_state_mapping: original_to_new_states_map)
+        for (const auto& original_state_mapping: state_renaming)
         {
             // ...add all transitions from 's' to some reachable state to the trimmed automaton.
             for (const auto& state_transitions_with_symbol: nfa.delta[original_state_mapping.first])
             {
                 Move new_state_trans_with_symbol(state_transitions_with_symbol.symbol);
                 for (State old_state_to: state_transitions_with_symbol.targets)
                 {
-                    auto iter_to_new_state_to = original_to_new_states_map.find(old_state_to);
-                    if (iter_to_new_state_to != original_to_new_states_map.end())
+                    auto iter_to_new_state_to = state_renaming.find(old_state_to);
+                    if (iter_to_new_state_to != state_renaming.end())
                     {
                         // We can push here, because we assume that new states follow the ordering of original states.
                         new_state_trans_with_symbol.insert(iter_to_new_state_to->second);
                     }
                 }
                 if (!new_state_trans_with_symbol.empty()) {
                     trimmed_aut.delta.get_mutable_post(original_state_mapping.second).insert(new_state_trans_with_symbol);
@@ -144,36 +142,36 @@
             }
         }
     }
 
     /**
      * Get a new trimmed automaton.
      * @param[in] nfa NFA to trim.
-     * @param[in] original_to_new_states_map Map of old states to new trimmed automaton states (new states should follow the ordering of old states).
+     * @param[in] original_to_new_state_renaming Map of old states to new trimmed automaton states (new states should follow the ordering of old states).
      * @return Newly created trimmed automaton.
      */
-    Nfa create_trimmed_aut(const Nfa& nfa, const StateToStateMap& original_to_new_states_map) {
-        Nfa trimmed_aut{ original_to_new_states_map.size() };
+    Nfa create_trimmed_aut(const Nfa& nfa, const StateRenaming& state_renaming) {
+        Nfa trimmed_aut{ state_renaming.size() };
 
         for (const State old_initial_state: nfa.initial)
         {
-            if (original_to_new_states_map.find(old_initial_state) != original_to_new_states_map.end())
+            if (state_renaming.find(old_initial_state) != state_renaming.end())
             {
-                trimmed_aut.initial.insert(original_to_new_states_map.at(old_initial_state));
+                trimmed_aut.initial.insert(state_renaming.at(old_initial_state));
             }
         }
         for (const State old_final_state: nfa.final)
         {
-            if (original_to_new_states_map.find(old_final_state) != original_to_new_states_map.end())
+            if (state_renaming.find(old_final_state) != state_renaming.end())
             {
-                trimmed_aut.final.insert(original_to_new_states_map.at(old_final_state));
+                trimmed_aut.final.insert(state_renaming.at(old_final_state));
             }
         }
 
-        add_trimmed_transitions(nfa, original_to_new_states_map, trimmed_aut);
+        add_trimmed_transitions(nfa, state_renaming, trimmed_aut);
         return trimmed_aut;
     }
 
     /**
      * Get directed transitions for digraph.
      * @param[in] nfa NFA to get directed transitions from.
      * @param[in] abstract_symbol Abstract symbol to use for transitions in digraph.
@@ -219,103 +217,100 @@
 
 StateSet Nfa::get_terminating_states() const
 {
     return revert(*this).get_reachable_states();
 }
 
 //TODO: probably can be removed, trim_inplace is faster.
-void Nfa::trim_reverting(StateToStateMap* state_map)
+void Nfa::trim_reverting(StateRenaming* state_renaming)
 {
-    if (!state_map) {
-        StateToStateMap tmp_state_map{};
-        *this = get_trimmed_automaton(&tmp_state_map);
+    if (!state_renaming) {
+        StateRenaming tmp_state_renaming{};
+        *this = get_trimmed_automaton(&tmp_state_renaming);
     } else {
-        state_map->clear();
-        *this = get_trimmed_automaton(state_map);
+        state_renaming->clear();
+        *this = get_trimmed_automaton(state_renaming);
     }
 }
 
-void Nfa::trim_inplace(StateToStateMap* state_map)
-{
+void Nfa::trim_inplace(StateRenaming* state_renaming) {
 #ifdef _STATIC_STRUCTURES_
     BoolVector useful_states{ useful_states() };
     useful_states.clear();
     useful_states = useful_states();
 #else
     BoolVector useful_states{ get_useful_states() };
 #endif
-
-    std::vector<State> renaming(useful_states.size());
-
-    State j=0;
-    for(State i = 0; i<useful_states.size(); i++) {
-        if (useful_states[i]) {
-            renaming[i] = j;
-            j++;
+    const size_t useful_states_size{ useful_states.size() };
+    std::vector<State> renaming(useful_states_size);
+    for(State new_state{ 0 }, orig_state{ 0 }; orig_state < useful_states_size; ++orig_state) {
+        if (useful_states[orig_state]) {
+            renaming[orig_state] = new_state;
+            ++new_state;
         }
     }
 
     delta.defragment(useful_states, renaming);
 
-    auto is_state_useful = [&useful_states](State q){return q < useful_states.size() && useful_states[q];};
+    auto is_state_useful = [&](State q){return q < useful_states.size() && useful_states[q];};
     initial.filter(is_state_useful);
     final.filter(is_state_useful);
-    auto rename_state = [&renaming](State q){return renaming[q];};
+    auto rename_state = [&](State q){return renaming[q];};
     initial.rename(rename_state);
     final.rename(rename_state);
     initial.truncate();
     final.truncate();
-
-    // TODO : this is actually only used in one test, remove state map?
-    if (state_map) {
-        state_map->clear();
-        state_map->reserve(useful_states.size());
-        for (State q=0;q<useful_states.size();q++)
-            if (useful_states[q])
-                (*state_map)[q] = renaming[q];
+    if (state_renaming != nullptr) {
+        state_renaming->clear();
+        state_renaming->reserve(useful_states_size);
+        for (State q{ 0 }; q < useful_states_size; ++q) {
+            if (useful_states[q]) {
+                (*state_renaming)[q] = renaming[q];
+            }
+        }
     }
 }
 
-Nfa Nfa::get_trimmed_automaton(StateToStateMap* state_map) const {
+Nfa Nfa::get_trimmed_automaton(StateRenaming* state_renaming) const {
     if (initial.empty() || final.empty()) { return Nfa{}; }
 
-    StateToStateMap tmp_state_map{};
-    if (!state_map) {
-        state_map = &tmp_state_map;
+    StateRenaming tmp_state_renaming{};
+    if (!state_renaming) {
+        state_renaming = &tmp_state_renaming;
     }
-    state_map->clear();
+    state_renaming->clear();
 
     const StateSet original_useful_states{get_useful_states_old() };
-    state_map->reserve(original_useful_states.size());
+    state_renaming->reserve(original_useful_states.size());
 
     size_t new_state_num{ 0 };
     for (const State original_state: original_useful_states) {
-        (*state_map)[original_state] = new_state_num;
+        (*state_renaming)[original_state] = new_state_num;
         ++new_state_num;
     }
-    return create_trimmed_aut(*this, *state_map);
+    return create_trimmed_aut(*this, *state_renaming);
 }
 
 namespace {
     // A structure to store metadata related to each state/node during the computation 
     // of useful states. It contains Tarjan's metadata and the state of the 
     // iteration through the successors. 
     struct TarjanNodeData {
-        Post::const_iterator post_it;
-        Post::const_iterator post_end;
+        Post::const_iterator post_it{};
+        Post::const_iterator post_end{};
         StateSet::const_iterator targets_it{};
         StateSet::const_iterator targets_end{};
         // index of a node (corresponds to the time of discovery)
-        unsigned long index {0};
+        unsigned long index{ 0 };
         // index of a lower node in the same SCC 
-        unsigned long lowlink {0};
+        unsigned long lowlink{ 0 };
         // was the node already initialized (=the initial phase of the Tarjan's recursive call was executed)
-        bool initilized {false};
+        bool initilized{ false };
         // is node on Tarjan's stack?
-        bool on_stack {false};
+        bool on_stack{ false };
 
         TarjanNodeData() = default;
 
         TarjanNodeData(State q, const Delta & delta, unsigned long index) 
             : post_it(delta[q].cbegin()), post_end(delta[q].cend()), index(index), lowlink(index), initilized(true), on_stack(true) {
             if (post_it != post_end) {
                 targets_it = post_it->cbegin();
@@ -566,17 +561,17 @@
     }
 
     for (Trans trans : delta) {
         output << "q" << trans.src << " " << trans.symb << " q" << trans.tgt << std::endl;
     }
 }
 
-TransSequence Nfa::get_trans_as_sequence() const
+std::vector<Trans> Nfa::get_trans_as_sequence() const
 {
-    TransSequence trans_sequence{};
+    std::vector<Trans> trans_sequence{};
 
     for (State state_from{ 0 }; state_from < delta.num_of_states(); ++state_from)
     {
         for (const auto& transition_from_state: delta[state_from])
         {
             for (State state_to: transition_from_state.targets)
             {
@@ -584,17 +579,17 @@
             }
         }
     }
 
     return trans_sequence;
 }
 
-TransSequence Nfa::get_trans_from_as_sequence(State state_from) const
+std::vector<Trans> Nfa::get_trans_from_as_sequence(State state_from) const
 {
-    TransSequence trans_sequence{};
+    std::vector<Trans> trans_sequence{};
 
     for (const auto& transition_from_state: delta[state_from])
     {
         for (State state_to: transition_from_state.targets)
         {
             trans_sequence.emplace_back(state_from, transition_from_state.symbol, state_to);
         }
@@ -609,16 +604,16 @@
     return digraph;
 }
 
 void Nfa::get_one_letter_aut(Nfa& result) const {
     result = get_one_letter_aut();
 }
 
-TransSequence Nfa::get_transitions_to(State state_to) const {
-    TransSequence transitions_to_state{};
+std::vector<Trans> Nfa::get_transitions_to(State state_to) const {
+    std::vector<Trans> transitions_to_state{};
     const size_t num_of_states{ delta.num_of_states() };
     for (State state_from{ 0 }; state_from < num_of_states; ++state_from) {
         for (const Move& state_from_move: delta[state_from]) {
             const auto target_state{ state_from_move.targets.find(state_to) };
             if (target_state != state_from_move.targets.end()) {
                 transitions_to_state.emplace_back(state_from, state_from_move.symbol, state_to );
             }
```

### Comparing `libmata-0.91.0/mata/src/nfa/operations.cc` & `libmata-0.92.0/mata/src/nfa/operations.cc`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 #include <mata/simlib/explicit_lts.hh>
 
 using std::tie;
 
 using namespace Mata::Util;
 using namespace Mata::Nfa;
 using Mata::Symbol;
-using Mata::BoolVector;
 
 using StateBoolArray = std::vector<bool>; ///< Bool array for states in the automaton.
 
 namespace {
     Simlib::Util::BinaryRelation compute_fw_direct_simulation(const Nfa& aut) {
         Symbol maxSymbol = 0;
         const size_t state_num = aut.size();
@@ -54,42 +53,42 @@
             LTSforSimulation.add_transition(finalState, maxSymbol + 1, finalState);
         }
 
         LTSforSimulation.init();
         return LTSforSimulation.compute_simulation();
     }
 
-	Nfa reduce_size_by_simulation(const Nfa& aut, StateToStateMap &state_map) {
+    Nfa reduce_size_by_simulation(const Nfa& aut, StateRenaming &state_renaming) {
         Nfa result;
         const auto sim_relation = Algorithms::compute_relation(
-                aut, StringMap{{"relation", "simulation"}, {"direction", "forward"}});
+                aut, ParameterMap{{ "relation", "simulation"}, { "direction", "forward"}});
 
         auto sim_relation_symmetric = sim_relation;
         sim_relation_symmetric.restrict_to_symmetric();
 
         // for State q, quot_proj[q] should be the representative state representing the symmetric class of states in simulation
         std::vector<size_t> quot_proj;
         sim_relation_symmetric.get_quotient_projection(quot_proj);
 
-		const size_t num_of_states = aut.size();
+        const size_t num_of_states = aut.size();
 
-		// map each state q of aut to the state of the reduced automaton representing the simulation class of q
-		for (State q = 0; q < num_of_states; ++q) {
-			const State qReprState = quot_proj[q];
-			if (state_map.count(qReprState) == 0) { // we need to map q's class to a new state in reducedAut
-				const State qClass = result.add_state();
-				state_map[qReprState] = qClass;
-				state_map[q] = qClass;
-			} else {
-				state_map[q] = state_map[qReprState];
-			}
-		}
+        // map each state q of aut to the state of the reduced automaton representing the simulation class of q
+        for (State q = 0; q < num_of_states; ++q) {
+            const State qReprState = quot_proj[q];
+            if (state_renaming.count(qReprState) == 0) { // we need to map q's class to a new state in reducedAut
+                const State qClass = result.add_state();
+                state_renaming[qReprState] = qClass;
+                state_renaming[q] = qClass;
+            } else {
+                state_renaming[q] = state_renaming[qReprState];
+            }
+        }
 
         for (State q = 0; q < num_of_states; ++q) {
-            const State q_class_state = state_map.at(q);
+            const State q_class_state = state_renaming.at(q);
 
             if (aut.initial[q]) { // if a symmetric class contains initial state, then the whole class should be initial
                 result.initial.insert(q_class_state);
             }
 
             if (quot_proj[q] == q) { // we process only transitions starting from the representative state, this is enough for simulation
                 for (const auto &q_trans : aut.get_moves_from(q)) {
@@ -108,15 +107,15 @@
                         for (const State p : representatives_of_states_to) {
                             if (s != p && sim_relation.get(s, p)) { // if p (different from s) simulates s
                                 is_state_important = false; // as p simulates s, the transition from q to s is not important to keep, as it is subsumed in transition from q to p
                                 break;
                             }
                         }
                         if (is_state_important) {
-                            representatives_class_states.insert(state_map.at(s));
+                            representatives_class_states.insert(state_renaming.at(s));
                         }
                     }
 
                     // add the transition 'q_class_state-q_trans.symbol->representatives_class_states' at the end of transition list of transitions starting from q_class_state
                     // as the q_trans.symbol should be the largest symbol we saw (as we iterate trough getTransitionsFromState(q) which is ordered)
                     result.delta.get_mutable_post(q_class_state).insert(Move(q_trans.symbol, representatives_class_states));
                 }
@@ -133,56 +132,14 @@
 
 std::ostream &std::operator<<(std::ostream &os, const Mata::Nfa::Trans &trans) { // {{{
     std::string result = "(" + std::to_string(trans.src) + ", " +
                          std::to_string(trans.symb) + ", " + std::to_string(trans.tgt) + ")";
     return os << result;
 }
 
-bool Mata::Nfa::are_state_disjoint(const Nfa& lhs, const Nfa& rhs)
-{ // {{{
-    // fill lhs_states with all states of lhs
-    std::unordered_set<State> lhs_states;
-    lhs_states.insert(lhs.initial.begin(), lhs.initial.end());
-    lhs_states.insert(lhs.final.begin(), lhs.final.end());
-
-    const size_t delta_size = lhs.delta.num_of_states();
-    for (size_t i = 0; i < delta_size; i++) {
-        lhs_states.insert(i);
-        for (const auto& symStates : lhs.delta[i])
-        {
-            lhs_states.insert(symStates.targets.begin(), symStates.targets.end());
-        }
-    }
-
-    // for every state found in rhs, check its presence in lhs_states
-    for (const auto& rhs_st : rhs.initial) {
-        if (haskey(lhs_states, rhs_st)) { return false; }
-    }
-
-    for (const auto& rhs_st : rhs.final) {
-        if (haskey(lhs_states, rhs_st)) { return false; }
-    }
-
-    const size_t lhs_post_size = lhs.delta.num_of_states();
-    for (size_t i = 0; i < lhs_post_size; i++) {
-        if (haskey(lhs_states, i))
-            return false;
-        for (const auto& symState : lhs.delta[i]) {
-            for (const auto& rhState : symState.targets) {
-                if (haskey(lhs_states,rhState)) {
-                    return false;
-                }
-            }
-        }
-    }
-
-    // no common state found
-    return true;
-} // are_disjoint }}}
-
 bool Mata::Nfa::make_complete(Nfa& aut, const Alphabet& alphabet, State sink_state) {
     return Mata::Nfa::make_complete(aut, alphabet.get_alphabet_symbols(), sink_state);
 }
 
 bool Mata::Nfa::make_complete(Nfa& aut, const Mata::Util::OrdVector<Symbol>& symbols, State sink_state) {
     bool was_something_added{ false };
 
@@ -583,24 +540,14 @@
         cur = aut.post(cur, sym);
         if (cur.empty()) { return false; }
     }
 
     return aut.final.intersects_with(cur);
 }
 
-/// serializes Nfa into a ParsedSection
-Mata::Parser::ParsedSection Mata::Nfa::serialize(
-        const Nfa&                aut,
-        const SymbolToStringMap*  symbol_map,
-        const StateToStringMap*   state_map) {
-    (void)aut; (void)symbol_map; (void)state_map;
-    assert(false && "Unimplemented.");
-    return {};
-}
-
 bool Mata::Nfa::is_lang_empty(const Nfa& aut, Run* cex)
 { // {{{
     std::list<State> worklist(
             aut.initial.begin(), aut.initial.end());
     std::unordered_set<State> processed(
             aut.initial.begin(), aut.initial.end());
 
@@ -667,70 +614,70 @@
 Nfa Mata::Nfa::Algorithms::minimize_brzozowski(const Nfa& aut) {
     //compute the minimal deterministic automaton, Brzozovski algorithm
     return determinize(revert(determinize(revert(aut))));
 }
 
 Nfa Mata::Nfa::minimize(
                 const Nfa& aut,
-                const StringMap& params)
+                const ParameterMap& params)
 {
-	Nfa result;
-	// setting the default algorithm
-	decltype(Algorithms::minimize_brzozowski)* algo = Algorithms::minimize_brzozowski;
-	if (!haskey(params, "algorithm")) {
-		throw std::runtime_error(std::to_string(__func__) +
-			" requires setting the \"algo\" key in the \"params\" argument; "
-			"received: " + std::to_string(params));
-	}
-
-	const std::string& str_algo = params.at("algorithm");
-	if ("brzozowski" == str_algo) {  /* default */ }
-	else {
-		throw std::runtime_error(std::to_string(__func__) +
-			" received an unknown value of the \"algo\" key: " + str_algo);
-	}
+    Nfa result;
+    // setting the default algorithm
+    decltype(Algorithms::minimize_brzozowski)* algo = Algorithms::minimize_brzozowski;
+    if (!haskey(params, "algorithm")) {
+        throw std::runtime_error(std::to_string(__func__) +
+            " requires setting the \"algo\" key in the \"params\" argument; "
+            "received: " + std::to_string(params));
+    }
+
+    const std::string& str_algo = params.at("algorithm");
+    if ("brzozowski" == str_algo) {  /* default */ }
+    else {
+        throw std::runtime_error(std::to_string(__func__) +
+            " received an unknown value of the \"algo\" key: " + str_algo);
+    }
 
-	return algo(aut);
+    return algo(aut);
 }
 
 Nfa Mata::Nfa::uni(const Nfa &lhs, const Nfa &rhs) {
-    Nfa unionAutomaton = rhs;
+    Nfa union_nfa{ rhs };
 
-    StateToStateMap thisStateToUnionState;
+    StateRenaming lhs_state_renaming;
     const size_t size = lhs.size();
-    for (State thisState = 0; thisState < size; ++thisState) {
-        thisStateToUnionState[thisState] = unionAutomaton.add_state();
+    for (State lhs_state = 0; lhs_state < size; ++lhs_state) {
+        lhs_state_renaming[lhs_state] = union_nfa.add_state();
     }
 
-    for (State thisInitialState : lhs.initial) {
-        unionAutomaton.initial.insert(thisStateToUnionState[thisInitialState]);
+    for (State lhs_initial_state : lhs.initial) {
+        union_nfa.initial.insert(lhs_state_renaming[lhs_initial_state]);
     }
 
-    for (State thisFinalState : lhs.final) {
-        unionAutomaton.final.insert(thisStateToUnionState[thisFinalState]);
+    for (State lhs_final_state : lhs.final) {
+        union_nfa.final.insert(lhs_state_renaming[lhs_final_state]);
     }
 
-    for (State thisState = 0; thisState < size; ++thisState) {
-        State unionState = thisStateToUnionState[thisState];
-        for (const Move &transitionFromThisState : lhs.delta[thisState]) {
+    for (State lhs_state = 0; lhs_state < size; ++lhs_state) {
+        State union_state = lhs_state_renaming[lhs_state];
+        for (const Move &lhs_move : lhs.delta[lhs_state]) {
 
-            Move transitionFromUnionState(transitionFromThisState.symbol, StateSet{});
+            Move union_move(lhs_move.symbol, StateSet{});
 
-            for (State stateTo : transitionFromThisState.targets) {
-                transitionFromUnionState.insert(thisStateToUnionState[stateTo]);
+            for (State stateTo : lhs_move.targets) {
+                union_move.insert(lhs_state_renaming[stateTo]);
             }
 
-            unionAutomaton.delta.get_mutable_post(unionState).insert(transitionFromUnionState);
+            union_nfa.delta.get_mutable_post(union_state).insert(union_move);
         }
     }
 
-    return unionAutomaton;
+    return union_nfa;
 }
 
-Simlib::Util::BinaryRelation Mata::Nfa::Algorithms::compute_relation(const Nfa& aut, const StringMap& params) {
+Simlib::Util::BinaryRelation Mata::Nfa::Algorithms::compute_relation(const Nfa& aut, const ParameterMap& params) {
     if (!haskey(params, "relation")) {
         throw std::runtime_error(std::to_string(__func__) +
                                  " requires setting the \"relation\" key in the \"params\" argument; "
                                  "received: " + std::to_string(params));
     }
     if (!haskey(params, "direction")) {
         throw std::runtime_error(std::to_string(__func__) +
@@ -745,48 +692,48 @@
     }
     else {
         throw std::runtime_error(std::to_string(__func__) +
                                  " received an unknown value of the \"relation\" key: " + relation);
     }
 }
 
-Nfa Mata::Nfa::reduce(const Nfa &aut, bool trim_input, StateToStateMap *state_map, const StringMap& params) {
+Nfa Mata::Nfa::reduce(const Nfa &aut, bool trim_input, StateRenaming *state_renaming, const ParameterMap& params) {
     if (!haskey(params, "algorithm")) {
         throw std::runtime_error(std::to_string(__func__) +
                                  " requires setting the \"algorithm\" key in the \"params\" argument; "
                                  "received: " + std::to_string(params));
     }
 
     Nfa aut_to_reduce{ aut };
-    StateToStateMap trimmed_state_map{};
+    StateRenaming trimmed_state_renaming{};
     if (trim_input) {
-        aut_to_reduce.trim(&trimmed_state_map);
+        aut_to_reduce.trim(&trimmed_state_renaming);
     }
 
     Nfa result;
     std::unordered_map<State,State> reduced_state_map;
     const std::string& algorithm = params.at("algorithm");
     if ("simulation" == algorithm) {
         result = reduce_size_by_simulation(aut_to_reduce, reduced_state_map);
     } else {
         throw std::runtime_error(std::to_string(__func__) +
                                  " received an unknown value of the \"algorithm\" key: " + algorithm);
     }
 
-    if (state_map) {
-        state_map->clear();
+    if (state_renaming) {
+        state_renaming->clear();
         if (trim_input) {
-            for (const auto& trimmed_mapping : trimmed_state_map) {
+            for (const auto& trimmed_mapping : trimmed_state_renaming) {
                 const auto reduced_mapping{ reduced_state_map.find(trimmed_mapping.second) };
                 if (reduced_mapping != reduced_state_map.end()) {
-                    (*state_map)[trimmed_mapping.first] = reduced_mapping->second;
+                    (*state_renaming)[trimmed_mapping.first] = reduced_mapping->second;
                 }
             }
         } else { // Input has not been trimmed, the reduced state map is the actual input to result state map.
-            *state_map = reduced_state_map;
+            *state_renaming = reduced_state_map;
         }
     }
 
     return result;
 }
 
 Nfa Mata::Nfa::determinize(
@@ -881,44 +828,42 @@
         for (const Trans& state_transitions: nfa.delta) {
             alphabet.update_next_symbol_value(state_transitions.symb);
             alphabet.try_add_new_symbol(std::to_string(state_transitions.symb), state_transitions.symb);
         }
     }
 }
 
-Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const ConstAutRefSequence& nfas) {
+Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const std::vector<std::reference_wrapper<const Nfa>>& nfas) {
     Mata::OnTheFlyAlphabet alphabet{};
     for (const auto& nfa: nfas) {
         fill_alphabet(nfa, alphabet);
     }
     return alphabet;
 }
 
-Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const AutRefSequence& nfas) {
+Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const std::vector<std::reference_wrapper<Nfa>>& nfas) {
     Mata::OnTheFlyAlphabet alphabet{};
     for (const auto& nfa: nfas) {
         fill_alphabet(nfa, alphabet);
     }
     return alphabet;
 }
 
-Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const ConstAutPtrSequence& nfas) {
+Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const std::vector<const Nfa *>& nfas) {
     Mata::OnTheFlyAlphabet alphabet{};
     for (const Mata::Nfa::Nfa* const nfa: nfas) {
         fill_alphabet(*nfa, alphabet);
     }
     return alphabet;
 }
 
-Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const AutPtrSequence& nfas) {
+Mata::OnTheFlyAlphabet Mata::Nfa::create_alphabet(const std::vector<Nfa*>& nfas) {
     Mata::OnTheFlyAlphabet alphabet{};
     for (const Mata::Nfa::Nfa* const nfa: nfas) {
         fill_alphabet(*nfa, alphabet);
     }
     return alphabet;
 }
 
-Run Mata::Nfa::encode_word(const Mata::StringToSymbolMap& symbol_map, const std::vector<std::string>& input) {
-    Run result;
-    for (const auto& str : input) { result.word.push_back(symbol_map.at(str)); }
-    return result;
+Run Mata::Nfa::encode_word(const Alphabet* alphabet, const std::vector<std::string>& input) {
+    return { .word = alphabet->translate_word(input) };
 }
```

### Comparing `libmata-0.91.0/mata/src/nfa/universal.cc` & `libmata-0.92.0/mata/src/nfa/universal.cc`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 } // }}}
 
 // The dispatching method that calls the correct one based on parameters
 bool Mata::Nfa::is_universal(
 	const Nfa&         aut,
 	const Alphabet&    alphabet,
 	Run*               cex,
-	const StringMap&  params)
+	const ParameterMap&  params)
 { // {{{
 
 	// setting the default algorithm
 	decltype(Algorithms::is_universal_naive)* algo = Algorithms::is_universal_naive;
 	if (!haskey(params, "algorithm")) {
 		throw std::runtime_error(std::to_string(__func__) +
 			" requires setting the \"algo\" key in the \"params\" argument; "
```

### Comparing `libmata-0.91.0/mata/src/parser.cc` & `libmata-0.92.0/mata/src/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/re2parser.cc` & `libmata-0.92.0/mata/src/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/src/strings/nfa-noodlification.cc` & `libmata-0.92.0/mata/src/strings/nfa-noodlification.cc`

 * *Files 9% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     // Compute number of all combinations of ε-transitions with one ε-transitions from each depth.
     size_t num_of_permutations{ get_num_of_permutations(epsilon_depths) };
     size_t epsilon_depths_size{ epsilon_depths.size() };
 
     NoodleSequence noodles{};
     // noodle of epsilon transitions (each from different depth)
-    TransSequence epsilon_noodle(epsilon_depths_size);
+    std::vector<Trans> epsilon_noodle(epsilon_depths_size);
     // for each combination of ε-transitions, create the automaton.
     // based on https://stackoverflow.com/questions/48270565/create-all-possible-combinations-of-multiple-vectors
     for (size_t index{ 0 }; index < num_of_permutations; ++index) {
         size_t temp{ index };
         for (size_t depth{ 0 }; depth < epsilon_depths_size; ++depth) {
             size_t num_of_trans_at_cur_depth = epsilon_depths.at(depth).size();
             size_t computed_index = temp % num_of_trans_at_cur_depth;
@@ -123,15 +123,15 @@
     }
     return noodles;
 }
 
 //todo: is this taking all final times all initial?
 // can it be done more efficiently? (only connected combinations through dfs)
 void SegNfa::segs_one_initial_final(
-    const Mata::Nfa::AutSequence& segments,
+    const std::vector<Nfa::Nfa>& segments,
     bool include_empty,
     const State& unused_state,
     std::map<std::pair<State, State>, std::shared_ptr<Nfa::Nfa>>& out) {
 
     for (auto iter = segments.begin(); iter != segments.end(); ++iter) {
         if (iter == segments.begin()) { // first segment will always have all initial states in noodles
             for (const State final_state: iter->final) {
@@ -170,19 +170,19 @@
     }
 }
 
 SegNfa::NoodleSubstSequence SegNfa::noodlify_mult_eps(const SegNfa& aut, const std::set<Symbol>& epsilons, bool include_empty) {
     Segmentation segmentation{ aut, epsilons };
     const auto& segments{ segmentation.get_untrimmed_segments() };
 
-    EpsCntMap def_eps_map;
+    VisitedEpsilonsCounterMap def_eps_map;
     for(const Symbol& eps : epsilons) {
         def_eps_map[eps] = 0;
     }
-    EpsCntVector def_eps_vector = process_eps_map(def_eps_map);
+    VisitedEpsilonsCounterVector def_eps_vector = process_eps_map(def_eps_map);
 
     if (segments.size() == 1) {
         std::shared_ptr<Nfa::Nfa> segment = std::make_shared<Nfa::Nfa>(segments[0]);
         segment->trim();
         if (segment->size() > 0 || include_empty) {
             return {{ {segment, def_eps_vector} } };
         } else {
@@ -203,15 +203,15 @@
     };
 
     NoodleSubstSequence noodles{};
     std::deque<SegItem> lifo;
 
     for(const State& fn : segments[0].final) {
         SegItem new_item;
-        Mata::Nfa::SharedPtrAut seg = segments_one_initial_final[{unused_state, fn}];
+        std::shared_ptr<Nfa::Nfa> seg = segments_one_initial_final[{unused_state, fn}];
         if(seg->final.size() != 1 || seg->get_num_of_trans() > 0) { // L(seg_iter) != {epsilon}
             new_item.noodle.emplace_back(seg, def_eps_vector);
         }
         new_item.seg_id = 0;
         new_item.fin = fn;
         lifo.push_back(new_item);
     }
@@ -255,35 +255,35 @@
                 lifo.push_back(new_item);
             }
         }
     }
     return noodles;
 }
 
-SegNfa::NoodleSequence SegNfa::noodlify_for_equation(const AutRefSequence& left_automata, const Nfa::Nfa& right_automaton,
-                                                     bool include_empty, const StringMap& params) {
-    const auto left_automata_begin{ left_automata.begin() };
-    const auto left_automata_end{ left_automata.end() };
-    for (auto left_aut_iter{ left_automata_begin }; left_aut_iter != left_automata_end;
-         ++left_aut_iter) {
-        (*left_aut_iter).get().unify_initial();
-        (*left_aut_iter).get().unify_final();
+SegNfa::NoodleSequence SegNfa::noodlify_for_equation(const std::vector<std::reference_wrapper<Nfa::Nfa>>& lhs_automata, const Nfa::Nfa& rhs_automaton,
+                                                     bool include_empty, const ParameterMap& params) {
+    const auto lhs_aut_begin{ lhs_automata.begin() };
+    const auto lhs_aut_end{ lhs_automata.end() };
+    for (auto lhs_aut_iter{ lhs_aut_begin }; lhs_aut_iter != lhs_aut_end;
+         ++lhs_aut_iter) {
+        (*lhs_aut_iter).get().unify_initial();
+        (*lhs_aut_iter).get().unify_final();
     }
 
-    if (left_automata.empty() || is_lang_empty(right_automaton)) { return NoodleSequence{}; }
+    if (lhs_automata.empty() || is_lang_empty(rhs_automaton)) { return NoodleSequence{}; }
 
     // Automaton representing the left side concatenated over epsilon transitions.
-    Nfa::Nfa concatenated_left_side{ *left_automata_begin };
-    for (auto next_left_automaton_it{ left_automata_begin + 1 }; next_left_automaton_it != left_automata_end;
-         ++next_left_automaton_it) {
-        concatenated_left_side = concatenate(concatenated_left_side, *next_left_automaton_it, EPSILON);
+    Nfa::Nfa concatenated_lhs{ *lhs_aut_begin };
+    for (auto next_lhs_aut_it{ lhs_aut_begin + 1 }; next_lhs_aut_it != lhs_aut_end;
+         ++next_lhs_aut_it) {
+        concatenated_lhs = concatenate(concatenated_lhs, *next_lhs_aut_it, EPSILON);
     }
 
     auto product_pres_eps_trans{
-            intersection(concatenated_left_side, right_automaton, true) };
+            intersection(concatenated_lhs, rhs_automaton, true) };
     product_pres_eps_trans.trim();
     if (is_lang_empty(product_pres_eps_trans)) {
         return NoodleSequence{};
     }
     if (Util::haskey(params, "reduce")) {
         const std::string& reduce_value = params.at("reduce");
         if (reduce_value == "forward" || reduce_value == "bidirectional") {
@@ -294,45 +294,45 @@
             product_pres_eps_trans = reduce(product_pres_eps_trans);
             product_pres_eps_trans = revert(product_pres_eps_trans);
         }
     }
     return noodlify(product_pres_eps_trans, EPSILON, include_empty);
 }
 
-SegNfa::NoodleSequence SegNfa::noodlify_for_equation(const AutPtrSequence& left_automata, const Nfa::Nfa& right_automaton,
-                                                     bool include_empty, const StringMap& params) {
-    const auto left_automata_begin{ left_automata.begin() };
-    const auto left_automata_end{ left_automata.end() };
+SegNfa::NoodleSequence SegNfa::noodlify_for_equation(const std::vector<Nfa::Nfa*>& lhs_automata, const Nfa::Nfa& rhs_automaton,
+                                                     bool include_empty, const ParameterMap& params) {
+    const auto lhs_aut_begin{ lhs_automata.begin() };
+    const auto lhs_aut_end{ lhs_automata.end() };
 
     std::string reduce_value{};
     if (Util::haskey(params, "reduce")) {
         reduce_value = params.at("reduce");
     }
 
     if (!reduce_value.empty()) {
         if (reduce_value == "forward" || reduce_value == "backward" || reduce_value == "bidirectional") {
-            for (auto left_aut_iter{ left_automata_begin }; left_aut_iter != left_automata_end;
-                 ++left_aut_iter) {
-                (*left_aut_iter)->unify_initial();
-                (*left_aut_iter)->unify_final();
+            for (auto lhs_aut_iter{ lhs_aut_begin }; lhs_aut_iter != lhs_aut_end;
+                 ++lhs_aut_iter) {
+                (*lhs_aut_iter)->unify_initial();
+                (*lhs_aut_iter)->unify_final();
             }
         }
     }
 
-    if (left_automata.empty() || is_lang_empty(right_automaton)) { return NoodleSequence{}; }
+    if (lhs_automata.empty() || is_lang_empty(rhs_automaton)) { return NoodleSequence{}; }
 
     // Automaton representing the left side concatenated over epsilon transitions.
-    Nfa::Nfa concatenated_left_side{ *(*left_automata_begin) };
-    for (auto next_left_automaton_it{ left_automata_begin + 1 }; next_left_automaton_it != left_automata_end;
-         ++next_left_automaton_it) {
-        concatenated_left_side = concatenate(concatenated_left_side, *(*next_left_automaton_it), EPSILON);
+    Nfa::Nfa concatenated_lhs{ *(*lhs_aut_begin) };
+    for (auto next_lhs_aut_it{ lhs_aut_begin + 1 }; next_lhs_aut_it != lhs_aut_end;
+         ++next_lhs_aut_it) {
+        concatenated_lhs = concatenate(concatenated_lhs, *(*next_lhs_aut_it), EPSILON);
     }
 
     auto product_pres_eps_trans{
-            intersection(concatenated_left_side, right_automaton, true) };
+            intersection(concatenated_lhs, rhs_automaton, true) };
     product_pres_eps_trans.trim();
     if (is_lang_empty(product_pres_eps_trans)) {
         return NoodleSequence{};
     }
     if (!reduce_value.empty()) {
         if (reduce_value == "forward" || reduce_value == "bidirectional") {
             product_pres_eps_trans = reduce(product_pres_eps_trans);
@@ -343,54 +343,54 @@
             product_pres_eps_trans = revert(product_pres_eps_trans);
         }
     }
     return noodlify(product_pres_eps_trans, EPSILON, include_empty);
 }
 
 
-SegNfa::NoodleSubstSequence SegNfa::noodlify_for_equation(const std::vector<std::shared_ptr<Nfa::Nfa>>& left_automata,
-    const std::vector<std::shared_ptr<Nfa::Nfa>>& right_automata, bool include_empty, const StringMap& params) {
-    if (left_automata.empty() || right_automata.empty()) { return NoodleSubstSequence{}; }
-
-    const auto left_automata_begin{ left_automata.begin() };
-    const auto left_automata_end{ left_automata.end() };
-    const auto right_automata_begin{ right_automata.begin() };
-    const auto right_automata_end{ right_automata.end() };
+SegNfa::NoodleSubstSequence SegNfa::noodlify_for_equation(const std::vector<std::shared_ptr<Nfa::Nfa>>& lhs_automata,
+    const std::vector<std::shared_ptr<Nfa::Nfa>>& rhs_automata, bool include_empty, const ParameterMap& params) {
+    if (lhs_automata.empty() || rhs_automata.empty()) { return NoodleSubstSequence{}; }
+
+    const auto lhs_aut_begin{ lhs_automata.begin() };
+    const auto lhs_aut_end{ lhs_automata.end() };
+    const auto rhs_aut_begin{ rhs_automata.begin() };
+    const auto rhs_aut_end{ rhs_automata.end() };
 
     std::unordered_set<std::shared_ptr<Nfa::Nfa>> unified_nfas; // Unify each automaton only once.
-    for (auto left_aut_iter{ left_automata_begin }; left_aut_iter != left_automata_end; ++left_aut_iter) {
-        if (unified_nfas.find(*left_aut_iter) == unified_nfas.end()) {
-            left_aut_iter->get()->unify_initial();
-            left_aut_iter->get()->unify_final();
-            unified_nfas.insert(*left_aut_iter);
+    for (auto lhs_aut_iter{ lhs_aut_begin }; lhs_aut_iter != lhs_aut_end; ++lhs_aut_iter) {
+        if (unified_nfas.find(*lhs_aut_iter) == unified_nfas.end()) {
+            lhs_aut_iter->get()->unify_initial();
+            lhs_aut_iter->get()->unify_final();
+            unified_nfas.insert(*lhs_aut_iter);
         }
     }
-    for (auto right_aut_iter{ right_automata_begin }; right_aut_iter != right_automata_end; ++right_aut_iter) {
-        if (unified_nfas.find(*right_aut_iter) == unified_nfas.end()) {
-            right_aut_iter->get()->unify_initial();
-            right_aut_iter->get()->unify_final();
-            unified_nfas.insert(*right_aut_iter);
+    for (auto rhs_aut_iter{ rhs_aut_begin }; rhs_aut_iter != rhs_aut_end; ++rhs_aut_iter) {
+        if (unified_nfas.find(*rhs_aut_iter) == unified_nfas.end()) {
+            rhs_aut_iter->get()->unify_initial();
+            rhs_aut_iter->get()->unify_final();
+            unified_nfas.insert(*rhs_aut_iter);
         }
     }
 
     // Automaton representing the left side concatenated over epsilon transitions.
-    Nfa::Nfa concatenated_left_side{ **left_automata_begin };
-    for (auto next_left_automaton_it{ left_automata_begin + 1 }; next_left_automaton_it != left_automata_end;
-         ++next_left_automaton_it) {
-        concatenated_left_side = concatenate_eps(concatenated_left_side, **next_left_automaton_it, EPSILON, true);
-    }
-    Nfa::Nfa concatenated_right_side{ **right_automata_begin };
-    for (auto next_right_automaton_it{ right_automata_begin + 1 }; next_right_automaton_it != right_automata_end;
-         ++next_right_automaton_it) {
-        concatenated_right_side = concatenate_eps(concatenated_right_side, **next_right_automaton_it, EPSILON-1, true); // we use EPSILON-1
+    Nfa::Nfa concatenated_lhs{ **lhs_aut_begin };
+    for (auto next_lhs_aut_it{ lhs_aut_begin + 1 }; next_lhs_aut_it != lhs_aut_end;
+         ++next_lhs_aut_it) {
+        concatenated_lhs = concatenate_eps(concatenated_lhs, **next_lhs_aut_it, EPSILON, true);
+    }
+    Nfa::Nfa concatenated_rhs{ **rhs_aut_begin };
+    for (auto next_rhs_aut_it{ rhs_aut_begin + 1 }; next_rhs_aut_it != rhs_aut_end;
+         ++next_rhs_aut_it) {
+        concatenated_rhs = concatenate_eps(concatenated_rhs, **next_rhs_aut_it, EPSILON-1, true); // we use EPSILON-1
     }
 
     const std::set<Symbol> epsilons({EPSILON, EPSILON-1});
     auto product_pres_eps_trans{
-            intersection_eps(concatenated_left_side, concatenated_right_side, true, epsilons) };
+            intersection_eps(concatenated_lhs, concatenated_rhs, true, epsilons) };
 
     product_pres_eps_trans.trim();
     if (is_lang_empty(product_pres_eps_trans)) {
         return NoodleSubstSequence{};
     }
     if (Util::haskey(params, "reduce")) {
         const std::string& reduce_value = params.at("reduce");
@@ -402,14 +402,14 @@
             product_pres_eps_trans = reduce(product_pres_eps_trans);
             product_pres_eps_trans = revert(product_pres_eps_trans);
         }
     }
     return noodlify_mult_eps(product_pres_eps_trans, epsilons, include_empty);
 }
 
-SegNfa::EpsCntVector SegNfa::process_eps_map(const EpsCntMap& eps_cnt) {
-    EpsCntVector ret;
+SegNfa::VisitedEpsilonsCounterVector SegNfa::process_eps_map(const VisitedEpsilonsCounterMap& eps_cnt) {
+    VisitedEpsilonsCounterVector ret;
     for(auto it = eps_cnt.rbegin(); it != eps_cnt.rend(); it++) {
         ret.push_back(it->second);
     }
     return ret;
 }
```

### Comparing `libmata-0.91.0/mata/src/strings/nfa-segmentation.cc` & `libmata-0.92.0/mata/src/strings/nfa-segmentation.cc`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 }
 
 void SegNfa::Segmentation::handle_epsilon_transitions(const StateDepthTuple& state_depth_pair,
                                                       const Move& move,
                                                       std::deque<StateDepthTuple>& worklist)
 {
     /// TODO: Maybe we don't need to keep the transitions in both structures
-    this->epsilon_depth_transitions.insert(std::make_pair(state_depth_pair.depth, TransSequence{}));
-    this->eps_depth_trans_map.insert({ state_depth_pair.depth, {{state_depth_pair.state, TransSequence{}}} });
+    this->epsilon_depth_transitions.insert(std::make_pair(state_depth_pair.depth, std::vector<Trans>{}));
+    this->eps_depth_trans_map.insert({ state_depth_pair.depth, {{state_depth_pair.state, std::vector<Trans>{}}} });
 
     std::map<Symbol, unsigned> visited_eps_aux(state_depth_pair.eps);
     visited_eps_aux[move.symbol]++;
 
     for (State target_state: move.targets)
     {
         this->epsilon_depth_transitions[state_depth_pair.depth].push_back(
@@ -91,23 +91,23 @@
         visited[state] = false;
     }
     return visited;
 }
 
 void SegNfa::Segmentation::split_aut_into_segments()
 {
-    segments_raw = AutSequence{ epsilon_depth_transitions.size() + 1, automaton };
+    segments_raw = { epsilon_depth_transitions.size() + 1, automaton };
     remove_inner_initial_and_final_states();
 
     // Construct segment automata.
-    std::unique_ptr<const TransSequence> depth_transitions{};
+    std::unique_ptr<const std::vector<Trans>> depth_transitions{};
     for (size_t depth{ 0 }; depth < epsilon_depth_transitions.size(); ++depth)
     {
         // Split the left segment from automaton into a new segment.
-        depth_transitions = std::make_unique<const TransSequence>(epsilon_depth_transitions[depth]);
+        depth_transitions = std::make_unique<const std::vector<Trans>>(epsilon_depth_transitions[depth]);
         for (const auto& transition: *depth_transitions)
         {
             update_current_segment(depth, transition);
             update_next_segment(depth, transition);
         }
     }
 }
@@ -143,25 +143,25 @@
     assert(segments_raw[next_depth].delta.contains(transition.src, transition.symb, transition.tgt));
 
     // we do not need to remove epsilon transitions in current_depth from the next segment (or the
     // segments after) as the initial states are after these transitions
     segments_raw[next_depth].initial.insert(transition.tgt);
 }
 
-const AutSequence& SegNfa::Segmentation::get_segments()
+const std::vector<Nfa>& SegNfa::Segmentation::get_segments()
 {
     if (segments.empty()) {
         get_untrimmed_segments();
         for (auto& seg_aut: segments_raw) { segments.push_back(seg_aut.get_trimmed_automaton()); }
     }
 
     return segments;
 }
 
-const AutSequence& SegNfa::Segmentation::get_untrimmed_segments()
+const std::vector<Nfa>& SegNfa::Segmentation::get_untrimmed_segments()
 {
     if (segments_raw.empty()) { split_aut_into_segments(); }
 
     return segments_raw;
 }
 
 void SegNfa::Segmentation::compute_epsilon_depths()
```

### Comparing `libmata-0.91.0/mata/src/strings/nfa-strings.cc` & `libmata-0.92.0/mata/src/strings/nfa-strings.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/CMakeLists.txt` & `libmata-0.92.0/mata/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/afa/afa.cc` & `libmata-0.92.0/mata/tests/afa/afa.cc`

 * *Files 2% similar despite different names*

```diff
@@ -466,20 +466,20 @@
 	REQUIRE(!antichain_concrete_backward_emptiness_test_new(aut2));
 }
 
 TEST_CASE("Mata::Afa::construct() from IntermediateAut correct calls")
 { // {{{
     Afa aut;
     Mata::IntermediateAut inter_aut;
-    Mata::StringToSymbolMap symbol_map;
+    Mata::OnTheFlyAlphabet alphabet;
 
     SECTION("construct an empty automaton")
     {
         inter_aut.automaton_type = Mata::IntermediateAut::AutomatonType::AFA;
-        aut = Mata::Afa::construct(inter_aut, &symbol_map);
+        aut = Mata::Afa::construct(inter_aut, &alphabet);
         REQUIRE(true);
     }
 
     SECTION("construct a simple non-empty automaton accepting the empty word from intermediate automaton")
     {
         std::string file =
                 "@AFA-explicit\n"
@@ -492,16 +492,15 @@
 
         aut = construct(inter_aut);
 
         REQUIRE(aut.initialstates.size() == 2);
         REQUIRE(aut.finalstates.size() == 2);
     }
 
-    SECTION("construct an automaton with more than one initial/final states from intermediate automaton")
-    {
+    SECTION("construct an automaton with more than one initial/final states from intermediate automaton") {
         std::string file =
                 "@AFA-explicit\n"
                 "%States-enum p q 3\n"
                 "%Alphabet-auto\n"
                 "%Initial p | q\n"
                 "%Final p & q & r\n";
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
@@ -555,15 +554,15 @@
                 "%Alphabet-auto\n"
                 "%Initial q1\n"
                 "%Final q2\n"
                 "q1 a & q2\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
-        construct(&aut, inter_aut, &symbol_map);
+        construct(&aut, inter_aut, &alphabet);
     }
 
     SECTION("construct a more complicated non-empty automaton from intermediate automaton")
     {
         std::string file =
                 "@AFA-explicit\n"
                 "%States-enum p q 3\n"
@@ -575,30 +574,30 @@
                 "q1 b & q3 & q4\n"
                 "q2 a & ((q3 & q4) | (q4 & q5) | (q3 & q6))\n"
                 "q3 a & ((q3 & q4) | (q4 & q5) | (q3 & q6 & q4) & q5)\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-        StringToStateMap state_map;
-        construct(&aut, inter_aut, &symbol_map, &state_map);
+        NameStateMap state_map;
+        construct(&aut, inter_aut, &alphabet, &state_map);
 
         REQUIRE(aut.trans_size() == 4);
-        REQUIRE(aut.get_trans_from_state(state_map["q1"], symbol_map["a"]).dst.size() == 3);
-        REQUIRE(aut.get_trans_from_state(state_map["q1"], symbol_map["a"]).dst.begin()->count(
+        REQUIRE(aut.get_trans_from_state(state_map["q1"], alphabet["a"]).dst.size() == 3);
+        REQUIRE(aut.get_trans_from_state(state_map["q1"], alphabet["a"]).dst.begin()->count(
                 state_map["q1"]));
-        REQUIRE(aut.get_trans_from_state(state_map["q1"], symbol_map["a"]).dst.begin()->count(
+        REQUIRE(aut.get_trans_from_state(state_map["q1"], alphabet["a"]).dst.begin()->count(
                 state_map["q3"]));
-        REQUIRE(aut.get_trans_from_state(state_map["q1"], symbol_map["b"]).dst.size() == 1);
-        REQUIRE(aut.get_trans_from_state(state_map["q1"], symbol_map["b"]).dst.begin()->count(
+        REQUIRE(aut.get_trans_from_state(state_map["q1"], alphabet["b"]).dst.size() == 1);
+        REQUIRE(aut.get_trans_from_state(state_map["q1"], alphabet["b"]).dst.begin()->count(
                 state_map["q3"]));
-        REQUIRE(aut.get_trans_from_state(state_map["q1"], symbol_map["b"]).dst.begin()->count(
+        REQUIRE(aut.get_trans_from_state(state_map["q1"], alphabet["b"]).dst.begin()->count(
                 state_map["q4"]));
-        REQUIRE(aut.get_trans_from_state(state_map["q2"], symbol_map["a"]).dst.size() == 3);
-        REQUIRE(aut.get_trans_from_state(state_map["q3"], symbol_map["a"]).dst.size() == 2);
+        REQUIRE(aut.get_trans_from_state(state_map["q2"], alphabet["a"]).dst.size() == 3);
+        REQUIRE(aut.get_trans_from_state(state_map["q3"], alphabet["a"]).dst.size() == 2);
     }
 
     SECTION("Initial formula in DNF")
     {
         std::string file =
                 "@AFA-explicit\n"
                 "%Initial qQC0_0 | (qQC0_1 & qQC1_1 & qQC1_0) \n"
@@ -608,16 +607,16 @@
                 "qQC0_2 a\n"
                 "qQC1_0 a & qQC1_1\n"
                 "qQC0_0 a & (qQC0_2 | qQC0_1)\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-        StringToStateMap state_map;
-        construct(&aut, inter_aut, &symbol_map, &state_map);
+        NameStateMap state_map;
+        construct(&aut, inter_aut, &alphabet, &state_map);
 
         REQUIRE(aut.initialstates.size() == 2);
         auto it = aut.initialstates.begin();
         REQUIRE(it->count(state_map["QC0_1"]));
         REQUIRE(it->count(state_map["QC1_1"]));
         REQUIRE(it->count(state_map["QC1_0"]));
         ++it;
@@ -634,16 +633,16 @@
                 "q1 a2 & (q2 & q3)\n"
                 "q2 a2 & (q0 & q3)\n"
                 "q3 a1 & (q0 | q2)\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-        StringToStateMap state_map;
-        construct(&aut, inter_aut, &symbol_map, &state_map);
+        NameStateMap state_map;
+        construct(&aut, inter_aut, &alphabet, &state_map);
 
         // Two initial nodes {q1} and {q2}
         REQUIRE(aut.initialstates.size() == 2);
         REQUIRE(!antichain_concrete_forward_emptiness_test_new(aut));
     }
 
     SECTION("AFA with a simple initial formula, just conjunction")
@@ -656,16 +655,16 @@
                 "q1 a2 & (q2 & q3)\n"
                 "q2 a2 & (q0 & q3)\n"
                 "q3 a1 & (q0 | q2)\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-        StringToStateMap state_map;
-        construct(&aut, inter_aut, &symbol_map, &state_map);
+        NameStateMap state_map;
+        construct(&aut, inter_aut, &alphabet, &state_map);
 
         // One initial node {q1, q2}
         REQUIRE(aut.initialstates.size() == 1);
         REQUIRE(antichain_concrete_forward_emptiness_test_new(aut));
     }
 
     SECTION("AFA final states from multiple negations")
@@ -678,26 +677,25 @@
                 "q1 a2 & q2\n"
                 "q2 a1 & (q3 | q2)\n"
                 "q2 a2 & (q4 & q1)\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-        StringToStateMap state_map;
-        construct(&aut, inter_aut, &symbol_map, &state_map);
+        NameStateMap state_map;
+        construct(&aut, inter_aut, &alphabet, &state_map);
 
         CHECK(aut.finalstates.size() == 2);
 		CHECK(aut.finalstates.count(state_map.at("2")));
 		CHECK(aut.finalstates.count(state_map.at("4")));
 
     }
 
 } // }}}
 
-/*
 TEST_CASE("Mata::Afa::construct() correct calls")
 { // {{{
 	Afa aut;
 	Mata::Parser::ParsedSection parsec;
 
 	SECTION("construct an empty automaton")
 	{
@@ -736,8 +734,8 @@
 		parsec.type = Mata::Afa::TYPE_AFA;
 		parsec.dict.insert({"Initial", {"q1"}});
 		parsec.dict.insert({"Final", {"q2"}});
 		parsec.body = { {"q1", "a AND q2"} };
 
 		construct(&aut, parsec);
 	}
-} // }}} */
+}
```

### Comparing `libmata-0.91.0/mata/tests/alphabet.cc` & `libmata-0.92.0/mata/tests/alphabet.cc`

 * *Files 6% similar despite different names*

```diff
@@ -34,33 +34,29 @@
     OnTheFlyAlphabet different_alphabet2{};
     CHECK(!alphabet1.is_equal(different_alphabet));
     CHECK(!different_alphabet.is_equal(different_alphabet2));
     CHECK(different_alphabet.is_equal(&different_alphabet));
 }
 
 TEST_CASE("Mata::OnTheFlyAlphabet::add_symbols_from()") {
-    OnTheFlyAlphabet alphabet{};
-    StringToSymbolMap symbol_map{ { "a", 4 }, { "b", 2 }, { "c", 10 } };
-    alphabet.add_symbols_from(symbol_map);
-
-    auto symbols{alphabet.get_alphabet_symbols() };
+    OnTheFlyAlphabet alphabet{ { "a", 4 }, { "b", 2 }, { "c", 10 } };
+    auto symbols{ alphabet.get_alphabet_symbols() };
     Mata::Util::OrdVector<Symbol> expected{ 4, 2, 10 };
     CHECK(symbols == expected);
     CHECK(alphabet.get_next_value() == 11);
-    CHECK(alphabet.get_symbol_map() == symbol_map);
+    CHECK(alphabet.get_symbol_map() == OnTheFlyAlphabet::StringToSymbolMap{ { "a", 4 }, { "b", 2 }, { "c", 10 } });
 
-    symbol_map["a"] = 6;
-    symbol_map["e"] = 7;
-    alphabet.add_symbols_from(symbol_map);
+    alphabet.add_new_symbol("e", 7);
+    CHECK_THROWS_AS(alphabet.add_new_symbol("a", 0), std::runtime_error);
 
     symbols = alphabet.get_alphabet_symbols();
     expected = Mata::Util::OrdVector<Symbol>{ 7, 4, 2, 10 };
     CHECK(symbols == expected);
     CHECK(alphabet.get_next_value() == 11);
-    CHECK(alphabet.get_symbol_map() == StringToSymbolMap{
+    CHECK(alphabet.get_symbol_map() == OnTheFlyAlphabet::StringToSymbolMap {
         { "a", 4 }, { "b", 2 }, { "c", 10 }, { "e", 7 }
     });
 }
 
 TEST_CASE("Mata::EnumAlphabet") {
     EnumAlphabet alphabet{};
     EnumAlphabet alphabet2{ 1, 2, 3, 4, 5 };
```

### Comparing `libmata-0.91.0/mata/tests/main.cc` & `libmata-0.92.0/mata/tests/main.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/mintermization.cc` & `libmata-0.92.0/mata/tests/mintermization.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/nfa/builder.cc` & `libmata-0.92.0/mata/tests/nfa/builder.cc`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 #include <fstream>
 
 #include "../3rdparty/catch.hpp"
 
 #include "mata/nfa/nfa.hh"
 #include "mata/nfa/builder.hh"
 
+using namespace Mata::Nfa;
 using Symbol = Mata::Symbol;
 using IntAlphabet = Mata::IntAlphabet;
 using OnTheFlyAlphabet = Mata::OnTheFlyAlphabet;
-using StringToSymbolMap = Mata::StringToSymbolMap;
 
 using Word = std::vector<Symbol>;
 
 TEST_CASE("parse_from_mata()") {
     Delta delta;
 
     SECTION("Simple automaton") {
```

### Comparing `libmata-0.91.0/mata/tests/nfa/nfa-concatenation.cc` & `libmata-0.92.0/mata/tests/nfa/nfa-concatenation.cc`

 * *Files 4% similar despite different names*

```diff
@@ -522,19 +522,19 @@
         lhs.final.insert(1);
         lhs.delta.add(0, 'b', 1);
         rhs.add_state();
         rhs.initial.insert(0);
         rhs.final.insert(0);
         rhs.delta.add(0, 'a', 0);
 
-        StateToStateMap lhs_map{};
-        StateToStateMap rhs_map{};
-        result = concatenate(lhs, rhs, true, &lhs_map, &rhs_map);
+        StateRenaming lhs_renaming{};
+        StateRenaming rhs_renaming{};
+        result = concatenate(lhs, rhs, true, &lhs_renaming, &rhs_renaming);
 
-        CHECK(rhs_map == StateToStateMap{ { 0, 2 } });
+        CHECK(rhs_renaming == StateRenaming{{ 0, 2 } });
 
         CHECK(result.initial[0]);
         CHECK(result.final[2]);
         CHECK(result.size() == 3);
         CHECK(result.get_num_of_trans() == 3);
         CHECK(result.delta.contains(0, 'b', 1));
         CHECK(result.delta.contains(2, 'a', 2));
```

### Comparing `libmata-0.91.0/mata/tests/nfa/nfa-intersection.cc` & `libmata-0.92.0/mata/tests/nfa/nfa-intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/nfa/nfa-profiling.cc` & `libmata-0.92.0/mata/tests/nfa/nfa-profiling.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/nfa/nfa-util.hh` & `libmata-0.92.0/mata/tests/nfa/nfa-util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/nfa/nfa.cc` & `libmata-0.92.0/mata/tests/nfa/nfa.cc`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,17 @@
 using namespace Mata::Strings;
 using namespace Mata::Nfa::Plumbing;
 using namespace Mata::Util;
 using namespace Mata::Parser;
 using Symbol = Mata::Symbol;
 using IntAlphabet = Mata::IntAlphabet;
 using OnTheFlyAlphabet = Mata::OnTheFlyAlphabet;
-using StringToSymbolMap = Mata::StringToSymbolMap;
 
 using Word = std::vector<Symbol>;
 
-template<class T> void unused(const T &) {}
-
 TEST_CASE("Mata::Nfa::size()") {
     Nfa nfa{};
     CHECK(nfa.size() == 0);
 
     nfa.add_state(3);
     CHECK(nfa.size() == 4);
 
@@ -47,22 +44,18 @@
     FILL_WITH_AUT_B(nfa);
     CHECK(nfa.size() == 15);
 
     nfa = Nfa{ 0, {}, {} };
     CHECK(nfa.size() == 0);
 }
 
-/*
-TEST_CASE("Mata::Nfa::Trans::operator<<")
-{ // {{{
-	Trans trans(1, 2, 3);
-
-	REQUIRE(std::to_string(trans) == "(1, 2, 3)");
-} // }}}
-*/
+TEST_CASE("Mata::Nfa::Trans::operator<<") {
+    Trans trans(1, 2, 3);
+    REQUIRE(std::to_string(trans) == "(1, 2, 3)");
+}
 
 TEST_CASE("Mata::Nfa::create_alphabet()") {
     Nfa a{1};
     a.delta.add(0, 'a', 0);
 
     Nfa b{1};
     b.delta.add(0, 'b', 0);
@@ -77,504 +70,350 @@
 
     //Mata::Nfa::create_alphabet(1, 3, 4); // Will not compile: '1', '3', '4' are not of the required type.
     //Mata::Nfa::create_alphabet(a, b, 4); // Will not compile: '4' is not of the required type.
 }
 
 TEST_CASE("Mata::Nfa::Nfa::delta.add()/delta.contains()")
 { // {{{
-	Nfa a(3);
+    Nfa a(3);
 
-	SECTION("Empty automata have now transitions")
-	{
-		REQUIRE(!a.delta.contains(1, 'a', 1));
-	}
-
-	SECTION("If I add a transition, it is in the automaton")
-	{
-		a.delta.add(1, 'a', 1);
-
-		REQUIRE(a.delta.contains(1, 'a', 1));
-	}
-
-	SECTION("If I add a transition, only it is added")
-	{
-		a.delta.add(1, 'a', 1);
-
-		REQUIRE(a.delta.contains(1, 'a', 1));
-		REQUIRE(!a.delta.contains(1, 'a', 2));
-		REQUIRE(!a.delta.contains(1, 'b', 2));
-		REQUIRE(!a.delta.contains(2, 'a', 1));
-	}
-
-	SECTION("Adding multiple transitions")
-	{
-		a.delta.add(2, 'b', {2,1,0});
-		REQUIRE(a.delta.contains(2, 'b', 0));
-		REQUIRE(a.delta.contains(2, 'b', 1));
-		REQUIRE(a.delta.contains(2, 'b', 2));
-		REQUIRE(!a.delta.contains(0, 'b', 0));
-
-		a.delta.add(0, 'b', StateSet({0}));
-		REQUIRE(a.delta.contains(0, 'b', 0));
-	}
+    SECTION("Empty automata have now transitions")
+    {
+        REQUIRE(!a.delta.contains(1, 'a', 1));
+    }
+
+    SECTION("If I add a transition, it is in the automaton")
+    {
+        a.delta.add(1, 'a', 1);
+
+        REQUIRE(a.delta.contains(1, 'a', 1));
+    }
+
+    SECTION("If I add a transition, only it is added")
+    {
+        a.delta.add(1, 'a', 1);
+
+        REQUIRE(a.delta.contains(1, 'a', 1));
+        REQUIRE(!a.delta.contains(1, 'a', 2));
+        REQUIRE(!a.delta.contains(1, 'b', 2));
+        REQUIRE(!a.delta.contains(2, 'a', 1));
+    }
+
+    SECTION("Adding multiple transitions")
+    {
+        a.delta.add(2, 'b', {2,1,0});
+        REQUIRE(a.delta.contains(2, 'b', 0));
+        REQUIRE(a.delta.contains(2, 'b', 1));
+        REQUIRE(a.delta.contains(2, 'b', 2));
+        REQUIRE(!a.delta.contains(0, 'b', 0));
+
+        a.delta.add(0, 'b', StateSet({0}));
+        REQUIRE(a.delta.contains(0, 'b', 0));
+    }
 
 } // }}}
 
 TEST_CASE("Mata::Nfa::Delta.transform/append")
 { // {{{
-	Nfa a(3);
-	a.delta.add(1, 'a', 1);
-	a.delta.add(2, 'b', {2,1,0});
-
-	SECTION("transform")
-	{
-		auto upd_fnc = [&](State st) {
-			return st + 5;
-		};
-		std::vector<Post> posts = a.delta.transform(upd_fnc);
-		a.delta.append(posts);
-
-		REQUIRE(a.delta.contains(4, 'a', 6));
-		REQUIRE(a.delta.contains(5, 'b', 7));
-		REQUIRE(a.delta.contains(5, 'b', 5));
-		REQUIRE(a.delta.contains(5, 'b', 6));
-	}
+    Nfa a(3);
+    a.delta.add(1, 'a', 1);
+    a.delta.add(2, 'b', {2,1,0});
+
+    SECTION("transform")
+    {
+        auto upd_fnc = [&](State st) {
+            return st + 5;
+        };
+        std::vector<Post> posts = a.delta.transform(upd_fnc);
+        a.delta.append(posts);
+
+        REQUIRE(a.delta.contains(4, 'a', 6));
+        REQUIRE(a.delta.contains(5, 'b', 7));
+        REQUIRE(a.delta.contains(5, 'b', 5));
+        REQUIRE(a.delta.contains(5, 'b', 6));
+    }
 
 } // }}}
 
 TEST_CASE("Mata::Nfa::Nfa iteration")
 { // {{{
-	Nfa aut;
+    Nfa aut;
 
-	SECTION("empty automaton")
-	{
-		auto it = aut.begin();
-		REQUIRE(it == aut.end());
-	}
+    SECTION("empty automaton")
+    {
+        auto it = aut.begin();
+        REQUIRE(it == aut.end());
+    }
 
     const size_t state_num = 'r'+1;
     aut.delta.increase_size(state_num);
 
-	SECTION("a non-empty automaton")
-	{
-		aut.delta.add('q', 'a', 'r');
-		aut.delta.add('q', 'b', 'r');
-		auto it = aut.delta.begin();
-		auto jt = aut.delta.begin();
-		REQUIRE(it == jt);
-		++it;
-		REQUIRE(it != jt);
-		REQUIRE((it != aut.delta.begin() && it != aut.delta.end()));
-		REQUIRE(jt == aut.delta.begin());
-
-		++jt;
-		REQUIRE(it == jt);
-		REQUIRE((jt != aut.delta.begin() && jt != aut.delta.end()));
+    SECTION("a non-empty automaton")
+    {
+        aut.delta.add('q', 'a', 'r');
+        aut.delta.add('q', 'b', 'r');
+        auto it = aut.delta.begin();
+        auto jt = aut.delta.begin();
+        REQUIRE(it == jt);
+        ++it;
+        REQUIRE(it != jt);
+        REQUIRE((it != aut.delta.begin() && it != aut.delta.end()));
+        REQUIRE(jt == aut.delta.begin());
+
+        ++jt;
+        REQUIRE(it == jt);
+        REQUIRE((jt != aut.delta.begin() && jt != aut.delta.end()));
 
         jt = aut.delta.end();
-		REQUIRE(it != jt);
-		REQUIRE((jt != aut.delta.begin() && jt == aut.delta.end()));
+        REQUIRE(it != jt);
+        REQUIRE((jt != aut.delta.begin() && jt == aut.delta.end()));
 
         it = aut.delta.end();
-		REQUIRE(it == jt);
-		REQUIRE((it != aut.delta.begin() && it == aut.delta.end()));
-	}
+        REQUIRE(it == jt);
+        REQUIRE((it != aut.delta.begin() && it == aut.delta.end()));
+    }
 } // }}}
 
-/*
-TEST_CASE("Mata::Nfa::are_state_disjoint()")
+TEST_CASE("Mata::Nfa::is_lang_empty()")
 { // {{{
-	Nfa a(50), b(50);
+    Nfa aut(14);
+    Run cex;
 
-	SECTION("Empty automata are state disjoint")
-	{
-		REQUIRE(are_state_disjoint(a, b));
-	}
-
-	SECTION("Left-hand side empty automaton is state disjoint with anything")
-	{
-		b.initial = {1, 4, 6};
-		b.final = {4, 7, 9, 0};
-		b.delta.add(1, 'a', 1);
-		b.delta.add(2, 'a', 8);
-		b.delta.add(0, 'c', 49);
-
-		REQUIRE(are_state_disjoint(a, b));
-	}
-
-	SECTION("Right-hand side empty automaton is state disjoint with anything")
-	{
-		a.initial = {1, 4, 6};
-		a.final = {4, 7, 9, 0};
-		a.delta.add(1, 'a', 1);
-		a.delta.add(2, 'a', 8);
-		a.delta.add(0, 'c', 49);
-
-		REQUIRE(are_state_disjoint(a, b));
-	}
-
-	SECTION("Automata with intersecting initial states are not state disjoint")
-	{
-		a.initial = {1, 4, 6};
-		b.initial = {3, 9, 6, 8};
-
-		REQUIRE(!are_state_disjoint(a, b));
-	}
-
-	SECTION("Automata with intersecting final states are not state disjoint")
-	{
-		a.final = {1, 4, 6};
-		b.final = {3, 9, 6, 8};
-
-		REQUIRE(!are_state_disjoint(a, b));
-	}
-
-	SECTION("Automata with disjoint sets of states are state disjoint")
-	{
-		a.initial = {0, 5, 16};
-		a.final = {1, 4, 6};
-
-		b.initial = {11, 3};
-		b.final = {3, 9, 8};
-
-		a.delta.add(1, 'a', 7);
-		a.delta.add(1, 'b', 7);
-		b.delta.add(3, 'b', 11);
-		b.delta.add(3, 'b', 9);
-
-		REQUIRE(are_state_disjoint(a, b));
-	}
-
-	SECTION("Automata with intersecting states are not disjoint")
-	{
-		a.initial = {0, 5, 16};
-		a.final = {1, 4};
-
-		b.initial = {11, 3};
-		b.final = {3, 9, 6, 8};
-
-		a.delta.add(1, 'a', 7);
-		a.delta.add(1, 'b', 7);
-		a.delta.add(1, 'c', 7);
-		b.delta.add(3, 'c', 11);
-		b.delta.add(3, 'c', 5);
-		b.delta.add(11, 'a', 3);
+    SECTION("An empty automaton has an empty language")
+    {
+        REQUIRE(is_lang_empty(aut));
+    }
 
-		REQUIRE(!are_state_disjoint(a, b));
-	}
-} // }}}
+    SECTION("An automaton with a state that is both initial and final does not have an empty language")
+    {
+        aut.initial = {1, 2};
+        aut.final = {2, 3};
 
-TEST_CASE("Mata::Nfa::union_norename()")
-{ // {{{
-	Nfa a(7), b(7), res;
+        bool is_empty = is_lang_empty(aut, &cex);
+        REQUIRE(!is_empty);
+    }
 
-	SECTION("Union of empty automata")
-	{
-		union_norename(&res, a, b);
-
-		REQUIRE(res.initial.empty());
-		REQUIRE(res.final.empty());
-		REQUIRE(res.delta.empty());
-	}
-
-	SECTION("Union of automata with no transitions")
-	{
-		a.initial = {1, 3};
-		a.final = {3, 5};
-
-		b.initial = {4, 6};
-		b.final = {4, 2};
-
-		union_norename(&res, a, b);
-
-		REQUIRE(!res.initial.empty());
-		REQUIRE(!res.final.empty());
-
-		REQUIRE(res.initial[1]);
-		REQUIRE(res.initial[3]);
-		REQUIRE(res.initial[4]);
-		REQUIRE(res.initial[6]);
-		REQUIRE(res.final[3]);
-		REQUIRE(res.final[5]);
-		REQUIRE(res.final[4]);
-		REQUIRE(res.final[2]);
-	}
-
-	SECTION("Union of automata with some transitions")
-	{
-		FILL_WITH_AUT_A(a);
-		FILL_WITH_AUT_B(b);
-
-		union_norename(&res, a, b);
-
-		OnTheFlyAlphabet alph{"a", "b"};
-		StringMap params;
-		params["algorithm"] = "antichains";
-
-		REQUIRE(is_included(a, res, &alph, params));
-		REQUIRE(is_included(b, res, &alph, params));
-	}
-
-	SECTION("Union of automata with some transitions but without a final state")
-	{
-		FILL_WITH_AUT_A(a);
-		FILL_WITH_AUT_B(b);
-		b.final = {};
-
-		union_norename(&res, a, b);
-
-		OnTheFlyAlphabet alph{"a", "b"};
-		StringMap params;
-		params["algorithm"] = "antichains";
+    SECTION("More complicated automaton")
+    {
+        aut.initial = {1, 2};
+        aut.delta.add(1, 'a', 2);
+        aut.delta.add(1, 'a', 3);
+        aut.delta.add(1, 'b', 4);
+        aut.delta.add(2, 'a', 2);
+        aut.delta.add(2, 'a', 3);
+        aut.delta.add(2, 'b', 4);
+        aut.delta.add(3, 'b', 4);
+        aut.delta.add(3, 'c', 7);
+        aut.delta.add(3, 'b', 2);
+        aut.delta.add(7, 'a', 8);
 
-		REQUIRE(is_included(a, res, &alph, params));
-		REQUIRE(is_included(res, a, &alph, params));
+        SECTION("with final states")
+        {
+            aut.final = {7};
+            REQUIRE(!is_lang_empty(aut));
+        }
 
-		WARN_PRINT("Insufficient testing of Mata::Nfa::union_norename()");
-	}
-} // }}}
-*/
+        SECTION("without final states")
+        {
+            REQUIRE(is_lang_empty(aut));
+        }
 
-TEST_CASE("Mata::Nfa::is_lang_empty()")
-{ // {{{
-	Nfa aut(14);
-	Run cex;
+        SECTION("another complicated automaton")
+        {
+            FILL_WITH_AUT_A(aut);
+
+            REQUIRE(!is_lang_empty(aut));
+        }
+
+        SECTION("a complicated automaton with unreachable final states")
+        {
+            FILL_WITH_AUT_A(aut);
+            aut.final = {13};
+
+            REQUIRE(is_lang_empty(aut));
+        }
+    }
+
+    SECTION("An automaton with a state that is both initial and final does not have an empty language")
+    {
+        aut.initial = {1, 2};
+        aut.final = {2, 3};
 
-	SECTION("An empty automaton has an empty language")
-	{
-		REQUIRE(is_lang_empty(aut));
-	}
-
-	SECTION("An automaton with a state that is both initial and final does not have an empty language")
-	{
-		aut.initial = {1, 2};
-		aut.final = {2, 3};
-
-		bool is_empty = is_lang_empty(aut, &cex);
-		REQUIRE(!is_empty);
-	}
-
-	SECTION("More complicated automaton")
-	{
-		aut.initial = {1, 2};
-		aut.delta.add(1, 'a', 2);
-		aut.delta.add(1, 'a', 3);
-		aut.delta.add(1, 'b', 4);
-		aut.delta.add(2, 'a', 2);
-		aut.delta.add(2, 'a', 3);
-		aut.delta.add(2, 'b', 4);
-		aut.delta.add(3, 'b', 4);
-		aut.delta.add(3, 'c', 7);
-		aut.delta.add(3, 'b', 2);
-		aut.delta.add(7, 'a', 8);
-
-		SECTION("with final states")
-		{
-			aut.final = {7};
-			REQUIRE(!is_lang_empty(aut));
-		}
-
-		SECTION("without final states")
-		{
-			REQUIRE(is_lang_empty(aut));
-		}
-
-		SECTION("another complicated automaton")
-		{
-			FILL_WITH_AUT_A(aut);
-
-			REQUIRE(!is_lang_empty(aut));
-		}
-
-		SECTION("a complicated automaton with unreachable final states")
-		{
-			FILL_WITH_AUT_A(aut);
-			aut.final = {13};
-
-			REQUIRE(is_lang_empty(aut));
-		}
-	}
-
-	SECTION("An automaton with a state that is both initial and final does not have an empty language")
-	{
-		aut.initial = {1, 2};
-		aut.final = {2, 3};
-
-		bool is_empty = is_lang_empty(aut, &cex);
-		REQUIRE(!is_empty);
-
-		// check the counterexample
-		REQUIRE(cex.path.size() == 1);
-		REQUIRE(cex.path[0] == 2);
-	}
-
-	SECTION("Counterexample of an automaton with non-empty language")
-	{
-		aut.initial = {1, 2};
-		aut.final = {8, 9};
-		aut.delta.add(1, 'c', 2);
-		aut.delta.add(2, 'a', 4);
-		aut.delta.add(2, 'c', 1);
-		aut.delta.add(2, 'c', 3);
-		aut.delta.add(3, 'e', 5);
-		aut.delta.add(4, 'c', 8);
-
-		bool is_empty = is_lang_empty(aut, &cex);
-		REQUIRE(!is_empty);
-
-		// check the counterexample
-		REQUIRE(cex.path.size() == 3);
-		REQUIRE(cex.path[0] == 2);
-		REQUIRE(cex.path[1] == 4);
-		REQUIRE(cex.path[2] == 8);
-	}
+        bool is_empty = is_lang_empty(aut, &cex);
+        REQUIRE(!is_empty);
+
+        // check the counterexample
+        REQUIRE(cex.path.size() == 1);
+        REQUIRE(cex.path[0] == 2);
+    }
+
+    SECTION("Counterexample of an automaton with non-empty language")
+    {
+        aut.initial = {1, 2};
+        aut.final = {8, 9};
+        aut.delta.add(1, 'c', 2);
+        aut.delta.add(2, 'a', 4);
+        aut.delta.add(2, 'c', 1);
+        aut.delta.add(2, 'c', 3);
+        aut.delta.add(3, 'e', 5);
+        aut.delta.add(4, 'c', 8);
+
+        bool is_empty = is_lang_empty(aut, &cex);
+        REQUIRE(!is_empty);
+
+        // check the counterexample
+        REQUIRE(cex.path.size() == 3);
+        REQUIRE(cex.path[0] == 2);
+        REQUIRE(cex.path[1] == 4);
+        REQUIRE(cex.path[2] == 8);
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::get_word_for_path()")
 { // {{{
-	Nfa aut(5);
-	Run path;
-	Word word;
-
-	SECTION("empty word")
-	{
-		path = { };
-
-		auto word_bool_pair = get_word_for_path(aut, path);
-		REQUIRE(word_bool_pair.second);
-		REQUIRE(word_bool_pair.first.word.empty());
-	}
-
-	SECTION("empty word 2")
-	{
-		aut.initial = {1};
-		path.path = {1};
-
-		auto word_bool_pair = get_word_for_path(aut, path);
-		REQUIRE(word_bool_pair.second);
-		REQUIRE(word_bool_pair.first.word.empty());
-	}
-
-	SECTION("nonempty word")
-	{
-		aut.initial = {1};
-		aut.delta.add(1, 'c', 2);
-		aut.delta.add(2, 'a', 4);
-		aut.delta.add(2, 'c', 1);
-		aut.delta.add(2, 'b', 3);
+    Nfa aut(5);
+    Run path;
+    Word word;
+
+    SECTION("empty word")
+    {
+        path = { };
+
+        auto word_bool_pair = get_word_for_path(aut, path);
+        REQUIRE(word_bool_pair.second);
+        REQUIRE(word_bool_pair.first.word.empty());
+    }
+
+    SECTION("empty word 2")
+    {
+        aut.initial = {1};
+        path.path = {1};
+
+        auto word_bool_pair = get_word_for_path(aut, path);
+        REQUIRE(word_bool_pair.second);
+        REQUIRE(word_bool_pair.first.word.empty());
+    }
+
+    SECTION("nonempty word")
+    {
+        aut.initial = {1};
+        aut.delta.add(1, 'c', 2);
+        aut.delta.add(2, 'a', 4);
+        aut.delta.add(2, 'c', 1);
+        aut.delta.add(2, 'b', 3);
 
         path.path = {1,2,3};
 
-		auto word_bool_pair = get_word_for_path(aut, path);
-		REQUIRE(word_bool_pair.second);
-		REQUIRE(word_bool_pair.first.word == Word({'c', 'b'}));
-	}
-
-	SECTION("longer word")
-	{
-		aut.initial = {1};
-		aut.delta.add(1, 'a', 2);
-		aut.delta.add(1, 'c', 2);
-		aut.delta.add(2, 'a', 4);
-		aut.delta.add(2, 'c', 1);
-		aut.delta.add(2, 'b', 3);
-		aut.delta.add(3, 'd', 2);
+        auto word_bool_pair = get_word_for_path(aut, path);
+        REQUIRE(word_bool_pair.second);
+        REQUIRE(word_bool_pair.first.word == Word({'c', 'b'}));
+    }
+
+    SECTION("longer word")
+    {
+        aut.initial = {1};
+        aut.delta.add(1, 'a', 2);
+        aut.delta.add(1, 'c', 2);
+        aut.delta.add(2, 'a', 4);
+        aut.delta.add(2, 'c', 1);
+        aut.delta.add(2, 'b', 3);
+        aut.delta.add(3, 'd', 2);
 
         path.path = {1,2,3,2,4};
 
-		auto word_bool_pair = get_word_for_path(aut, path);
-		std::set<Word> possible({
-			Word({'c', 'b', 'd', 'a'}),
-			Word({'a', 'b', 'd', 'a'})});
-		REQUIRE(word_bool_pair.second);
-		REQUIRE(haskey(possible, word_bool_pair.first.word));
-	}
-
-	SECTION("invalid path")
-	{
-		aut.initial = {1};
-		aut.delta.add(1, 'a', 2);
-		aut.delta.add(1, 'c', 2);
-		aut.delta.add(2, 'a', 4);
-		aut.delta.add(2, 'c', 1);
-		aut.delta.add(2, 'b', 3);
-		aut.delta.add(3, 'd', 2);
-
-		path.path = {1,2,3,1,2};
-
-		auto word_bool_pair = get_word_for_path(aut, path);
-		REQUIRE(!word_bool_pair.second);
-	}
+        auto word_bool_pair = get_word_for_path(aut, path);
+        std::set<Word> possible({
+            Word({'c', 'b', 'd', 'a'}),
+            Word({'a', 'b', 'd', 'a'})});
+        REQUIRE(word_bool_pair.second);
+        REQUIRE(haskey(possible, word_bool_pair.first.word));
+    }
+
+    SECTION("invalid path")
+    {
+        aut.initial = {1};
+        aut.delta.add(1, 'a', 2);
+        aut.delta.add(1, 'c', 2);
+        aut.delta.add(2, 'a', 4);
+        aut.delta.add(2, 'c', 1);
+        aut.delta.add(2, 'b', 3);
+        aut.delta.add(3, 'd', 2);
+
+        path.path = {1,2,3,1,2};
+
+        auto word_bool_pair = get_word_for_path(aut, path);
+        REQUIRE(!word_bool_pair.second);
+    }
 }
 
 
 TEST_CASE("Mata::Nfa::is_lang_empty_cex()")
 {
-	Nfa aut(10);
-	Run cex;
+    Nfa aut(10);
+    Run cex;
 
-	SECTION("Counterexample of an automaton with non-empty language")
-	{
-		aut.initial = {1, 2};
-		aut.final = {8, 9};
-		aut.delta.add(1, 'c', 2);
-		aut.delta.add(2, 'a', 4);
-		aut.delta.add(2, 'c', 1);
-		aut.delta.add(2, 'c', 3);
-		aut.delta.add(3, 'e', 5);
-		aut.delta.add(4, 'c', 8);
-
-		bool is_empty = is_lang_empty(aut, &cex);
-		REQUIRE(!is_empty);
-
-		// check the counterexample
-		REQUIRE(cex.word.size() == 2);
-		REQUIRE(cex.word[0] == 'a');
-		REQUIRE(cex.word[1] == 'c');
-	}
+    SECTION("Counterexample of an automaton with non-empty language")
+    {
+        aut.initial = {1, 2};
+        aut.final = {8, 9};
+        aut.delta.add(1, 'c', 2);
+        aut.delta.add(2, 'a', 4);
+        aut.delta.add(2, 'c', 1);
+        aut.delta.add(2, 'c', 3);
+        aut.delta.add(3, 'e', 5);
+        aut.delta.add(4, 'c', 8);
+
+        bool is_empty = is_lang_empty(aut, &cex);
+        REQUIRE(!is_empty);
+
+        // check the counterexample
+        REQUIRE(cex.word.size() == 2);
+        REQUIRE(cex.word[0] == 'a');
+        REQUIRE(cex.word[1] == 'c');
+    }
 }
 
 
 TEST_CASE("Mata::Nfa::determinize()")
 {
-	Nfa aut(3);
-	Nfa result;
-	std::unordered_map<StateSet, State> subset_map;
-
-	SECTION("empty automaton")
-	{
-		result = determinize(aut);
+    Nfa aut(3);
+    Nfa result;
+    std::unordered_map<StateSet, State> subset_map;
 
-		REQUIRE(result.final.empty());
-		REQUIRE(result.delta.empty());
+    SECTION("empty automaton")
+    {
+        result = determinize(aut);
+
+        REQUIRE(result.final.empty());
+        REQUIRE(result.delta.empty());
         CHECK(is_lang_empty(result));
-	}
+    }
+
+    SECTION("simple automaton 1")
+    {
+        aut.initial = {1 };
+        aut.final = {1 };
+        result = determinize(aut, &subset_map);
+
+        REQUIRE(result.initial[subset_map[{1}]]);
+        REQUIRE(result.final[subset_map[{1}]]);
+        REQUIRE(result.delta.empty());
+    }
 
-	SECTION("simple automaton 1")
-	{
-		aut.initial = {1 };
-		aut.final = {1 };
-		result = determinize(aut, &subset_map);
-
-		REQUIRE(result.initial[subset_map[{1}]]);
-		REQUIRE(result.final[subset_map[{1}]]);
-		REQUIRE(result.delta.empty());
-	}
-
-	SECTION("simple automaton 2")
-	{
-		aut.initial = {1 };
-		aut.final = {2 };
-		aut.delta.add(1, 'a', 2);
-		result = determinize(aut, &subset_map);
+    SECTION("simple automaton 2")
+    {
+        aut.initial = {1 };
+        aut.final = {2 };
+        aut.delta.add(1, 'a', 2);
+        result = determinize(aut, &subset_map);
 
-		REQUIRE(result.initial[subset_map[{1}]]);
+        REQUIRE(result.initial[subset_map[{1}]]);
         REQUIRE(result.final[subset_map[{2}]]);
-		REQUIRE(result.delta.contains(subset_map[{1}], 'a', subset_map[{2}]));
-	}
+        REQUIRE(result.delta.contains(subset_map[{1}], 'a', subset_map[{2}]));
+    }
 
     SECTION("This broke Delta when delta[q] could cause re-allocation of post")
     {
         Nfa x{};
         x.initial.insert(0);
         x.final.insert(4);
         x.delta.add(0, 1, 3);
@@ -631,140 +470,140 @@
     aut.delta.add(3, 111, 3);
     aut.delta.add(3, 114, 3);
     minimize(&result, aut);
 }
 
 TEST_CASE("Mata::Nfa::construct() correct calls")
 { // {{{
-	Nfa aut(10);
-	Mata::Parser::ParsedSection parsec;
-	StringToSymbolMap symbol_map;
-
-	SECTION("construct an empty automaton")
-	{
-		parsec.type = Mata::Nfa::TYPE_NFA;
-
-		aut = Builder::construct(parsec);
-
-		REQUIRE(is_lang_empty(aut));
-	}
-
-	SECTION("construct a simple non-empty automaton accepting the empty word")
-	{
-		parsec.type = Mata::Nfa::TYPE_NFA;
-		parsec.dict.insert({"Initial", {"q1"}});
-		parsec.dict.insert({"Final", {"q1"}});
-
-		aut = Builder::construct(parsec);
-
-		REQUIRE(!is_lang_empty(aut));
-	}
-
-	SECTION("construct an automaton with more than one initial/final states")
-	{
-		parsec.type = Mata::Nfa::TYPE_NFA;
-		parsec.dict.insert({"Initial", {"q1", "q2"}});
-		parsec.dict.insert({"Final", {"q1", "q2", "q3"}});
-
-		aut = Builder::construct(parsec);
-
-		REQUIRE(aut.initial.size() == 2);
-		REQUIRE(aut.final.size() == 3);
-	}
-
-	SECTION("construct a simple non-empty automaton accepting only the word 'a'")
-	{
-		parsec.type = Mata::Nfa::TYPE_NFA;
-		parsec.dict.insert({"Initial", {"q1"}});
-		parsec.dict.insert({"Final", {"q2"}});
-		parsec.body = { {"q1", "a", "q2"} };
-
-		aut = Builder::construct(parsec, &symbol_map);
-
-		Run cex;
-		REQUIRE(!is_lang_empty(aut, &cex));
-		auto word_bool_pair = get_word_for_path(aut, cex);
-		REQUIRE(word_bool_pair.second);
-		REQUIRE(word_bool_pair.first.word == encode_word(symbol_map, {"a"}).word);
-
-		REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"a"})));
-	}
-
-	SECTION("construct a more complicated non-empty automaton")
-	{
-		parsec.type = Mata::Nfa::TYPE_NFA;
-		parsec.dict.insert({"Initial", {"q1", "q3"}});
-		parsec.dict.insert({"Final", {"q5"}});
-		parsec.body.push_back({"q1", "a", "q3"});
-		parsec.body.push_back({"q1", "a", "q10"});
-		parsec.body.push_back({"q1", "b", "q7"});
-		parsec.body.push_back({"q3", "a", "q7"});
-		parsec.body.push_back({"q3", "b", "q9"});
-		parsec.body.push_back({"q9", "a", "q9"});
-		parsec.body.push_back({"q7", "b", "q1"});
-		parsec.body.push_back({"q7", "a", "q3"});
-		parsec.body.push_back({"q7", "c", "q3"});
-		parsec.body.push_back({"q10", "a", "q7"});
-		parsec.body.push_back({"q10", "b", "q7"});
-		parsec.body.push_back({"q10", "c", "q7"});
-		parsec.body.push_back({"q7", "a", "q5"});
-		parsec.body.push_back({"q5", "a", "q5"});
-		parsec.body.push_back({"q5", "c", "q9"});
-
-		aut = Builder::construct(parsec, &symbol_map);
-
-		// some samples
-		REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"b", "a"})));
-		REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"a", "c", "a", "a"})));
-		REQUIRE(is_in_lang(aut, encode_word(symbol_map,
-			{"a", "a", "a", "a", "a", "a", "a", "a", "a", "a", "a", "a"})));
-		// some wrong samples
-		REQUIRE(!is_in_lang(aut, encode_word(symbol_map, {"b", "c"})));
-		REQUIRE(!is_in_lang(aut, encode_word(symbol_map, {"a", "c", "c", "a"})));
-		REQUIRE(!is_in_lang(aut, encode_word(symbol_map, {"b", "a", "c", "b"})));
-	}
+    Nfa aut(10);
+    Mata::Parser::ParsedSection parsec;
+    OnTheFlyAlphabet alphabet;
+
+    SECTION("construct an empty automaton")
+    {
+        parsec.type = Mata::Nfa::TYPE_NFA;
+
+        aut = Builder::construct(parsec);
+
+        REQUIRE(is_lang_empty(aut));
+    }
+
+    SECTION("construct a simple non-empty automaton accepting the empty word")
+    {
+        parsec.type = Mata::Nfa::TYPE_NFA;
+        parsec.dict.insert({"Initial", {"q1"}});
+        parsec.dict.insert({"Final", {"q1"}});
+
+        aut = Builder::construct(parsec);
+
+        REQUIRE(!is_lang_empty(aut));
+    }
+
+    SECTION("construct an automaton with more than one initial/final states")
+    {
+        parsec.type = Mata::Nfa::TYPE_NFA;
+        parsec.dict.insert({"Initial", {"q1", "q2"}});
+        parsec.dict.insert({"Final", {"q1", "q2", "q3"}});
+
+        aut = Builder::construct(parsec);
+
+        REQUIRE(aut.initial.size() == 2);
+        REQUIRE(aut.final.size() == 3);
+    }
+
+    SECTION("construct a simple non-empty automaton accepting only the word 'a'")
+    {
+        parsec.type = Mata::Nfa::TYPE_NFA;
+        parsec.dict.insert({"Initial", {"q1"}});
+        parsec.dict.insert({"Final", {"q2"}});
+        parsec.body = { {"q1", "a", "q2"} };
+
+        aut = Builder::construct(parsec, &alphabet);
+
+        Run cex;
+        REQUIRE(!is_lang_empty(aut, &cex));
+        auto word_bool_pair = get_word_for_path(aut, cex);
+        REQUIRE(word_bool_pair.second);
+        REQUIRE(word_bool_pair.first.word == encode_word(&alphabet, { "a"}).word);
+
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "a"})));
+    }
+
+    SECTION("construct a more complicated non-empty automaton")
+    {
+        parsec.type = Mata::Nfa::TYPE_NFA;
+        parsec.dict.insert({"Initial", {"q1", "q3"}});
+        parsec.dict.insert({"Final", {"q5"}});
+        parsec.body.push_back({"q1", "a", "q3"});
+        parsec.body.push_back({"q1", "a", "q10"});
+        parsec.body.push_back({"q1", "b", "q7"});
+        parsec.body.push_back({"q3", "a", "q7"});
+        parsec.body.push_back({"q3", "b", "q9"});
+        parsec.body.push_back({"q9", "a", "q9"});
+        parsec.body.push_back({"q7", "b", "q1"});
+        parsec.body.push_back({"q7", "a", "q3"});
+        parsec.body.push_back({"q7", "c", "q3"});
+        parsec.body.push_back({"q10", "a", "q7"});
+        parsec.body.push_back({"q10", "b", "q7"});
+        parsec.body.push_back({"q10", "c", "q7"});
+        parsec.body.push_back({"q7", "a", "q5"});
+        parsec.body.push_back({"q5", "a", "q5"});
+        parsec.body.push_back({"q5", "c", "q9"});
+
+        aut = Builder::construct(parsec, &alphabet);
+
+        // some samples
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "b", "a"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "a", "c", "a", "a"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet,
+                                            {"a", "a", "a", "a", "a", "a", "a", "a", "a", "a", "a", "a"})));
+        // some wrong samples
+        REQUIRE(!is_in_lang(aut, encode_word(&alphabet, { "b", "c"})));
+        REQUIRE(!is_in_lang(aut, encode_word(&alphabet, { "a", "c", "c", "a"})));
+        REQUIRE(!is_in_lang(aut, encode_word(&alphabet, { "b", "a", "c", "b"})));
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::construct() invalid calls")
 { // {{{
-	Nfa aut;
-	Mata::Parser::ParsedSection parsec;
+    Nfa aut;
+    Mata::Parser::ParsedSection parsec;
 
-	SECTION("construct() call with invalid ParsedSection object")
-	{
-		parsec.type = "FA";
+    SECTION("construct() call with invalid ParsedSection object")
+    {
+        parsec.type = "FA";
 
-		CHECK_THROWS_WITH(Builder::construct(parsec),
+        CHECK_THROWS_WITH(Builder::construct(parsec),
                           Catch::Contains("expecting type"));
-	}
+    }
 
-	SECTION("construct() call with an epsilon transition")
-	{
-		parsec.type = Mata::Nfa::TYPE_NFA;
-		parsec.body = { {"q1", "q2"} };
+    SECTION("construct() call with an epsilon transition")
+    {
+        parsec.type = Mata::Nfa::TYPE_NFA;
+        parsec.body = { {"q1", "q2"} };
 
-		CHECK_THROWS_WITH(Builder::construct(parsec),
+        CHECK_THROWS_WITH(Builder::construct(parsec),
                           Catch::Contains("Epsilon transition"));
-	}
+    }
 
-	SECTION("construct() call with a nonsense transition")
-	{
-		parsec.type = Mata::Nfa::TYPE_NFA;
-		parsec.body = { {"q1", "a", "q2", "q3"} };
-
-		CHECK_THROWS_WITH(Plumbing::construct(&aut, parsec),
-			Catch::Contains("Invalid transition"));
-	}
+    SECTION("construct() call with a nonsense transition")
+    {
+        parsec.type = Mata::Nfa::TYPE_NFA;
+        parsec.body = { {"q1", "a", "q2", "q3"} };
+
+        CHECK_THROWS_WITH(Plumbing::construct(&aut, parsec),
+            Catch::Contains("Invalid transition"));
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::construct() from IntermediateAut correct calls")
 { // {{{
     Nfa aut;
     Mata::IntermediateAut inter_aut;
-    StringToSymbolMap symbol_map;
+    OnTheFlyAlphabet alphabet;
 
     SECTION("construct an empty automaton")
     {
         inter_aut.automaton_type = Mata::IntermediateAut::AutomatonType::NFA;
         REQUIRE(is_lang_empty(aut));
         aut = Builder::construct(inter_aut);
         REQUIRE(is_lang_empty(aut));
@@ -845,23 +684,23 @@
                 "%Alphabet-auto\n"
                 "%Initial q1\n"
                 "%Final q2\n"
                 "q1 a q2\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
-        Plumbing::construct(&aut, inter_aut, &symbol_map);
+        Plumbing::construct(&aut, inter_aut, &alphabet);
 
         Run cex;
         REQUIRE(!is_lang_empty(aut, &cex));
         auto word_bool_pair = get_word_for_path(aut, cex);
         REQUIRE(word_bool_pair.second);
-        REQUIRE(word_bool_pair.first.word == encode_word(symbol_map, {"a"}).word);
+        REQUIRE(word_bool_pair.first.word == encode_word(&alphabet, { "a" }).word);
 
-        REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"a"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "a" })));
     }
 
     SECTION("construct a more complicated non-empty automaton from intermediate automaton")
     {
         std::string file =
                 "@NFA-explicit\n"
                 "%States-enum p q 3\n"
@@ -882,25 +721,25 @@
                 "q10 c q7\n"
                 "q7 a q5\n"
                 "q5 c q9\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-        Plumbing::construct(&aut, inter_aut, &symbol_map);
+        Plumbing::construct(&aut, inter_aut, &alphabet);
 
         // some samples
-        REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"b", "a"})));
-        REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"a", "c", "a", "a"})));
-        REQUIRE(is_in_lang(aut, encode_word(symbol_map,
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "b", "a"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "a", "c", "a", "a"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet,
                                             {"a", "a", "a", "a", "a", "a", "a", "a", "a", "a", "a", "a"})));
         // some wrong samples
-        REQUIRE(!is_in_lang(aut, encode_word(symbol_map, {"b", "c"})));
-        REQUIRE(!is_in_lang(aut, encode_word(symbol_map, {"a", "c", "c", "a"})));
-        REQUIRE(!is_in_lang(aut, encode_word(symbol_map, {"b", "a", "c", "b"})));
+        REQUIRE(!is_in_lang(aut, encode_word(&alphabet, { "b", "c"})));
+        REQUIRE(!is_in_lang(aut, encode_word(&alphabet, { "a", "c", "c", "a"})));
+        REQUIRE(!is_in_lang(aut, encode_word(&alphabet, { "b", "a", "c", "b"})));
     }
 
     SECTION("construct - final states from negation")
     {
         std::string file =
                 "@NFA-bits\n"
                 "%Alphabet-auto\n"
@@ -913,20 +752,20 @@
                 "q3 a5 q5\n"
                 "q3 a6 q6\n"
                 "q5 a7 q7\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-        Plumbing::construct(&aut, inter_aut, &symbol_map);
+        Plumbing::construct(&aut, inter_aut, &alphabet);
         REQUIRE(aut.final.size() == 4);
-        REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"a1", "a2"})));
-        REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"a1", "a2", "a3"})));
-        REQUIRE(!is_in_lang(aut, encode_word(symbol_map, {"a1", "a2", "a3", "a4"})));
-        REQUIRE(is_in_lang(aut, encode_word(symbol_map, {"a1", "a2", "a3", "a5", "a7"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "a1", "a2"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "a1", "a2", "a3"})));
+        REQUIRE(!is_in_lang(aut, encode_word(&alphabet, { "a1", "a2", "a3", "a4"})));
+        REQUIRE(is_in_lang(aut, encode_word(&alphabet, { "a1", "a2", "a3", "a5", "a7"})));
     }
 
     SECTION("construct - final states given as true")
     {
         std::string file =
                 "@NFA-bits\n"
                 "%Alphabet-auto\n"
@@ -939,26 +778,26 @@
                 "q3 a5 q5\n"
                 "q3 a6 q6\n"
                 "q5 a7 q7\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-		Mata::Nfa::StringToStateMap state_map;
-        Plumbing::construct(&aut, inter_aut, &symbol_map, &state_map);
+        Mata::Nfa::Builder::NameStateMap state_map;
+        Plumbing::construct(&aut, inter_aut, &alphabet, &state_map);
         CHECK(aut.final.size() == 9);
-		CHECK(aut.final[state_map.at("0")]);
-		CHECK(aut.final[state_map.at("1")]);
-		CHECK(aut.final[state_map.at("2")]);
-		CHECK(aut.final[state_map.at("3")]);
-		CHECK(aut.final[state_map.at("4")]);
-		CHECK(aut.final[state_map.at("5")]);
-		CHECK(aut.final[state_map.at("6")]);
-		CHECK(aut.final[state_map.at("7")]);
-		CHECK(aut.final[state_map.at("8")]);
+        CHECK(aut.final[state_map.at("0")]);
+        CHECK(aut.final[state_map.at("1")]);
+        CHECK(aut.final[state_map.at("2")]);
+        CHECK(aut.final[state_map.at("3")]);
+        CHECK(aut.final[state_map.at("4")]);
+        CHECK(aut.final[state_map.at("5")]);
+        CHECK(aut.final[state_map.at("6")]);
+        CHECK(aut.final[state_map.at("7")]);
+        CHECK(aut.final[state_map.at("8")]);
     }
 
     SECTION("construct - final states given as false")
     {
         std::string file =
                 "@NFA-bits\n"
                 "%Alphabet-auto\n"
@@ -971,788 +810,682 @@
                 "q3 a5 q5\n"
                 "q3 a6 q6\n"
                 "q5 a7 q7\n";
 
         const auto auts = Mata::IntermediateAut::parse_from_mf(parse_mf(file));
         inter_aut = auts[0];
 
-		Mata::Nfa::StringToStateMap state_map;
-        Plumbing::construct(&aut, inter_aut, &symbol_map, &state_map);
+        Mata::Nfa::Builder::NameStateMap state_map;
+        Plumbing::construct(&aut, inter_aut, &alphabet, &state_map);
         CHECK(aut.final.empty());
     }
 } // }}}
 
-/*
-TEST_CASE("Mata::Nfa::serialize() and operator<<()")
+TEST_CASE("Mata::Nfa::make_complete()")
 { // {{{
-	Nfa aut;
+    Nfa aut(11);
 
-	SECTION("empty automaton")
-	{
-		std::string str;
-
-		SECTION("serialize()")
-		{
-			str = std::to_string(serialize(aut));
-		}
-
-		SECTION("operator<<")
-		{
-			std::ostringstream os;
-			os << aut;
-			str = os.str();
-		}
-
-		Mata::Parser::ParsedSection parsec = Mata::Parser::parse_vtf_section(str);
-		Nfa res = construct(parsec);
-
-		REQUIRE(res.initial.empty());
-		REQUIRE(res.final.empty());
-		REQUIRE(res.delta.empty());
-	}
-
-	SECTION("small automaton")
-	{
-		aut.initial = { 'q', 'r', 's' };
-		aut.final = { 'r', 's', 't' };
-
-		aut.delta.add('q', 'a', 'r');
-		aut.delta.add('r', 'b', 'q');
-		aut.delta.add('s', 'c', 'q');
-		aut.delta.add('s', 'd', 'q');
-		aut.delta.add('q', 'a', 'q');
-
-		Mata::Nfa::StateToStringMap state_dict =
-			{{'q', "q"}, {'r', "r"}, {'s', "s"}, {'t', "t"}};
-		Mata::Nfa::SymbolToStringMap symb_dict =
-			{{'a', "a"}, {'b', "b"}, {'c', "c"}, {'d', "d"}};
-		std::string str = std::to_string(serialize(aut, &symb_dict, &state_dict));
-
-		ParsedSection parsec = Mata::Parser::parse_mf_section(str);
-
-		Mata::Nfa::StringToStateMap inv_state_dict =
-			Mata::util::invert_map(state_dict);
-		Mata::Nfa::StringToSymbolMap inv_symb_dict =
-			Mata::util::invert_map(symb_dict);
-		Nfa res = construct(parsec, &inv_symb_dict, &inv_state_dict);
-
-		REQUIRE(res.initial == aut.initial);
-		REQUIRE(res.final == aut.final);
-		REQUIRE(res.trans_size() == aut.trans_size());
-		REQUIRE(res.delta.has_trans('q', 'a', 'r'));
-		REQUIRE(res.delta.has_trans('r', 'b', 'q'));
-		REQUIRE(res.delta.has_trans('s', 'c', 'q'));
-		REQUIRE(res.delta.has_trans('s', 'd', 'q'));
-		REQUIRE(res.delta.contains('q', 'a', 'q'));
-	}
-
-	SECTION("implicit state and symbol mapper")
-	{
-		aut.delta.add(1, 2, 3);
-
-		ParsedSection parsec = serialize(aut);
-
-		REQUIRE(parsec.body.size() == 1);
-		REQUIRE(*parsec.body.cbegin() == BodyLine({"q1", "a2", "q3"}));
-	}
-
-	SECTION("incorrect state mapper")
-	{
-		Mata::Nfa::StateToStringMap state_dict = {{'q', "q"}};
-		Mata::Nfa::SymbolToStringMap symb_dict = {{'a', "a"}};
-		aut.delta.add('q', 'a', 'r');
-
-		CHECK_THROWS_WITH(serialize(aut, &symb_dict, &state_dict),
-			Catch::Contains("cannot translate state"));
-	}
-
-	SECTION("incorrect symbol mapper")
-	{
-		Mata::Nfa::StateToStringMap state_dict = {{'q', "q"}, {'r', "r"}};
-		Mata::Nfa::SymbolToStringMap symb_dict = {{'a', "a"}};
-		aut.delta.add('q', 'b', 'r');
-
-		CHECK_THROWS_WITH(serialize(aut, &symb_dict, &state_dict),
-			Catch::Contains("cannot translate symbol"));
-	}
-} // }}}
-*/
+    SECTION("empty automaton, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
 
-TEST_CASE("Mata::Nfa::make_complete()")
-{ // {{{
-	Nfa aut(11);
+        make_complete(aut, alph, 0);
+
+        REQUIRE(aut.initial.empty());
+        REQUIRE(aut.final.empty());
+        REQUIRE(aut.delta.empty());
+    }
+
+    SECTION("empty automaton")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
+
+        make_complete(aut, alph, 0);
+
+        REQUIRE(aut.initial.empty());
+        REQUIRE(aut.final.empty());
+        REQUIRE(aut.delta.contains(0, alph["a"], 0));
+        REQUIRE(aut.delta.contains(0, alph["b"], 0));
+    }
+
+    SECTION("non-empty automaton, empty alphabet")
+    {
+        OnTheFlyAlphabet alphabet{};
+
+        aut.initial = {1};
+
+        make_complete(aut, alphabet, 0);
+
+        REQUIRE(aut.initial.size() == 1);
+        REQUIRE(*aut.initial.begin() == 1);
+        REQUIRE(aut.final.empty());
+        REQUIRE(aut.delta.empty());
+    }
+
+    SECTION("one-state automaton")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
+        const State SINK = 10;
+
+        aut.initial = {1};
 
-	SECTION("empty automaton, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-
-		make_complete(aut, alph, 0);
-
-		REQUIRE(aut.initial.empty());
-		REQUIRE(aut.final.empty());
-		REQUIRE(aut.delta.empty());
-	}
-
-	SECTION("empty automaton")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-
-		make_complete(aut, alph, 0);
-
-		REQUIRE(aut.initial.empty());
-		REQUIRE(aut.final.empty());
-		REQUIRE(aut.delta.contains(0, alph["a"], 0));
-		REQUIRE(aut.delta.contains(0, alph["b"], 0));
-	}
-
-	SECTION("non-empty automaton, empty alphabet")
-	{
-		OnTheFlyAlphabet alphabet{};
-
-		aut.initial = {1};
-
-		make_complete(aut, alphabet, 0);
-
-		REQUIRE(aut.initial.size() == 1);
-		REQUIRE(*aut.initial.begin() == 1);
-		REQUIRE(aut.final.empty());
-		REQUIRE(aut.delta.empty());
-	}
-
-	SECTION("one-state automaton")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		const State SINK = 10;
-
-		aut.initial = {1};
-
-		make_complete(aut, alph, SINK);
-
-		REQUIRE(aut.initial.size() == 1);
-		REQUIRE(*aut.initial.begin() == 1);
-		REQUIRE(aut.final.empty());
-		REQUIRE(aut.delta.contains(1, alph["a"], SINK));
-		REQUIRE(aut.delta.contains(1, alph["b"], SINK));
-		REQUIRE(aut.delta.contains(SINK, alph["a"], SINK));
-		REQUIRE(aut.delta.contains(SINK, alph["b"], SINK));
-	}
-
-	SECTION("bigger automaton")
-	{
-		OnTheFlyAlphabet alph{"a", "b", "c"};
-		const State SINK = 9;
-
-		aut.initial = {1, 2};
-		aut.final = {8};
-		aut.delta.add(1, alph["a"], 2);
-		aut.delta.add(2, alph["a"], 4);
-		aut.delta.add(2, alph["c"], 1);
-		aut.delta.add(2, alph["c"], 3);
-		aut.delta.add(3, alph["b"], 5);
-		aut.delta.add(4, alph["c"], 8);
-
-		make_complete(aut, alph, SINK);
-
-		REQUIRE(aut.delta.contains(1, alph["a"], 2));
-		REQUIRE(aut.delta.contains(1, alph["b"], SINK));
-		REQUIRE(aut.delta.contains(1, alph["c"], SINK));
-		REQUIRE(aut.delta.contains(2, alph["a"], 4));
-		REQUIRE(aut.delta.contains(2, alph["c"], 1));
-		REQUIRE(aut.delta.contains(2, alph["c"], 3));
-		REQUIRE(aut.delta.contains(2, alph["b"], SINK));
-		REQUIRE(aut.delta.contains(3, alph["b"], 5));
-		REQUIRE(aut.delta.contains(3, alph["a"], SINK));
-		REQUIRE(aut.delta.contains(3, alph["c"], SINK));
-		REQUIRE(aut.delta.contains(4, alph["c"], 8));
-		REQUIRE(aut.delta.contains(4, alph["a"], SINK));
-		REQUIRE(aut.delta.contains(4, alph["b"], SINK));
-		REQUIRE(aut.delta.contains(5, alph["a"], SINK));
-		REQUIRE(aut.delta.contains(5, alph["b"], SINK));
-		REQUIRE(aut.delta.contains(5, alph["c"], SINK));
-		REQUIRE(aut.delta.contains(8, alph["a"], SINK));
-		REQUIRE(aut.delta.contains(8, alph["b"], SINK));
-		REQUIRE(aut.delta.contains(8, alph["c"], SINK));
-		REQUIRE(aut.delta.contains(SINK, alph["a"], SINK));
-		REQUIRE(aut.delta.contains(SINK, alph["b"], SINK));
-		REQUIRE(aut.delta.contains(SINK, alph["c"], SINK));
-	}
+        make_complete(aut, alph, SINK);
+
+        REQUIRE(aut.initial.size() == 1);
+        REQUIRE(*aut.initial.begin() == 1);
+        REQUIRE(aut.final.empty());
+        REQUIRE(aut.delta.contains(1, alph["a"], SINK));
+        REQUIRE(aut.delta.contains(1, alph["b"], SINK));
+        REQUIRE(aut.delta.contains(SINK, alph["a"], SINK));
+        REQUIRE(aut.delta.contains(SINK, alph["b"], SINK));
+    }
+
+    SECTION("bigger automaton")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b", "c" } };
+        const State SINK = 9;
+
+        aut.initial = {1, 2};
+        aut.final = {8};
+        aut.delta.add(1, alph["a"], 2);
+        aut.delta.add(2, alph["a"], 4);
+        aut.delta.add(2, alph["c"], 1);
+        aut.delta.add(2, alph["c"], 3);
+        aut.delta.add(3, alph["b"], 5);
+        aut.delta.add(4, alph["c"], 8);
+
+        make_complete(aut, alph, SINK);
+
+        REQUIRE(aut.delta.contains(1, alph["a"], 2));
+        REQUIRE(aut.delta.contains(1, alph["b"], SINK));
+        REQUIRE(aut.delta.contains(1, alph["c"], SINK));
+        REQUIRE(aut.delta.contains(2, alph["a"], 4));
+        REQUIRE(aut.delta.contains(2, alph["c"], 1));
+        REQUIRE(aut.delta.contains(2, alph["c"], 3));
+        REQUIRE(aut.delta.contains(2, alph["b"], SINK));
+        REQUIRE(aut.delta.contains(3, alph["b"], 5));
+        REQUIRE(aut.delta.contains(3, alph["a"], SINK));
+        REQUIRE(aut.delta.contains(3, alph["c"], SINK));
+        REQUIRE(aut.delta.contains(4, alph["c"], 8));
+        REQUIRE(aut.delta.contains(4, alph["a"], SINK));
+        REQUIRE(aut.delta.contains(4, alph["b"], SINK));
+        REQUIRE(aut.delta.contains(5, alph["a"], SINK));
+        REQUIRE(aut.delta.contains(5, alph["b"], SINK));
+        REQUIRE(aut.delta.contains(5, alph["c"], SINK));
+        REQUIRE(aut.delta.contains(8, alph["a"], SINK));
+        REQUIRE(aut.delta.contains(8, alph["b"], SINK));
+        REQUIRE(aut.delta.contains(8, alph["c"], SINK));
+        REQUIRE(aut.delta.contains(SINK, alph["a"], SINK));
+        REQUIRE(aut.delta.contains(SINK, alph["b"], SINK));
+        REQUIRE(aut.delta.contains(SINK, alph["c"], SINK));
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::complement()")
 { // {{{
-	Nfa aut(3);
-	Nfa cmpl;
+    Nfa aut(3);
+    Nfa cmpl;
 
-	SECTION("empty automaton, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
+    SECTION("empty automaton, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "false"}});
         Nfa empty_string_nfa{ Mata::Nfa::Builder::create_sigma_star_nfa(&alph) };
         CHECK(Mata::Nfa::are_equivalent(cmpl, empty_string_nfa));
-	}
+    }
 
-	SECTION("empty automaton")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
+    SECTION("empty automaton")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "false"}});
 
-		REQUIRE(is_in_lang(cmpl, {}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"] },{}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["b"] }, {}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["a"]}, {}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["b"], alph["b"], alph["a"] }, {}}));
+        REQUIRE(is_in_lang(cmpl, {}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"] },{}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["b"] }, {}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["a"]}, {}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["b"], alph["b"], alph["a"] }, {}}));
 
         Nfa sigma_star_nfa{ Mata::Nfa::Builder::create_sigma_star_nfa(&alph) };
         CHECK(Mata::Nfa::are_equivalent(cmpl, sigma_star_nfa));
-	}
+    }
 
-	SECTION("empty automaton accepting epsilon, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-		aut.initial = {1};
-		aut.final = {1};
+    SECTION("empty automaton accepting epsilon, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
+        aut.initial = {1};
+        aut.final = {1};
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "false"}});
 
-		CHECK(is_lang_empty(cmpl));
-	}
+        CHECK(is_lang_empty(cmpl));
+    }
 
-	SECTION("empty automaton accepting epsilon")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1};
-		aut.final = {1};
+    SECTION("empty automaton accepting epsilon")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
+        aut.initial = {1};
+        aut.final = {1};
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "false"}});
 
-		REQUIRE(!is_in_lang(cmpl, { }));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"]}, {}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["b"]}, {}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["a"]}, {}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["b"], alph["b"], alph["a"]},{}}));
-		REQUIRE(cmpl.initial.size() == 1);
-		REQUIRE(cmpl.final.size() == 1);
-		size_t sum = 0;
-		for (const auto& x : cmpl) {
-            unused(x);
-            sum++;
-		}
-		REQUIRE(sum == 4);
-	}
-
-	SECTION("non-empty automaton accepting a*b*")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1, 2};
-		aut.final = {1, 2};
-
-		aut.delta.add(1, alph["a"], 1);
-		aut.delta.add(1, alph["a"], 2);
-		aut.delta.add(2, alph["b"], 2);
+        REQUIRE(!is_in_lang(cmpl, { }));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"]}, {}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["b"]}, {}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["a"]}, {}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["b"], alph["b"], alph["a"]},{}}));
+        REQUIRE(cmpl.initial.size() == 1);
+        REQUIRE(cmpl.final.size() == 1);
+        REQUIRE(cmpl.get_num_of_trans() == 4);
+    }
+
+    SECTION("non-empty automaton accepting a*b*")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
+        aut.initial = {1, 2};
+        aut.final = {1, 2};
+
+        aut.delta.add(1, alph["a"], 1);
+        aut.delta.add(1, alph["a"], 2);
+        aut.delta.add(2, alph["b"], 2);
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "false"}});
 
-		REQUIRE(!is_in_lang(cmpl, { }));
-		REQUIRE(!is_in_lang(cmpl, {{ alph["a"] }, {}}));
-		REQUIRE(!is_in_lang(cmpl, {{ alph["b"] }, {}}));
-		REQUIRE(!is_in_lang(cmpl, {{ alph["a"], alph["a"] }, {}}));
-		REQUIRE(is_in_lang(cmpl, {{ alph["a"], alph["b"], alph["b"], alph["a"] }, {}}));
-		REQUIRE(!is_in_lang(cmpl, {{ alph["a"], alph["a"], alph["b"], alph["b"] }, {}}));
-		REQUIRE(is_in_lang(cmpl, {{ alph["b"], alph["a"], alph["a"], alph["a"] }, {}}));
-
-		REQUIRE(cmpl.initial.size() == 1);
-		REQUIRE(cmpl.final.size() == 1);
-		size_t sum = 0;
-		for (const auto& x : cmpl) {
-            unused(x);
-            sum++;
-		}
-		REQUIRE(sum == 6);
-	}
-
-	SECTION("empty automaton, empty alphabet, minimization")
-	{
-		OnTheFlyAlphabet alph{};
+        REQUIRE(!is_in_lang(cmpl, { }));
+        REQUIRE(!is_in_lang(cmpl, {{ alph["a"] }, {}}));
+        REQUIRE(!is_in_lang(cmpl, {{ alph["b"] }, {}}));
+        REQUIRE(!is_in_lang(cmpl, {{ alph["a"], alph["a"] }, {}}));
+        REQUIRE(is_in_lang(cmpl, {{ alph["a"], alph["b"], alph["b"], alph["a"] }, {}}));
+        REQUIRE(!is_in_lang(cmpl, {{ alph["a"], alph["a"], alph["b"], alph["b"] }, {}}));
+        REQUIRE(is_in_lang(cmpl, {{ alph["b"], alph["a"], alph["a"], alph["a"] }, {}}));
+
+        REQUIRE(cmpl.initial.size() == 1);
+        REQUIRE(cmpl.final.size() == 1);
+        REQUIRE(cmpl.get_num_of_trans() == 6);
+    }
+
+    SECTION("empty automaton, empty alphabet, minimization")
+    {
+        OnTheFlyAlphabet alph{};
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "true"}});
         Nfa empty_string_nfa{ Mata::Nfa::Builder::create_sigma_star_nfa(&alph) };
         CHECK(Mata::Nfa::are_equivalent(empty_string_nfa, cmpl));
-	}
+    }
 
-	SECTION("empty automaton, minimization")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
+    SECTION("empty automaton, minimization")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "true"}});
 
-		REQUIRE(is_in_lang(cmpl, {}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"] },{}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["b"] }, {}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["a"]}, {}}));
-		REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["b"], alph["b"], alph["a"] }, {}}));
+        REQUIRE(is_in_lang(cmpl, {}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"] },{}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["b"] }, {}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["a"]}, {}}));
+        REQUIRE(is_in_lang(cmpl, Mata::Nfa::Run{{ alph["a"], alph["b"], alph["b"], alph["a"] }, {}}));
 
         Nfa sigma_star_nfa{ Mata::Nfa::Builder::create_sigma_star_nfa(&alph) };
         CHECK(Mata::Nfa::are_equivalent(sigma_star_nfa, cmpl));
-	}
+    }
 
-	SECTION("minimization vs no minimization")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {0, 1};
-		aut.final = {1, 2};
-
-		aut.delta.add(1, alph["b"], 1);
-		aut.delta.add(1, alph["a"], 2);
-		aut.delta.add(2, alph["b"], 2);
-		aut.delta.add(0, alph["a"], 1);
-		aut.delta.add(0, alph["a"], 2);
+    SECTION("minimization vs no minimization")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
+        aut.initial = {0, 1};
+        aut.final = {1, 2};
+
+        aut.delta.add(1, alph["b"], 1);
+        aut.delta.add(1, alph["a"], 2);
+        aut.delta.add(2, alph["b"], 2);
+        aut.delta.add(0, alph["a"], 1);
+        aut.delta.add(0, alph["a"], 2);
 
-		cmpl = complement(aut, alph, {{"algorithm", "classical"},
+        cmpl = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "false"}});
 
-		Nfa cmpl_min = complement(aut, alph, {{"algorithm", "classical"},
+        Nfa cmpl_min = complement(aut, alph, {{"algorithm", "classical"},
                                     {"minimize", "true"}});
 
-		CHECK(are_equivalent(cmpl, cmpl_min, &alph));
-		CHECK(cmpl_min.size() == 4);
-		CHECK(cmpl.size() == 5);
-	}
+        CHECK(are_equivalent(cmpl, cmpl_min, &alph));
+        CHECK(cmpl_min.size() == 4);
+        CHECK(cmpl.size() == 5);
+    }
 
 } // }}}
 
 TEST_CASE("Mata::Nfa::is_universal()")
 { // {{{
-	Nfa aut(6);
-	Run cex;
-	StringMap params;
-
-	const std::unordered_set<std::string> ALGORITHMS = {
-		"naive",
-		"antichains",
-	};
-
-	SECTION("empty automaton, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, params);
-
-			REQUIRE(!is_univ);
-		}
-	}
-
-	SECTION("empty automaton accepting epsilon, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-		aut.initial = {1};
-		aut.final = {1};
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, &cex, params);
-
-			REQUIRE(is_univ);
-			REQUIRE(Word{ } == cex.word);
-		}
-	}
-
-	SECTION("empty automaton accepting epsilon")
-	{
-		OnTheFlyAlphabet alph{"a"};
-		aut.initial = {1};
-		aut.final = {1};
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, &cex, params);
-
-			REQUIRE(!is_univ);
-			REQUIRE(((cex.word == Word{alph["a"]}) || (cex.word == Word{alph["b"]})));
-		}
-	}
-
-	SECTION("automaton for a*b*")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1, 2};
-		aut.final = {1, 2};
-
-		aut.delta.add(1, alph["a"], 1);
-		aut.delta.add(1, alph["a"], 2);
-		aut.delta.add(2, alph["b"], 2);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, params);
-
-			REQUIRE(!is_univ);
-		}
-	}
-
-	SECTION("automaton for a* + b*")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1, 2};
-		aut.final = {1, 2};
-
-		aut.delta.add(1, alph["a"], 1);
-		aut.delta.add(2, alph["b"], 2);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, params);
-
-			REQUIRE(!is_univ);
-		}
-	}
-
-	SECTION("automaton for (a + b)*")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1};
-		aut.final = {1};
-
-		aut.delta.add(1, alph["a"], 1);
-		aut.delta.add(1, alph["b"], 1);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, params);
-
-			REQUIRE(is_univ);
-		}
-	}
-
-	SECTION("automaton for eps + (a+b) + (a+b)(a+b)(a* + b*)")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1};
-		aut.final = {1, 2, 3, 4, 5};
-
-		aut.delta.add(1, alph["a"], 2);
-		aut.delta.add(1, alph["b"], 2);
-		aut.delta.add(2, alph["a"], 3);
-		aut.delta.add(2, alph["b"], 3);
-
-		aut.delta.add(3, alph["a"], 4);
-		aut.delta.add(4, alph["a"], 4);
-
-		aut.delta.add(3, alph["b"], 5);
-		aut.delta.add(5, alph["b"], 5);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, &cex, params);
-
-			REQUIRE(!is_univ);
-
-			REQUIRE(cex.word.size() == 4);
-			REQUIRE((cex.word[0] == alph["a"] || cex.word[0] == alph["b"]));
-			REQUIRE((cex.word[1] == alph["a"] || cex.word[1] == alph["b"]));
-			REQUIRE((cex.word[2] == alph["a"] || cex.word[2] == alph["b"]));
-			REQUIRE((cex.word[3] == alph["a"] || cex.word[3] == alph["b"]));
-			REQUIRE(cex.word[2] != cex.word[3]);
-		}
-	}
-
-	SECTION("automaton for epsilon + a(a + b)* + b(a + b)*")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1, 3};
-		aut.final = {1, 2, 4};
-
-		aut.delta.add(1, alph["a"], 2);
-		aut.delta.add(2, alph["a"], 2);
-		aut.delta.add(2, alph["b"], 2);
-		aut.delta.add(3, alph["b"], 4);
-		aut.delta.add(4, alph["a"], 4);
-		aut.delta.add(4, alph["b"], 4);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, &cex, params);
-
-			REQUIRE(is_univ);
-		}
-	}
-
-	SECTION("example from Abdulla et al. TACAS'10")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		aut.initial = {1, 2};
-		aut.final = {1, 2, 3};
-
-		aut.delta.add(1, alph["b"], 1);
-		aut.delta.add(1, alph["a"], 2);
-		aut.delta.add(1, alph["b"], 4);
-		aut.delta.add(2, alph["b"], 2);
-		aut.delta.add(2, alph["a"], 3);
-		aut.delta.add(3, alph["b"], 3);
-		aut.delta.add(3, alph["a"], 1);
-		aut.delta.add(4, alph["b"], 2);
-		aut.delta.add(4, alph["b"], 3);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, &cex, params);
-
-			REQUIRE(is_univ);
-		}
-	}
-
-	SECTION("subsumption-pruning in processed")
-	{
-		OnTheFlyAlphabet alph{"a"};
-		aut.initial = {1, 2};
-		aut.final = {1};
-
-		aut.delta.add(1, alph["a"], 1);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_univ = is_universal(aut, alph, &cex, params);
-
-			REQUIRE(is_univ);
-		}
-	}
-
-	SECTION("wrong parameters 1")
-	{
-		OnTheFlyAlphabet alph{};
-
-		CHECK_THROWS_WITH(is_universal(aut, alph, params),
-			Catch::Contains("requires setting the \"algo\" key"));
-	}
-
-	SECTION("wrong parameters 2")
-	{
-		OnTheFlyAlphabet alph{};
-		params["algorithm"] = "foo";
-
-		CHECK_THROWS_WITH(is_universal(aut, alph, params),
-			Catch::Contains("received an unknown value"));
-	}
+    Nfa aut(6);
+    Run cex;
+    ParameterMap params;
+
+    const std::unordered_set<std::string> ALGORITHMS = {
+        "naive",
+        "antichains",
+    };
+
+    SECTION("empty automaton, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, params);
+
+            REQUIRE(!is_univ);
+        }
+    }
+
+    SECTION("empty automaton accepting epsilon, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
+        aut.initial = {1};
+        aut.final = {1};
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, &cex, params);
+
+            REQUIRE(is_univ);
+            REQUIRE(cex.word.empty());
+        }
+    }
+
+    SECTION("empty automaton accepting epsilon")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a" } };
+        aut.initial = {1};
+        aut.final = {1};
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, &cex, params);
+
+            REQUIRE(!is_univ);
+            REQUIRE(((cex.word == Word{alph["a"]}) || (cex.word == Word{alph["b"]})));
+        }
+    }
+
+    SECTION("automaton for a*b*")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b" } };
+        aut.initial = {1, 2};
+        aut.final = {1, 2};
+
+        aut.delta.add(1, alph["a"], 1);
+        aut.delta.add(1, alph["a"], 2);
+        aut.delta.add(2, alph["b"], 2);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, params);
+
+            REQUIRE(!is_univ);
+        }
+    }
+
+    SECTION("automaton for a* + b*")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        aut.initial = {1, 2};
+        aut.final = {1, 2};
+
+        aut.delta.add(1, alph["a"], 1);
+        aut.delta.add(2, alph["b"], 2);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, params);
+
+            REQUIRE(!is_univ);
+        }
+    }
+
+    SECTION("automaton for (a + b)*")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        aut.initial = {1};
+        aut.final = {1};
+
+        aut.delta.add(1, alph["a"], 1);
+        aut.delta.add(1, alph["b"], 1);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, params);
+
+            REQUIRE(is_univ);
+        }
+    }
+
+    SECTION("automaton for eps + (a+b) + (a+b)(a+b)(a* + b*)")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        aut.initial = {1};
+        aut.final = {1, 2, 3, 4, 5};
+
+        aut.delta.add(1, alph["a"], 2);
+        aut.delta.add(1, alph["b"], 2);
+        aut.delta.add(2, alph["a"], 3);
+        aut.delta.add(2, alph["b"], 3);
+
+        aut.delta.add(3, alph["a"], 4);
+        aut.delta.add(4, alph["a"], 4);
+
+        aut.delta.add(3, alph["b"], 5);
+        aut.delta.add(5, alph["b"], 5);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, &cex, params);
+
+            REQUIRE(!is_univ);
+
+            REQUIRE(cex.word.size() == 4);
+            REQUIRE((cex.word[0] == alph["a"] || cex.word[0] == alph["b"]));
+            REQUIRE((cex.word[1] == alph["a"] || cex.word[1] == alph["b"]));
+            REQUIRE((cex.word[2] == alph["a"] || cex.word[2] == alph["b"]));
+            REQUIRE((cex.word[3] == alph["a"] || cex.word[3] == alph["b"]));
+            REQUIRE(cex.word[2] != cex.word[3]);
+        }
+    }
+
+    SECTION("automaton for epsilon + a(a + b)* + b(a + b)*")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        aut.initial = {1, 3};
+        aut.final = {1, 2, 4};
+
+        aut.delta.add(1, alph["a"], 2);
+        aut.delta.add(2, alph["a"], 2);
+        aut.delta.add(2, alph["b"], 2);
+        aut.delta.add(3, alph["b"], 4);
+        aut.delta.add(4, alph["a"], 4);
+        aut.delta.add(4, alph["b"], 4);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, &cex, params);
+
+            REQUIRE(is_univ);
+        }
+    }
+
+    SECTION("example from Abdulla et al. TACAS'10")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        aut.initial = {1, 2};
+        aut.final = {1, 2, 3};
+
+        aut.delta.add(1, alph["b"], 1);
+        aut.delta.add(1, alph["a"], 2);
+        aut.delta.add(1, alph["b"], 4);
+        aut.delta.add(2, alph["b"], 2);
+        aut.delta.add(2, alph["a"], 3);
+        aut.delta.add(3, alph["b"], 3);
+        aut.delta.add(3, alph["a"], 1);
+        aut.delta.add(4, alph["b"], 2);
+        aut.delta.add(4, alph["b"], 3);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, &cex, params);
+
+            REQUIRE(is_univ);
+        }
+    }
+
+    SECTION("subsumption-pruning in processed")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a" } };
+        aut.initial = {1, 2};
+        aut.final = {1};
+
+        aut.delta.add(1, alph["a"], 1);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_univ = is_universal(aut, alph, &cex, params);
+
+            REQUIRE(is_univ);
+        }
+    }
+
+    SECTION("wrong parameters 1")
+    {
+        OnTheFlyAlphabet alph{};
+
+        CHECK_THROWS_WITH(is_universal(aut, alph, params),
+            Catch::Contains("requires setting the \"algo\" key"));
+    }
+
+    SECTION("wrong parameters 2")
+    {
+        OnTheFlyAlphabet alph{};
+        params["algorithm"] = "foo";
+
+        CHECK_THROWS_WITH(is_universal(aut, alph, params),
+            Catch::Contains("received an unknown value"));
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::is_included()")
 { // {{{
-	Nfa smaller(10);
-	Nfa bigger(16);
-	Run cex;
-	StringMap params;
-
-	const std::unordered_set<std::string> ALGORITHMS = {
-		"naive",
-		"antichains",
-	};
-
-	SECTION("{} <= {}, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_incl = is_included(smaller, bigger, &alph, params);
-			CHECK(is_incl);
+    Nfa smaller(10);
+    Nfa bigger(16);
+    Run cex;
+    ParameterMap params;
+
+    const std::unordered_set<std::string> ALGORITHMS = {
+        "naive",
+        "antichains",
+    };
+
+    SECTION("{} <= {}, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_incl = is_included(smaller, bigger, &alph, params);
+            CHECK(is_incl);
 
             is_incl = is_included(bigger, smaller, &alph, params);
             CHECK(is_incl);
-		}
-	}
+        }
+    }
+
+    SECTION("{} <= {epsilon}, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
+        bigger.initial = {1};
+        bigger.final = {1};
 
-	SECTION("{} <= {epsilon}, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-		bigger.initial = {1};
-		bigger.final = {1};
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
             CHECK(is_incl);
 
             is_incl = is_included(bigger, smaller, &cex, &alph, params);
             CHECK(!is_incl);
-		}
-	}
+        }
+    }
 
-	SECTION("{epsilon} <= {epsilon}, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-		smaller.initial = {1};
-		smaller.final = {1};
-		bigger.initial = {11};
-		bigger.final = {11};
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
+    SECTION("{epsilon} <= {epsilon}, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
+        smaller.initial = {1};
+        smaller.final = {1};
+        bigger.initial = {11};
+        bigger.final = {11};
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
             CHECK(is_incl);
 
             is_incl = is_included(bigger, smaller, &cex, &alph, params);
             CHECK(is_incl);
-		}
-	}
+        }
+    }
+
+    SECTION("{epsilon} !<= {}, empty alphabet")
+    {
+        OnTheFlyAlphabet alph{};
+        smaller.initial = {1};
+        smaller.final = {1};
 
-	SECTION("{epsilon} !<= {}, empty alphabet")
-	{
-		OnTheFlyAlphabet alph{};
-		smaller.initial = {1};
-		smaller.final = {1};
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
 
-			REQUIRE(!is_incl);
-			REQUIRE(cex.word == Word{});
+            REQUIRE(!is_incl);
+            REQUIRE(cex.word.empty());
 
             is_incl = is_included(bigger, smaller, &cex, &alph, params);
-            REQUIRE(cex.word == Word{});
+            REQUIRE(cex.word.empty());
             REQUIRE(is_incl);
-		}
-	}
+        }
+    }
+
+    SECTION("a* + b* <= (a+b)*")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        smaller.initial = {1, 2};
+        smaller.final = {1, 2};
+        smaller.delta.add(1, alph["a"], 1);
+        smaller.delta.add(2, alph["b"], 2);
+
+        bigger.initial = {11};
+        bigger.final = {11};
+        bigger.delta.add(11, alph["a"], 11);
+        bigger.delta.add(11, alph["b"], 11);
 
-	SECTION("a* + b* <= (a+b)*")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		smaller.initial = {1, 2};
-		smaller.final = {1, 2};
-		smaller.delta.add(1, alph["a"], 1);
-		smaller.delta.add(2, alph["b"], 2);
-
-		bigger.initial = {11};
-		bigger.final = {11};
-		bigger.delta.add(11, alph["a"], 11);
-		bigger.delta.add(11, alph["b"], 11);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_incl = is_included(smaller, bigger, &alph, params);
-			REQUIRE(is_incl);
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_incl = is_included(smaller, bigger, &alph, params);
+            REQUIRE(is_incl);
 
             is_incl = is_included(bigger, smaller, &alph, params);
             REQUIRE(!is_incl);
-		}
-	}
+        }
+    }
+
+    SECTION("(a+b)* !<= a* + b*")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        smaller.initial = {1};
+        smaller.final = {1};
+        smaller.delta.add(1, alph["a"], 1);
+        smaller.delta.add(1, alph["b"], 1);
+
+        bigger.initial = {11, 12};
+        bigger.final = {11, 12};
+        bigger.delta.add(11, alph["a"], 11);
+        bigger.delta.add(12, alph["b"], 12);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
 
-	SECTION("(a+b)* !<= a* + b*")
-	{
-		OnTheFlyAlphabet alph{"a", "b"};
-		smaller.initial = {1};
-		smaller.final = {1};
-		smaller.delta.add(1, alph["a"], 1);
-		smaller.delta.add(1, alph["b"], 1);
-
-		bigger.initial = {11, 12};
-		bigger.final = {11, 12};
-		bigger.delta.add(11, alph["a"], 11);
-		bigger.delta.add(12, alph["b"], 12);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-
-			bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
-
-			REQUIRE(!is_incl);
-			REQUIRE((
-				cex.word == Word{alph["a"], alph["b"]} ||
-				cex.word == Word{alph["b"], alph["a"]}));
+            bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
+
+            REQUIRE(!is_incl);
+            REQUIRE((
+                cex.word == Word{alph["a"], alph["b"]} ||
+                cex.word == Word{alph["b"], alph["a"]}));
 
             is_incl = is_included(bigger, smaller, &cex, &alph, params);
             REQUIRE(is_incl);
             REQUIRE((
                 cex.word == Word{alph["a"], alph["b"]} ||
                 cex.word == Word{alph["b"], alph["a"]}));
-		}
-	}
+        }
+    }
+
+    SECTION("(a+b)* !<= eps + (a+b) + (a+b)(a+b)(a* + b*)")
+    {
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
+        smaller.initial = {1};
+        smaller.final = {1};
+        smaller.delta.add(1, alph["a"], 1);
+        smaller.delta.add(1, alph["b"], 1);
+
+        bigger.initial = {11};
+        bigger.final = {11, 12, 13, 14, 15};
+
+        bigger.delta.add(11, alph["a"], 12);
+        bigger.delta.add(11, alph["b"], 12);
+        bigger.delta.add(12, alph["a"], 13);
+        bigger.delta.add(12, alph["b"], 13);
 
-	SECTION("(a+b)* !<= eps + (a+b) + (a+b)(a+b)(a* + b*)")
-	{
-        OnTheFlyAlphabet alph{"a", "b"};
-		smaller.initial = {1};
-		smaller.final = {1};
-		smaller.delta.add(1, alph["a"], 1);
-		smaller.delta.add(1, alph["b"], 1);
-
-		bigger.initial = {11};
-		bigger.final = {11, 12, 13, 14, 15};
-
-		bigger.delta.add(11, alph["a"], 12);
-		bigger.delta.add(11, alph["b"], 12);
-		bigger.delta.add(12, alph["a"], 13);
-		bigger.delta.add(12, alph["b"], 13);
-
-		bigger.delta.add(13, alph["a"], 14);
-		bigger.delta.add(14, alph["a"], 14);
-
-		bigger.delta.add(13, alph["b"], 15);
-		bigger.delta.add(15, alph["b"], 15);
-
-		for (const auto& algo : ALGORITHMS) {
-			params["algorithm"] = algo;
-			bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
-			REQUIRE(!is_incl);
-
-			REQUIRE(cex.word.size() == 4);
-			REQUIRE((cex.word[0] == alph["a"] || cex.word[0] == alph["b"]));
-			REQUIRE((cex.word[1] == alph["a"] || cex.word[1] == alph["b"]));
-			REQUIRE((cex.word[2] == alph["a"] || cex.word[2] == alph["b"]));
-			REQUIRE((cex.word[3] == alph["a"] || cex.word[3] == alph["b"]));
-			REQUIRE(cex.word[2] != cex.word[3]);
+        bigger.delta.add(13, alph["a"], 14);
+        bigger.delta.add(14, alph["a"], 14);
+
+        bigger.delta.add(13, alph["b"], 15);
+        bigger.delta.add(15, alph["b"], 15);
+
+        for (const auto& algo : ALGORITHMS) {
+            params["algorithm"] = algo;
+            bool is_incl = is_included(smaller, bigger, &cex, &alph, params);
+            REQUIRE(!is_incl);
+
+            REQUIRE(cex.word.size() == 4);
+            REQUIRE((cex.word[0] == alph["a"] || cex.word[0] == alph["b"]));
+            REQUIRE((cex.word[1] == alph["a"] || cex.word[1] == alph["b"]));
+            REQUIRE((cex.word[2] == alph["a"] || cex.word[2] == alph["b"]));
+            REQUIRE((cex.word[3] == alph["a"] || cex.word[3] == alph["b"]));
+            REQUIRE(cex.word[2] != cex.word[3]);
 
             is_incl = is_included(bigger, smaller, &cex, &alph, params);
             REQUIRE(is_incl);
 
             REQUIRE(cex.word.size() == 4);
             REQUIRE((cex.word[0] == alph["a"] || cex.word[0] == alph["b"]));
             REQUIRE((cex.word[1] == alph["a"] || cex.word[1] == alph["b"]));
             REQUIRE((cex.word[2] == alph["a"] || cex.word[2] == alph["b"]));
             REQUIRE((cex.word[3] == alph["a"] || cex.word[3] == alph["b"]));
             REQUIRE(cex.word[2] != cex.word[3]);
-		}
-	}
+        }
+    }
 
-	SECTION("wrong parameters 1")
-	{
+    SECTION("wrong parameters 1")
+    {
         OnTheFlyAlphabet alph{};
 
-		CHECK_THROWS_WITH(is_included(smaller, bigger, &alph, params),
-			Catch::Contains("requires setting the \"algo\" key"));
+        CHECK_THROWS_WITH(is_included(smaller, bigger, &alph, params),
+            Catch::Contains("requires setting the \"algo\" key"));
         CHECK_NOTHROW(is_included(smaller, bigger, &alph));
-	}
+    }
 
-	SECTION("wrong parameters 2")
-	{
+    SECTION("wrong parameters 2")
+    {
         OnTheFlyAlphabet alph{};
-		params["algorithm"] = "foo";
+        params["algorithm"] = "foo";
 
-		CHECK_THROWS_WITH(is_included(smaller, bigger, &alph, params),
-			Catch::Contains("received an unknown value"));
+        CHECK_THROWS_WITH(is_included(smaller, bigger, &alph, params),
+            Catch::Contains("received an unknown value"));
         CHECK_NOTHROW(is_included(smaller, bigger, &alph));
-	}
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::are_equivalent")
 {
     Nfa smaller(10);
     Nfa bigger(16);
     Word cex;
-    StringMap params;
+    ParameterMap params;
 
     const std::unordered_set<std::string> ALGORITHMS = {
             "naive",
             "antichains",
     };
 
     SECTION("{} == {}, empty alphabet")
@@ -1810,15 +1543,15 @@
             CHECK(are_equivalent(bigger, smaller, params));
             CHECK(are_equivalent(bigger, smaller));
         }
     }
 
     SECTION("a* + b* == (a+b)*")
     {
-        OnTheFlyAlphabet alph{"a", "b"};
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
         smaller.initial = {1, 2};
         smaller.final = {1, 2};
         smaller.delta.add(1, alph["a"], 1);
         smaller.delta.add(2, alph["b"], 2);
 
         bigger.initial = {11};
         bigger.final = {11};
@@ -1848,15 +1581,15 @@
         Mata::Nfa::Nfa aut2;
         Mata::Parser::create_nfa(&aut2, "(a|b)*");
         CHECK(!Mata::Nfa::are_equivalent(aut, aut2));
     }
 
     SECTION("(a+b)* !<= eps + (a+b) + (a+b)(a+b)(a* + b*)")
     {
-        OnTheFlyAlphabet alph{"a", "b"};
+        OnTheFlyAlphabet alph{ std::vector<std::string>{ "a", "b"} };
         smaller.initial = {1};
         smaller.final = {1};
         smaller.delta.add(1, alph["a"], 1);
         smaller.delta.add(1, alph["b"], 1);
 
         bigger.initial = {11};
         bigger.final = {11, 12, 13, 14, 15};
@@ -1907,313 +1640,313 @@
                           Catch::Contains("received an unknown value"));
         CHECK_NOTHROW(are_equivalent(smaller, bigger));
     }
 }
 
 TEST_CASE("Mata::Nfa::revert()")
 { // {{{
-	Nfa aut(9);
+    Nfa aut(9);
 
-	SECTION("empty automaton")
-	{
-		Nfa result = revert(aut);
-
-		REQUIRE(result.delta.empty());
-		REQUIRE(result.initial.size() == 0);
-		REQUIRE(result.final.size() == 0);
-	}
-
-	SECTION("no-transition automaton")
-	{
-		aut.initial.insert(1);
-		aut.initial.insert(3);
-
-		aut.final.insert(2);
-		aut.final.insert(5);
-
-		Nfa result = revert(aut);
-
-		REQUIRE(result.delta.empty());
-		REQUIRE(result.initial[2]);
-		REQUIRE(result.initial[5]);
-		REQUIRE(result.final[1]);
-		REQUIRE(result.final[3]);
-	}
-
-	SECTION("one-transition automaton")
-	{
-		aut.initial.insert(1);
-		aut.final.insert(2);
-		aut.delta.add(1, 'a', 2);
-
-		Nfa result = revert(aut);
-
-		REQUIRE(result.initial[2]);
-		REQUIRE(result.final[1]);
-		REQUIRE(result.delta.contains(2, 'a', 1));
-		REQUIRE(result.delta.size() == aut.delta.size());
-	}
-
-	SECTION("bigger automaton")
-	{
-		aut.initial = {1, 2};
-		aut.delta.add(1, 'a', 2);
-		aut.delta.add(1, 'a', 3);
-		aut.delta.add(1, 'b', 4);
-		aut.delta.add(2, 'a', 2);
-		aut.delta.add(2, 'a', 3);
-		aut.delta.add(2, 'b', 4);
-		aut.delta.add(3, 'b', 4);
-		aut.delta.add(3, 'c', 7);
-		aut.delta.add(3, 'b', 2);
-		aut.delta.add(7, 'a', 8);
-		aut.final = {3};
+    SECTION("empty automaton")
+    {
+        Nfa result = revert(aut);
+
+        REQUIRE(result.delta.empty());
+        REQUIRE(result.initial.empty());
+        REQUIRE(result.final.empty());
+    }
 
-		Nfa result = revert(aut);
-		//REQUIRE(result.final == StateSet({1, 2}));
+    SECTION("no-transition automaton")
+    {
+        aut.initial.insert(1);
+        aut.initial.insert(3);
+
+        aut.final.insert(2);
+        aut.final.insert(5);
+
+        Nfa result = revert(aut);
+
+        REQUIRE(result.delta.empty());
+        REQUIRE(result.initial[2]);
+        REQUIRE(result.initial[5]);
+        REQUIRE(result.final[1]);
+        REQUIRE(result.final[3]);
+    }
+
+    SECTION("one-transition automaton")
+    {
+        aut.initial.insert(1);
+        aut.final.insert(2);
+        aut.delta.add(1, 'a', 2);
+
+        Nfa result = revert(aut);
+
+        REQUIRE(result.initial[2]);
+        REQUIRE(result.final[1]);
+        REQUIRE(result.delta.contains(2, 'a', 1));
+        REQUIRE(result.delta.size() == aut.delta.size());
+    }
+
+    SECTION("bigger automaton")
+    {
+        aut.initial = {1, 2};
+        aut.delta.add(1, 'a', 2);
+        aut.delta.add(1, 'a', 3);
+        aut.delta.add(1, 'b', 4);
+        aut.delta.add(2, 'a', 2);
+        aut.delta.add(2, 'a', 3);
+        aut.delta.add(2, 'b', 4);
+        aut.delta.add(3, 'b', 4);
+        aut.delta.add(3, 'c', 7);
+        aut.delta.add(3, 'b', 2);
+        aut.delta.add(7, 'a', 8);
+        aut.final = {3};
+
+        Nfa result = revert(aut);
+        //REQUIRE(result.final == StateSet({1, 2}));
         REQUIRE(StateSet(result.final) == StateSet({1, 2}));
-		REQUIRE(result.delta.contains(2, 'a', 1));
-		REQUIRE(result.delta.contains(3, 'a', 1));
-		REQUIRE(result.delta.contains(4, 'b', 1));
-		REQUIRE(result.delta.contains(2, 'a', 2));
-		REQUIRE(result.delta.contains(3, 'a', 2));
-		REQUIRE(result.delta.contains(4, 'b', 2));
-		REQUIRE(result.delta.contains(4, 'b', 3));
-		REQUIRE(result.delta.contains(7, 'c', 3));
-		REQUIRE(result.delta.contains(2, 'b', 3));
-		REQUIRE(result.delta.contains(8, 'a', 7));
-		REQUIRE(StateSet(result.initial) == StateSet({3}));
-	}
-
-	SECTION("Automaton A") {
-		Nfa nfa{ 11 };
-		FILL_WITH_AUT_A(nfa);
-		Nfa res = revert(nfa);
-		CHECK(res.initial[5]);
-		CHECK(res.final[1]);
-		CHECK(res.final[3]);
-		CHECK(res.get_num_of_trans() == 15);
-		CHECK(res.delta.contains(5, 'a', 5));
-		CHECK(res.delta.contains(5, 'a', 7));
-		CHECK(res.delta.contains(9, 'a', 9));
-		CHECK(res.delta.contains(9, 'c', 5));
-		CHECK(res.delta.contains(9, 'b', 3));
-		CHECK(res.delta.contains(7, 'a', 3));
-		CHECK(res.delta.contains(7, 'a', 10));
-		CHECK(res.delta.contains(7, 'b', 10));
-		CHECK(res.delta.contains(7, 'c', 10));
-		CHECK(res.delta.contains(7, 'b', 1));
-		CHECK(res.delta.contains(3, 'a', 7));
-		CHECK(res.delta.contains(3, 'c', 7));
-		CHECK(res.delta.contains(3, 'a', 1));
-		CHECK(res.delta.contains(1, 'b', 7));
-		CHECK(res.delta.contains(10, 'a', 1));
-	}
-
-	SECTION("Automaton B") {
-		Nfa nfa{ 15 };
-		FILL_WITH_AUT_B(nfa);
-		Nfa res = revert(nfa);
-		CHECK(res.initial[2]);
-		CHECK(res.initial[12]);
-		CHECK(res.final[4]);
-		CHECK(res.get_num_of_trans() == 12);
-		CHECK(res.delta.contains(8, 'a', 4));
-		CHECK(res.delta.contains(8, 'c', 4));
-		CHECK(res.delta.contains(4, 'b', 8));
-		CHECK(res.delta.contains(6, 'b', 4));
-		CHECK(res.delta.contains(6, 'a', 4));
-		CHECK(res.delta.contains(2, 'a', 6));
-		CHECK(res.delta.contains(2, 'a', 0));
-		CHECK(res.delta.contains(2, 'b', 2));
-		CHECK(res.delta.contains(0, 'a', 2));
-		CHECK(res.delta.contains(12, 'c', 2));
-		CHECK(res.delta.contains(12, 'b', 14));
-		CHECK(res.delta.contains(14, 'a', 12));
-	}
+        REQUIRE(result.delta.contains(2, 'a', 1));
+        REQUIRE(result.delta.contains(3, 'a', 1));
+        REQUIRE(result.delta.contains(4, 'b', 1));
+        REQUIRE(result.delta.contains(2, 'a', 2));
+        REQUIRE(result.delta.contains(3, 'a', 2));
+        REQUIRE(result.delta.contains(4, 'b', 2));
+        REQUIRE(result.delta.contains(4, 'b', 3));
+        REQUIRE(result.delta.contains(7, 'c', 3));
+        REQUIRE(result.delta.contains(2, 'b', 3));
+        REQUIRE(result.delta.contains(8, 'a', 7));
+        REQUIRE(StateSet(result.initial) == StateSet({3}));
+    }
+
+    SECTION("Automaton A") {
+        Nfa nfa{ 11 };
+        FILL_WITH_AUT_A(nfa);
+        Nfa res = revert(nfa);
+        CHECK(res.initial[5]);
+        CHECK(res.final[1]);
+        CHECK(res.final[3]);
+        CHECK(res.get_num_of_trans() == 15);
+        CHECK(res.delta.contains(5, 'a', 5));
+        CHECK(res.delta.contains(5, 'a', 7));
+        CHECK(res.delta.contains(9, 'a', 9));
+        CHECK(res.delta.contains(9, 'c', 5));
+        CHECK(res.delta.contains(9, 'b', 3));
+        CHECK(res.delta.contains(7, 'a', 3));
+        CHECK(res.delta.contains(7, 'a', 10));
+        CHECK(res.delta.contains(7, 'b', 10));
+        CHECK(res.delta.contains(7, 'c', 10));
+        CHECK(res.delta.contains(7, 'b', 1));
+        CHECK(res.delta.contains(3, 'a', 7));
+        CHECK(res.delta.contains(3, 'c', 7));
+        CHECK(res.delta.contains(3, 'a', 1));
+        CHECK(res.delta.contains(1, 'b', 7));
+        CHECK(res.delta.contains(10, 'a', 1));
+    }
+
+    SECTION("Automaton B") {
+        Nfa nfa{ 15 };
+        FILL_WITH_AUT_B(nfa);
+        Nfa res = revert(nfa);
+        CHECK(res.initial[2]);
+        CHECK(res.initial[12]);
+        CHECK(res.final[4]);
+        CHECK(res.get_num_of_trans() == 12);
+        CHECK(res.delta.contains(8, 'a', 4));
+        CHECK(res.delta.contains(8, 'c', 4));
+        CHECK(res.delta.contains(4, 'b', 8));
+        CHECK(res.delta.contains(6, 'b', 4));
+        CHECK(res.delta.contains(6, 'a', 4));
+        CHECK(res.delta.contains(2, 'a', 6));
+        CHECK(res.delta.contains(2, 'a', 0));
+        CHECK(res.delta.contains(2, 'b', 2));
+        CHECK(res.delta.contains(0, 'a', 2));
+        CHECK(res.delta.contains(12, 'c', 2));
+        CHECK(res.delta.contains(12, 'b', 14));
+        CHECK(res.delta.contains(14, 'a', 12));
+    }
 } // }}}
 
 
 TEST_CASE("Mata::Nfa::is_deterministic()")
 { // {{{
-	Nfa aut('s'+1);
+    Nfa aut('s'+1);
+
+    SECTION("(almost) empty automaton")
+    {
+        // no initial states
+        REQUIRE(!is_deterministic(aut));
+
+        // add an initial state
+        aut.initial.insert('q');
+        REQUIRE(is_deterministic(aut));
+
+        // add the same initial state
+        aut.initial.insert('q');
+        REQUIRE(is_deterministic(aut));
+
+        // add another initial state
+        aut.initial.insert('r');
+        REQUIRE(!is_deterministic(aut));
+
+        // add a final state
+        aut.final.insert('q');
+        REQUIRE(!is_deterministic(aut));
+    }
+
+    SECTION("trivial automata")
+    {
+        aut.initial.insert('q');
+        aut.delta.add('q', 'a', 'r');
+        REQUIRE(is_deterministic(aut));
 
-	SECTION("(almost) empty automaton")
-	{
-		// no initial states
-		REQUIRE(!is_deterministic(aut));
-
-		// add an initial state
-		aut.initial.insert('q');
-		REQUIRE(is_deterministic(aut));
-
-		// add the same initial state
-		aut.initial.insert('q');
-		REQUIRE(is_deterministic(aut));
-
-		// add another initial state
-		aut.initial.insert('r');
-		REQUIRE(!is_deterministic(aut));
-
-		// add a final state
-		aut.final.insert('q');
-		REQUIRE(!is_deterministic(aut));
-	}
-
-	SECTION("trivial automata")
-	{
-		aut.initial.insert('q');
-		aut.delta.add('q', 'a', 'r');
-		REQUIRE(is_deterministic(aut));
-
-		// unreachable states
-		aut.delta.add('s', 'a', 'r');
-		REQUIRE(is_deterministic(aut));
-
-		// transitions over a different symbol
-		aut.delta.add('q', 'b', 'h');
-		REQUIRE(is_deterministic(aut));
-
-		// nondeterminism
-		aut.delta.add('q', 'a', 's');
-		REQUIRE(!is_deterministic(aut));
-	}
-
-	SECTION("larger automaton 1")
-	{
-		FILL_WITH_AUT_A(aut);
-		REQUIRE(!is_deterministic(aut));
-	}
-
-	SECTION("larger automaton 2")
-	{
-		FILL_WITH_AUT_B(aut);
-		REQUIRE(!is_deterministic(aut));
-	}
+        // unreachable states
+        aut.delta.add('s', 'a', 'r');
+        REQUIRE(is_deterministic(aut));
+
+        // transitions over a different symbol
+        aut.delta.add('q', 'b', 'h');
+        REQUIRE(is_deterministic(aut));
+
+        // nondeterminism
+        aut.delta.add('q', 'a', 's');
+        REQUIRE(!is_deterministic(aut));
+    }
+
+    SECTION("larger automaton 1")
+    {
+        FILL_WITH_AUT_A(aut);
+        REQUIRE(!is_deterministic(aut));
+    }
+
+    SECTION("larger automaton 2")
+    {
+        FILL_WITH_AUT_B(aut);
+        REQUIRE(!is_deterministic(aut));
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::is_complete()")
 { // {{{
-	Nfa aut('q'+1);
+    Nfa aut('q'+1);
+
+    SECTION("empty automaton")
+    {
+        OnTheFlyAlphabet alph{};
+
+        // is complete for the empty alphabet
+        REQUIRE(is_complete(aut, alph));
 
-	SECTION("empty automaton")
-	{
-		OnTheFlyAlphabet alph{};
+        alph.translate_symb("a1");
+        alph.translate_symb("a2");
 
-		// is complete for the empty alphabet
-		REQUIRE(is_complete(aut, alph));
+        // the empty automaton is complete even for a non-empty alphabet
+        REQUIRE(is_complete(aut, alph));
 
-		alph.translate_symb("a1");
-		alph.translate_symb("a2");
+        // add a non-reachable state (the automaton should still be complete)
+        aut.delta.add('q', alph["a1"], 'q');
+        REQUIRE(is_complete(aut, alph));
+    }
+
+    SECTION("small automaton")
+    {
+        OnTheFlyAlphabet alph{};
+
+        aut.initial.insert(4);
+        aut.delta.add(4, alph["a"], 8);
+        aut.delta.add(4, alph["c"], 8);
+        aut.delta.add(4, alph["a"], 6);
+        aut.delta.add(4, alph["b"], 6);
+        aut.delta.add(8, alph["b"], 4);
+        aut.delta.add(6, alph["a"], 2);
+        aut.delta.add(2, alph["b"], 2);
+        aut.delta.add(2, alph["a"], 0);
+        aut.delta.add(2, alph["c"], 12);
+        aut.delta.add(0, alph["a"], 2);
+        aut.delta.add(12, alph["a"], 14);
+        aut.delta.add(14, alph["b"], 12);
+        aut.final.insert({2, 12});
 
-		// the empty automaton is complete even for a non-empty alphabet
-		REQUIRE(is_complete(aut, alph));
+        REQUIRE(!is_complete(aut, alph));
 
-		// add a non-reachable state (the automaton should still be complete)
-		aut.delta.add('q', alph["a1"], 'q');
-		REQUIRE(is_complete(aut, alph));
-	}
+        make_complete(aut, alph, 100);
+        REQUIRE(is_complete(aut, alph));
+    }
 
-	SECTION("small automaton")
-	{
-		OnTheFlyAlphabet alph{};
+    SECTION("using a non-alphabet symbol")
+    {
+        OnTheFlyAlphabet alph{};
 
         aut.initial.insert(4);
-		aut.delta.add(4, alph["a"], 8);
-		aut.delta.add(4, alph["c"], 8);
-		aut.delta.add(4, alph["a"], 6);
-		aut.delta.add(4, alph["b"], 6);
-		aut.delta.add(8, alph["b"], 4);
-		aut.delta.add(6, alph["a"], 2);
-		aut.delta.add(2, alph["b"], 2);
-		aut.delta.add(2, alph["a"], 0);
-		aut.delta.add(2, alph["c"], 12);
-		aut.delta.add(0, alph["a"], 2);
-		aut.delta.add(12, alph["a"], 14);
-		aut.delta.add(14, alph["b"], 12);
-		aut.final.insert({2, 12});
-
-		REQUIRE(!is_complete(aut, alph));
-
-		make_complete(aut, alph, 100);
-		REQUIRE(is_complete(aut, alph));
-	}
-
-	SECTION("using a non-alphabet symbol")
-	{
-		OnTheFlyAlphabet alph{};
-
-		aut.initial.insert(4);
-		aut.delta.add(4, alph["a"], 8);
-		aut.delta.add(4, alph["c"], 8);
-		aut.delta.add(4, alph["a"], 6);
-		aut.delta.add(4, alph["b"], 6);
-		aut.delta.add(6, 100, 4);
-
-		CHECK_THROWS_WITH(is_complete(aut, alph),
-			Catch::Contains("symbol that is not in the provided alphabet"));
-	}
+        aut.delta.add(4, alph["a"], 8);
+        aut.delta.add(4, alph["c"], 8);
+        aut.delta.add(4, alph["a"], 6);
+        aut.delta.add(4, alph["b"], 6);
+        aut.delta.add(6, 100, 4);
+
+        CHECK_THROWS_WITH(is_complete(aut, alph),
+            Catch::Contains("symbol that is not in the provided alphabet"));
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::is_prfx_in_lang()")
 { // {{{
-	Nfa aut('q'+1);
+    Nfa aut('q'+1);
+
+    SECTION("empty automaton")
+    {
+        Run w;
+        w.word = {'a', 'b', 'd'};
+        REQUIRE(!is_prfx_in_lang(aut, w));
 
-	SECTION("empty automaton")
-	{
-		Run w;
-		w.word = {'a', 'b', 'd'};
-		REQUIRE(!is_prfx_in_lang(aut, w));
-
-		w.word = { };
-		REQUIRE(!is_prfx_in_lang(aut, w));
-	}
-
-	SECTION("automaton accepting only epsilon")
-	{
-		aut.initial.insert('q');
-		aut.final.insert('q');
-
-		Run w;
-		w.word = { };
-		REQUIRE(is_prfx_in_lang(aut, w));
-
-		w.word = {'a', 'b'};
-		REQUIRE(is_prfx_in_lang(aut, w));
-	}
-
-	SECTION("small automaton")
-	{
-		FILL_WITH_AUT_B(aut);
+        w.word = { };
+        REQUIRE(!is_prfx_in_lang(aut, w));
+    }
+
+    SECTION("automaton accepting only epsilon")
+    {
+        aut.initial.insert('q');
+        aut.final.insert('q');
+
+        Run w;
+        w.word = { };
+        REQUIRE(is_prfx_in_lang(aut, w));
+
+        w.word = {'a', 'b'};
+        REQUIRE(is_prfx_in_lang(aut, w));
+    }
+
+    SECTION("small automaton")
+    {
+        FILL_WITH_AUT_B(aut);
 
         Run w;
-		w.word = {'b', 'a'};
-		REQUIRE(is_prfx_in_lang(aut, w));
+        w.word = {'b', 'a'};
+        REQUIRE(is_prfx_in_lang(aut, w));
 
-		w.word = { };
-		REQUIRE(!is_prfx_in_lang(aut, w));
+        w.word = { };
+        REQUIRE(!is_prfx_in_lang(aut, w));
 
-		w.word = {'c', 'b', 'a'};
-		REQUIRE(!is_prfx_in_lang(aut, w));
+        w.word = {'c', 'b', 'a'};
+        REQUIRE(!is_prfx_in_lang(aut, w));
 
-		w.word = {'c', 'b', 'a', 'a'};
-		REQUIRE(is_prfx_in_lang(aut, w));
+        w.word = {'c', 'b', 'a', 'a'};
+        REQUIRE(is_prfx_in_lang(aut, w));
 
-		w.word = {'a', 'a'};
-		REQUIRE(is_prfx_in_lang(aut, w));
+        w.word = {'a', 'a'};
+        REQUIRE(is_prfx_in_lang(aut, w));
 
-		w.word = {'c', 'b', 'b', 'a', 'c', 'b'};
-		REQUIRE(is_prfx_in_lang(aut, w));
+        w.word = {'c', 'b', 'b', 'a', 'c', 'b'};
+        REQUIRE(is_prfx_in_lang(aut, w));
 
-		w.word = Word(100000, 'a');
-		REQUIRE(is_prfx_in_lang(aut, w));
+        w.word = Word(100000, 'a');
+        REQUIRE(is_prfx_in_lang(aut, w));
 
-		w.word = Word(100000, 'b');
-		REQUIRE(!is_prfx_in_lang(aut, w));
-	}
+        w.word = Word(100000, 'b');
+        REQUIRE(!is_prfx_in_lang(aut, w));
+    }
 } // }}}
 
 TEST_CASE("Mata::Nfa::fw-direct-simulation()")
 { // {{{
     Nfa aut;
 
     SECTION("empty automaton")
@@ -2289,106 +2022,106 @@
         REQUIRE(result.get(8,2));
         REQUIRE(result.get(8,5));
     }
 } // }}
 
 TEST_CASE("Mata::Nfa::reduce_size_by_simulation()")
 {
-	Nfa aut;
-	StateToStateMap state_map;
+    Nfa aut;
+    StateRenaming state_renaming;
+
+    SECTION("empty automaton")
+    {
+        Nfa result = reduce(aut, false, &state_renaming);
 
-	SECTION("empty automaton")
-	{
-		Nfa result = reduce(aut, false, &state_map);
-
-		REQUIRE(result.delta.empty());
-		REQUIRE(result.initial.empty());
-		REQUIRE(result.final.empty());
-	}
-
-	SECTION("simple automaton")
-	{
-		aut.add_state(2);
+        REQUIRE(result.delta.empty());
+        REQUIRE(result.initial.empty());
+        REQUIRE(result.final.empty());
+    }
+
+    SECTION("simple automaton")
+    {
+        aut.add_state(2);
         aut.initial.insert(1);
 
         aut.final.insert(2);
-		Nfa result = reduce(aut, false, &state_map);
+        Nfa result = reduce(aut, false, &state_renaming);
 
-		REQUIRE(result.delta.empty());
-		REQUIRE(result.initial[state_map[1]]);
-		REQUIRE(result.final[state_map[2]]);
-		REQUIRE(result.size() == 2);
-		REQUIRE(state_map[1] == state_map[0]);
-		REQUIRE(state_map[2] != state_map[0]);
-	}
-
-	SECTION("big automaton")
-	{
-		aut.add_state(9);
-		aut.initial = {1, 2};
-		aut.delta.add(1, 'a', 2);
-		aut.delta.add(1, 'a', 3);
-		aut.delta.add(1, 'b', 4);
-		aut.delta.add(2, 'a', 2);
-		aut.delta.add(2, 'b', 2);
-		aut.delta.add(2, 'a', 3);
-		aut.delta.add(2, 'b', 4);
-		aut.delta.add(3, 'b', 4);
-		aut.delta.add(3, 'c', 7);
-		aut.delta.add(3, 'b', 2);
-		aut.delta.add(5, 'c', 3);
-		aut.delta.add(7, 'a', 8);
-		aut.delta.add(9, 'b', 2);
-		aut.delta.add(9, 'c', 0);
-		aut.delta.add(0, 'a', 4);
-		aut.final = {3, 9};
-
-
-		Nfa result = reduce(aut, false, &state_map);
-
-		REQUIRE(result.size() == 6);
-		REQUIRE(result.initial[state_map[1]]);
-		REQUIRE(result.initial[state_map[2]]);
-		REQUIRE(result.delta.contains(state_map[9], 'c', state_map[0]));
-		REQUIRE(result.delta.contains(state_map[9], 'c', state_map[7]));
-		REQUIRE(result.delta.contains(state_map[3], 'c', state_map[0]));
-		REQUIRE(result.delta.contains(state_map[0], 'a', state_map[8]));
-		REQUIRE(result.delta.contains(state_map[7], 'a', state_map[4]));
-		REQUIRE(result.delta.contains(state_map[1], 'a', state_map[3]));
-		REQUIRE(!result.delta.contains(state_map[3], 'b', state_map[4]));
-		REQUIRE(result.delta.contains(state_map[2], 'a', state_map[2]));
-		REQUIRE(result.final[state_map[9]]);
-		REQUIRE(result.final[state_map[3]]);
+        REQUIRE(result.delta.empty());
+        REQUIRE(result.initial[state_renaming[1]]);
+        REQUIRE(result.final[state_renaming[2]]);
+        REQUIRE(result.size() == 2);
+        REQUIRE(state_renaming[1] == state_renaming[0]);
+        REQUIRE(state_renaming[2] != state_renaming[0]);
+    }
+
+    SECTION("big automaton")
+    {
+        aut.add_state(9);
+        aut.initial = {1, 2};
+        aut.delta.add(1, 'a', 2);
+        aut.delta.add(1, 'a', 3);
+        aut.delta.add(1, 'b', 4);
+        aut.delta.add(2, 'a', 2);
+        aut.delta.add(2, 'b', 2);
+        aut.delta.add(2, 'a', 3);
+        aut.delta.add(2, 'b', 4);
+        aut.delta.add(3, 'b', 4);
+        aut.delta.add(3, 'c', 7);
+        aut.delta.add(3, 'b', 2);
+        aut.delta.add(5, 'c', 3);
+        aut.delta.add(7, 'a', 8);
+        aut.delta.add(9, 'b', 2);
+        aut.delta.add(9, 'c', 0);
+        aut.delta.add(0, 'a', 4);
+        aut.final = {3, 9};
+
+
+        Nfa result = reduce(aut, false, &state_renaming);
+
+        REQUIRE(result.size() == 6);
+        REQUIRE(result.initial[state_renaming[1]]);
+        REQUIRE(result.initial[state_renaming[2]]);
+        REQUIRE(result.delta.contains(state_renaming[9], 'c', state_renaming[0]));
+        REQUIRE(result.delta.contains(state_renaming[9], 'c', state_renaming[7]));
+        REQUIRE(result.delta.contains(state_renaming[3], 'c', state_renaming[0]));
+        REQUIRE(result.delta.contains(state_renaming[0], 'a', state_renaming[8]));
+        REQUIRE(result.delta.contains(state_renaming[7], 'a', state_renaming[4]));
+        REQUIRE(result.delta.contains(state_renaming[1], 'a', state_renaming[3]));
+        REQUIRE(!result.delta.contains(state_renaming[3], 'b', state_renaming[4]));
+        REQUIRE(result.delta.contains(state_renaming[2], 'a', state_renaming[2]));
+        REQUIRE(result.final[state_renaming[9]]);
+        REQUIRE(result.final[state_renaming[3]]);
 
-        result = reduce(aut, true, &state_map);
+        result = reduce(aut, true, &state_renaming);
         CHECK(result.size() == 3);
         CHECK(result.initial.size() == 2);
         for (State initial : result.initial) {
-            CHECK(((initial == state_map[1]) || (initial == state_map[2])));
+            CHECK(((initial == state_renaming[1]) || (initial == state_renaming[2])));
         }
         REQUIRE(result.final.size() == 1);
         for (State final : result.final) {
-            CHECK(final == state_map[3]);
+            CHECK(final == state_renaming[3]);
         }
         CHECK(result.delta.size() == 6);
-        CHECK(result.delta.contains(state_map[1], 'a', state_map[3]));
-        CHECK(result.delta.contains(state_map[1], 'a', state_map[2]));
-        CHECK(result.delta.contains(state_map[2], 'a', state_map[2]));
-        CHECK(result.delta.contains(state_map[2], 'b', state_map[2]));
-        CHECK(result.delta.contains(state_map[2], 'a', state_map[3]));
-        CHECK(result.delta.contains(state_map[3], 'b', state_map[2]));
-	}
-
-	SECTION("no transitions from non-final state")
-	{
-		aut.delta.add(0, 'a', 1);
-		aut.initial = { 0 };
-		Nfa result = reduce(aut, true, &state_map);
-		CHECK(Mata::Nfa::are_equivalent(result, aut));
-	}
+        CHECK(result.delta.contains(state_renaming[1], 'a', state_renaming[3]));
+        CHECK(result.delta.contains(state_renaming[1], 'a', state_renaming[2]));
+        CHECK(result.delta.contains(state_renaming[2], 'a', state_renaming[2]));
+        CHECK(result.delta.contains(state_renaming[2], 'b', state_renaming[2]));
+        CHECK(result.delta.contains(state_renaming[2], 'a', state_renaming[3]));
+        CHECK(result.delta.contains(state_renaming[3], 'b', state_renaming[2]));
+    }
+
+    SECTION("no transitions from non-final state")
+    {
+        aut.delta.add(0, 'a', 1);
+        aut.initial = { 0 };
+        Nfa result = reduce(aut, true, &state_renaming);
+        CHECK(Mata::Nfa::are_equivalent(result, aut));
+    }
 }
 
 TEST_CASE("Mata::Nfa::union_norename()") {
     Run one{{1},{}};
     Run zero{{0}, {}};
 
     Nfa lhs(2);
@@ -2476,65 +2209,57 @@
             REQUIRE(!aut.delta.contains(4, 'a', 8));
             REQUIRE(!aut.delta.contains(4, 'c', 8));
             REQUIRE(aut.delta[4].size() == 1);
         }
     }
 }
 
-TEST_CASE("Mafa::Nfa::get_moves_from()")
-{
+TEST_CASE("Mafa::Nfa::get_moves_from()") {
     Nfa aut{};
 
-    SECTION("Add new states within the limit")
-    {
+    SECTION("Add new states within the limit") {
         aut.add_state(19);
         aut.initial.insert(0);
         aut.initial.insert(1);
         aut.initial.insert(2);
         REQUIRE_NOTHROW(aut.get_moves_from(0));
         REQUIRE_NOTHROW(aut.get_moves_from(1));
         REQUIRE_NOTHROW(aut.get_moves_from(2));
         REQUIRE(aut.get_moves_from(0).empty());
         REQUIRE(aut.get_moves_from(1).empty());
         REQUIRE(aut.get_moves_from(2).empty());
     }
 
-    SECTION("Add new states over the limit")
-    {
+    SECTION("Add new states over the limit") {
         aut.add_state(1);
         REQUIRE_NOTHROW(aut.initial.insert(0));
         REQUIRE_NOTHROW(aut.initial.insert(1));
-        //REQUIRE_THROWS_AS(aut.initial.insert(2), std::runtime_error);
         REQUIRE_NOTHROW(aut.get_moves_from(0));
         REQUIRE_NOTHROW(aut.get_moves_from(1));
-        //REQUIRE_THROWS(aut.get_moves_from(2)); // FIXME: Fails on assert. Catch2 cannot catch assert failure.
+        REQUIRE_THROWS(aut.get_moves_from(2));
         REQUIRE(aut.get_moves_from(0).empty());
         REQUIRE(aut.get_moves_from(1).empty());
-        //REQUIRE_THROWS(aut.get_moves_from(2)); // FIXME: Fails on assert. Catch2 cannot catch assert failure.
+        REQUIRE_THROWS(aut.get_moves_from(2));
     }
 
-    //TODO: modify or remove these
-    //SECTION("Add new states without specifying the number of states")
-    //{
-    //    REQUIRE_THROWS_AS(aut.initial.insert(0), std::runtime_error);
-    //    //REQUIRE_THROWS(aut.get_moves_from(2)); // FIXME: Fails on assert. Catch2 cannot catch assert failure.
-    //}
+    SECTION("Add new states without specifying the number of states") {
+        CHECK_NOTHROW(aut.initial.insert(0));
+        CHECK_THROWS_AS(aut.get_moves_from(2), std::runtime_error);
+    }
 
-    //SECTION("Add new initial without specifying the number of states with over +1 number")
-    //{
-    //    REQUIRE_THROWS_AS(aut.initial.insert(25), std::runtime_error);
-    //    //REQUIRE_THROWS(aut.get_moves_from(25)); // FIXME: Fails on assert. Catch2 cannot catch assert failure.
-    //}
+    SECTION("Add new initial without specifying the number of states with over +1 number") {
+        REQUIRE_NOTHROW(aut.initial.insert(25));
+        CHECK_NOTHROW(aut.get_moves_from(25));
+        CHECK_THROWS(aut.get_moves_from(26));
+    }
 }
 
-
-TEST_CASE("Mata::Nfa::get_trans_as_sequence(}")
-{
+TEST_CASE("Mata::Nfa::get_trans_as_sequence(}") {
     Nfa aut('q' + 1);
-    TransSequence expected{};
+    std::vector<Trans> expected{};
 
     aut.delta.add(1, 2, 3);
     expected.emplace_back(1, 2, 3);
     aut.delta.add(1, 3, 4);
     expected.emplace_back(1, 3, 4);
     aut.delta.add(2, 3, 4);
     expected.emplace_back(2, 3, 4);
@@ -2717,15 +2442,15 @@
         aut.trim();
         CHECK(aut.delta.empty());
         CHECK(aut.size() == 0);
     }
 
     SECTION("With state map") {
         Nfa aut{orig_aut};
-        StateToStateMap state_map{};
+        StateRenaming state_map{};
         aut.trim(&state_map);
         CHECK(aut.initial.size() == orig_aut.initial.size());
         CHECK(aut.final.size() == orig_aut.final.size());
         CHECK(aut.size() == 4);
         for (const Word& word: get_shortest_words(orig_aut))
         {
             CHECK(is_in_lang(aut, Run{word,{}}));
@@ -2962,19 +2687,19 @@
     CHECK(state_eps_trans->targets == StateSet{3, 4, 6 });
 
     CHECK(aut.get_epsilon_transitions(1) == aut.get_moves_from(1).end());
     CHECK(aut.get_epsilon_transitions(5) == aut.get_moves_from(5).end());
     CHECK(aut.get_epsilon_transitions(19) == aut.get_moves_from(19).end());
 
     Post post{ aut.delta[0] };
-    state_eps_trans = aut.get_epsilon_transitions(post);
+    state_eps_trans = Nfa::get_epsilon_transitions(post);
     CHECK(state_eps_trans->symbol == EPSILON);
     CHECK(state_eps_trans->targets == StateSet{3 });
     post = aut.delta[3];
-    state_eps_trans = aut.get_epsilon_transitions(post);
+    state_eps_trans = Nfa::get_epsilon_transitions(post);
     CHECK(state_eps_trans->symbol == EPSILON);
     CHECK(state_eps_trans->targets == StateSet{3, 4 });
 
     post = aut.get_moves_from(1);
     CHECK(aut.get_epsilon_transitions(post) == post.end());
     post = aut.get_moves_from(5);
     CHECK(aut.get_epsilon_transitions(post) == post.end());
@@ -3000,52 +2725,50 @@
 }
 
 TEST_CASE("Mata::Nfa:: create simple automata") {
     Nfa nfa{ Builder::create_empty_string_nfa() };
     CHECK(is_in_lang(nfa, { {}, {} }));
     CHECK(get_word_lengths(nfa) == std::set<std::pair<int, int>>{ std::make_pair(0, 0) });
 
-    OnTheFlyAlphabet alphabet{};
-    StringToSymbolMap symbol_map{ { "a", 0 }, { "b", 1 }, { "c", 2 } };
-    alphabet.add_symbols_from(symbol_map);
+    OnTheFlyAlphabet alphabet{ { "a", 0 }, { "b", 1 }, { "c", 2 } };
     nfa = Builder::create_sigma_star_nfa(&alphabet);
     CHECK(is_in_lang(nfa, { {}, {} }));
     CHECK(is_in_lang(nfa, { { 0 }, {} }));
     CHECK(is_in_lang(nfa, { { 1 }, {} }));
     CHECK(is_in_lang(nfa, { { 2 }, {} }));
     CHECK(is_in_lang(nfa, { { 0, 1 }, {} }));
     CHECK(is_in_lang(nfa, { { 1, 0 }, {} }));
     CHECK(is_in_lang(nfa, { { 2, 2, 2 }, {} }));
     CHECK(is_in_lang(nfa, { { 0, 1, 2, 2, 0, 1, 2, 1, 0, 0, 2, 1 }, {} }));
     CHECK(!is_in_lang(nfa, { { 3 }, {} }));
 }
 
 TEST_CASE("Mata::Nfa:: print_to_mata") {
-	Nfa aut_big;
-	aut_big.initial = {1, 2};
-	aut_big.delta.add(1, 'a', 2);
-	aut_big.delta.add(1, 'a', 3);
-	aut_big.delta.add(1, 'b', 4);
-	aut_big.delta.add(2, 'a', 2);
-	aut_big.delta.add(2, 'b', 2);
-	aut_big.delta.add(2, 'a', 3);
-	aut_big.delta.add(2, 'b', 4);
-	aut_big.delta.add(3, 'b', 4);
-	aut_big.delta.add(3, 'c', 7);
-	aut_big.delta.add(3, 'b', 2);
-	aut_big.delta.add(5, 'c', 3);
-	aut_big.delta.add(7, 'a', 8);
-	aut_big.final = {3};
-
-	std::string aut_big_mata = aut_big.print_to_mata();
-	// for parsing output of print_to_mata() we need to use IntAlphabet to get the same alphabet
-	IntAlphabet int_alph;
-	Nfa aut_big_from_mata = Builder::construct(Mata::IntermediateAut::parse_from_mf(parse_mf(aut_big_mata))[0], &int_alph);
+    Nfa aut_big;
+    aut_big.initial = {1, 2};
+    aut_big.delta.add(1, 'a', 2);
+    aut_big.delta.add(1, 'a', 3);
+    aut_big.delta.add(1, 'b', 4);
+    aut_big.delta.add(2, 'a', 2);
+    aut_big.delta.add(2, 'b', 2);
+    aut_big.delta.add(2, 'a', 3);
+    aut_big.delta.add(2, 'b', 4);
+    aut_big.delta.add(3, 'b', 4);
+    aut_big.delta.add(3, 'c', 7);
+    aut_big.delta.add(3, 'b', 2);
+    aut_big.delta.add(5, 'c', 3);
+    aut_big.delta.add(7, 'a', 8);
+    aut_big.final = {3};
+
+    std::string aut_big_mata = aut_big.print_to_mata();
+    // for parsing output of print_to_mata() we need to use IntAlphabet to get the same alphabet
+    IntAlphabet int_alph;
+    Nfa aut_big_from_mata = Builder::construct(Mata::IntermediateAut::parse_from_mf(parse_mf(aut_big_mata))[0], &int_alph);
 
-	CHECK(are_equivalent(aut_big, aut_big_from_mata));
+    CHECK(are_equivalent(aut_big, aut_big_from_mata));
 }
 
 TEST_CASE("Mata::Nfa::trim bug") {
 	Nfa aut(5, {0}, {4});
 	aut.delta.add(0, 122, 1);
 	aut.delta.add(1, 98, 1);
 	aut.delta.add(1, 122, 1);
```

### Comparing `libmata-0.91.0/mata/tests/ord-vector.cc` & `libmata-0.92.0/mata/tests/ord-vector.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/parser.cc` & `libmata-0.92.0/mata/tests/parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/re2parser.cc` & `libmata-0.92.0/mata/tests/re2parser.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/sparse-set.cc` & `libmata-0.92.0/mata/tests/sparse-set.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/strings/nfa-noodlification.cc` & `libmata-0.92.0/mata/tests/strings/nfa-noodlification.cc`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
     SECTION("Simple automata") {
         Nfa x, y, z, w;
         create_nfa(&x, "a*");
         create_nfa(&y, "(a|b)*");
         create_nfa(&z, "(a|b)*");
         create_nfa(&w, "(a|b)*");
 
-        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::EpsCntVector>>>( {
+        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::VisitedEpsilonsCounterVector>>>({
                 {{x, {0, 0} }, {x, {0, 1} }, {y, {1, 1} }},
                 {{x, {0, 0} }, {y, {1, 0} }, {y, {1, 1} }} } );
         SegNfa::NoodleSubstSequence noodles = SegNfa::noodlify_for_equation(
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(x), std::make_shared<Nfa>(y) },
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(z), std::make_shared<Nfa>(w)});
         for(size_t i = 0; i < noodles.size(); i++) {
             for(size_t j = 0; j < noodles[i].size(); j++) {
@@ -387,15 +387,15 @@
         Nfa x, y, z, w, astar;
         create_nfa(&x, "a+");
         create_nfa(&y, "(a|b)*");
         create_nfa(&z, "(a|b)*");
         create_nfa(&w, "(a|b)+");
         create_nfa(&astar, "a*");
 
-        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::EpsCntVector>>>( {
+        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::VisitedEpsilonsCounterVector>>>({
                 {{x, {0, 1} }, {z, {1, 1} }},
                 {{x, {0, 0} }, {w, {1, 1} }},
                 {{x, {0, 0} }, {x, {0, 1} }, {z, {1, 1} }},
                 {{x, {0, 0} }, {z, {1, 0} }, {w, {1, 1} }},
          } );
         SegNfa::NoodleSubstSequence noodles = SegNfa::noodlify_for_equation(
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(x), std::make_shared<Nfa>(y) },
@@ -413,15 +413,15 @@
     SECTION("Simple automata -- epsilon input") {
         Nfa x, y, z, w;
         create_nfa(&x, "");
         create_nfa(&y, "(a|b)*");
         create_nfa(&z, "(a|b)*");
         create_nfa(&w, "(a|b)*");
 
-        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::EpsCntVector>>>( {} );
+        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::VisitedEpsilonsCounterVector>>>({} );
        SegNfa::NoodleSubstSequence noodles = SegNfa::noodlify_for_equation(
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(x) },
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(y), std::make_shared<Nfa>(z), std::make_shared<Nfa>(w)});
         CHECK(noodles.size() == 1);
         for(size_t i = 0; i < noodles.size(); i++) {
             for(size_t j = 0; j < noodles[i].size(); j++) {
                 CHECK(noodles[i][j].second == res[i][j].second);
@@ -435,15 +435,15 @@
     SECTION("Simple automata -- epsilon input 2") {
         Nfa x, y, z, w;
         create_nfa(&x, "");
         create_nfa(&y, "(a|b)*");
         create_nfa(&z, "(a|b)*");
         create_nfa(&w, "(a|b)*");
 
-        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::EpsCntVector>>>( {
+        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::VisitedEpsilonsCounterVector>>>({
                 {{y, {1, 1} }},
                 {{y, {1, 0} }, {y, {1, 1} }},
             } );
         SegNfa::NoodleSubstSequence noodles = SegNfa::noodlify_for_equation(
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(x), std::make_shared<Nfa>(y) },
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(z), std::make_shared<Nfa>(w)});
         CHECK(noodles.size() == 2);
@@ -460,15 +460,15 @@
     SECTION("Simple automata -- regex 1") {
         Nfa x, y, z, u;
         create_nfa(&x, "a");
         create_nfa(&y, "ab*");
         create_nfa(&z, "ab*");
         create_nfa(&u, "a*");
 
-        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::EpsCntVector>>>( {
+        auto res = std::vector<std::vector<std::pair<Nfa, SegNfa::VisitedEpsilonsCounterVector>>>({
                 {{x, {0, 0} }, {x, {1, 1} }},
             } );
         SegNfa::NoodleSubstSequence noodles = SegNfa::noodlify_for_equation(
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(x), std::make_shared<Nfa>(y) },
             std::vector<std::shared_ptr<Nfa>>{std::make_shared<Nfa>(z), std::make_shared<Nfa>(u)});
         CHECK(noodles.size() == 1);
         for(size_t i = 0; i < noodles.size(); i++) {
@@ -503,12 +503,12 @@
     right_side.delta.add(1, 'a', 2);
     right_side.delta.add(2, 'b', 3);
     right_side.delta.add(0, 'b', 4);
     right_side.delta.add(4, 'a', 5);
     right_side.delta.add(5, 'b', 6);
     right_side.final.insert({3, 6});
 
-    AutPtrSequence left_side{ &left1, &left2, &left3 };
+    std::vector<Nfa*> left_side{ &left1, &left2, &left3 };
     for (size_t i{}; i < 10000; ++i) {
         SegNfa::noodlify_for_equation(left_side, right_side);
     }
 }
```

### Comparing `libmata-0.91.0/mata/tests/strings/nfa-segmentation.cc` & `libmata-0.92.0/mata/tests/strings/nfa-segmentation.cc`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
         aut.delta.add(6, epsilon, 7);
         aut.delta.add(7, epsilon, 8);
 
         auto segmentation{SegNfa::Segmentation{aut, epsilons } };
         const auto& epsilon_depth_transitions{ segmentation.get_epsilon_depths() };
 
         REQUIRE(epsilon_depth_transitions == SegNfa::Segmentation::EpsilonDepthTransitions{
-                {0, TransSequence{{1, epsilon, 2}}},
-                {1, TransSequence{{6, epsilon, 7}}},
-                {2, TransSequence{{7, epsilon, 8}}},
+                {0, std::vector<Trans>{{1, epsilon, 2}}},
+                {1, std::vector<Trans>{{6, epsilon, 7}}},
+                {2, std::vector<Trans>{{7, epsilon, 8}}},
         });
     }
 
 }
 
 TEST_CASE("Mata::Nfa::Segmentation::split_segment_automaton()") {
     Symbol epsilon{ 'c' };
```

### Comparing `libmata-0.91.0/mata/tests/strings/nfa-string-solving.cc` & `libmata-0.92.0/mata/tests/strings/nfa-string-solving.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/mata/tests/synchronized-iterator.cc` & `libmata-0.92.0/mata/tests/synchronized-iterator.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.91.0/setup.py` & `libmata-0.92.0/setup.py`

 * *Files identical despite different names*

