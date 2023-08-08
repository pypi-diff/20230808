# Comparing `tmp/armulator-1.1.2.tar.gz` & `tmp/armulator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armulator-1.1.2.tar", last modified: Sun May 29 19:23:51 2022, max compression
+gzip compressed data, was "armulator-1.1.3.tar", last modified: Tue Aug  8 04:59:00 2023, max compression
```

## Comparing `armulator-1.1.2.tar` & `armulator-1.1.3.tar`

### file list

```diff
@@ -1,1006 +1,1006 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.392457 armulator-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-05-29 19:23:42.000000 armulator-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-05-29 19:23:51.392457 armulator-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-05-29 19:23:42.000000 armulator-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.280456 armulator-1.1.2/armulator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.280456 armulator-1.1.2/armulator/armv6/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/address_descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.284456 armulator-1.1.2/armulator/armv6/all_registers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/abstract_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/cpacr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/cpsr.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/dacr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/dbgdidr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/dfsr.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/fcseidr.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/fpexc.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/hcptr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/hcr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/hdcr.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/hpfar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/hsctlr.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/hsr.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/hstr.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/htcr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/id_pfr1.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/jmcr.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/midr.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/mpuir.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/nmrr.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/nsacr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/pmcr.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/prrr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/racr.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/rgnr.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/rsr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/scr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/sctlr.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/sder.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/sunavcr.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/teecr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/ttbcr.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/vbar.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/all_registers/vtcr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/arm_configurations.json
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/arm_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    89184 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/arm_v6.py
--rw-r--r--   0 runner    (1001) docker     (121)     4302 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/bits_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/configurations.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/full_address.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/memory_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/memory_controller_hub.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/memory_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.284456 armulator-1.1.2/armulator/armv6/opcodes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.328456 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adc_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adc_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adc_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_register_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_register_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adr.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/and_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/and_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/and_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/asr_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/asr_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/b.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bfc.py
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bfi.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bic_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bic_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bic_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bkpt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bl_blx_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/blx_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bxj.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cbz.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cdp_cdp2.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/clrex.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/clz.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmn_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmn_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmn_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmp_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmp_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmp_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cps_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cps_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/dsb.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/enterx_leavex.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eor_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eor_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eor_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eret.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/isb.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/it.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_exception_return.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_user_registers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldmda.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldmdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldmib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_register_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_register_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrbt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrd_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrd_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrd_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrex.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrexb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrexd.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrexh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrht.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsb_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsb_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsb_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsbt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsh_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsh_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsh_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsht.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrt.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsl_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsl_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsr_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsr_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mcr_mcr2.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mcrr_mcrr2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mla.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mls.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mov_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mov_register_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mov_register_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/movt.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mrc_mrc2.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mrrc_mrrc2.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mrs_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mrs_system.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_system.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_register_application.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_register_system.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mul.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mvn_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mvn_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mvn_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/nop.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orn_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orn_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orr_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orr_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orr_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pkh.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pld_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pld_literal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pld_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pop_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pop_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/push.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qadd.py
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qadd16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qadd8.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qasx.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qdadd.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qdsub.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsax.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsub.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsub16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsub8.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rbit.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rev.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rev16.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/revsh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rfe.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ror_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ror_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rrx.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsb_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsb_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsb_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsc_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsc_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsc_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sadd16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sadd8.py
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sasx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbc_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbc_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbc_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbfx.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sdiv.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sel.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/setend.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sev.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shadd16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shadd8.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shasx.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shsax.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shsub16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shsub8.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smla.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlald.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlalxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlaw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlsd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlsld.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smmla.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smmls.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smmul.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smuad.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smul.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smull.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smulw.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smusd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/srs_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/srs_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssat.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssat16.py
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssax.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssub16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssub8.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stc_stc2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stm_user_registers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stmda.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stmdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stmib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/str_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/str_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/str_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strb_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strbt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strd_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strd_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strex.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strexb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strexd.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strexh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strh_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strht.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strt.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_thumb.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/svc.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtab.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtab16.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtah.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtb.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtb16.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tbb_tbh.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/teq_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/teq_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/teq_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tst_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tst_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tst_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uadd16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uadd8.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uasx.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ubfx.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/udf.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/udiv.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhadd16.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhadd8.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhasx.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhsax.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhsub16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhsub8.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/umaal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/umlal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/umull.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqadd16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqadd8.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqasx.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqsax.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqsub16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqsub8.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usad8.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usada8.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usat.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usat16.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usax.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usub16.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usub8.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtab.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtab16.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtah.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtb.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtb16.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxth.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/wfe.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/wfi.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/yield_.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.388457 armulator-1.1.2/armulator/armv6/opcodes/concrete/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_thumb_t4.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t4.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adr_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adr_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adr_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adr_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/adr_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/and_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/and_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/b_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/b_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/b_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/b_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/b_t4.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bfc_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bfc_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bfi_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bfi_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bkpt_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bkpt_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bl_blx_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bl_blx_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bl_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bl_immediate_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/blx_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/blx_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bxj_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/bxj_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cbz_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cdp_cdp2_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cdp_cdp2_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cdp_cdp2_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cdp_cdp2_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/clrex_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/clrex_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/clz_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/clz_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cps_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cps_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/cps_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/dsb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/dsb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/enterx_leavex_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/eret_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/isb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/isb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/it_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_exception_return_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_user_registers_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmda_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmdb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmdb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmib_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t4.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_literal_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_register_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_register_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_register_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrbt_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrbt_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrbt_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrex_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrex_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrexb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrexb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrexd_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrexd_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrexh_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrexh_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrht_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrht_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrht_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsbt_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsbt_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsbt_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsht_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsht_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsht_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrt_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrt_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrt_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcr_mcr2_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcr_mcr2_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcr_mcr2_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcr_mcr2_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcrr_mcrr2_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcrr_mcrr2_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcrr_mcrr2_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mcrr_mcrr2_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mla_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mla_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mls_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mls_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_register_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_register_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_register_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_register_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/movt_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/movt_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrc_mrc2_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrc_mrc2_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrc_mrc2_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrc_mrc2_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrrc_mrrc2_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrrc_mrrc2_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrs_application_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrs_application_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrs_system_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mrs_system_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_immediate_application_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_immediate_system_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_application_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_application_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_system_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_system_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mul_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mul_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mul_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/nop_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/nop_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/nop_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orn_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orn_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pkh_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pkh_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_literal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_literal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_arm_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/push_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/push_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/push_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/push_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/push_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qadd16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qadd16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qadd8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qadd8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qadd_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qadd_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qasx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qasx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qdadd_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qdadd_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qdsub_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qdsub_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsax_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsax_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsub16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsub16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsub8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsub8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsub_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/qsub_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rbit_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rbit_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rev16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rev16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rev16_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rev_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rev_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rev_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/revsh_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/revsh_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/revsh_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rfe_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rfe_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rfe_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rrx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rrx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsc_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsc_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/rsc_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sadd16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sadd16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sadd8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sadd8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sasx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sasx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbfx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sbfx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sdiv_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sdiv_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sel_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sel_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/setend_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/setend_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sev_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sev_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sev_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shadd16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shadd16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shadd8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shadd8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shasx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shasx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shsax_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shsax_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shsub16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shsub16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shsub8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/shsub8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smc_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smc_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smla_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smla_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlad_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlad_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlald_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlald_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlalxy_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlalxy_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlaw_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlaw_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsd_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsd_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsld_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsld_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smmla_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smmla_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smmls_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smmls_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smmul_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smmul_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smuad_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smuad_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smul_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smul_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smull_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smull_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smulw_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smulw_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smusd_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/smusd_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/srs_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/srs_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/srs_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssat16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssat16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssat_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssat_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssax_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssax_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssub16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssub16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssub8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ssub8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_stc2_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_stc2_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_stc2_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stm_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stm_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stm_user_registers_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stmda_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stmdb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stmdb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/stmib_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_thumb_t4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/str_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strbt_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strbt_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strbt_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strd_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strd_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strd_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strex_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strex_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strexb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strexb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strexd_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strexd_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strexh_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strexh_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strht_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strht_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strht_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strt_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strt_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/strt_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t4.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t3.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a2.py
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/subs_pc_lr_thumb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/svc_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/svc_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtah_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtah_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtb16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtb16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxth_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxth_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/sxth_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/tbb_tbh_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_immediate_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_immediate_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_register_shifted_register_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_register_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_register_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uadd16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uadd16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uadd8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uadd8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uasx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uasx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ubfx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/ubfx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/udf_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/udf_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/udf_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/udiv_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/udiv_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhadd16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhadd16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhadd8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhadd8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhasx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhasx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhsax_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhsax_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhsub16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhsub16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhsub8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uhsub8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/umaal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/umaal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/umlal_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/umlal_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/umull_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/umull_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqadd16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqadd16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqadd8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqadd8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqasx_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqasx_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqsax_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqsax_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqsub16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqsub16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqsub8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uqsub8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usad8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usad8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usada8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usada8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usat16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usat16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usat_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usat_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usax_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usax_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usub16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usub16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usub8_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/usub8_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtah_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtah_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtb16_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtb16_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtb_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtb_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtb_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxth_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxth_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/uxth_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/wfe_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/wfe_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/wfe_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/wfi_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/wfi_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/wfi_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/yield_a1.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/yield_t1.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/concrete/yield_t2.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decode_instruction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.392457 armulator-1.1.2/armulator/armv6/opcodes/decoders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_branch_branch_with_link_and_block_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_coprocessor_instructions_and_supervisor_call.py
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_and_miscellaneous_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5970 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_register_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     4141 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions_unprivileged.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_halfword_multiply_and_multiply_accumulate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_instruction_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_load_store_word_and_unsigned_byte.py
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_media_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_memory_hints_advanced_simd_instructions_and_miscellaneous_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_miscellaneous_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_msr_immediate_and_hints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_multiply_and_multiply_accumulate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_packing_unpacking_saturation_and_reversal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_signed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_unsigned.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_saturating_addition_and_subtraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_signed_multiply_signed_and_unsigned_divide.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_synchronization_primitives.py
--rw-r--r--   0 runner    (1001) docker     (121)     3049 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_unconditional_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_branches_and_miscellaneous_control.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_change_processor_state_and_hints.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_conditional_branch_and_supervisor_call.py
--rw-r--r--   0 runner    (1001) docker     (121)     4609 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_coprocessor_advanced_simd_and_floating_point_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_modified_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_plain_binary_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_shifted_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_if_then_and_hints.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_instruction_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_16_bit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5092 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_32_bit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4138 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_byte_memory_hints.py
--rw-r--r--   0 runner    (1001) docker     (121)     3415 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_halfword_memory_hints.py
--rw-r--r--   0 runner    (1001) docker     (121)     2831 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_store_dual_load_store_exclusive_table_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_store_multiple.py
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_store_single_data_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_word.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_long_multiply_long_multiply_accumulate_and_divide.py
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_miscellaneous_16_bit_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_miscellaneous_control_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_miscellaneous_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_move_register_and_immediate_shifts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_multiply_multiply_accumulate_and_absolute_difference.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_signed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_unsigned.py
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_shift_immediate_add_subtract_move_and_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_special_data_instructions_and_branch_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_store_single_data_item.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/opcodes/opcode.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)    31309 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/registers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/shift.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-29 19:23:42.000000 armulator-1.1.2/armulator/armv6/tlb_record.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 19:23:51.280456 armulator-1.1.2/armulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-05-29 19:23:51.000000 armulator-1.1.2/armulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    51317 2022-05-29 19:23:51.000000 armulator-1.1.2/armulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 19:23:51.000000 armulator-1.1.2/armulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-29 19:23:51.000000 armulator-1.1.2/armulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 19:23:51.392457 armulator-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-05-29 19:23:42.000000 armulator-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.502286 armulator-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 04:58:51.000000 armulator-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-08 04:59:00.502286 armulator-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-08 04:58:51.000000 armulator-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.366245 armulator-1.1.3/armulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.366245 armulator-1.1.3/armulator/armv6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/address_descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.370246 armulator-1.1.3/armulator/armv6/all_registers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/abstract_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/cpacr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/cpsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/dacr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/dbgdidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/dfsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/fcseidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/fpexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/hcptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/hcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/hdcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/hpfar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/hsctlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/hsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/hstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/htcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/id_pfr1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/jmcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/midr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/mpuir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/nmrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/nsacr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/pmcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/prrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/racr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/rgnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/rsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/scr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/sctlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/sder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/sunavcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/teecr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/ttbcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/vbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/all_registers/vtcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/arm_configurations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/arm_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89113 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/arm_v6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/bits_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/full_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/memory_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/memory_controller_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/memory_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.370246 armulator-1.1.3/armulator/armv6/opcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.398255 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adc_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adc_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adc_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_register_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_register_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/and_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/and_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/and_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/asr_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/asr_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bic_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bic_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bic_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bkpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bl_blx_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/blx_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bxj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cbz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cdp_cdp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/clrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/clz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmn_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmn_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmn_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmp_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmp_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmp_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cps_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cps_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/dsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/enterx_leavex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eor_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eor_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eor_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/isb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_exception_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_user_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldmda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldmib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_register_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_register_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrd_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrd_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrd_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrexb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrexd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrexh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsb_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsb_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsb_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsh_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsh_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsh_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsl_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsl_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsr_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsr_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mcr_mcr2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mcrr_mcrr2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mov_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mov_register_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mov_register_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/movt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mrc_mrc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mrrc_mrrc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mrs_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mrs_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_register_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_register_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mul.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mvn_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mvn_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mvn_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orn_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orn_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orr_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orr_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orr_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pkh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pld_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pld_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pld_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pop_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pop_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qadd16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qadd8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qdadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qdsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsub16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsub8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rev16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/revsh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ror_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ror_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsb_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsb_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsb_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsc_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsc_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsc_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sadd16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sadd8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbc_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbc_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbc_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sdiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/setend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shadd16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shadd8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shsax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shsub16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shsub8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlald.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlalxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlsld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smmla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smmls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smuad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smulw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smusd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/srs_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/srs_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssat16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssub16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssub8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stc_stc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stm_user_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stmda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stmib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/str_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/str_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/str_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strb_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strd_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strd_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strexb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strexd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strexh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strh_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_thumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtab16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtb16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tbb_tbh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/teq_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/teq_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/teq_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tst_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tst_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tst_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uadd16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uadd8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ubfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/udf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/udiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhadd16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhadd8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhsax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhsub16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhsub8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/umaal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/umlal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/umull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqadd16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqadd8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqsax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqsub16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqsub8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usad8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usada8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usat16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usub16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usub8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtab16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtb16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/wfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/wfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/yield_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.494284 armulator-1.1.3/armulator/armv6/opcodes/concrete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_thumb_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adr_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adr_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adr_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adr_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/adr_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/and_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/and_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/b_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/b_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/b_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/b_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/b_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bfc_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bfc_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bfi_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bfi_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bkpt_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bkpt_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bl_blx_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bl_blx_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bl_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bl_immediate_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/blx_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/blx_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bxj_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/bxj_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cbz_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cdp_cdp2_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cdp_cdp2_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cdp_cdp2_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cdp_cdp2_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/clrex_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/clrex_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/clz_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/clz_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cps_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cps_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/cps_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/dsb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/dsb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/enterx_leavex_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/eret_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/isb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/isb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/it_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_exception_return_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_user_registers_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmda_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmdb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmdb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmib_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_literal_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_register_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_register_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_register_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrbt_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrbt_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrbt_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrex_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrex_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrexb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrexb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrexd_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrexd_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrexh_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrexh_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrht_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrht_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrht_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsbt_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsbt_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsbt_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsht_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsht_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsht_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrt_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrt_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrt_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcr_mcr2_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcr_mcr2_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcr_mcr2_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcr_mcr2_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcrr_mcrr2_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcrr_mcrr2_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcrr_mcrr2_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mcrr_mcrr2_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mla_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mla_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mls_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mls_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_register_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_register_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_register_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_register_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/movt_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/movt_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrc_mrc2_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrc_mrc2_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrc_mrc2_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrc_mrc2_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrrc_mrrc2_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrrc_mrrc2_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrs_application_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrs_application_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrs_system_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mrs_system_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_immediate_application_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_immediate_system_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_application_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_application_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_system_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_system_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mul_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mul_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mul_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/nop_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/nop_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/nop_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orn_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orn_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pkh_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pkh_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_literal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_literal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_arm_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/push_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/push_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/push_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/push_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/push_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qadd16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qadd16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qadd8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qadd8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qadd_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qadd_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qasx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qasx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qdadd_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qdadd_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qdsub_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qdsub_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsax_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsax_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsub16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsub16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsub8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsub8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsub_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/qsub_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rbit_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rbit_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rev16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rev16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rev16_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rev_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rev_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rev_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/revsh_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/revsh_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/revsh_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rfe_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rfe_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rfe_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rrx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rrx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsc_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsc_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/rsc_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sadd16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sadd16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sadd8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sadd8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sasx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sasx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbfx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sbfx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sdiv_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sdiv_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sel_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sel_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/setend_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/setend_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sev_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sev_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sev_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shadd16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shadd16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shadd8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shadd8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shasx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shasx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shsax_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shsax_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shsub16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shsub16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shsub8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/shsub8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smc_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smc_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smla_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smla_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlad_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlad_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlald_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlald_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlalxy_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlalxy_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlaw_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlaw_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsd_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsd_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsld_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsld_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smmla_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smmla_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smmls_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smmls_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smmul_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smmul_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smuad_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smuad_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smul_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smul_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smull_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smull_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smulw_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smulw_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smusd_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/smusd_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/srs_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/srs_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/srs_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssat16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssat16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssat_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssat_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssax_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssax_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssub16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssub16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssub8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ssub8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_stc2_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_stc2_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_stc2_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stm_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stm_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stm_user_registers_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stmda_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stmdb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stmdb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/stmib_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_thumb_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/str_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strbt_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strbt_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strbt_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strd_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strd_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strd_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strex_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strex_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strexb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strexb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strexd_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strexd_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strexh_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strexh_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strht_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strht_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strht_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strt_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strt_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/strt_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/subs_pc_lr_thumb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/svc_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/svc_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtah_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtah_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtb16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtb16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxth_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxth_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/sxth_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/tbb_tbh_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_immediate_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_immediate_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_register_shifted_register_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_register_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_register_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uadd16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uadd16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uadd8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uadd8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uasx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uasx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ubfx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/ubfx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/udf_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/udf_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/udf_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/udiv_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/udiv_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhadd16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhadd16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhadd8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhadd8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhasx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhasx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhsax_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhsax_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhsub16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhsub16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhsub8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uhsub8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/umaal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/umaal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/umlal_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/umlal_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/umull_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/umull_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqadd16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqadd16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqadd8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqadd8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqasx_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqasx_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqsax_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqsax_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqsub16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqsub16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqsub8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uqsub8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usad8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usad8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usada8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usada8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usat16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usat16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usat_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usat_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usax_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usax_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usub16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usub16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usub8_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/usub8_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtah_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtah_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtb16_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtb16_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtb_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtb_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtb_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxth_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxth_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/uxth_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/wfe_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/wfe_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/wfe_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/wfi_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/wfi_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/wfi_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/yield_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/yield_t1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/concrete/yield_t2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decode_instruction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.502286 armulator-1.1.3/armulator/armv6/opcodes/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_branch_branch_with_link_and_block_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_coprocessor_instructions_and_supervisor_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_and_miscellaneous_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_register_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions_unprivileged.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_halfword_multiply_and_multiply_accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_instruction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_load_store_word_and_unsigned_byte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_media_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_memory_hints_advanced_simd_instructions_and_miscellaneous_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_miscellaneous_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_msr_immediate_and_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_multiply_and_multiply_accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_packing_unpacking_saturation_and_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_unsigned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_saturating_addition_and_subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_signed_multiply_signed_and_unsigned_divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_synchronization_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_unconditional_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_branches_and_miscellaneous_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_change_processor_state_and_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_conditional_branch_and_supervisor_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_coprocessor_advanced_simd_and_floating_point_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_modified_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_plain_binary_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_shifted_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_if_then_and_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_instruction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_16_bit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_32_bit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_byte_memory_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_halfword_memory_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_store_dual_load_store_exclusive_table_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_store_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_store_single_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_long_multiply_long_multiply_accumulate_and_divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_miscellaneous_16_bit_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_miscellaneous_control_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_miscellaneous_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_move_register_and_immediate_shifts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_multiply_multiply_accumulate_and_absolute_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_unsigned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_shift_immediate_add_subtract_move_and_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_special_data_instructions_and_branch_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_store_single_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/opcodes/opcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31309 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 04:58:51.000000 armulator-1.1.3/armulator/armv6/tlb_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:59:00.366245 armulator-1.1.3/armulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-08 04:59:00.000000 armulator-1.1.3/armulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    51317 2023-08-08 04:59:00.000000 armulator-1.1.3/armulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 04:59:00.000000 armulator-1.1.3/armulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 04:59:00.000000 armulator-1.1.3/armulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 04:59:00.502286 armulator-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-08 04:58:51.000000 armulator-1.1.3/setup.py
```

### Comparing `armulator-1.1.2/LICENSE` & `armulator-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/PKG-INFO` & `armulator-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: armulator
-Version: 1.1.2
+Version: 1.1.3
 Summary: A pure Python ARM processor emulator
 Home-page: https://github.com/matan1008/armulator
 Author: Matan Perelman
 Author-email: matan1008@gmail.com
 License: MIT
 Keywords: arm emulator
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 
 A pure python ARM emulator
 
@@ -100,9 +100,7 @@
 ```
 
 # Acknowledgments
 
 * At first, I did it to learn the ARM architecture better. I guess I was carried away.
 * Feel free to report bugs.
 * Feel free to ask for more features.
-
-
```

### Comparing `armulator-1.1.2/README.md` & `armulator-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/abstract_register.py` & `armulator-1.1.3/armulator/armv6/all_registers/abstract_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/cpacr.py` & `armulator-1.1.3/armulator/armv6/all_registers/cpacr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/cpsr.py` & `armulator-1.1.3/armulator/armv6/all_registers/cpsr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/dbgdidr.py` & `armulator-1.1.3/armulator/armv6/all_registers/dbgdidr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/dfsr.py` & `armulator-1.1.3/armulator/armv6/all_registers/dfsr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/hcptr.py` & `armulator-1.1.3/armulator/armv6/all_registers/hcptr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/hcr.py` & `armulator-1.1.3/armulator/armv6/all_registers/hcr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/hdcr.py` & `armulator-1.1.3/armulator/armv6/all_registers/hdcr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/hsctlr.py` & `armulator-1.1.3/armulator/armv6/all_registers/hsctlr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/hsr.py` & `armulator-1.1.3/armulator/armv6/all_registers/hsr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/hstr.py` & `armulator-1.1.3/armulator/armv6/all_registers/hstr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/htcr.py` & `armulator-1.1.3/armulator/armv6/all_registers/htcr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/id_pfr1.py` & `armulator-1.1.3/armulator/armv6/all_registers/id_pfr1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/midr.py` & `armulator-1.1.3/armulator/armv6/all_registers/midr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/mpuir.py` & `armulator-1.1.3/armulator/armv6/all_registers/mpuir.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/nmrr.py` & `armulator-1.1.3/armulator/armv6/all_registers/nmrr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/nsacr.py` & `armulator-1.1.3/armulator/armv6/all_registers/nsacr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/pmcr.py` & `armulator-1.1.3/armulator/armv6/all_registers/pmcr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/prrr.py` & `armulator-1.1.3/armulator/armv6/all_registers/prrr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/racr.py` & `armulator-1.1.3/armulator/armv6/all_registers/racr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/rsr.py` & `armulator-1.1.3/armulator/armv6/all_registers/rsr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/scr.py` & `armulator-1.1.3/armulator/armv6/all_registers/scr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/sctlr.py` & `armulator-1.1.3/armulator/armv6/all_registers/sctlr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/ttbcr.py` & `armulator-1.1.3/armulator/armv6/all_registers/ttbcr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/all_registers/vtcr.py` & `armulator-1.1.3/armulator/armv6/all_registers/vtcr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/arm_configurations.json` & `armulator-1.1.3/armulator/armv6/arm_configurations.json`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/arm_exceptions.py` & `armulator-1.1.3/armulator/armv6/arm_exceptions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/arm_v6.py` & `armulator-1.1.3/armulator/armv6/arm_v6.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,32 +33,37 @@
         self.is_wait_for_event = False
         self.is_wait_for_interrupt = False
         self.executed_opcode = None
 
     def start(self):
         self.take_reset()
 
+    def format_registers(self):
+        return (
+            f"R0: 0x{self.registers.get(0):08X}\n"
+            f"R1: 0x{self.registers.get(1):08X}\n"
+            f"R2: 0x{self.registers.get(2):08X}\n"
+            f"R3: 0x{self.registers.get(3):08X}\n"
+            f"R4: 0x{self.registers.get(4):08X}\n"
+            f"R5: 0x{self.registers.get(5):08X}\n"
+            f"R6: 0x{self.registers.get(6):08X}\n"
+            f"R7: 0x{self.registers.get(7):08X}\n"
+            f"R8: 0x{self.registers.get(8):08X}\n"
+            f"R9: 0x{self.registers.get(9):08X}\n"
+            f"R10: 0x{self.registers.get(10):08X}\n"
+            f"R11: 0x{self.registers.get(11):08X}\n"
+            f"R12: 0x{self.registers.get(12):08X}\n"
+            f"SP: 0x{self.registers.get_sp():08X}\n"
+            f"LR: 0x{self.registers.get_lr():08X}\n"
+            f"PC: 0x{self.registers.pc_store_value():08X}\n"
+            f"CPSR: 0x{self.registers.cpsr.value:08X}\n"
+        )
+
     def print_registers(self):
-        print("{0}:{1}".format("R0", self.registers.get(0)))
-        print("{0}:{1}".format("R1", self.registers.get(1)))
-        print("{0}:{1}".format("R2", self.registers.get(2)))
-        print("{0}:{1}".format("R3", self.registers.get(3)))
-        print("{0}:{1}".format("R4", self.registers.get(4)))
-        print("{0}:{1}".format("R5", self.registers.get(5)))
-        print("{0}:{1}".format("R6", self.registers.get(6)))
-        print("{0}:{1}".format("R7", self.registers.get(7)))
-        print("{0}:{1}".format("R8", self.registers.get(8)))
-        print("{0}:{1}".format("R9", self.registers.get(9)))
-        print("{0}:{1}".format("R10", self.registers.get(10)))
-        print("{0}:{1}".format("R11", self.registers.get(11)))
-        print("{0}:{1}".format("R12", self.registers.get(12)))
-        print("{0}:{1}".format("SP", self.registers.get_sp()))
-        print("{0}:{1}".format("LR", self.registers.get_lr()))
-        print("{0}:{1}".format("PC", self.registers.pc_store_value()))
-        print("{0}:{1}".format("CPSR", self.registers.cpsr.value))
+        print(self.format_registers())
 
     def take_reset(self):
         self.registers.cpsr.m = 0b10011
         if have_security_ext():
             self.registers.scr.ns = 0
         self.registers.reset_control_registers()
         if have_adv_simd_or_vfp():
```

### Comparing `armulator-1.1.2/armulator/armv6/bits_ops.py` & `armulator-1.1.3/armulator/armv6/bits_ops.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/configurations.py` & `armulator-1.1.3/armulator/armv6/configurations.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/enums.py` & `armulator-1.1.3/armulator/armv6/enums.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/memory_controller_hub.py` & `armulator-1.1.3/armulator/armv6/memory_controller_hub.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/memory_types.py` & `armulator-1.1.3/armulator/armv6/memory_types.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adc_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adc_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adc_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adc_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adc_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adc_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_register_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_register_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_register_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_register_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/add_sp_plus_register_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/adr.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/adr.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/and_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/and_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/and_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/and_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/and_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/and_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/asr_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/asr_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/asr_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/asr_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bfc.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bfc.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bfi.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bfi.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bic_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bic_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bic_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bic_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bic_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bic_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bl_blx_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bl_blx_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/blx_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/blx_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/bxj.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/bxj.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmn_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmn_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmn_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmn_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmn_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmn_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmp_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmp_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmp_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmp_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cmp_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cmp_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cps_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cps_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/cps_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/cps_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/dsb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/dsb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/enterx_leavex.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/enterx_leavex.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eor_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eor_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eor_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eor_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eor_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eor_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/eret.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/eret.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldc_ldc2_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_exception_return.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_exception_return.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldm_user_registers.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldm_user_registers.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldmda.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldmda.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldmdb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldmdb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldmib.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldmib.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_register_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_register_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldr_register_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldr_register_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrb_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrb_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrbt.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrbt.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrd_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrd_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrd_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrd_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrd_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrd_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrex.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrex.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrexb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrexb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrexd.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrexd.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrexh.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrexh.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrh_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrh_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrht.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrht.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsb_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsb_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsb_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsb_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsb_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsb_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsbt.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsbt.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsh_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsh_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsh_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsh_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsh_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsh_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrsht.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrsht.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ldrt.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ldrt.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsl_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsl_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsl_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsl_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsr_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsr_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/lsr_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/lsr_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mcr_mcr2.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mcr_mcr2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mcrr_mcrr2.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mcrr_mcrr2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mla.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mla.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mls.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mls.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mov_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mov_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mov_register_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mov_register_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mov_register_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mov_register_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mrc_mrc2.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mrc_mrc2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mrrc_mrrc2.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mrrc_mrrc2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mrs_system.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mrs_system.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_application.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_application.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_system.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_immediate_system.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_register_application.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_register_application.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/msr_register_system.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/msr_register_system.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mul.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mul.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mvn_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mvn_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mvn_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mvn_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/mvn_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/mvn_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orn_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orn_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orn_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orn_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orr_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orr_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orr_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orr_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/orr_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/orr_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pkh.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pkh.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pld_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pld_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pld_literal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pld_literal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pld_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pld_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pop_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pop_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/pop_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/pop_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/push.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/push.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qadd.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qadd.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qadd16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qadd16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qadd8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qadd8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qasx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qasx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qdadd.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qdadd.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qdsub.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qdsub.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsax.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsax.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsub.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsub.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsub16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsub16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/qsub8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/qsub8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rbit.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rbit.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rev.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rev.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rev16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rev16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/revsh.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/revsh.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rfe.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rfe.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ror_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ror_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ror_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ror_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rrx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rrx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsb_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsb_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsb_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsb_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsb_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsb_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsc_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsc_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsc_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsc_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/rsc_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/rsc_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sadd16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sadd16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sadd8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sadd8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sasx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sasx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbc_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbc_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbc_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbc_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbc_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbc_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sbfx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sbfx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sdiv.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sdiv.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sel.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sel.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shadd16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shadd16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shadd8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shadd8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shasx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shasx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shsax.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shsax.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shsub16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shsub16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/shsub8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/shsub8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smc.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smc.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smla.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smla.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlad.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlad.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlald.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlald.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlalxy.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlalxy.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlaw.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlaw.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlsd.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlsd.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smlsld.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smlsld.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smmla.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smmla.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smmls.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smmls.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smmul.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smmul.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smuad.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smuad.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smul.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smul.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smull.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smull.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smulw.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smulw.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/smusd.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/smusd.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/srs_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/srs_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/srs_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/srs_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssat.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssat.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssat16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssat16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssax.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssax.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssub16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssub16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ssub8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ssub8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stc_stc2.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stc_stc2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stm_user_registers.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stm_user_registers.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stmda.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stmda.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stmdb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stmdb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/stmib.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/stmib.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/str_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/str_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/str_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/str_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/str_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/str_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strb_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strb_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strb_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strbt.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strbt.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strd_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strd_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strd_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strd_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strex.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strex.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strexb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strexb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strexd.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strexd.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strexh.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strexh.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strh_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strh_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strh_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strht.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strht.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/strt.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/strt.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_immediate_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sub_sp_minus_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_arm.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_arm.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_thumb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/subs_pc_lr_thumb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtab.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtab.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtab16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtab16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtah.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtah.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxtb16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxtb16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/sxth.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/sxth.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tbb_tbh.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tbb_tbh.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/teq_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/teq_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/teq_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/teq_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/teq_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/teq_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tst_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tst_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tst_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tst_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/tst_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/tst_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uadd16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uadd16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uadd8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uadd8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uasx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uasx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/ubfx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/ubfx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/udiv.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/udiv.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhadd16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhadd16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhadd8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhadd8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhasx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhasx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhsax.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhsax.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhsub16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhsub16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uhsub8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uhsub8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/umaal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/umaal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/umlal.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/umlal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/umull.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/umull.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqadd16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqadd16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqadd8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqadd8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqasx.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqasx.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqsax.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqsax.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqsub16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqsub16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uqsub8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uqsub8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usad8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usad8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usada8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usada8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usat.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usat.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usat16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usat16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usax.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usax.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usub16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usub16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/usub8.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/usub8.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtab.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtab.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtab16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtab16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtah.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtah.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtb.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtb.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxtb16.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxtb16.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/uxth.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/uxth.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/wfe.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/wfe.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/abstract_opcodes/wfi.py` & `armulator-1.1.3/armulator/armv6/opcodes/abstract_opcodes/wfi.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adc_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adc_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_immediate_thumb_t4.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_immediate_thumb_t4.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_register_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_register_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t4.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_immediate_t4.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/add_sp_plus_register_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adr_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adr_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/adr_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/adr_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/and_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/and_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/and_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/and_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/and_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/and_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/asr_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/asr_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/b_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/b_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/b_t4.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/b_t4.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bfc_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bfc_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bfi_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bfi_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bic_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bic_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bl_blx_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bl_blx_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bl_blx_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bl_blx_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/bl_immediate_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/bl_immediate_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmn_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmn_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cmp_register_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cmp_register_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cps_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cps_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cps_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cps_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/cps_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/cps_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/eor_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/eor_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_ldc2_literal_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldc_literal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldc_literal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_exception_return_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_exception_return_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldm_user_registers_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldm_user_registers_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmda_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmda_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmdb_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmdb_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmdb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmdb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldmib_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldmib_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t4.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_immediate_thumb_t4.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_literal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_literal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_literal_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_literal_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_register_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_register_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_register_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_register_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldr_register_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldr_register_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from armulator.armv6.bits_ops import substring
-from armulator.armv6.opcodes.abstract_opcodes.ldrb_immediate_thumb import LdrbImmediateThumb
+from armulator.armv6.opcodes.abstract_opcodes.ldrh_immediate_thumb import LdrhImmediateThumb
 
 
-class LdrbImmediateThumbT1(LdrbImmediateThumb):
+class LdrhImmediateThumbT1(LdrhImmediateThumb):
     @staticmethod
     def from_bitarray(instr, processor):
         rt = substring(instr, 2, 0)
         rn = substring(instr, 5, 3)
         imm5 = substring(instr, 10, 6)
         index = True
         add = True
         wback = False
-        imm32 = imm5 << 2
-        return LdrbImmediateThumbT1(instr, add=add, wback=wback, index=index, t=rt, n=rn, imm32=imm32)
+        imm32 = imm5 << 1
+        return LdrhImmediateThumbT1(instr, add=add, wback=wback, index=index, t=rt, n=rn, imm32=imm32)
```

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_literal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_literal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrb_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrbt_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrbt_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrbt_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrbt_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrbt_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrbt_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_literal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_literal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_literal_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_literal_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrd_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrd_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrb_immediate_thumb_t1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from armulator.armv6.bits_ops import substring
-from armulator.armv6.opcodes.abstract_opcodes.ldrh_immediate_thumb import LdrhImmediateThumb
+from armulator.armv6.opcodes.abstract_opcodes.ldrb_immediate_thumb import LdrbImmediateThumb
 
 
-class LdrhImmediateThumbT1(LdrhImmediateThumb):
+class LdrbImmediateThumbT1(LdrbImmediateThumb):
     @staticmethod
     def from_bitarray(instr, processor):
         rt = substring(instr, 2, 0)
         rn = substring(instr, 5, 3)
         imm5 = substring(instr, 10, 6)
         index = True
         add = True
         wback = False
-        imm32 = imm5 << 2
-        return LdrhImmediateThumbT1(instr, add=add, wback=wback, index=index, t=rt, n=rn, imm32=imm32)
+        return LdrbImmediateThumbT1(instr, add=add, wback=wback, index=index, t=rt, n=rn, imm32=imm5)
```

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_literal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_literal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrh_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrh_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrht_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrht_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrht_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrht_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrht_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrht_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_literal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_literal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsb_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsb_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsbt_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsbt_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsbt_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsbt_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsbt_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsbt_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_literal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_literal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsh_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsh_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsht_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsht_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsht_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsht_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrsht_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrsht_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrt_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrt_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrt_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrt_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ldrt_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ldrt_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsl_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsl_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/lsr_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/lsr_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mcr_mcr2_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mcr_mcr2_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mcr_mcr2_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mcr_mcr2_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mcrr_mcrr2_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mcrr_mcrr2_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mcrr_mcrr2_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mcrr_mcrr2_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mla_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mla_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mla_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mla_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mls_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mls_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_immediate_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_immediate_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_register_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_register_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mov_register_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mov_register_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/movt_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/movt_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mrc_mrc2_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mrc_mrc2_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mrc_mrc2_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mrc_mrc2_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mrrc_mrrc2_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mrrc_mrrc2_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mrrc_mrrc2_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_immediate_application_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_immediate_application_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_immediate_system_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_immediate_system_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_application_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_application_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_application_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_application_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_system_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_system_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/msr_register_system_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/msr_register_system_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mul_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mul_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mul_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mul_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/mvn_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/mvn_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orn_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orn_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orn_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orn_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/orr_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/orr_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pkh_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pkh_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pkh_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pkh_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pld_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pld_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/pop_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/pop_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/push_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/push_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/push_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/push_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rfe_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rfe_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rfe_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rfe_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rfe_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rfe_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ror_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ror_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsb_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsb_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsc_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsc_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsc_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsc_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/rsc_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/rsc_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sbc_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sbc_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sbfx_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sbfx_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smla_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smla_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smla_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smla_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlad_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlad_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlad_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlad_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlal_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlal_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlald_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlald_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlald_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlald_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlalxy_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlalxy_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlalxy_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlalxy_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlaw_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlaw_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlaw_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlaw_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsd_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsd_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsd_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsd_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsld_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsld_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smlsld_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smlsld_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smmla_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smmla_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smmla_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smmla_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smmls_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smmls_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smmls_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smmls_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smmul_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smmul_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smuad_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smuad_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smul_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smul_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smul_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smul_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smull_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smull_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smull_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smull_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smulw_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smulw_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/smusd_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/smusd_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ssat16_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ssat16_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ssat_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ssat_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ssat_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ssat_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_stc2_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_stc2_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_stc2_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_stc2_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stc_stc2_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stc_stc2_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stm_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stm_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stm_user_registers_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stm_user_registers_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stmda_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stmda_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stmdb_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stmdb_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stmdb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stmdb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/stmib_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/stmib_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/str_immediate_thumb_t4.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/str_immediate_thumb_t4.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/str_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/str_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/str_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/str_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/str_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/str_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t1.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     def from_bitarray(instr, processor):
         rt = substring(instr, 2, 0)
         rn = substring(instr, 5, 3)
         imm5 = substring(instr, 10, 6)
         index = True
         add = True
         wback = False
-        imm32 = imm5 * 4
+        imm32 = imm5
         return StrbImmediateThumbT1(instr, add=add, wback=wback, index=index, t=rt, n=rn, imm32=imm32)
```

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strb_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strb_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strbt_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strbt_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strbt_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strbt_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strbt_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strbt_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strd_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strd_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strd_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strd_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strd_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strd_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strex_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strex_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strexd_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strexd_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strexd_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strexd_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     def from_bitarray(instr, processor):
         rt = substring(instr, 2, 0)
         rn = substring(instr, 5, 3)
         imm5 = substring(instr, 10, 6)
         index = True
         add = True
         wback = False
-        imm32 = imm5 << 2
+        imm32 = imm5 << 1
         return StrhImmediateThumbT1(instr, add=add, wback=wback, index=index, t=rt, n=rn, imm32=imm32)
```

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strh_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strh_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strht_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strht_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strht_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strht_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strht_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strht_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strt_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strt_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strt_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strt_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/strt_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/strt_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t4.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_immediate_thumb_t4.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t3.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_immediate_t3.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sub_sp_minus_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sub_sp_minus_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/subs_pc_lr_arm_a2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/subs_pc_lr_thumb_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/subs_pc_lr_thumb_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab16_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab16_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab16_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab16_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtab_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtab_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtah_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtah_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/sxtah_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/sxtah_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/tbb_tbh_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/tbb_tbh_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/teq_register_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/teq_register_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_immediate_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_immediate_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_register_shifted_register_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_register_shifted_register_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/tst_register_t2.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/tst_register_t2.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/ubfx_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/ubfx_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/umaal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/umaal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/umaal_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/umaal_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/umlal_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/umlal_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/umlal_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/umlal_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/umull_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/umull_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/umull_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/umull_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/usada8_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/usada8_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/usat_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/usat_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/usat_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/usat_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab16_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab16_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab16_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab16_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtab_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtab_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtah_a1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtah_a1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/concrete/uxtah_t1.py` & `armulator-1.1.3/armulator/armv6/opcodes/concrete/uxtah_t1.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decode_instruction.py` & `armulator-1.1.3/armulator/armv6/opcodes/decode_instruction.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_branch_branch_with_link_and_block_data_transfer.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_branch_branch_with_link_and_block_data_transfer.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_coprocessor_instructions_and_supervisor_call.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_coprocessor_instructions_and_supervisor_call.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_and_miscellaneous_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_and_miscellaneous_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_data_processing_register_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_data_processing_register_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions_unprivileged.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_extra_load_store_instructions_unprivileged.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_halfword_multiply_and_multiply_accumulate.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_halfword_multiply_and_multiply_accumulate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_instruction_set.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_instruction_set.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_load_store_word_and_unsigned_byte.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_load_store_word_and_unsigned_byte.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_media_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_media_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_memory_hints_advanced_simd_instructions_and_miscellaneous_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_memory_hints_advanced_simd_instructions_and_miscellaneous_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_miscellaneous_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_miscellaneous_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_msr_immediate_and_hints.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_msr_immediate_and_hints.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_multiply_and_multiply_accumulate.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_multiply_and_multiply_accumulate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_packing_unpacking_saturation_and_reversal.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_packing_unpacking_saturation_and_reversal.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_signed.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_signed.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_unsigned.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_parallel_addition_and_subtraction_unsigned.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_saturating_addition_and_subtraction.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_saturating_addition_and_subtraction.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_signed_multiply_signed_and_unsigned_divide.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_signed_multiply_signed_and_unsigned_divide.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_synchronization_primitives.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_synchronization_primitives.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/arm_unconditional_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/arm_unconditional_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_branches_and_miscellaneous_control.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_branches_and_miscellaneous_control.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_change_processor_state_and_hints.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_change_processor_state_and_hints.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_conditional_branch_and_supervisor_call.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_conditional_branch_and_supervisor_call.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_coprocessor_advanced_simd_and_floating_point_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_coprocessor_advanced_simd_and_floating_point_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_modified_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_modified_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_plain_binary_immediate.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_plain_binary_immediate.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_data_processing_shifted_register.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_data_processing_shifted_register.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_if_then_and_hints.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_if_then_and_hints.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_instruction_set.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_instruction_set.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_16_bit.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_16_bit.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_32_bit.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_instruction_set_encoding_32_bit.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_byte_memory_hints.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_byte_memory_hints.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_halfword_memory_hints.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_halfword_memory_hints.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_store_dual_load_store_exclusive_table_branch.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_store_dual_load_store_exclusive_table_branch.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_store_multiple.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_store_multiple.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_store_single_data_item.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_store_single_data_item.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_load_word.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_load_word.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_long_multiply_long_multiply_accumulate_and_divide.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_long_multiply_long_multiply_accumulate_and_divide.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_miscellaneous_16_bit_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_miscellaneous_16_bit_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_miscellaneous_control_instructions.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_miscellaneous_control_instructions.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_miscellaneous_operations.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_miscellaneous_operations.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_move_register_and_immediate_shifts.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_move_register_and_immediate_shifts.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_multiply_multiply_accumulate_and_absolute_difference.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_multiply_multiply_accumulate_and_absolute_difference.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_signed.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_signed.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_unsigned.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_parallel_addition_and_subtraction_unsigned.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_shift_immediate_add_subtract_move_and_compare.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_shift_immediate_add_subtract_move_and_compare.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_special_data_instructions_and_branch_and_exchange.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_special_data_instructions_and_branch_and_exchange.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/opcodes/decoders/thumb_store_single_data_item.py` & `armulator-1.1.3/armulator/armv6/opcodes/decoders/thumb_store_single_data_item.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/registers.py` & `armulator-1.1.3/armulator/armv6/registers.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/shift.py` & `armulator-1.1.3/armulator/armv6/shift.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator/armv6/tlb_record.py` & `armulator-1.1.3/armulator/armv6/tlb_record.py`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/armulator.egg-info/PKG-INFO` & `armulator-1.1.3/armulator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: armulator
-Version: 1.1.2
+Version: 1.1.3
 Summary: A pure Python ARM processor emulator
 Home-page: https://github.com/matan1008/armulator
 Author: Matan Perelman
 Author-email: matan1008@gmail.com
 License: MIT
 Keywords: arm emulator
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 
 A pure python ARM emulator
 
@@ -100,9 +100,7 @@
 ```
 
 # Acknowledgments
 
 * At first, I did it to learn the ARM architecture better. I guess I was carried away.
 * Feel free to report bugs.
 * Feel free to ask for more features.
-
-
```

### Comparing `armulator-1.1.2/armulator.egg-info/SOURCES.txt` & `armulator-1.1.3/armulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `armulator-1.1.2/setup.py` & `armulator-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 BASE_DIR = Path(__file__).parent.resolve(strict=True)
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 PACKAGES = [p for p in find_packages() if not p.startswith('tests')]
 
 
 def get_description():
     return (BASE_DIR / 'README.md').read_text()
 
 
@@ -23,14 +23,15 @@
         author_email='matan1008@gmail.com',
         classifiers=[
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
         ],
         keywords='arm emulator',
         packages=PACKAGES,
         license='MIT',
         package_data={
             'armulator': ['armv6/arm_configurations.json'],
         },
```

