# Comparing `tmp/naluconfigs-11.3.1.tar.gz` & `tmp/naluconfigs-12.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-11.3.1.tar", last modified: Wed Jul 26 18:58:25 2023, max compression
+gzip compressed data, was "naluconfigs-12.1.0.tar", last modified: Tue Aug  8 01:34:19 2023, max compression
```

## Comparing `naluconfigs-11.3.1.tar` & `naluconfigs-12.1.0.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.941800 naluconfigs-11.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-26 18:58:25.941800 naluconfigs-11.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:58:25.941800 naluconfigs-11.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.933800 naluconfigs-11.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.933800 naluconfigs-11.3.1/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.933800 naluconfigs-11.3.1/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.933800 naluconfigs-11.3.1/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/chips/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.937800 naluconfigs-11.3.1/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.941800 naluconfigs-11.3.1/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (123)    21676 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33686 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.933800 naluconfigs-11.3.1/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-26 18:58:25.000000 naluconfigs-11.3.1/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-26 18:58:25.000000 naluconfigs-11.3.1/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:58:25.000000 naluconfigs-11.3.1/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 18:58:25.000000 naluconfigs-11.3.1/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 18:58:25.000000 naluconfigs-11.3.1/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:58:25.941800 naluconfigs-11.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-26 18:58:09.000000 naluconfigs-11.3.1/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.706742 naluconfigs-12.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-08 01:34:19.706742 naluconfigs-12.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:34:19.706742 naluconfigs-12.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.698742 naluconfigs-12.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.698742 naluconfigs-12.1.0/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.698742 naluconfigs-12.1.0/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.698742 naluconfigs-12.1.0/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/chips/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.702742 naluconfigs-12.1.0/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.706742 naluconfigs-12.1.0/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21676 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    33686 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.698742 naluconfigs-12.1.0/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-08 01:34:19.000000 naluconfigs-12.1.0/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-08 01:34:19.000000 naluconfigs-12.1.0/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:34:19.000000 naluconfigs-12.1.0/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 01:34:19.000000 naluconfigs-12.1.0/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 01:34:19.000000 naluconfigs-12.1.0/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:34:19.706742 naluconfigs-12.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-08-08 01:34:01.000000 naluconfigs-12.1.0/tests/test_range_keys.py
```

### Comparing `naluconfigs-11.3.1/PKG-INFO` & `naluconfigs-12.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.3.1
+Version: 12.1.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.3.1/README.md` & `naluconfigs-12.1.0/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/pyproject.toml` & `naluconfigs-12.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/setup.py` & `naluconfigs-12.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/__init__.py` & `naluconfigs-12.1.0/src/naluconfigs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from . import _constructors
 from ._version import __version__
 from .helpers import CLOCKS_DIR, REGISTERS_DIR
 
 _VALID_BOARDS = [
     "aardvarcv2",
     "aardvarcv3",
-    "aardvarcv3_gbe",
     "aardvarcv4",
     "aodsv1",
     "aodsv2_eval",
     "asoc",
     "asocv2",
     "asocv3",
     "trbhm",
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/_constructors.py` & `naluconfigs-12.1.0/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/chips/aardvarcv4.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/chips/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/chips/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/chips/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-12.1.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,326 +1,325 @@
-model: aardvarcv3
+model: aodsv1
 features:
-  adc2mv: true
-  calibration_channel: true
+  adc2mv: false
   dac_sweep: true
   ext_dac: true
   pedestals: true
   threshold_scan: true
   tia_dac: false
-  timing_calibration: true
+  timing_calibration: false
   naludaq_rs: true
 params:
-  chanmask: 3072
+  chanmask: 1536
   channels: 4
-  chanshift: 10
+  chanshift: 9
   chips:
     0:
       !include_chip
-      from: aardvarcv3::params
-  clock_file: Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+      from: aodsv1::params
+  clock_file: AODS_300GCC.txt  #  AODS_debugpulse_240MGCC_10Mref.txt
   connections:
     - serial
     - d2xx
-    - udp
   si5341_address: 0xE8
   default_baud:
-    115200: 53
-  default_baudrate: 115200
-  default_clock: 100000000.0
+    111111: 53
+  default_baudrate: 111111
+  default_clock: 200000000.0
   default_divider: 53
-  default_trigger_value: 1500
+  default_trigger_value: 2000
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
   ext_dac:
-    chip: dac7578
-    max_mv: 1200
+    chip: ad5671
+    max_mv: 2500
     max_counts: 4095
     channels:
-      0..3: 2048
+      0: 2048
+      1: 2175
+      2: 1968
+      3: 2048
     address_mapping:
-      0..3: 0x4E
+      0..3: 0xC
     channel_mapping:
-      0: 2
-      1: 6
-      2: 3
-      3: 7
-    cal:
-      channel: 1
-      address: 0x4E
-      value: 2048
+      0: 1
+      1: 0
+      2: 5
+      3: 4
   headers: 3
-  new_firmware: True
-  numregs: 64
-  pedestals_blocks: 16
+  numregs: 36
+  pedestals_blocks: 32
   peripherals:
-    current_1v2:
+    current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
-      r_sense: 0.05
-    current_2v5:
-      chan: 1
-      addr: 0xD0
-      bits: 16
-      gain: 8
-      r_sense: 0.05
     vadjn:
       chan: 0
       addr: 0xD8
       bits: 16
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
+    eeprom:
+      addr: 0x50 # 7-bit
+      capacity: 0x20000 # bytes
+      page_size: 256 # bytes
+      segments:
+        analog_registers:
+          begin: 0
+          length: 300
+        digital_registers:
+          begin: 300
+          length: 330
+        control_registers:
+          begin: 630
+          length: 70
   possible_bauds:
-    115200: 53
-    230400: 26
-    691200: 8
-    1041667: 5
+    111111: 53
+    1500000: 3
   resolution: 12
   samples: 64
-  samplingrate: 10.0
+  samplingrate: 1.0
   stop_word: !!binary |
     +s4=
-  strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
-  strobe_correction_keys:
-    - calstrb_le
-    - calstrb_te
-    - wrstrb1_le
-    - wrstrb1_te
-    - wrstrb2_le
-    - wrstrb2_te
-    - wrsync1_le
-    - wrsync1_te
-    - wrsync2_le
-    - wrsync2_te
   wait: AE000001
-  wbias: 2000
-  windmask: 1022
-  windows: 510
+  wbias: 848
+  windmask: 510
+  windows: 254
 registers:
   analog_registers:
     !include_registers
-      from: aardvarcv3::registers::analog_registers
+      from: aodsv1::registers::analog_registers
   digital_registers:
     !include_registers
-      from: aardvarcv3::registers::digital_registers
-      delete:
-        - pllmisc
-        - txspeed
-        - waitread
+      from: aodsv1::registers::digital_registers
   control_registers:
-    1v2_en:
-      address: 0x17
-      bitposition: 1
-      bitwidth: 1
-      description: ''
+    trig_mux:
+      address: 0x22
+      bitposition: 5
+      bitwidth: 4
+      description: 'evttrig driver'
       readwrite: rw
-      value: true
-    2v5_en:
-      address: 0x17
+      value: 3
+    fpga_misc_t:
+      address: 0x22
       bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 4
+      description: 'fpga misc output disable'
       readwrite: rw
-      value: true
-    3v3_i2c_en:
-      address: 0x17
-      bitposition: 2
+      value: 15
+    2v5_en:
+      address: 0x16
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    8b10b_en:
-      address: 0x19
-      bitposition: 12
+    2v5_pll_en:
+      address: 0x16
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     addr:
-      address: 0x16
+      address: 0x15
       bitposition: 0
       bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
     addr_user:
-      address: 0x16
+      address: 0x15
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    brightness_blue:
+      address: 0x0A
+      bitposition: 0
+      bitwidth: 8
+      description: ''
+      readwrite: rw
+      value: 0
+    brightness_red:
+      address: 0x0B
+      bitposition: 0
+      bitwidth: 8
+      description: ''
+      readwrite: rw
+      value: 0
+    brightness_white:
+      address: 0x0A
+      bitposition: 8
+      bitwidth: 8
+      description: ''
+      readwrite: rw
+      value: 0
     chansel:
       address: 0x06
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    clk1v8_en:
-      address: 0x17
-      bitposition: 4
+    clk_1v8_nshutdown:
+      address: 0x16
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
+    clk_2v5_en:
+      address: 0x16
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_fdec:
-      address: 0x17
-      bitposition: 9
+    clk_i2c_sel:
+      address: 0x16
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    clk_finc:
-      address: 0x17
-      bitposition: 8
+      value: true
+    clk_noe:
+      address: 0x16
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_i2c_sel:
-      address: 0x17
-      bitposition: 5
+    clk_nrst:
+      address: 0x16
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_reset:
-      address: 0x17
+    clk_nsync:
+      address: 0x16
       bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_sync:
-      address: 0x17
+    dac_nrst:
+      address: 0x16
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: 1
     data:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     data_user:
       address: 0x14
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    debug_data:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
-      value: 0
-    debug_data_user:
-      address: 0x15
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
     digrst:
       address: 0x16
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    digser_rst:
-      address: 0x19
-      bitposition: 13
+    ext_en:
+      address: 0x0B
+      bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: true
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    fake:
+      address: 0x06
+      bitposition: 0
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
     gccclr:
       address: 0x04
-      bitposition: 4
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    i2c_switch:
+      address: 0x16
+      bitposition: 8
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
     identifier:
       address: 0x00
       bitposition: 0
       bitwidth: 16
       description: ''
+      readwrite: r
+      value: 41173
+    in_sel:
+      address: 0x0B
+      bitposition: 12
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 43714
+      value: true
     iomode0:
       address: 0x04
-      bitposition: 0
+      bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: 1
     iomode1:
       address: 0x04
-      bitposition: 6
+      bitposition: 8
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    leds:
-      address: 0x18
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
       value: 0
     loadwait:
       address: 0x07
       bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
     nramp:
       address: 0x04
-      bitposition: 5
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     nrw:
       address: 0x04
       bitposition: 11
@@ -331,38 +330,45 @@
     numwinds:
       address: 0x08
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 1
+    out_sel:
+      address: 0x0B
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
     pclk:
       address: 0x04
-      bitposition: 2
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     pclkwidth:
       address: 0x07
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    ramplen:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 12
+    rden:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 2000
+      value: false
     regclr:
       address: 0x04
-      bitposition: 1
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     runevs:
       address: 0x05
       bitposition: 0
@@ -452,78 +458,71 @@
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     selany:
       address: 0x04
-      bitposition: 3
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    slow_sysclk:
-      address: 0x19
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
     stopacq:
       address: 0x04
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    switch_nen:
+      address: 0x0B
+      bitposition: 13
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
     syncloc:
-      address: 0x09
+      address: 0x0E
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    sysclk:
-      address: 0x04
-      bitposition: 8
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
     sysrst:
       address: 0x04
-      bitposition: 9
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    tx_en:
-      address: 0x19
-      bitposition: 11
+      value: false
+    trig_sel:
+      address: 0x0B
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    wrstrboff:
+    wren:
       address: 0x04
-      bitposition: 7
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
   i2c_registers:
     i2c_en:
-      address: 0x0F
+      address: 0x09
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
     i2c_send:
       address: 0x0F
@@ -571,34 +570,34 @@
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x48
+      address: 0x2C
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x49
+      address: 0x2D
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x4A
+      address: 0x2E
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x4B
+      address: 0x2F
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 model: aardvarcv3
 features:
   adc2mv: true
+  calibration_channel: true
   dac_sweep: true
   ext_dac: true
   pedestals: true
   threshold_scan: true
   tia_dac: false
   timing_calibration: true
   naludaq_rs: true
@@ -22,15 +23,15 @@
     - d2xx
     - udp
   si5341_address: 0xE8
   default_baud:
     2_000_000: 50
   default_baudrate: 2_000_000
   default_clock: 100000000.0
-  default_divider: 53
+  default_divider: 50
   default_trigger_value: 1500
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
@@ -44,15 +45,20 @@
     address_mapping:
       0..3: 0x4E
     channel_mapping:
       0: 2
       1: 6
       2: 3
       3: 7
+    cal:
+      channel: 1
+      address: 0x4E
+      value: 2048
   headers: 3
+  minimum_firmware_version: 96
   new_firmware: True
   numregs: 64
   pedestals_blocks: 16
   peripherals:
     current_1v2:
       chan: 0
       addr: 0xD0
@@ -72,15 +78,18 @@
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
   possible_bauds:
+    115_200: 868
+    1_000_000: 100
     2_000_000: 50
+    3_000_000: 33
   resolution: 12
   samples: 64
   samplingrate: 10.0
   stop_word: !!binary |
     +s4=
   strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
   strobe_correction_keys:
@@ -568,14 +577,21 @@
     tx_en:
       address: 0x19
       bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
+    version:
+      address: 0x01
+      bitposition: 0
+      bitwidth: 16
+      description: 'Current firmware version'
+      readwrite: r
+      value: 0
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     0..1:
       !include_chip
       from: aodsv2::params
   # clock_file: '' # AODSoC boards have fixed clocks
   connections:
     - serial
     - d2xx
+    - udp
   si5341_address: 0xEE
   timing_hack: false
   default_baud:
     115200: 868
   default_baudrate: 115200
   default_clock: 100000000.0
   default_divider: 868
@@ -48,14 +49,15 @@
       1: 5
       2: 3
       3: 1
       4: 0
       5: 2
       6: 4
       7: 6
+  ext_trig_cycles: 10
   headers: 3
   numregs: 64
   pedestals_blocks: 16
   peripherals:
     vadjn_0:
       chan: 3
       addr: 0x4C
@@ -604,14 +606,91 @@
     testmode:
       address: 0x20
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
+    eth_addr_sel:
+      address: 0x28
+      bitposition: 0
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
+      readwrite: rw
+      value: 0
+    eth_port_sel:
+      address: 0x28
+      bitposition: 2
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
+      readwrite: rw
+      value: 0
+    tx_mode:
+      address: 0x28
+      bitposition: 4
+      bitwidth: 1
+      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
+      readwrite: rw
+      value: 0
+    eth_ar_en:
+      address: 0x28
+      bitposition: 5
+      bitwidth: 1
+      description: 'enables auto-response destination IP address; currently unused'
+      readwrite: rw
+      value: 0
+    eth_dhcp_en:
+      address: 0x28
+      bitposition: 6
+      bitwidth: 1
+      description: 'enables DHCP resolution of source IP address; currently unused'
+      readwrite: rw
+      value: 0
+    eth_dest_addr15_0:
+      address: 0x29
+      bitposition: 0
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet destination IP address'
+      readwrite: rw
+      value: 0
+    eth_dest_addr31_16:
+      address: 0x2A
+      bitposition: 0
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet destination IP address'
+      readwrite: rw
+      value: 0
+    eth_src_addr15_0:
+      address: 0x2B
+      bitposition: 0
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet source IP address'
+      readwrite: rw
+      value: 0
+    eth_src_addr31_16:
+      address: 0x2C
+      bitposition: 0
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet source IP address'
+      readwrite: rw
+      value: 0
+    eth_dest_port:
+      address: 0x2D
+      bitposition: 0
+      bitwidth: 16
+      description: 'UDP destination port'
+      readwrite: rw
+      value: 0
+    eth_src_port:
+      address: 0x2E
+      bitposition: 0
+      bitwidth: 16
+      description: 'UDP source port'
+      readwrite: rw
+      value: 0
   i2c_registers:
     i2c_en:
       address: 0x0F
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/asocv3.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,331 +1,387 @@
-model: aodsoc_asoc
+model: asocv3
 features:
-  adc2mv: false
-  dac_sweep: false
+  adc2mv: true
+  dac_sweep: true
   ext_dac: true
   pedestals: true
   threshold_scan: true
   tia_dac: false
-  timing_calibration: false
+  timing_calibration: true
   naludaq_rs: true
 params:
-  chanmask: 0x300
-  channels: 8
-  chanshift: 8
+  chanmask: 1536
+  channels: 4
+  chanshift: 9
   chips:
-    0..1:
+    0:
       !include_chip
       from: asocv3::params
-  # clock_file: '' # AODSoC boards have fixed clocks
+  clock_file: Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
   connections:
     - serial
     - d2xx
-  si5341_address: 0xEE
-  timing_hack: true
+    - udp
+  si5341_address: 0xE8
   default_baud:
     115200: 868
   default_baudrate: 115200
-  default_clock: 100000000.0
+  default_clock: 96000000.0
   default_divider: 868
-  default_trigger_value: 1500
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
   ext_dac:
-    chip: dac7578
+    chip: ad5671
     max_mv: 2500
     max_counts: 4095
     channels:
-      0..7: 2048
+      0..3: 2048
     address_mapping:
-      0..7: 0x48
+      0..3: 0xC
     channel_mapping:
-      0: 7
-      1: 5
-      2: 3
-      3: 1
-      4: 0
-      5: 2
-      6: 4
-      7: 6
+      0: 1
+      1: 0
+      2: 5
+      3: 4
   headers: 3
   numregs: 64
-  pedestals_blocks: 16
+  pedestals_blocks: 32
   peripherals:
-    vadjn_0:
-      chan: 3
-      addr: 0x4C
-    vadjn_1:
-      chan: 2
-      addr: 0x4C
-    ldo_voltage:
+    current:
+      chan: 0
+      addr: 0xD0
+      bits: 16
+      gain: 8
+    vadjn:
+      chan: 0
+      addr: 0xD8
+      bits: 16
+      gain: 1
+    vadjp:
       chan: 1
-      addr: 0x4C
-    chip_voltage:
-      chan: 2
-      addr: 0x4C
-    current_resistor: 0.010
+      addr: 0xD8
+      bits: 16
+      gain: 1
+    eeprom:
+      addr: 0x50 # 7-bit
+      capacity: 0x20000 # bytes
+      page_size: 256 # bytes
+      segments:
+        analog_registers:
+          begin: 0
+          length: 300
+        digital_registers:
+          begin: 300
+          length: 330
+        control_registers:
+          begin: 630
+          length: 70
   possible_bauds:
     115200: 868
-    1000000: 100
     2000000: 50
-    3000000: 33
+  roi_enabled: true
   resolution: 12
   samples: 64
   samplingrate: 3.2
-  stop_word: "cafe"
+  stop_word: !!binary |
+    +s4=
   wait: AE000001
   wbias: 848
-  windmask: 0x0FF
+  windmask: 510
   windows: 254
+  yaml_version: 35.0
 registers:
   analog_registers:
     !include_registers
       from: asocv3::registers::analog_registers
-      value_count: 2
-      override:
-        isel:
-          value: [2610, 2627]
   digital_registers:
     !include_registers
       from: asocv3::registers::digital_registers
-      value_count: 2
   control_registers:
-    1v2_en:
-      address: 0x17
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
     2v5_en:
-      address: 0x17
+      address: 0x16
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    3v3_i2c_en:
-      address: 0x17
-      bitposition: 2
+    2v5_pll_en:
+      address: 0x16
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    8b10b_en:
-      address: 0x19
-      bitposition: 12
-      bitwidth: 1
+      value: false
+    addr:
+      address: 0x15
+      bitposition: 0
+      bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
-    amp_pwrdn_out:
-      address: 0x1A
+    addr_user:
+      address: 0x15
+      bitposition: 15
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    brightness_blue:
+      address: 0x0A
       bitposition: 0
       bitwidth: 8
-      description: 'Onboard amplifiers active high means amp off'
+      description: ''
       readwrite: rw
       value: 0
-    addr:
-      address: 0x16
+    brightness_red:
+      address: 0x0B
       bitposition: 0
-      bitwidth: 9
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    addr_user:
-      address: 0x16
-      bitposition: 15
-      bitwidth: 1
+    brightness_white:
+      address: 0x0A
+      bitposition: 8
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: false
+      value: 0
     chansel:
       address: 0x06
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    clk1v8_en:
-      address: 0x17
-      bitposition: 4
+    clk_1v8_nshutdown:
+      address: 0x16
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
+    clk_2v5_en:
+      address: 0x16
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_fdec:
-      address: 0x17
-      bitposition: 9
+    clk_i2c_sel:
+      address: 0x16
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    clk_finc:
-      address: 0x17
-      bitposition: 8
+      value: true
+    clk_noe:
+      address: 0x16
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_i2c_sel:
-      address: 0x17
-      bitposition: 5
+    clk_nrst:
+      address: 0x16
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    clk_reset:
-      address: 0x17
+    clk_nsync:
+      address: 0x16
       bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    clk_sync:
-      address: 0x17
+    dac_nrst:
+      address: 0x16
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
+      value: 1
     data:
       address: 0x14
       bitposition: 0
       bitwidth: 12
       description: ''
       readwrite: rw
       value: 0
     data_user:
       address: 0x14
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    debug_data:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
+    digrst:
+      address: 0x16
+      bitposition: 9
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    debug_data_user:
-      address: 0x15
-      bitposition: 15
+    digser_8b10b_en:
+      address: 0x1D
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    digrst:
-      address: 0x16
-      bitposition: 9
-      bitwidth: 1
+    digser_numwords:
+      address: 0x1D
+      bitposition: 2
+      bitwidth: 6
       description: ''
       readwrite: rw
       value: 0
-    digser_rst:
-      address: 0x19
+    digser_oneshot:
+      address: 0x1D
+      bitposition: 1
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    digser_reset:
+      address: 0x1D
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    exttrig:
-      address: 0x04
+      value: false
+    digser_rx_en:
+      address: 0x1D
+      bitposition: 0
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    digser_slow_sysclk:
+      address: 0x1D
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
+      value: 0
+    digser_speed:
+      address: 0x1D
+      bitposition: 8
+      bitwidth: 2
+      description: ''
+      readwrite: rw
+      value: 0
+    digser_tx_en:
+      address: 0x1D
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
       value: false
-    gccclr:
+    ext_en:
+      address: 0x0B
+      bitposition: 9
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    exttrig:
       address: 0x04
-      bitposition: 4
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    idac_ldac:
-      address: 0x1B
+    fake:
+      address: 0x06
       bitposition: 0
       bitwidth: 1
-      description: 'pin on AD7578'
+      description: ''
       readwrite: rw
       value: 0
-    idac_nclr:
-      address: 0x1B
-      bitposition: 1
+    gccclr:
+      address: 0x04
+      bitposition: 3
       bitwidth: 1
-      description: 'pin on AD7578'
+      description: ''
       readwrite: rw
-      value: 1
-    fifo_unload_or_event_en:
-      address: 0x1F
-      bitposition: 0
+      value: false
+    i2c_sel:
+      address: 0x16
+      bitposition: 11
       bitwidth: 1
-      description: 'Once data is loaded into the FIFO it will not be sent out to the UART until the end of the current event. Use this mode for capturing sampled data events. '
+      description: ''
+      readwrite: rw
+      value: true
+    i2c_switch:
+      address: 0x16
+      bitposition: 8
+      bitwidth: 1
+      description: ''
       readwrite: rw
       value: 0
     identifier:
       address: 0x00
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 309
-    iomode0:
-      address: 0x04
+      value: 42435
+    version:
+      address: 0x01
       bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    in_sel:
+      address: 0x0B
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    iomode1:
+    iomode0:
       address: 0x04
-      bitposition: 6
+      bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    leds:
-      address: 0x18
-      bitposition: 0
-      bitwidth: 16
+      value: 1
+    iomode1:
+      address: 0x04
+      bitposition: 8
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
     loadwait:
       address: 0x07
       bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
+    nasa_trig_sel_ext:
+      address: 0x1D
+      bitposition: 15
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
     nramp:
       address: 0x04
-      bitposition: 5
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     nrw:
       address: 0x04
       bitposition: 11
@@ -336,49 +392,98 @@
     numwinds:
       address: 0x08
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 1
+    out_sel:
+      address: 0x0B
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
     pclk:
       address: 0x04
-      bitposition: 2
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     pclkwidth:
       address: 0x07
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    ramplen:
-      address: 0x06
-      bitposition: 0
-      bitwidth: 12
+    rden:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
       description: ''
       readwrite: rw
-      value: 2000
+      value: false
     regclr:
       address: 0x04
-      bitposition: 1
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     runevs:
       address: 0x05
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
+    rx_data0:
+      address: 0x1A
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data1:
+      address: 0x1B
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data2:
+      address: 0x1C
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data4:
+      address: 0x1E
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data5:
+      address: 0x1F
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    rx_data6:
+      address: 0x20
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
     rx_en:
       address: 0x19
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
@@ -408,230 +513,174 @@
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
     selany:
       address: 0x04
-      bitposition: 3
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    slow_sysclk:
-      address: 0x19
-      bitposition: 10
+    sst_speed:
+      address: 0x1D
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: false
     stopacq:
       address: 0x04
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
+    switch_nen:
+      address: 0x0B
+      bitposition: 13
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
     syncloc:
-      address: 0x09
+      address: 0x0E
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    sysclk:
+    sysrst:
       address: 0x04
-      bitposition: 8
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    sysrst:
-      address: 0x04
-      bitposition: 9
+    trig_sel:
+      address: 0x0B
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    tx_en:
-      address: 0x19
-      bitposition: 11
-      bitwidth: 1
-      description: ''
+      value: false
+    trigger_mux:
+      address: 0x22
+      bitposition: 5
+      bitwidth: 4
+      description: 'Change which trigger type is used to trigger the chip, there are 9 different modes.'
       readwrite: rw
-      value: 0
+      value: 8
     windsel:
       address: 0x07
       bitposition: 0
       bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    wrstrboff:
+    wren:
       address: 0x04
-      bitposition: 7
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
-    rxout_pol:
-      address: 0x22
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 6400
-    txin_pol:
-      address: 0x23
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 4412
-    ard_header:
-      address: 0x21
-      bitposition: 0
-      bitwidth: 1
-      description: 'Enable AARDVARC debug header.'
-      readwrite: rw
-      value: 1
-    ard_rx_en:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 16
-      description: 'TR-BHM ASIC Rx Enable register 29dec. Bit 0 and 1 enable transmitting data to ASICs. Need to set these bits to send data to the ASICs'
-      readwrite: rw
-      value: 3
-    ard_tx_en:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 16
-      description: 'TR-BHM ASIC Tx Enable register 30dec. Bit 0 and 1 enable receiving data from ASICs. Need to set these bits to get data back from the ASICs'
-      readwrite: rw
-      value: 3
-    ard0_clk_sel:
-      address: 0x24
+    eth_addr_sel:
+      address: 0x28
       bitposition: 0
       bitwidth: 2
-      description: ''
+      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
       readwrite: rw
       value: 0
-    ard1_clk_sel:
-      address: 0x25
-      bitposition: 0
+    eth_port_sel:
+      address: 0x28
+      bitposition: 2
       bitwidth: 2
-      description: ''
-      readwrite: rw
-      value: 1
-    motor_trig_en:
-      address: 0x27
-      bitposition: 0
-      bitwidth: 1
-      description: ''
+      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
       readwrite: rw
       value: 0
-    motor_trig_evts:
-      address: 0x26
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 1
-    oleas_en_trig:
-      address: 0x0A
-      bitposition: 10
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    oleas_pol_a:
-      address: 0x0A
-      bitposition: 11
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: 0
-    oleas_pol_b:
-      address: 0x0A
-      bitposition: 12
+    tx_mode:
+      address: 0x28
+      bitposition: 4
       bitwidth: 1
-      description: ''
+      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
       readwrite: rw
       value: 0
-    oleas_en_a:
-      address: 0x0A
-      bitposition: 13
+    eth_ar_en:
+      address: 0x28
+      bitposition: 5
       bitwidth: 1
-      description: ''
+      description: 'enables auto-response destination IP address; currently unused'
       readwrite: rw
       value: 0
-    oleas_en_b:
-      address: 0x0A
-      bitposition: 14
+    eth_dhcp_en:
+      address: 0x28
+      bitposition: 6
       bitwidth: 1
-      description: ''
+      description: 'enables DHCP resolution of source IP address; currently unused'
       readwrite: rw
       value: 0
-    oleas_loop:
-      address: 0x0A
+    eth_dest_addr15_0:
+      address: 0x29
       bitposition: 0
-      bitwidth: 5
-      description: ''
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet destination IP address'
       readwrite: rw
-      value: 15
-    oleas_length_a:
-      address: 0x0B
+      value: 0
+    eth_dest_addr31_16:
+      address: 0x2A
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'upper 16 bits of ethernet destination IP address'
       readwrite: rw
       value: 0
-    oleas_length_b:
-      address: 0x0D
+    eth_src_addr15_0:
+      address: 0x2B
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'lower 16 bits of ethernet source IP address'
       readwrite: rw
       value: 0
-    oleas_delay_a:
-      address: 0x0C
+    eth_src_addr31_16:
+      address: 0x2C
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'upper 16 bits of ethernet source IP address'
       readwrite: rw
       value: 0
-    oleas_delay_b:
-      address: 0x0E
+    eth_dest_port:
+      address: 0x2D
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'UDP destination port'
       readwrite: rw
       value: 0
-    testmode:
-      address: 0x20
+    eth_src_port:
+      address: 0x2E
       bitposition: 0
-      bitwidth: 1
-      description: ''
+      bitwidth: 16
+      description: 'UDP source port'
       readwrite: rw
       value: 0
   i2c_registers:
     i2c_en:
-      address: 0x0F
+      address: 0x09
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: true
-    # i2c_send:
-    #   address: 0x0F
-    #   bitposition: 15
-    #   bitwidth: 1
-    #   description: ''
-    #   readwrite: rw
-    #   value: 0
+    i2c_send:
+      address: 0x0F
+      bitposition: 15
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
     i2c_words:
       address: 0x0F
       bitposition: 8
       bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-model: aodsv1
+model: aodsv2_eval
 features:
+  threshold_scan: true
+  timing_calibration: false
   adc2mv: false
-  dac_sweep: true
-  ext_dac: true
+  dac_sweep: false
   pedestals: true
-  threshold_scan: true
   tia_dac: false
-  timing_calibration: false
+  ext_dac: true
   naludaq_rs: true
 params:
   chanmask: 1536
   channels: 4
   chanshift: 9
   chips:
     0:
       !include_chip
-      from: aodsv1::params
+      from: aodsv2::params
   clock_file: AODS_300GCC.txt  #  AODS_debugpulse_240MGCC_10Mref.txt
   connections:
     - serial
     - d2xx
+    - udp
   si5341_address: 0xE8
   default_baud:
-    111111: 53
-  default_baudrate: 111111
-  default_clock: 200000000.0
-  default_divider: 53
+    115200: 868
+  default_baudrate: 115200
+  default_clock: 96000000.0
+  default_divider: 868
   default_trigger_value: 2000
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
   ext_dac:
     chip: ad5671
     max_mv: 2500
-    max_counts: 4095
+    max_counts: 4096
     channels:
       0: 2048
       1: 2175
       2: 1968
       3: 2048
     address_mapping:
       0..3: 0xC
     channel_mapping:
       0: 1
       1: 0
       2: 5
       3: 4
   headers: 3
-  numregs: 36
+  numregs: 64
   pedestals_blocks: 32
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
@@ -80,32 +81,32 @@
         digital_registers:
           begin: 300
           length: 330
         control_registers:
           begin: 630
           length: 70
   possible_bauds:
-    111111: 53
-    1500000: 3
+    115200: 868
+    2000000: 50
   resolution: 12
   samples: 64
   samplingrate: 1.0
   stop_word: !!binary |
     +s4=
   wait: AE000001
   wbias: 848
   windmask: 510
   windows: 254
 registers:
   analog_registers:
     !include_registers
-      from: aodsv1::registers::analog_registers
+    from: aodsv2::registers::analog_registers
   digital_registers:
     !include_registers
-      from: aodsv1::registers::digital_registers
+    from: aodsv2::registers::digital_registers
   control_registers:
     trig_mux:
       address: 0x22
       bitposition: 5
       bitwidth: 4
       description: 'evttrig driver'
       readwrite: rw
@@ -245,15 +246,15 @@
       value: 0
     ext_en:
       address: 0x0B
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: false
     exttrig:
       address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: false
@@ -570,34 +571,34 @@
       address: 0x13
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x2C
+      address: 0x48
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x2D
+      address: 0x49
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x2E
+      address: 0x4A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x2F
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/udc16.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,604 +1,549 @@
-model: aodsv2_eval
+model: udc16
 features:
-  threshold_scan: true
-  timing_calibration: false
   adc2mv: false
-  dac_sweep: false
+  dac_sweep: true
+  ext_dac: true
   pedestals: true
+  threshold_scan: false
   tia_dac: false
-  ext_dac: true
+  timing_calibration: false
   naludaq_rs: true
 params:
-  chanmask: 1536
-  channels: 4
-  chanshift: 9
+  chanmask: 0xFF00
+  channels: 16
+  chanshift: 8
   chips:
     0:
       !include_chip
-      from: aodsv2::params
-  clock_file: AODS_300GCC.txt  #  AODS_debugpulse_240MGCC_10Mref.txt
+      from: udc16::params
+  clock_file: Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
   connections:
     - serial
     - d2xx
     - udp
-  si5341_address: 0xE8
+  si5341_address: 0xEE
   default_baud:
-    115200: 868
-  default_baudrate: 115200
-  default_clock: 96000000.0
-  default_divider: 868
-  default_trigger_value: 2000
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
+    2000000: 50
+  default_baudrate: 2000000
+  default_clock: 200000000.0
+  default_divider: 50
+  default_trigger_value: 0
+  intamp_bias_mode_chan0_7: 'c'
+  intamp_bias_mode_chan8_15: 'c'
   ext_dac:
-    chip: ad5671
-    max_mv: 2500
-    max_counts: 4096
+    chip: dac7578
+    max_mv: 1250
+    max_counts: 3930
+    min_counts: 0
     channels:
-      0: 2048
-      1: 2175
-      2: 1968
-      3: 2048
+      0..15: 2000
     address_mapping:
-      0..3: 0xC
+      0..7: 0x4B
+      8..15: 0x48
     channel_mapping:
-      0: 1
-      1: 0
-      2: 5
-      3: 4
-  headers: 3
-  numregs: 64
-  pedestals_blocks: 32
+      0, 08: 0
+      1, 09: 1
+      2, 10: 2
+      3, 11: 3
+      4, 12: 4
+      5, 13: 5
+      6, 14: 6
+      7, 15: 7
+  trigger:
+    max_val: 2047
+    min_val: 0
+    default: false
+  num_trigger_channels: 8
+  headers: 0
+  last_window_fix_amount: 47
+  lastbits: 0
+  numregs: 32
+  pedestals_blocks: 8
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
-      chan: 0
+      chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
     vadjp:
-      chan: 1
+      chan: 0
       addr: 0xD8
       bits: 16
       gain: 1
-    eeprom:
-      addr: 0x50 # 7-bit
-      capacity: 0x20000 # bytes
-      page_size: 256 # bytes
-      segments:
-        analog_registers:
-          begin: 0
-          length: 300
-        digital_registers:
-          begin: 300
-          length: 330
-        control_registers:
-          begin: 630
-          length: 70
   possible_bauds:
-    115200: 868
     2000000: 50
-  resolution: 12
+  resolution: 10
   samples: 64
-  samplingrate: 1.0
-  stop_word: !!binary |
-    +s4=
+  samplingrate: 9.2
+  stop_word: CAFE
+  strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
+  strobe_correction_keys:
+    - digsync_le
+    - digsync_te
+    - wrstrb1_le
+    - wrstrb1_te
+    - wrstrb2_le
+    - wrstrb2_te
+    - wrsync1_le
+    - wrsync1_te
+    - wrsync2_le
+    - wrsync2_te
   wait: AE000001
-  wbias: 848
-  windmask: 510
-  windows: 254
+  wbias: 750
+  windmask: 0x00FF
+  windows: 64
 registers:
   analog_registers:
     !include_registers
-    from: aodsv2::registers::analog_registers
+      from: udc16::registers::analog_registers
   digital_registers:
     !include_registers
-    from: aodsv2::registers::digital_registers
+      from: udc16::registers::digital_registers
   control_registers:
-    trig_mux:
-      address: 0x22
-      bitposition: 5
-      bitwidth: 4
-      description: 'evttrig driver'
-      readwrite: rw
-      value: 3
-    fpga_misc_t:
-      address: 0x22
-      bitposition: 0
-      bitwidth: 4
-      description: 'fpga misc output disable'
-      readwrite: rw
-      value: 15
-    2v5_en:
-      address: 0x16
+    identifier:
+      address: 0x00
       bitposition: 0
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    2v5_pll_en:
-      address: 0x16
-      bitposition: 1
-      bitwidth: 1
-      description: ''
+      bitwidth: 16
+      description: 'Unique board identifier'
       readwrite: rw
-      value: false
-    addr:
-      address: 0x15
+      value: 0x4D5C
+    version:
+      address: 0x01
       bitposition: 0
-      bitwidth: 9
-      description: ''
+      bitwidth: 16
+      description: 'Current firmware version'
       readwrite: rw
       value: 0
-    addr_user:
-      address: 0x15
+    data_iot:
+      address: 0x04
       bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    brightness_blue:
-      address: 0x0A
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
       value: 0
-    brightness_red:
-      address: 0x0B
-      bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
-      value: 0
-    brightness_white:
-      address: 0x0A
-      bitposition: 8
-      bitwidth: 8
+    stopacq:
+      address: 0x04
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    chansel:
-      address: 0x06
+    sel:
+      address: 0x04
       bitposition: 12
-      bitwidth: 4
-      description: ''
-      readwrite: rw
-      value: 15
-    clk_1v8_nshutdown:
-      address: 0x16
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_2v5_en:
-      address: 0x16
-      bitposition: 6
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_i2c_sel:
-      address: 0x16
-      bitposition: 5
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_noe:
-      address: 0x16
-      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    clk_nrst:
-      address: 0x16
-      bitposition: 3
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    clk_nsync:
-      address: 0x16
-      bitposition: 7
+      value: 0
+    nrw:
+      address: 0x04
+      bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    dac_nrst:
-      address: 0x16
+      value: 0
+    exttrig:
+      address: 0x04
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    data:
-      address: 0x14
-      bitposition: 0
-      bitwidth: 12
-      description: ''
-      readwrite: rw
       value: 0
-    data_user:
-      address: 0x14
-      bitposition: 15
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    digrst:
-      address: 0x16
+    sysrst:
+      address: 0x04
       bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    ext_en:
-      address: 0x0B
-      bitposition: 9
+    iomode1:
+      address: 0x04
+      bitposition: 6
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    exttrig:
+      value: 1
+    nramp:
       address: 0x04
-      bitposition: 10
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    fake:
-      address: 0x06
-      bitposition: 0
+      value: 0
+    gccclr:
+      address: 0x04
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    gccclr:
+    selany:
       address: 0x04
       bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    i2c_switch:
-      address: 0x16
-      bitposition: 8
+      value: 0
+    pclk:
+      address: 0x04
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    identifier:
-      address: 0x00
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: r
-      value: 41173
-    in_sel:
-      address: 0x0B
-      bitposition: 12
+    regclr:
+      address: 0x04
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: 0
     iomode0:
       address: 0x04
-      bitposition: 7
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    iomode1:
-      address: 0x04
+      value: 0
+    pclkwidth:
+      address: 0x07
       bitposition: 8
-      bitwidth: 1
+      bitwidth: 4
       description: ''
       readwrite: rw
-      value: 0
+      value: 15
     loadwait:
       address: 0x07
-      bitposition: 8
+      bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    nramp:
-      address: 0x04
-      bitposition: 4
+    udc_arm:
+      address: 0x09
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    nrw:
-      address: 0x04
-      bitposition: 11
+      value: 0
+    reread_data:
+      address: 0x0C
+      bitposition: 0
       bitwidth: 1
-      description: ''
+      description: 'Ask the FPGA to send whatever event is in the output buffer'
       readwrite: rw
-      value: false
-    numwinds:
-      address: 0x08
+      value: 0
+    debug_data_to_write:
+      address: 0x14
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 12
       description: ''
       readwrite: rw
-      value: 1
-    out_sel:
-      address: 0x0B
-      bitposition: 11
-      bitwidth: 1
+      value: 0
+    debug_addr:
+      address: 0x15
+      bitposition: 0
+      bitwidth: 12
       description: ''
       readwrite: rw
-      value: false
-    pclk:
-      address: 0x04
-      bitposition: 1
+      value: 0
+    wave_fifo_reset:
+      address: 0x16
+      bitposition: 10
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    pclkwidth:
-      address: 0x07
-      bitposition: 12
-      bitwidth: 4
-      description: ''
+      description: 'Reset the waveform FIFO, effectively flushing any data in the output FIFO'
       readwrite: rw
-      value: 15
-    rden:
-      address: 0x04
-      bitposition: 6
+      value: 0
+    digrst:
+      address: 0x16
+      bitposition: 9
       bitwidth: 1
-      description: ''
+      description: 'Toggle the digital reset pin, resets the ASIC.'
       readwrite: rw
-      value: false
-    regclr:
-      address: 0x04
+      value: 0
+    2v5_en:
+      address: 0x17
       bitposition: 0
       bitwidth: 1
-      description: ''
+      description: 'Enable the 2.5V rail'
       readwrite: rw
-      value: false
-    runevs:
-      address: 0x05
-      bitposition: 0
-      bitwidth: 16
-      description: ''
-      readwrite: rw
-      value: 1
-    rx_data0:
-      address: 0x1A
-      bitposition: 0
-      bitwidth: 16
-      description: ''
+      value: 0
+    1v2_en:
+      address: 0x17
+      bitposition: 1
+      bitwidth: 1
+      description: 'Enable the 1.2V rail'
       readwrite: rw
       value: 0
-    rx_data1:
-      address: 0x1B
-      bitposition: 0
-      bitwidth: 16
-      description: ''
+    clk2v5_en:
+      address: 0x17
+      bitposition: 3
+      bitwidth: 1
+      description: 'Enable the clock specific 2.5V rail.'
       readwrite: rw
       value: 0
-    rx_data2:
-      address: 0x1C
-      bitposition: 0
-      bitwidth: 16
-      description: ''
+    clk1v8_en:
+      address: 0x17
+      bitposition: 4
+      bitwidth: 1
+      description: 'Enable the clock specific 1.8V rail.'
       readwrite: rw
       value: 0
-    rx_data3:
-      address: 0x1D
-      bitposition: 0
-      bitwidth: 16
+    clk_oeb:
+      address: 0x17
+      bitposition: 6
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_data4:
-      address: 0x1E
-      bitposition: 0
-      bitwidth: 16
+    clk_reset:
+      address: 0x17
+      bitposition: 7
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_data5:
-      address: 0x1F
-      bitposition: 0
-      bitwidth: 16
+    clk_sync:
+      address: 0x17
+      bitposition: 10
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_data6:
-      address: 0x20
+    tx_packet_marker:
+      address: 0x18
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 6
       description: ''
       readwrite: rw
       value: 0
-    rx_en:
+    rx_enable:
       address: 0x19
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_num_words:
-      address: 0x19
-      bitposition: 2
-      bitwidth: 6
-      description: ''
-      readwrite: rw
-      value: 0
-    rx_oneshot:
+    rx_reg_polarity:
       address: 0x19
       bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_speed:
+    rx_divider:
       address: 0x19
-      bitposition: 8
-      bitwidth: 2
+      bitposition: 4
+      bitwidth: 4
       description: ''
       readwrite: rw
       value: 0
-    sel:
-      address: 0x04
+    tx_enable:
+      address: 0x19
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    selany:
-      address: 0x04
-      bitposition: 2
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    stopacq:
-      address: 0x04
+      value: 0
+    tx_reg_polarity:
+      address: 0x19
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    switch_nen:
-      address: 0x0B
-      bitposition: 13
+      value: 0
+    tx_10_bit_data:
+      address: 0x19
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    syncloc:
-      address: 0x0E
+      value: 0
+    analog_debug_en:
+      address: 0x1F
       bitposition: 0
-      bitwidth: 8
-      description: ''
+      bitwidth: 1
+      description: 'Enable analog debug mode, bypassing the digital side of the chip. Allows the user to communicate directly with the analog side.'
       readwrite: rw
       value: 0
-    sysrst:
-      address: 0x04
-      bitposition: 14
+    v1v2_power_good:
+      address: 0x46
+      bitposition: 0
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    trig_sel:
-      address: 0x0B
-      bitposition: 10
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    temperature_event:
+      address: 0x46
+      bitposition: 1
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    windsel:
-      address: 0x07
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    udc_mon_in:
+      address: 0x47
       bitposition: 0
-      bitwidth: 8
-      description: ''
-      readwrite: rw
+      bitwidth: 1
+      description: 'Read-Only status register'
+      readwrite: r
       value: 0
-    wren:
-      address: 0x04
-      bitposition: 5
+    i2c_dataout_genwr_3:
+      address: 0x48
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    i2c_dataout_genwr_2:
+      address: 0x49
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    i2c_dataout_genwr_1:
+      address: 0x4A
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    i2c_dataout_genwr_0:
+      address: 0x4B
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    udc_triggerout_in:
+      address: 0x4C
+      bitposition: 2
       bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    si5341a_intr_n_in:
+      address: 0x4C
+      bitposition: 1
+      bitwidth: 1
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    si5341a_lol_n_in:
+      address: 0x4C
+      bitposition: 0
+      bitwidth: 1
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    system_clock_locked:
+      address: 0x59
+      bitposition: 0
+      bitwidth: 1
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    sys_clock_locked:
+      address: 0x59
+      bitposition: 1
+      bitwidth: 1
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    idigser_tx_idle_locked:
+      address: 0x59
+      bitposition: 2
+      bitwidth: 1
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
+    udc_busy_locked_in:
+      address: 0x59
+      bitposition: 3
+      bitwidth: 1
+      description: 'Read-Only status register'
+      readwrite: r
+      value: 0
   i2c_registers:
     i2c_en:
-      address: 0x09
-      bitposition: 14
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: true
-    i2c_send:
       address: 0x0F
-      bitposition: 15
+      bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
+      value: 1
     i2c_words:
       address: 0x0F
       bitposition: 8
-      bitwidth: 3
-      description: ''
+      bitwidth: 4
+      description: 'number of words to send in the i2c command.'
       readwrite: rw
       value: 0
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
-      description: ''
+      description: 'i2c address for the commands in the string builder'
       readwrite: rw
       value: 0
     i2c_data0:
       address: 0x10
       bitposition: 0
-      bitwidth: 16
-      description: ''
+      bitwidth: 8
+      description: 'Data storage used by the i2c string builder, for both rx and tx data'
       readwrite: rw
       value: 0
     i2c_data1:
       address: 0x11
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'Data storage used by the i2c string builder, for both rx and tx data'
       readwrite: rw
       value: 0
     i2c_data2:
       address: 0x12
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'Data storage used by the i2c string builder, for both rx and tx data'
       readwrite: rw
       value: 0
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
-      description: ''
+      description: 'Data storage used by the i2c string builder, for both rx and tx data'
       readwrite: rw
       value: 0
     response0:
-      address: 0x48
+      address: 0x28
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x49
+      address: 0x29
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x4A
+      address: 0x2A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x4B
+      address: 0x2B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/upaci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,40 @@
-model: asocv3
-features:
-  adc2mv: true
-  dac_sweep: true
-  ext_dac: true
-  pedestals: true
-  threshold_scan: true
-  tia_dac: false
-  timing_calibration: true
-  naludaq_rs: true
+model: upaci
 params:
-  chanmask: 1536
-  channels: 4
-  chanshift: 9
-  chips:
-    0:
-      !include_chip
-      from: asocv3::params
-  clock_file: Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+  chanmask: 511
+  channels: 32
+  chanshift: 3
   connections:
     - serial
     - d2xx
-    - udp
-  si5341_address: 0xE8
   default_baud:
-    115200: 868
+    115200: 434
   default_baudrate: 115200
-  default_clock: 96000000.0
-  default_divider: 868
-  threshold_scan:
-    min_vref: 0
-    max_vref: 2500
-    start: 500
-    stop: 3500
-    stepsize: 5
-    units: counts
+  default_clock: 200000000.0
+  default_divider: 434
+  default_trigger_value: 0
   ext_dac:
-    chip: ad5671
-    max_mv: 2500
-    max_counts: 4095
+    max_mv: 1200
+    max_counts: 65535
     channels:
-      0..3: 2048
-    address_mapping:
-      0..3: 0xC
-    channel_mapping:
-      0: 1
-      1: 0
-      2: 5
-      3: 4
-  headers: 3
-  numregs: 64
-  pedestals_blocks: 32
+      0: 30000
+      8: 30000
+      16: 30000
+      24: 30000
+  trigger:
+    triggers_available: 8
+    max_val: 2047
+    min_val: 0
+    default: false
+  num_trigger_channels: 8
+  headers: 0
+  last_window_fix_amount: 47
+  lastbits: 0
+  numregs: 32
+  pedestals_blocks: 8
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
@@ -62,688 +43,747 @@
       bits: 16
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
-    eeprom:
-      addr: 0x50 # 7-bit
-      capacity: 0x20000 # bytes
-      page_size: 256 # bytes
-      segments:
-        analog_registers:
-          begin: 0
-          length: 300
-        digital_registers:
-          begin: 300
-          length: 330
-        control_registers:
-          begin: 630
-          length: 70
   possible_bauds:
-    115200: 868
-    2000000: 50
-  roi_enabled: true
-  resolution: 12
-  samples: 64
-  samplingrate: 3.2
+    115200: 434
+    2000000: 25
+  resolution: 11
+  samples: 132
+  samplingrate: 9.2
   stop_word: !!binary |
     +s4=
   wait: AE000001
-  wbias: 848
-  windmask: 510
-  windows: 254
-  yaml_version: 35.0
+  wbias: 750
+  windmask: 7
+  windows: 8
 registers:
-  analog_registers:
-    !include_registers
-      from: asocv3::registers::analog_registers
-  digital_registers:
-    !include_registers
-      from: asocv3::registers::digital_registers
   control_registers:
-    2v5_en:
-      address: 0x16
+    avdd_en:
+      address: 0x28
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    2v5_pll_en:
-      address: 0x16
-      bitposition: 1
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    addr:
-      address: 0x15
+      value: 0
+    baud_rate_divisor:
+      address: 0x03
       bitposition: 0
-      bitwidth: 9
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    addr_user:
-      address: 0x15
+      value: 108
+    cdce62002_power_down_n:
+      address: 0x13
       bitposition: 15
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    brightness_blue:
-      address: 0x0A
+      value: 1
+    cdce62002_read_register_0_lsw:
+      address: 0x92
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    brightness_red:
-      address: 0x0B
+      value: 21976
+    cdce62002_read_register_0_msw:
+      address: 0x91
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    brightness_white:
-      address: 0x0A
-      bitposition: 8
-      bitwidth: 8
+      value: 1104
+    cdce62002_read_register_1_lsw:
+      address: 0x94
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    chansel:
-      address: 0x06
-      bitposition: 12
-      bitwidth: 4
+      value: 903
+    cdce62002_read_register_1_msw:
+      address: 0x93
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 15
-    clk_1v8_nshutdown:
-      address: 0x16
-      bitposition: 2
-      bitwidth: 1
+      value: 57376
+    cdce62002_read_register_2_lsw:
+      address: 0x96
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    clk_2v5_en:
-      address: 0x16
-      bitposition: 6
-      bitwidth: 1
+      value: 24832
+    cdce62002_read_register_2_msw:
+      address: 0x95
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    clk_i2c_sel:
-      address: 0x16
-      bitposition: 5
-      bitwidth: 1
+      value: 14850
+    cdce62002_register_0_lsw_out:
+      address: 0x0C
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    clk_noe:
-      address: 0x16
-      bitposition: 4
-      bitwidth: 1
+      value: 1104  # same
+    cdce62002_register_0_msw_out:
+      address: 0x0D
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    clk_nrst:
-      address: 0x16
-      bitposition: 3
-      bitwidth: 1
+      value: 0x5550  # 21976
+    cdce62002_register_1_lsw_out:
+      address: 0x0E
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    clk_nsync:
-      address: 0x16
-      bitposition: 7
-      bitwidth: 1
+      value: 0xa091  # 57377
+    cdce62002_register_1_msw_out:
+      address: 0x0F
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    dac_nrst:
-      address: 0x16
-      bitposition: 10
+      value: 0x838d  # 33671
+    cdce62002_write_strobe:
+      address: 0x13
+      bitposition: 11
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    data:
+      value: 0
+    conversion_wait_count_value:
       address: 0x14
       bitposition: 0
-      bitwidth: 12
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    data_user:
-      address: 0x14
-      bitposition: 15
-      bitwidth: 1
+    dac_rovcp_1_out:
+      address: 0x08
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    digrst:
-      address: 0x16
-      bitposition: 9
-      bitwidth: 1
+      value: 256
+    dac_rovcp_2_out:
+      address: 0x09
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    digser_8b10b_en:
-      address: 0x1D
-      bitposition: 12
-      bitwidth: 1
+      value: 256
+    dac_vbias00_07_out:
+      address: 0x04
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    digser_numwords:
-      address: 0x1D
-      bitposition: 2
-      bitwidth: 6
+      value: 27306
+    dac_vbias08_15_out:
+      address: 0x05
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    digser_oneshot:
-      address: 0x1D
-      bitposition: 1
-      bitwidth: 1
+      value: 27306
+    dac_vbias16_23_out:
+      address: 0x0A
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    digser_reset:
-      address: 0x1D
-      bitposition: 13
-      bitwidth: 1
+      value: 27306
+    dac_vbias24_31_out:
+      address: 0x0B
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    digser_rx_en:
-      address: 0x1D
+      value: 27306
+    dac_vreset1_2_out:
+      address: 0x06
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    digser_slow_sysclk:
-      address: 0x1D
-      bitposition: 10
+      value: 11264
+    dac_vreset3_4_out:
+      address: 0x07
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 11264
+    dac_write_strobe:
+      address: 0x13
+      bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    digser_speed:
-      address: 0x1D
-      bitposition: 8
-      bitwidth: 2
+    diagnostic_read_data:
+      address: 0x10
+      bitposition: 4
+      bitwidth: 4
       description: ''
       readwrite: rw
       value: 0
-    digser_tx_en:
-      address: 0x1D
-      bitposition: 11
+    # dll_start:
+    #   address: 0x13
+    #   bitposition: 7
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    ftdi_cts:
+      address: 0x29
+      bitposition: 2
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    ext_en:
-      address: 0x0B
-      bitposition: 9
-      bitwidth: 1
+      value: 0
+    ftdi_rts_bit_0:
+      address: 0x88
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    exttrig:
-      address: 0x04
-      bitposition: 10
-      bitwidth: 1
+      value: 0
+    gpio_pd:
+      address: 0x28
+      bitposition: 2
+      bitwidth: 5
       description: ''
       readwrite: rw
-      value: false
-    fake:
-      address: 0x06
+      value: 0
+    gpio_input_header_5:
+      address: 0x85
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 8
       description: ''
       readwrite: rw
-      value: 0
-    gccclr:
-      address: 0x04
-      bitposition: 3
-      bitwidth: 1
+      value: 255
+    identifier:
+      address: 0x00
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    i2c_sel:
-      address: 0x16
-      bitposition: 11
+      value: 57005
+    # mclk_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 10
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    optical_trigger_en:
+      address: 0x29
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    i2c_switch:
-      address: 0x16
-      bitposition: 8
+      value: 0
+    optical_trigger_input_bit_0:
+      address: 0x8A
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 0
+    pd_bias_en:
+      address: 0x29
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    identifier:
-      address: 0x00
+    # pll_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 9
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 1
+    # pll_clockout:
+    #   address: 0x28
+    #   bitposition: 11
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    pll_lock_bit_0:
+      address: 0x86
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 42435
-    version:
-      address: 0x01
+      value: 1
+    psec4a_a_ro_feedback_calculated_value:
+      address: 0xA8
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    in_sel:
-      address: 0x0B
-      bitposition: 12
-      bitwidth: 1
+      value: 247
+    psec4a_a_ro_monitor_clock_count_lsw:
+      address: 0x99
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    iomode0:
-      address: 0x04
-      bitposition: 7
-      bitwidth: 1
+      value: 0
+    psec4a_a_ro_monitor_clock_count_msw:
+      address: 0x98
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1
-    iomode1:
-      address: 0x04
-      bitposition: 8
-      bitwidth: 1
+      value: 0
+    psec4a_a_vcdl_monitor_clock_count_lsw:
+      address: 0xA1
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    loadwait:
-      address: 0x07
-      bitposition: 8
-      bitwidth: 4
+    psec4a_a_vcdl_monitor_clock_count_msw:
+      address: 0xA0
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 15
-    nasa_trig_sel_ext:
-      address: 0x1D
-      bitposition: 15
-      bitwidth: 1
+      value: 0
+    psec4a_b_ro_feedback_calculated_value:
+      address: 0xA9
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    nramp:
-      address: 0x04
-      bitposition: 4
-      bitwidth: 1
+      value: 269
+    psec4a_b_ro_monitor_clock_count_lsw:
+      address: 0x9B
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    nrw:
-      address: 0x04
-      bitposition: 11
-      bitwidth: 1
+      value: 0
+    psec4a_b_ro_monitor_clock_count_msw:
+      address: 0x9A
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    numwinds:
-      address: 0x08
+      value: 0
+    psec4a_b_vcdl_monitor_clock_count_lsw:
+      address: 0xA3
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1
-    out_sel:
-      address: 0x0B
-      bitposition: 11
-      bitwidth: 1
+      value: 0
+    psec4a_b_vcdl_monitor_clock_count_msw:
+      address: 0xA2
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    pclk:
-      address: 0x04
-      bitposition: 1
-      bitwidth: 1
+      value: 0
+    psec4a_biascomp_out:
+      address: 0x1A
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    pclkwidth:
-      address: 0x07
-      bitposition: 12
-      bitwidth: 4
+      value: 512
+    psec4a_biasdllfirst_out:
+      address: 0x1C
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 15
-    rden:
-      address: 0x04
-      bitposition: 6
-      bitwidth: 1
+      value: 256
+    psec4a_biasdlllast_out:
+      address: 0x1B
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    regclr:
-      address: 0x04
+      value: 256
+    psec4a_biasdlln_out:
+      address: 0x1E
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    runevs:
-      address: 0x05
+      value: 592
+    psec4a_biasdllp_out:
+      address: 0x1D
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 1
-    rx_data0:
-      address: 0x1A
+      value: 416
+    psec4a_biasrampbuf_out:
+      address: 0x19
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    rx_data1:
-      address: 0x1B
+      value: 432
+    psec4a_biasrampslope_out:
+      address: 0x27
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    rx_data2:
-      address: 0x1C
+    psec4a_biastrign_out:
+      address: 0x17
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    rx_data4:
-      address: 0x1E
+      value: 0x0200  # 0
+    psec4a_biasxfer_out:
+      address: 0x18
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
+      value: 512
+    psec4a_mclk_source_clock_count_lsw:
+      address: 0x8F
+      bitposition: 0
+      bitwidth: 16
+      description: 'Read-only Debug clock, should be the same as VCDL when read out'
+      readwrite: r
       value: 0
-    rx_data5:
-      address: 0x1F
+    psec4a_mclk_source_clock_count_msw:
+      address: 0x8E
       bitposition: 0
       bitwidth: 16
-      description: ''
-      readwrite: rw
+      description: 'Read-only Debug clock, should be the same as VCDL when read out'
+      readwrite: r
       value: 0
-    rx_data6:
-      address: 0x20
+    psec4a_c_ro_feedback_calculated_value:
+      address: 0xAA
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    rx_en:
-      address: 0x19
+      value: 326
+    psec4a_c_ro_monitor_clock_count_lsw:
+      address: 0x9D
       bitposition: 0
-      bitwidth: 1
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    rx_num_words:
-      address: 0x19
-      bitposition: 2
-      bitwidth: 6
+    psec4a_c_ro_monitor_clock_count_msw:
+      address: 0x9C
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    rx_oneshot:
-      address: 0x19
-      bitposition: 1
-      bitwidth: 1
+    psec4a_c_vcdl_monitor_clock_count_lsw:
+      address: 0xA5
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    rx_speed:
-      address: 0x19
-      bitposition: 8
-      bitwidth: 2
+    psec4a_c_vcdl_monitor_clock_count_msw:
+      address: 0xA4
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    sel:
-      address: 0x04
-      bitposition: 12
-      bitwidth: 1
-      description: ''
-      readwrite: rw
-      value: false
-    selany:
-      address: 0x04
-      bitposition: 2
-      bitwidth: 1
+    psec4a_d_ro_feedback_calculated_value:
+      address: 0xAB
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    sst_speed:
-      address: 0x1D
-      bitposition: 14
-      bitwidth: 1
+      value: 246
+    psec4a_d_ro_monitor_clock_count_lsw:
+      address: 0x9F
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    stopacq:
-      address: 0x04
-      bitposition: 13
-      bitwidth: 1
+      value: 0
+    psec4a_d_ro_monitor_clock_count_msw:
+      address: 0x9E
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    switch_nen:
-      address: 0x0B
-      bitposition: 13
-      bitwidth: 1
+      value: 0
+    psec4a_d_vcdl_monitor_clock_count_lsw:
+      address: 0xA7
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: true
-    syncloc:
-      address: 0x0E
+      value: 0
+    psec4a_d_vcdl_monitor_clock_count_msw:
+      address: 0xA6
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
       value: 0
-    sysrst:
-      address: 0x04
-      bitposition: 14
+    # psec4a_mode:
+    #   address: 0x13
+    #   bitposition: 5
+    #   bitwidth: 2
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    xref_address_mode:
+      address: 0x13
+      bitposition: 5
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: false
-    trig_sel:
-      address: 0x0B
-      bitposition: 10
-      bitwidth: 1
+      value: 0
+    psec4a_rovcp:
+      address: 0x16
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    trigger_mux:
-      address: 0x22
-      bitposition: 5
-      bitwidth: 4
-      description: 'Change which trigger type is used to trigger the chip, there are 9 different modes.'
-      readwrite: rw
-      value: 8
-    windsel:
-      address: 0x07
+      value: 300
+    psec4a_status:
+      address: 0x84
       bitposition: 0
-      bitwidth: 8
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: 0
-    wren:
-      address: 0x04
-      bitposition: 5
-      bitwidth: 1
+      value: 4852
+    psec4a_trigthresh1_out:
+      address: 0x1F
+      bitposition: 0
+      bitwidth: 16
       description: ''
       readwrite: rw
-      value: false
-    eth_addr_sel:
-      address: 0x28
+      value: 1536  # 0
+    psec4a_trigthresh2_out:
+      address: 0x20
       bitposition: 0
-      bitwidth: 2
-      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
-      readwrite: rw
-      value: 0
-    eth_port_sel:
-      address: 0x28
-      bitposition: 2
-      bitwidth: 2
-      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
-      readwrite: rw
-      value: 0
-    tx_mode:
-      address: 0x28
-      bitposition: 4
-      bitwidth: 1
-      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    eth_ar_en:
-      address: 0x28
-      bitposition: 5
-      bitwidth: 1
-      description: 'enables auto-response destination IP address; currently unused'
+      value: 1536  # 0
+    psec4a_trigthresh3_out:
+      address: 0x21
+      bitposition: 0
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    eth_dhcp_en:
-      address: 0x28
-      bitposition: 6
-      bitwidth: 1
-      description: 'enables DHCP resolution of source IP address; currently unused'
+      value: 1536  # 0
+    psec4a_trigthresh4_out:
+      address: 0x22
+      bitposition: 0
+      bitwidth: 16
+      description: ''
       readwrite: rw
-      value: 0
-    eth_dest_addr15_0:
-      address: 0x29
+      value: 1536  # 0
+    psec4a_trigthresh5_out:
+      address: 0x23
       bitposition: 0
       bitwidth: 16
-      description: 'lower 16 bits of ethernet destination IP address'
+      description: ''
       readwrite: rw
-      value: 0
-    eth_dest_addr31_16:
-      address: 0x2A
+      value: 1536  # 0
+    psec4a_trigthresh6_out:
+      address: 0x24
       bitposition: 0
       bitwidth: 16
-      description: 'upper 16 bits of ethernet destination IP address'
+      description: ''
       readwrite: rw
-      value: 0
-    eth_src_addr15_0:
-      address: 0x2B
+      value: 1536  # 0
+    psec4a_trigthresh7_out:
+      address: 0x25
       bitposition: 0
       bitwidth: 16
-      description: 'lower 16 bits of ethernet source IP address'
+      description: ''
       readwrite: rw
-      value: 0
-    eth_src_addr31_16:
-      address: 0x2C
+      value: 1536  # 0
+    psec4a_trigthresh8_out:
+      address: 0x26
       bitposition: 0
       bitwidth: 16
-      description: 'upper 16 bits of ethernet source IP address'
+      description: ''
+      readwrite: rw
+      value: 1536  # 0
+    reread_data:
+      address: 0x10
+      bitposition: 9
+      bitwidth: 1
+      description: ''
       readwrite: rw
       value: 0
-    eth_dest_port:
-      address: 0x2D
+    ring_oscillator_feedback_target_value_lsw:
+      address: 0x11
       bitposition: 0
       bitwidth: 16
-      description: 'UDP destination port'
+      description: ''
       readwrite: rw
-      value: 0
-    eth_src_port:
-      address: 0x2E
+      value: 29529
+    ring_oscillator_feedback_target_value_msw:
+      address: 0x12
       bitposition: 0
       bitwidth: 16
-      description: 'UDP source port'
+      description: ''
       readwrite: rw
-      value: 0
-  i2c_registers:
-    i2c_en:
-      address: 0x09
-      bitposition: 14
+      value: 7
+    ro_feedback_enable:
+      address: 0x13
+      bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
-    i2c_send:
-      address: 0x0F
-      bitposition: 15
+      value: 1
+    ro_monitor_reset:
+      address: 0x29
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    i2c_words:
-      address: 0x0F
-      bitposition: 8
-      bitwidth: 3
-      description: ''
+    self_trigger_or_enable:
+      address: 0x13
+      bitposition: 6
+      bitwidth: 1
+      description: 'Enable Self Trigger OR function in PSEC4A'
       readwrite: rw
-      value: 0
-    i2c_addr:
-      address: 0x0F
-      bitposition: 0
-      bitwidth: 8
+      value: 1
+    serial_data_select:
+      address: 0x28
+      bitposition: 12
+      bitwidth: 4
       description: ''
       readwrite: rw
       value: 0
-    i2c_data0:
+    serial_write_strobe:
       address: 0x10
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    i2c_data1:
-      address: 0x11
-      bitposition: 0
-      bitwidth: 16
+    software_trigger:
+      address: 0x13
+      bitposition: 4
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    i2c_data2:
-      address: 0x12
-      bitposition: 0
-      bitwidth: 16
+    speed_select:
+      address: 0x13
+      bitposition: 3
+      bitwidth: 1
       description: ''
       readwrite: rw
+      value: 1
+    # system_clock_monitor:
+    #   address: 0x28
+    #   bitposition: 8
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 1
+    trig_out1:
+      address: 0x90
+      bitposition: 0
+      bitwidth: 4
+      description: 'DCBA chiporder'
+      readwrite: rw
       value: 0
-    i2c_data3:
+    trigger_mask_enable:
+      address: 0x29
+      bitposition: 8
+      bitwidth: 8
+      description: 'Trigger mask where each bit is a corresponding chip'
+      readwrite: rw
+      value: 255  # '11111111'
+    trigger_mode:
+      address: 0x29
+      bitposition: 5
+      bitwidth: 2
+      description: '<html><head/><body><p>Set the triggermode:<br/>
+        00: Software Trigger, the default.<br/>
+        01: Auto Trigger, 2Hz auto trigger rate.<br/>
+        10: External Trigger, trigger on trig in.<br/>
+        11: Self Trigger, trigger on signal levels.
+        </p></body></html>'
+      readwrite: rw
+      value: 0
+    trigger_reset:
       address: 0x13
-      bitposition: 0
-      bitwidth: 16
+      bitposition: 13
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    response0:
-      address: 0x48
-      bitposition: 0
-      bitwidth: 16
+    # trigger_scaler:
+    #   address: 0x97
+    #   bitposition: 0
+    #   bitwidth: 8
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
+    trigger_sign:
+      address: 0x13
+      bitposition: 1
+      bitwidth: 1
       description: ''
-      readwrite: r
+      readwrite: rw
       value: 0
-    response1:
-      address: 0x49
+    uart_status:
+      address: 0x81
       bitposition: 0
-      bitwidth: 16
+      bitwidth: 8
       description: ''
-      readwrite: r
-      value: 0
-    response2:
-      address: 0x4A
-      bitposition: 0
-      bitwidth: 16
+      readwrite: rw
+      value: 84
+    uart_handshake_en_out:
+      address: 0x10
+      bitposition: 8
+      bitwidth: 1
       description: ''
-      readwrite: r
-      value: 0
-    response3:
-      address: 0x4B
+      readwrite: rw
+      value: false
+    version_number:
+      address: 0x80
       bitposition: 0
       bitwidth: 16
       description: ''
-      readwrite: r
+      readwrite: rw
+      value: 4101
+    wave_fifo_reset:
+      address: 0x10
+      bitposition: 1
+      bitwidth: 1
+      description: ''
+      readwrite: rw
       value: 0
+    xfer_reset:
+      address: 0x13
+      bitposition: 2
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 1
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,549 +1,779 @@
-model: udc16
+model: aodsoc_asoc
 features:
   adc2mv: false
-  dac_sweep: true
+  dac_sweep: false
   ext_dac: true
   pedestals: true
-  threshold_scan: false
+  threshold_scan: true
   tia_dac: false
   timing_calibration: false
   naludaq_rs: true
 params:
-  chanmask: 0xFF00
-  channels: 16
+  chanmask: 0x300
+  channels: 8
   chanshift: 8
   chips:
-    0:
+    0..1:
       !include_chip
-      from: udc16::params
-  clock_file: Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+      from: asocv3::params
+  # clock_file: '' # AODSoC boards have fixed clocks
   connections:
     - serial
     - d2xx
     - udp
   si5341_address: 0xEE
+  timing_hack: true
   default_baud:
-    2000000: 50
-  default_baudrate: 2000000
-  default_clock: 200000000.0
-  default_divider: 50
-  default_trigger_value: 0
-  intamp_bias_mode_chan0_7: 'c'
-  intamp_bias_mode_chan8_15: 'c'
+    115200: 868
+  default_baudrate: 115200
+  default_clock: 100000000.0
+  default_divider: 868
+  default_trigger_value: 1500
+  threshold_scan:
+    min_vref: 0
+    max_vref: 2500
+    start: 500
+    stop: 3500
+    stepsize: 5
+    units: counts
   ext_dac:
     chip: dac7578
-    max_mv: 1250
-    max_counts: 3930
-    min_counts: 0
+    max_mv: 2500
+    max_counts: 4095
     channels:
-      0..15: 2000
+      0..7: 2048
     address_mapping:
-      0..7: 0x4B
-      8..15: 0x48
+      0..7: 0x48
     channel_mapping:
-      0, 08: 0
-      1, 09: 1
-      2, 10: 2
-      3, 11: 3
-      4, 12: 4
-      5, 13: 5
-      6, 14: 6
-      7, 15: 7
-  trigger:
-    max_val: 2047
-    min_val: 0
-    default: false
-  num_trigger_channels: 8
-  headers: 0
-  last_window_fix_amount: 47
-  lastbits: 0
-  numregs: 32
-  pedestals_blocks: 8
+      0: 7
+      1: 5
+      2: 3
+      3: 1
+      4: 0
+      5: 2
+      6: 4
+      7: 6
+  ext_trig_cycles: 10
+  headers: 3
+  numregs: 64
+  pedestals_blocks: 16
   peripherals:
-    current:
-      chan: 0
-      addr: 0xD0
-      bits: 16
-      gain: 8
-    vadjn:
+    vadjn_0:
+      chan: 3
+      addr: 0x4C
+    vadjn_1:
+      chan: 2
+      addr: 0x4C
+    ldo_voltage:
       chan: 1
-      addr: 0xD8
-      bits: 16
-      gain: 1
-    vadjp:
-      chan: 0
-      addr: 0xD8
-      bits: 16
-      gain: 1
+      addr: 0x4C
+    chip_voltage:
+      chan: 2
+      addr: 0x4C
+    current_resistor: 0.010
   possible_bauds:
+    115200: 868
+    1000000: 100
     2000000: 50
-  resolution: 10
+    3000000: 33
+  resolution: 12
   samples: 64
-  samplingrate: 9.2
-  stop_word: CAFE
-  strobe_values_correction: True  # Shift the strobe values on certain boards with swapped internal routing.
-  strobe_correction_keys:
-    - digsync_le
-    - digsync_te
-    - wrstrb1_le
-    - wrstrb1_te
-    - wrstrb2_le
-    - wrstrb2_te
-    - wrsync1_le
-    - wrsync1_te
-    - wrsync2_le
-    - wrsync2_te
+  samplingrate: 3.2
+  stop_word: "cafe"
   wait: AE000001
-  wbias: 750
-  windmask: 0x00FF
-  windows: 64
+  wbias: 848
+  windmask: 0x0FF
+  windows: 254
 registers:
   analog_registers:
     !include_registers
-      from: udc16::registers::analog_registers
+      from: asocv3::registers::analog_registers
+      value_count: 2
+      override:
+        isel:
+          value: [2610, 2627]
   digital_registers:
     !include_registers
-      from: udc16::registers::digital_registers
+      from: asocv3::registers::digital_registers
+      value_count: 2
   control_registers:
-    identifier:
-      address: 0x00
+    1v2_en:
+      address: 0x17
+      bitposition: 1
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
+    2v5_en:
+      address: 0x17
       bitposition: 0
-      bitwidth: 16
-      description: 'Unique board identifier'
+      bitwidth: 1
+      description: ''
       readwrite: rw
-      value: 0x4D5C
-    version:
-      address: 0x01
+      value: true
+    3v3_i2c_en:
+      address: 0x17
+      bitposition: 2
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
+    8b10b_en:
+      address: 0x19
+      bitposition: 12
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: 0
+    amp_pwrdn_out:
+      address: 0x1A
       bitposition: 0
-      bitwidth: 16
-      description: 'Current firmware version'
+      bitwidth: 8
+      description: 'Onboard amplifiers active high means amp off'
       readwrite: rw
       value: 0
-    data_iot:
-      address: 0x04
-      bitposition: 15
-      bitwidth: 1
+    addr:
+      address: 0x16
+      bitposition: 0
+      bitwidth: 9
       description: ''
       readwrite: rw
       value: 0
-    stopacq:
-      address: 0x04
-      bitposition: 13
+    addr_user:
+      address: 0x16
+      bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    sel:
-      address: 0x04
+      value: false
+    chansel:
+      address: 0x06
       bitposition: 12
+      bitwidth: 4
+      description: ''
+      readwrite: rw
+      value: 15
+    clk1v8_en:
+      address: 0x17
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    nrw:
-      address: 0x04
-      bitposition: 11
+      value: true
+    clk2v5_en:
+      address: 0x17
+      bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    exttrig:
-      address: 0x04
+      value: true
+    clk_fdec:
+      address: 0x17
+      bitposition: 9
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_finc:
+      address: 0x17
+      bitposition: 8
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_i2c_sel:
+      address: 0x17
+      bitposition: 5
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: true
+    clk_oeb:
+      address: 0x17
+      bitposition: 6
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_reset:
+      address: 0x17
+      bitposition: 7
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    clk_sync:
+      address: 0x17
       bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
+      value: false
+    data:
+      address: 0x14
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
       value: 0
-    sysrst:
-      address: 0x04
-      bitposition: 9
+    data_user:
+      address: 0x14
+      bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
+      value: false
+    debug_data:
+      address: 0x15
+      bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
       value: 0
-    iomode1:
-      address: 0x04
-      bitposition: 6
+    debug_data_user:
+      address: 0x15
+      bitposition: 15
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
-    nramp:
-      address: 0x04
-      bitposition: 5
+      value: false
+    digrst:
+      address: 0x16
+      bitposition: 9
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    gccclr:
-      address: 0x04
-      bitposition: 4
+    digser_rst:
+      address: 0x19
+      bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    selany:
+    exttrig:
       address: 0x04
-      bitposition: 3
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    pclk:
+      value: false
+    gccclr:
       address: 0x04
-      bitposition: 2
+      bitposition: 4
       bitwidth: 1
       description: ''
       readwrite: rw
+      value: false
+    idac_ldac:
+      address: 0x1B
+      bitposition: 0
+      bitwidth: 1
+      description: 'pin on AD7578'
+      readwrite: rw
       value: 0
-    regclr:
-      address: 0x04
+    idac_nclr:
+      address: 0x1B
       bitposition: 1
       bitwidth: 1
-      description: ''
+      description: 'pin on AD7578'
+      readwrite: rw
+      value: 1
+    fifo_unload_or_event_en:
+      address: 0x1F
+      bitposition: 0
+      bitwidth: 1
+      description: 'Once data is loaded into the FIFO it will not be sent out to the UART until the end of the current event. Use this mode for capturing sampled data events. '
       readwrite: rw
       value: 0
+    identifier:
+      address: 0x00
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 309
     iomode0:
       address: 0x04
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
+      value: true
+    iomode1:
+      address: 0x04
+      bitposition: 6
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    leds:
+      address: 0x18
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
       value: 0
-    pclkwidth:
+    loadwait:
       address: 0x07
       bitposition: 8
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    loadwait:
+    nramp:
+      address: 0x04
+      bitposition: 5
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    nrw:
+      address: 0x04
+      bitposition: 11
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    numwinds:
+      address: 0x08
+      bitposition: 0
+      bitwidth: 8
+      description: ''
+      readwrite: rw
+      value: 1
+    pclk:
+      address: 0x04
+      bitposition: 2
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    pclkwidth:
       address: 0x07
       bitposition: 12
       bitwidth: 4
       description: ''
       readwrite: rw
       value: 15
-    udc_arm:
-      address: 0x09
+    ramplen:
+      address: 0x06
       bitposition: 0
+      bitwidth: 12
+      description: ''
+      readwrite: rw
+      value: 2000
+    regclr:
+      address: 0x04
+      bitposition: 1
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    reread_data:
-      address: 0x0C
+      value: false
+    runevs:
+      address: 0x05
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 1
+    rx_en:
+      address: 0x19
       bitposition: 0
       bitwidth: 1
-      description: 'Ask the FPGA to send whatever event is in the output buffer'
+      description: ''
       readwrite: rw
       value: 0
-    debug_data_to_write:
-      address: 0x14
-      bitposition: 0
-      bitwidth: 12
+    rx_num_words:
+      address: 0x19
+      bitposition: 2
+      bitwidth: 6
       description: ''
       readwrite: rw
       value: 0
-    debug_addr:
-      address: 0x15
-      bitposition: 0
-      bitwidth: 12
+    rx_oneshot:
+      address: 0x19
+      bitposition: 1
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    wave_fifo_reset:
-      address: 0x16
+    rx_speed:
+      address: 0x19
+      bitposition: 8
+      bitwidth: 2
+      description: ''
+      readwrite: rw
+      value: 0
+    sel:
+      address: 0x04
+      bitposition: 12
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    selany:
+      address: 0x04
+      bitposition: 3
+      bitwidth: 1
+      description: ''
+      readwrite: rw
+      value: false
+    slow_sysclk:
+      address: 0x19
       bitposition: 10
       bitwidth: 1
-      description: 'Reset the waveform FIFO, effectively flushing any data in the output FIFO'
+      description: ''
       readwrite: rw
       value: 0
-    digrst:
-      address: 0x16
-      bitposition: 9
+    stopacq:
+      address: 0x04
+      bitposition: 13
       bitwidth: 1
-      description: 'Toggle the digital reset pin, resets the ASIC.'
+      description: ''
       readwrite: rw
-      value: 0
-    2v5_en:
-      address: 0x17
+      value: false
+    syncloc:
+      address: 0x09
       bitposition: 0
-      bitwidth: 1
-      description: 'Enable the 2.5V rail'
+      bitwidth: 8
+      description: ''
       readwrite: rw
       value: 0
-    1v2_en:
-      address: 0x17
-      bitposition: 1
+    sysclk:
+      address: 0x04
+      bitposition: 8
       bitwidth: 1
-      description: 'Enable the 1.2V rail'
+      description: ''
       readwrite: rw
-      value: 0
-    clk2v5_en:
-      address: 0x17
-      bitposition: 3
+      value: false
+    sysrst:
+      address: 0x04
+      bitposition: 9
       bitwidth: 1
-      description: 'Enable the clock specific 2.5V rail.'
+      description: ''
       readwrite: rw
-      value: 0
-    clk1v8_en:
-      address: 0x17
-      bitposition: 4
+      value: true
+    tx_en:
+      address: 0x19
+      bitposition: 11
       bitwidth: 1
-      description: 'Enable the clock specific 1.8V rail.'
+      description: ''
       readwrite: rw
       value: 0
-    clk_oeb:
-      address: 0x17
-      bitposition: 6
-      bitwidth: 1
+    windsel:
+      address: 0x07
+      bitposition: 0
+      bitwidth: 8
       description: ''
       readwrite: rw
       value: 0
-    clk_reset:
-      address: 0x17
+    wrstrboff:
+      address: 0x04
       bitposition: 7
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 0
-    clk_sync:
-      address: 0x17
-      bitposition: 10
+      value: false
+    rxout_pol:
+      address: 0x22
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 6400
+    txin_pol:
+      address: 0x23
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 4412
+    ard_header:
+      address: 0x21
+      bitposition: 0
       bitwidth: 1
+      description: 'Enable AARDVARC debug header.'
+      readwrite: rw
+      value: 1
+    ard_rx_en:
+      address: 0x1D
+      bitposition: 0
+      bitwidth: 16
+      description: 'TR-BHM ASIC Rx Enable register 29dec. Bit 0 and 1 enable transmitting data to ASICs. Need to set these bits to send data to the ASICs'
+      readwrite: rw
+      value: 3
+    ard_tx_en:
+      address: 0x1E
+      bitposition: 0
+      bitwidth: 16
+      description: 'TR-BHM ASIC Tx Enable register 30dec. Bit 0 and 1 enable receiving data from ASICs. Need to set these bits to get data back from the ASICs'
+      readwrite: rw
+      value: 3
+    ard0_clk_sel:
+      address: 0x24
+      bitposition: 0
+      bitwidth: 2
       description: ''
       readwrite: rw
       value: 0
-    tx_packet_marker:
-      address: 0x18
+    ard1_clk_sel:
+      address: 0x25
       bitposition: 0
-      bitwidth: 6
+      bitwidth: 2
       description: ''
       readwrite: rw
-      value: 0
-    rx_enable:
-      address: 0x19
+      value: 1
+    motor_trig_en:
+      address: 0x27
       bitposition: 0
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_reg_polarity:
-      address: 0x19
-      bitposition: 1
+    motor_trig_evts:
+      address: 0x26
+      bitposition: 0
+      bitwidth: 16
+      description: ''
+      readwrite: rw
+      value: 1
+    oleas_en_trig:
+      address: 0x0A
+      bitposition: 10
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    rx_divider:
-      address: 0x19
-      bitposition: 4
-      bitwidth: 4
+    oleas_pol_a:
+      address: 0x0A
+      bitposition: 11
+      bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    tx_enable:
-      address: 0x19
+    oleas_pol_b:
+      address: 0x0A
       bitposition: 12
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    tx_reg_polarity:
-      address: 0x19
+    oleas_en_a:
+      address: 0x0A
       bitposition: 13
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    tx_10_bit_data:
-      address: 0x19
+    oleas_en_b:
+      address: 0x0A
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
       value: 0
-    analog_debug_en:
-      address: 0x1F
+    oleas_loop:
+      address: 0x0A
       bitposition: 0
-      bitwidth: 1
-      description: 'Enable analog debug mode, bypassing the digital side of the chip. Allows the user to communicate directly with the analog side.'
+      bitwidth: 5
+      description: ''
       readwrite: rw
-      value: 0
-    v1v2_power_good:
-      address: 0x46
+      value: 15
+    oleas_length_a:
+      address: 0x0B
       bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
-      value: 0
-    temperature_event:
-      address: 0x46
-      bitposition: 1
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+      bitwidth: 16
+      description: ''
+      readwrite: rw
       value: 0
-    udc_mon_in:
-      address: 0x47
+    oleas_length_b:
+      address: 0x0D
       bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+      bitwidth: 16
+      description: ''
+      readwrite: rw
       value: 0
-    i2c_dataout_genwr_3:
-      address: 0x48
+    oleas_delay_a:
+      address: 0x0C
       bitposition: 0
       bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
+      description: ''
+      readwrite: rw
       value: 0
-    i2c_dataout_genwr_2:
-      address: 0x49
+    oleas_delay_b:
+      address: 0x0E
       bitposition: 0
       bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
+      description: ''
+      readwrite: rw
       value: 0
-    i2c_dataout_genwr_1:
-      address: 0x4A
+    testmode:
+      address: 0x20
       bitposition: 0
-      bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
+      bitwidth: 1
+      description: ''
+      readwrite: rw
       value: 0
-    i2c_dataout_genwr_0:
-      address: 0x4B
+    eth_addr_sel:
+      address: 0x28
       bitposition: 0
-      bitwidth: 16
-      description: 'Read-Only status register'
-      readwrite: r
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) IP addresses'
+      readwrite: rw
       value: 0
-    udc_triggerout_in:
-      address: 0x4C
+    eth_port_sel:
+      address: 0x28
       bitposition: 2
+      bitwidth: 2
+      description: 'enables manually set destination (bit 0) and source (bit 1) UDP ports'
+      readwrite: rw
+      value: 0
+    tx_mode:
+      address: 0x28
+      bitposition: 4
       bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+      description: 'selects ethernet (value = 1) or UART (value = 0) transmission'
+      readwrite: rw
       value: 0
-    si5341a_intr_n_in:
-      address: 0x4C
-      bitposition: 1
+    eth_ar_en:
+      address: 0x28
+      bitposition: 5
       bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+      description: 'enables auto-response destination IP address; currently unused'
+      readwrite: rw
       value: 0
-    si5341a_lol_n_in:
-      address: 0x4C
-      bitposition: 0
+    eth_dhcp_en:
+      address: 0x28
+      bitposition: 6
       bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+      description: 'enables DHCP resolution of source IP address; currently unused'
+      readwrite: rw
       value: 0
-    system_clock_locked:
-      address: 0x59
+    eth_dest_addr15_0:
+      address: 0x29
       bitposition: 0
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet destination IP address'
+      readwrite: rw
       value: 0
-    sys_clock_locked:
-      address: 0x59
-      bitposition: 1
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+    eth_dest_addr31_16:
+      address: 0x2A
+      bitposition: 0
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet destination IP address'
+      readwrite: rw
       value: 0
-    idigser_tx_idle_locked:
-      address: 0x59
-      bitposition: 2
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+    eth_src_addr15_0:
+      address: 0x2B
+      bitposition: 0
+      bitwidth: 16
+      description: 'lower 16 bits of ethernet source IP address'
+      readwrite: rw
       value: 0
-    udc_busy_locked_in:
-      address: 0x59
-      bitposition: 3
-      bitwidth: 1
-      description: 'Read-Only status register'
-      readwrite: r
+    eth_src_addr31_16:
+      address: 0x2C
+      bitposition: 0
+      bitwidth: 16
+      description: 'upper 16 bits of ethernet source IP address'
+      readwrite: rw
+      value: 0
+    eth_dest_port:
+      address: 0x2D
+      bitposition: 0
+      bitwidth: 16
+      description: 'UDP destination port'
+      readwrite: rw
+      value: 0
+    eth_src_port:
+      address: 0x2E
+      bitposition: 0
+      bitwidth: 16
+      description: 'UDP source port'
+      readwrite: rw
       value: 0
   i2c_registers:
     i2c_en:
       address: 0x0F
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: 1
+      value: true
+    # i2c_send:
+    #   address: 0x0F
+    #   bitposition: 15
+    #   bitwidth: 1
+    #   description: ''
+    #   readwrite: rw
+    #   value: 0
     i2c_words:
       address: 0x0F
       bitposition: 8
-      bitwidth: 4
-      description: 'number of words to send in the i2c command.'
+      bitwidth: 3
+      description: ''
       readwrite: rw
       value: 0
     i2c_addr:
       address: 0x0F
       bitposition: 0
       bitwidth: 8
-      description: 'i2c address for the commands in the string builder'
+      description: ''
       readwrite: rw
       value: 0
     i2c_data0:
       address: 0x10
       bitposition: 0
-      bitwidth: 8
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      bitwidth: 16
+      description: ''
       readwrite: rw
       value: 0
     i2c_data1:
       address: 0x11
       bitposition: 0
       bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: ''
       readwrite: rw
       value: 0
     i2c_data2:
       address: 0x12
       bitposition: 0
       bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: ''
       readwrite: rw
       value: 0
     i2c_data3:
       address: 0x13
       bitposition: 0
       bitwidth: 16
-      description: 'Data storage used by the i2c string builder, for both rx and tx data'
+      description: ''
       readwrite: rw
       value: 0
     response0:
-      address: 0x28
+      address: 0x48
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response1:
-      address: 0x29
+      address: 0x49
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response2:
-      address: 0x2A
+      address: 0x4A
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
     response3:
-      address: 0x2B
+      address: 0x4B
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: r
       value: 0
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/upac96.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-12.1.0/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-model: upaci
+model: zdigitizer
 params:
   chanmask: 511
   channels: 32
   chanshift: 3
   connections:
     - serial
     - d2xx
   default_baud:
-    115200: 434
+    115200: 217
   default_baudrate: 115200
   default_clock: 200000000.0
-  default_divider: 434
+  default_divider: 217
   default_trigger_value: 0
   ext_dac:
     max_mv: 1200
     max_counts: 65535
     channels:
       0: 30000
       8: 30000
@@ -44,16 +44,16 @@
       gain: 1
     vadjp:
       chan: 1
       addr: 0xD8
       bits: 16
       gain: 1
   possible_bauds:
-    115200: 434
-    2000000: 25
+    115200: 217
+    1000000: 25
   resolution: 11
   samples: 132
   samplingrate: 9.2
   stop_word: !!binary |
     +s4=
   wait: AE000001
   wbias: 750
@@ -323,14 +323,28 @@
     pll_lock_bit_0:
       address: 0x86
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 1
+    # psec4a_mclk_source_clock_count_lsw:
+    #   address: 0x8F
+    #   bitposition: 0
+    #   bitwidth: 16
+    #   description: 'Read-only Debug clock, should be the same as VCDL when read out'
+    #   readwrite: r
+    #   value: 0
+    # psec4a_mclk_source_clock_count_msw:
+    #   address: 0x8E
+    #   bitposition: 0
+    #   bitwidth: 16
+    #   description: 'Read-only Debug clock, should be the same as VCDL when read out'
+    #   readwrite: r
+    #   value: 0
     psec4a_a_ro_feedback_calculated_value:
       address: 0xA8
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 247
@@ -456,28 +470,14 @@
     psec4a_biasxfer_out:
       address: 0x18
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 512
-    psec4a_mclk_source_clock_count_lsw:
-      address: 0x8F
-      bitposition: 0
-      bitwidth: 16
-      description: 'Read-only Debug clock, should be the same as VCDL when read out'
-      readwrite: r
-      value: 0
-    psec4a_mclk_source_clock_count_msw:
-      address: 0x8E
-      bitposition: 0
-      bitwidth: 16
-      description: 'Read-only Debug clock, should be the same as VCDL when read out'
-      readwrite: r
-      value: 0
     psec4a_c_ro_feedback_calculated_value:
       address: 0xAA
       bitposition: 0
       bitwidth: 16
       description: ''
       readwrite: rw
       value: 326
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs/exceptions.py` & `naluconfigs-12.1.0/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/helpers.py` & `naluconfigs-12.1.0/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs/postprocess.py` & `naluconfigs-12.1.0/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-12.1.0/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.3.1
+Version: 12.1.0
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.3.1/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-12.1.0/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
 src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
 src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
 src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
 src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
 src/naluconfigs/data/registers/aardvarcv2.yml
 src/naluconfigs/data/registers/aardvarcv3.yml
-src/naluconfigs/data/registers/aardvarcv3_gbe.yml
 src/naluconfigs/data/registers/aardvarcv4.yml
 src/naluconfigs/data/registers/aodsoc_aods.yml
 src/naluconfigs/data/registers/aodsoc_asoc.yml
 src/naluconfigs/data/registers/aodsv1.yml
 src/naluconfigs/data/registers/aodsv2_eval.yml
 src/naluconfigs/data/registers/asoc.yml
 src/naluconfigs/data/registers/asocv2.yml
```

### Comparing `naluconfigs-11.3.1/tests/test_hex_addr_converter.py` & `naluconfigs-12.1.0/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/tests/test_i2c_registers.py` & `naluconfigs-12.1.0/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/tests/test_multichip.py` & `naluconfigs-12.1.0/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/tests/test_post_processing.py` & `naluconfigs-12.1.0/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.3.1/tests/test_range_keys.py` & `naluconfigs-12.1.0/tests/test_range_keys.py`

 * *Files identical despite different names*

