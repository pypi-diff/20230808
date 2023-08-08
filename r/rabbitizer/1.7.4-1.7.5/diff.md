# Comparing `tmp/rabbitizer-1.7.4.tar.gz` & `tmp/rabbitizer-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.7.4.tar", last modified: Tue Jun 13 18:40:57 2023, max compression
+gzip compressed data, was "rabbitizer-1.7.5.tar", last modified: Tue Aug  8 16:47:20 2023, max compression
```

## Comparing `rabbitizer-1.7.4.tar` & `rabbitizer-1.7.5.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.198539 rabbitizer-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-13 18:40:57.198539 rabbitizer-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.158539 rabbitizer-1.7.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.162539 rabbitizer-1.7.4/docs/r3000gte/
--rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/docs/r3000gte/gte_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    72630 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/docs/r3000gte/gte_macros_volatile.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.162539 rabbitizer-1.7.4/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.162539 rabbitizer-1.7.4/include/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/analysis/RabbitizerLoPairingInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/analysis/RabbitizerRegistersTracker.h
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/analysis/RabbitizerTrackedRegisterState.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.166539 rabbitizer-1.7.4/include/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/common/RabbitizerConfig.h
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/common/RabbitizerVersion.h
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/common/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.166539 rabbitizer-1.7.4/include/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/Abi_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/AccessType_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrCategory_Names_array.h
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrCategory_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)   113991 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrDescriptor_Descriptors_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrIdType_Names_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrIdType_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)    35665 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrId_Names_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrId_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/InstrSuffix_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/OperandType_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/OperandType_function_declarations.h
--rw-r--r--   0 runner    (1001) docker     (123)    23522 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/RegisterDescriptor_Descriptors_arrays.h
--rw-r--r--   0 runner    (1001) docker     (123)    29398 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/Registers_Names_arrays.h
--rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/Registers_enums.h
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/generated/instrOpercandCallbacks_array.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.170539 rabbitizer-1.7.4/include/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerAccessType.h
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstrCategory.h
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstrDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstrId.h
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstrIdType.h
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstrSuffix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstruction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstructionR3000GTE.h
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstructionR5900.h
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerInstructionRsp.h
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerOperandType.h
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerRegister.h
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/instructions/RabbitizerRegisterDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/include/rabbitizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.174539 rabbitizer-1.7.4/rabbitizer/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/Abi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/AccessType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/Config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/Enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/InstrCategory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/InstrId.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/InstrIdType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/LoPairingInfo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/OperandType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/RegCop1N32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/RegCop1N64.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/RegCop1O32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/RegGprN32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/RegGprO32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/RegistersTracker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/TrackedRegisterState.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/Utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.178539 rabbitizer-1.7.4/rabbitizer/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/enums_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/enums_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_Abi.c
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_AccessType.c
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_InstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_InstrIdType.c
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_type_Enum.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.178539 rabbitizer-1.7.4/rabbitizer/enums/registers/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_global_config.c
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_module.h
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_submodule_Utils.c
--rw-r--r--   0 runner    (1001) docker     (123)    22974 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_type_Instruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_type_LoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_type_RegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/rabbitizer/rabbitizer_type_TrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.174539 rabbitizer-1.7.4/rabbitizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-13 18:40:57.000000 rabbitizer-1.7.4/rabbitizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-06-13 18:40:57.000000 rabbitizer-1.7.4/rabbitizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:40:57.000000 rabbitizer-1.7.4/rabbitizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 18:40:57.000000 rabbitizer-1.7.4/rabbitizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:40:57.198539 rabbitizer-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.158539 rabbitizer-1.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.178539 rabbitizer-1.7.4/src/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/analysis/RabbitizerLoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/analysis/RabbitizerRegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/analysis/RabbitizerTrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.178539 rabbitizer-1.7.4/src/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/common/RabbitizerConfig.c
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/common/RabbitizerVersion.c
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/common/Utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.178539 rabbitizer-1.7.4/src/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstrDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstrIdType.c
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstrSuffix.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.178539 rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
--rw-r--r--   0 runner    (1001) docker     (123)    17798 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.182539 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionCpu/
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.182539 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR3000GTE/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.182539 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR5900/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.182539 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionRsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerRegister.c
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/src/instructions/RabbitizerRegisterDescriptor.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.182539 rabbitizer-1.7.4/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.182539 rabbitizer-1.7.4/tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/Abi.inc
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/AccessType.inc
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/InstrCategory.inc
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/InstrIdType.inc
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/InstrIds.inc
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/InstrSuffix.inc
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/OperandTypes.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.186539 rabbitizer-1.7.4/tables/tables/instr_id/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.186539 rabbitizer-1.7.4/tables/tables/instr_id/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1.inc
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.186539 rabbitizer-1.7.4/tables/tables/instr_id/r3000gte/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.190539 rabbitizer-1.7.4/tables/tables/instr_id/r5900/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2_special1.inc
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2_special2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_3.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.190539 rabbitizer-1.7.4/tables/tables/instr_id/rsp/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_cop2_vu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_normal_swc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.190539 rabbitizer-1.7.4/tables/tables/instr_id_types/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id_types/InstrIdType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id_types/InstrIdType_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id_types/InstrIdType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/instr_id_types/InstrIdType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.190539 rabbitizer-1.7.4/tables/tables/operands/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/operands/RabbitizerOperandType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/operands/RabbitizerOperandType_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/operands/RabbitizerOperandType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/operands/RabbitizerOperandType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.194539 rabbitizer-1.7.4/tables/tables/registers/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1N32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1N64.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1O32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_GprN32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_GprO32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_R5900VF.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_R5900VI.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspCop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspCop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspGpr.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspVector.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.162539 rabbitizer-1.7.4/tables/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.194539 rabbitizer-1.7.4/tables/templates/c/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/Abi_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/AccessType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrCategory_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrCategory_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrDescriptor_Descriptors_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrIdType_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrIdType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrId_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrId_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/InstrSuffix_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/OperandType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/OperandType_function_declarations.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/Registers_Names_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/Registers_enums.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/c/instrOpercandCallbacks_array.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.198539 rabbitizer-1.7.4/tables/templates/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/cplusplus/AccessType_enum_class.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/cplusplus/InstrIdType_enum_class.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/cplusplus/OperandType_enum_class.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/cplusplus/Registers_enum_classes.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/cplusplus/UniqueId_enum_class.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.198539 rabbitizer-1.7.4/tables/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/Abi.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/AccessType.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/InstrCategory.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/InstrId.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/InstrIdType.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/OperandType.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/RegCop1N32.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/RegCop1N64.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/RegCop1O32.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/RegGprN32.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/python/RegGprO32.tablepyi.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.198539 rabbitizer-1.7.4/tables/templates/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/abi_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/access_type_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/instr_category_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/instr_id_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/instr_id_type_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/instr_suffix_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/operand_type_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/templates/rust/registers_enum.tablers.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:40:57.198539 rabbitizer-1.7.4/tables/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tools/c_table_gen.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tools/pyi_table_gen.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-13 18:40:47.000000 rabbitizer-1.7.4/tables/tools/rs_table_gen.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.728424 rabbitizer-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-08-08 16:47:20.728424 rabbitizer-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.688423 rabbitizer-1.7.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.692424 rabbitizer-1.7.5/docs/r3000gte/
+-rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/docs/r3000gte/gte_macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    72630 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/docs/r3000gte/gte_macros_volatile.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.692424 rabbitizer-1.7.5/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.692424 rabbitizer-1.7.5/include/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/analysis/RabbitizerLoPairingInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/analysis/RabbitizerRegistersTracker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/analysis/RabbitizerTrackedRegisterState.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.692424 rabbitizer-1.7.5/include/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/common/RabbitizerConfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/common/RabbitizerVersion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/common/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.696424 rabbitizer-1.7.5/include/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/Abi_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/AccessType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrCategory_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrCategory_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)   113991 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrDescriptor_Descriptors_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrIdType_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrIdType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35665 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrId_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrId_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/InstrSuffix_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/OperandType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/OperandType_function_declarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23522 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/RegisterDescriptor_Descriptors_arrays.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29398 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/Registers_Names_arrays.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/Registers_enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/generated/instrOpercandCallbacks_array.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.696424 rabbitizer-1.7.5/include/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerAccessType.h
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstrCategory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstrDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstrId.h
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstrIdType.h
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstrSuffix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstruction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstructionR3000GTE.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstructionR5900.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerInstructionRsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerOperandType.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerRegister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/instructions/RabbitizerRegisterDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/include/rabbitizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.700424 rabbitizer-1.7.5/rabbitizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/Abi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/AccessType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/Config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/Enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/InstrCategory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/InstrId.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/InstrIdType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/LoPairingInfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/OperandType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/RegCop1N32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/RegCop1N64.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/RegCop1O32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/RegGprN32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/RegGprO32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/RegistersTracker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/TrackedRegisterState.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/Utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.700424 rabbitizer-1.7.5/rabbitizer/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/enums_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/enums_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_Abi.c
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_AccessType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_InstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_InstrIdType.c
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_type_Enum.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.704424 rabbitizer-1.7.5/rabbitizer/enums/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_global_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_module.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_submodule_Utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24126 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_type_Instruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_type_LoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_type_RegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/rabbitizer/rabbitizer_type_TrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.700424 rabbitizer-1.7.5/rabbitizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-08-08 16:47:20.000000 rabbitizer-1.7.5/rabbitizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-08-08 16:47:20.000000 rabbitizer-1.7.5/rabbitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:47:20.000000 rabbitizer-1.7.5/rabbitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 16:47:20.000000 rabbitizer-1.7.5/rabbitizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:47:20.728424 rabbitizer-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.692424 rabbitizer-1.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.704424 rabbitizer-1.7.5/src/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/analysis/RabbitizerLoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/analysis/RabbitizerRegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/analysis/RabbitizerTrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.704424 rabbitizer-1.7.5/src/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/common/RabbitizerConfig.c
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/common/RabbitizerVersion.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/common/Utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.704424 rabbitizer-1.7.5/src/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstrDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstrIdType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstrSuffix.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.708424 rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17798 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.708424 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionCpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.708424 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR3000GTE/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.708424 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR5900/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.708424 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionRsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerRegister.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/src/instructions/RabbitizerRegisterDescriptor.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.708424 rabbitizer-1.7.5/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.708424 rabbitizer-1.7.5/tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/Abi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/AccessType.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/InstrCategory.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/InstrIdType.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/InstrIds.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/InstrSuffix.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/OperandTypes.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.712424 rabbitizer-1.7.5/tables/tables/instr_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.712424 rabbitizer-1.7.5/tables/tables/instr_id/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.712424 rabbitizer-1.7.5/tables/tables/instr_id/r3000gte/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.716424 rabbitizer-1.7.5/tables/tables/instr_id/r5900/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2_special1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2_special2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_3.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.716424 rabbitizer-1.7.5/tables/tables/instr_id/rsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_cop2_vu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_normal_swc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.716424 rabbitizer-1.7.5/tables/tables/instr_id_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id_types/InstrIdType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id_types/InstrIdType_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id_types/InstrIdType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/instr_id_types/InstrIdType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.720424 rabbitizer-1.7.5/tables/tables/operands/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/operands/RabbitizerOperandType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/operands/RabbitizerOperandType_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/operands/RabbitizerOperandType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/operands/RabbitizerOperandType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.720424 rabbitizer-1.7.5/tables/tables/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1N32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1N64.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1O32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_GprN32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_GprO32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_R5900VF.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_R5900VI.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspCop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspCop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspGpr.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspVector.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.692424 rabbitizer-1.7.5/tables/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.724424 rabbitizer-1.7.5/tables/templates/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/Abi_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/AccessType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrCategory_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrCategory_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrDescriptor_Descriptors_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrIdType_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrIdType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrId_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrId_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/InstrSuffix_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/OperandType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/OperandType_function_declarations.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/Registers_Names_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/Registers_enums.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/c/instrOpercandCallbacks_array.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.724424 rabbitizer-1.7.5/tables/templates/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/cplusplus/AccessType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/cplusplus/InstrIdType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/cplusplus/OperandType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/cplusplus/Registers_enum_classes.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/cplusplus/UniqueId_enum_class.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.728424 rabbitizer-1.7.5/tables/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/Abi.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/AccessType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/InstrCategory.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/InstrId.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/InstrIdType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/OperandType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/RegCop1N32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/RegCop1N64.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/RegCop1O32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/RegGprN32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/python/RegGprO32.tablepyi.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.728424 rabbitizer-1.7.5/tables/templates/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/abi_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/access_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/instr_category_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/instr_id_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/instr_id_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/instr_suffix_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/operand_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/templates/rust/registers_enum.tablers.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:47:20.728424 rabbitizer-1.7.5/tables/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tools/c_table_gen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tools/pyi_table_gen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-08-08 16:47:12.000000 rabbitizer-1.7.5/tables/tools/rs_table_gen.sh
```

### Comparing `rabbitizer-1.7.4/LICENSE` & `rabbitizer-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/PKG-INFO` & `rabbitizer-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.7.4
+Version: 1.7.5
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.7.4/README.md` & `rabbitizer-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/docs/r3000gte/gte_macros.h` & `rabbitizer-1.7.5/docs/r3000gte/gte_macros.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/docs/r3000gte/gte_macros_volatile.h` & `rabbitizer-1.7.5/docs/r3000gte/gte_macros_volatile.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/analysis/RabbitizerLoPairingInfo.h` & `rabbitizer-1.7.5/include/analysis/RabbitizerLoPairingInfo.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/analysis/RabbitizerRegistersTracker.h` & `rabbitizer-1.7.5/include/analysis/RabbitizerRegistersTracker.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/analysis/RabbitizerTrackedRegisterState.h` & `rabbitizer-1.7.5/include/analysis/RabbitizerTrackedRegisterState.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/common/RabbitizerConfig.h` & `rabbitizer-1.7.5/include/common/RabbitizerConfig.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/common/RabbitizerVersion.h` & `rabbitizer-1.7.5/include/common/RabbitizerVersion.h`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 extern "C" {
 #endif
 
 
 // Header version
 #define RAB_VERSION_MAJOR 1
 #define RAB_VERSION_MINOR 7
-#define RAB_VERSION_PATCH 4
+#define RAB_VERSION_PATCH 5
 
 #define RAB_VERSION_STR RAB_STRINGIFY(RAB_VERSION_MAJOR) "." RAB_STRINGIFY(RAB_VERSION_MINOR) "." RAB_STRINGIFY(RAB_VERSION_PATCH)
 
 // Compiled library version
 extern const int RabVersion_Major;
 extern const int RabVersion_Minor;
 extern const int RabVersion_Patch;
```

### Comparing `rabbitizer-1.7.4/include/common/Utils.h` & `rabbitizer-1.7.5/include/common/Utils.h`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 #else
 #  define UNREACHABLE
 #endif
 
 
 #define ARRAY_COUNT(arr) (sizeof(arr) / sizeof((arr)[0]))
 
+#define RAB_MAX(a, b)    ((a) > (b) ? (a) : (b))
+#define RAB_MIN(a, b)    ((a) < (b) ? (a) : (b))
+
 #define RAB_STRINGIFY2(x) #x
 #define RAB_STRINGIFY(x) RAB_STRINGIFY2(x)
 
 #define MASK(v, w) ((v) & ((1 << (w)) - 1))
 
 /*
  * the SHIFT macros take a value, a shift amount, and a width.
```

### Comparing `rabbitizer-1.7.4/include/generated/InstrDescriptor_Descriptors_array.h` & `rabbitizer-1.7.5/include/generated/InstrDescriptor_Descriptors_array.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/InstrIdType_Names_array.h` & `rabbitizer-1.7.5/include/generated/InstrIdType_Names_array.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/InstrIdType_enum.h` & `rabbitizer-1.7.5/include/generated/InstrIdType_enum.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/InstrId_Names_array.h` & `rabbitizer-1.7.5/include/generated/InstrId_Names_array.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/InstrId_enum.h` & `rabbitizer-1.7.5/include/generated/InstrId_enum.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/OperandType_enum.h` & `rabbitizer-1.7.5/include/generated/OperandType_enum.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/OperandType_function_declarations.h` & `rabbitizer-1.7.5/include/generated/OperandType_function_declarations.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/RegisterDescriptor_Descriptors_arrays.h` & `rabbitizer-1.7.5/include/generated/RegisterDescriptor_Descriptors_arrays.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/Registers_Names_arrays.h` & `rabbitizer-1.7.5/include/generated/Registers_Names_arrays.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/Registers_enums.h` & `rabbitizer-1.7.5/include/generated/Registers_enums.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/generated/instrOpercandCallbacks_array.h` & `rabbitizer-1.7.5/include/generated/instrOpercandCallbacks_array.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerInstrDescriptor.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerInstrDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerInstrId.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerInstrId.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerInstrSuffix.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerInstrSuffix.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerInstruction.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerInstruction.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerInstructionR3000GTE.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerInstructionR3000GTE.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerInstructionR5900.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerInstructionR5900.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerInstructionRsp.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerInstructionRsp.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerOperandType.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerOperandType.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerRegister.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerRegister.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/instructions/RabbitizerRegisterDescriptor.h` & `rabbitizer-1.7.5/include/instructions/RabbitizerRegisterDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/include/rabbitizer.h` & `rabbitizer-1.7.5/include/rabbitizer.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/pyproject.toml` & `rabbitizer-1.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "rabbitizer"
 # Version should be synced with include/common/RabbitizerVersion.h
-version = "1.7.4"
+version = "1.7.5"
 description = "MIPS instruction decoder"
 # license = "MIT"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name="Anghelo Carvajal", email="angheloalf95@gmail.com" },
 ]
```

### Comparing `rabbitizer-1.7.4/rabbitizer/Config.pyi` & `rabbitizer-1.7.5/rabbitizer/Config.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/Enum.pyi` & `rabbitizer-1.7.5/rabbitizer/Enum.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/InstrId.pyi` & `rabbitizer-1.7.5/rabbitizer/InstrId.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/InstrIdType.pyi` & `rabbitizer-1.7.5/rabbitizer/InstrIdType.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/OperandType.pyi` & `rabbitizer-1.7.5/rabbitizer/OperandType.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/RegCop1N32.pyi` & `rabbitizer-1.7.5/rabbitizer/RegCop1N32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/RegCop1N64.pyi` & `rabbitizer-1.7.5/rabbitizer/RegCop1N64.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/RegCop1O32.pyi` & `rabbitizer-1.7.5/rabbitizer/RegCop1O32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/RegGprN32.pyi` & `rabbitizer-1.7.5/rabbitizer/RegGprN32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/RegGprO32.pyi` & `rabbitizer-1.7.5/rabbitizer/RegGprO32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/RegistersTracker.pyi` & `rabbitizer-1.7.5/rabbitizer/RegistersTracker.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/__init__.pyi` & `rabbitizer-1.7.5/rabbitizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/enums_utils.c` & `rabbitizer-1.7.5/rabbitizer/enums/enums_utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/enums_utils.h` & `rabbitizer-1.7.5/rabbitizer/enums/enums_utils.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_Abi.c` & `rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_Abi.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_AccessType.c` & `rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_AccessType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_InstrCategory.c` & `rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_InstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_InstrId.c` & `rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_InstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_InstrIdType.c` & `rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_InstrIdType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_enum_OperandType.c` & `rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_enum_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/rabbitizer_type_Enum.c` & `rabbitizer-1.7.5/rabbitizer/enums/rabbitizer_type_Enum.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c` & `rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c` & `rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c` & `rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c` & `rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c` & `rabbitizer-1.7.5/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer.pyi` & `rabbitizer-1.7.5/rabbitizer/rabbitizer.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_global_config.c` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_global_config.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_module.c` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_module.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_module.h` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_module.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_submodule_Utils.c` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_submodule_Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_type_Instruction.c` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_type_Instruction.c`

 * *Files 2% similar despite different names*

```diff
@@ -459,14 +459,15 @@
 
 static PyObject *rabbitizer_type_Instruction_disassemble(PyRabbitizerInstruction *self, PyObject *args, PyObject *kwds) {
     static char *kwlist[] = {"immOverride", "extraLJust", NULL};
     const char *immOverride = NULL;
     size_t immOverrideLength = 0;
     int extraLJust = 0;
     size_t bufferSize;
+    size_t disassembledSize;
     char *buffer;
     PyObject *ret;
 
     if (!PyArg_ParseTupleAndKeywords(args, kwds, "|zi", kwlist, &immOverride, &extraLJust)) {
         return NULL;
     }
 
@@ -474,19 +475,26 @@
         immOverrideLength = strlen(immOverride);
     }
 
     bufferSize = RabbitizerInstruction_getSizeForBuffer(&self->instr, immOverrideLength, extraLJust);
 
     buffer = malloc(bufferSize+1);
     if (buffer == NULL) {
-        // TODO: signal an exception?
+        PyErr_SetString(PyExc_MemoryError, "Not able to allocate enough space for decoded instruction.");
         return NULL;
     }
 
-    RabbitizerInstruction_disassemble(&self->instr, buffer, immOverride, immOverrideLength, extraLJust);
+    disassembledSize = RabbitizerInstruction_disassemble(&self->instr, buffer, immOverride, immOverrideLength, extraLJust);
+    if (disassembledSize > bufferSize) {
+        PyErr_SetString(PyExc_AssertionError, "Decoded instruction does not fit in the allocated buffer.\n"
+                                              "This will produce a memory corruption error.\n"
+                                              "This is not an user error, please report this bug.");
+        free(buffer);
+        return NULL;
+    }
 
     ret = PyUnicode_FromString(buffer);
     free(buffer);
     return ret;
 }
 
 
@@ -597,42 +605,52 @@
     { 0 },
 };
 
 
 static PyObject *rabbitizer_type_Instruction_repr(PyRabbitizerInstruction *self) {
     PyObject *ret;
     size_t disasmBufferSize;
+    size_t bufferSize;
+    size_t disassembledSize;
     char *bufferStart;
     char *buffer;
     size_t typeNameLength;
     size_t extraSize = 3 + 8 + 4; // "(0x" + 32bits hex + ") # "
     int len;
 
     typeNameLength = strlen("rabbitizer.Instruction");
 
     disasmBufferSize = RabbitizerInstruction_getSizeForBuffer(&self->instr, 0, 0);
 
-    buffer = bufferStart = malloc(disasmBufferSize+1 + typeNameLength + extraSize);
+    bufferSize = disasmBufferSize + typeNameLength + extraSize;
+    buffer = bufferStart = malloc(bufferSize + 1);
     if (buffer == NULL) {
-        // TODO: signal an exception?
+        PyErr_SetString(PyExc_MemoryError, "Not able to allocate enough space for decoded instruction.");
         return NULL;
     }
 
     memcpy(buffer, "rabbitizer.Instruction", typeNameLength);
     buffer += typeNameLength;
 
     len = sprintf(buffer, "(0x%08X) # ", RabbitizerInstruction_getRaw(&self->instr));
     if (len != 15) {
-        // bad stuff
-        // TODO: exception?
+        PyErr_SetString(PyExc_AssertionError, "This should not be triggered. assertion: len == 15");
+        return NULL;
     }
     assert(len == 15);
     buffer += len;
 
-    RabbitizerInstruction_disassemble(&self->instr, buffer, NULL, 0, 0);
+    disassembledSize = RabbitizerInstruction_disassemble(&self->instr, buffer, NULL, 0, 0);
+    if (disassembledSize > bufferSize) {
+        PyErr_SetString(PyExc_AssertionError, "Decoded instruction does not fit in the allocated buffer.\n"
+                                              "This will produce a memory corruption error.\n"
+                                              "This is not an user error, please report this bug.");
+        free(bufferStart);
+        return NULL;
+    }
 
     ret = PyUnicode_FromString(bufferStart);
     free(bufferStart);
     return ret;
 }
 
 static PyObject *rabbitizer_type_Instruction_str(PyRabbitizerInstruction *self) {
```

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_type_LoPairingInfo.c` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_type_LoPairingInfo.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_type_RegistersTracker.c` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_type_RegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer/rabbitizer_type_TrackedRegisterState.c` & `rabbitizer-1.7.5/rabbitizer/rabbitizer_type_TrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/rabbitizer.egg-info/PKG-INFO` & `rabbitizer-1.7.5/rabbitizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.7.4
+Version: 1.7.5
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.7.4/rabbitizer.egg-info/SOURCES.txt` & `rabbitizer-1.7.5/rabbitizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/setup.py` & `rabbitizer-1.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/analysis/RabbitizerRegistersTracker.c` & `rabbitizer-1.7.5/src/analysis/RabbitizerRegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/analysis/RabbitizerTrackedRegisterState.c` & `rabbitizer-1.7.5/src/analysis/RabbitizerTrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/common/RabbitizerConfig.c` & `rabbitizer-1.7.5/src/common/RabbitizerConfig.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/common/Utils.c` & `rabbitizer-1.7.5/src/common/Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstrCategory.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstrDescriptor.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstrDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstrId.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstrSuffix.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstrSuffix.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,22 @@
 
     *dst = '\0';
     return totalSize;
 }
 
 size_t RabbitizerInstruction_getSizeForBufferDataDisasm(UNUSED const RabbitizerInstruction *self, int extraLJust) {
     size_t totalSize = 0;
+    int tempLJust;
 
     totalSize += strlen(".word");
-    totalSize += RabbitizerConfig_Cfg.misc.opcodeLJust + extraLJust;
+
+    tempLJust = RabbitizerConfig_Cfg.misc.opcodeLJust + extraLJust;
+    tempLJust = RAB_MAX(tempLJust, 0);
+    totalSize += tempLJust;
+
     totalSize += 11;
     return totalSize;
 }
 
 size_t RabbitizerInstruction_disassembleAsData(const RabbitizerInstruction *self, char *dst, int extraLJust) {
     size_t totalSize = 0;
```

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerRegister.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerRegister.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/src/instructions/RabbitizerRegisterDescriptor.c` & `rabbitizer-1.7.5/src/instructions/RabbitizerRegisterDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/Makefile` & `rabbitizer-1.7.5/tables/Makefile`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_cpu.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_r5900.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/RabbitizerInstrId_rsp.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/RabbitizerInstrId_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop0.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_cop2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_normal.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_regimm.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/cpu/cpu_special.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/cpu/cpu_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2_special1.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2_special1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_cop2_special2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_cop2_special2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_0.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_1.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_mmi_3.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_mmi_3.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_normal.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_regimm.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/r5900/r5900_special.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/r5900/r5900_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_cop0.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_cop2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_cop2_vu.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_cop2_vu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_normal.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_normal_swc2.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_normal_swc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_regimm.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id/rsp/rsp_special.inc` & `rabbitizer-1.7.5/tables/tables/instr_id/rsp/rsp_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id_types/InstrIdType_cpu.inc` & `rabbitizer-1.7.5/tables/tables/instr_id_types/InstrIdType_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id_types/InstrIdType_r5900.inc` & `rabbitizer-1.7.5/tables/tables/instr_id_types/InstrIdType_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/instr_id_types/InstrIdType_rsp.inc` & `rabbitizer-1.7.5/tables/tables/instr_id_types/InstrIdType_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/operands/RabbitizerOperandType_cpu.inc` & `rabbitizer-1.7.5/tables/tables/operands/RabbitizerOperandType_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/operands/RabbitizerOperandType_r5900.inc` & `rabbitizer-1.7.5/tables/tables/operands/RabbitizerOperandType_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/operands/RabbitizerOperandType_rsp.inc` & `rabbitizer-1.7.5/tables/tables/operands/RabbitizerOperandType_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop0.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1Control.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1N32.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1N32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1N64.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1N64.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop1O32.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop1O32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_Cop2.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_Cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_GprN32.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_GprN32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_GprO32.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_GprO32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_R5900VF.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_R5900VF.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_R5900VI.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_R5900VI.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspCop0.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspCop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspCop2.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspCop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspGpr.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspGpr.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tables/registers/RabbitizerRegister_RspVector.inc` & `rabbitizer-1.7.5/tables/tables/registers/RabbitizerRegister_RspVector.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/c/InstrDescriptor_Descriptors_array.table.template` & `rabbitizer-1.7.5/tables/templates/c/InstrDescriptor_Descriptors_array.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/c/InstrId_enum.table.template` & `rabbitizer-1.7.5/tables/templates/c/InstrId_enum.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template` & `rabbitizer-1.7.5/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/c/Registers_Names_arrays.table.template` & `rabbitizer-1.7.5/tables/templates/c/Registers_Names_arrays.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/c/Registers_enums.table.template` & `rabbitizer-1.7.5/tables/templates/c/Registers_enums.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/cplusplus/Registers_enum_classes.table.template` & `rabbitizer-1.7.5/tables/templates/cplusplus/Registers_enum_classes.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/python/InstrId.tablepyi.template` & `rabbitizer-1.7.5/tables/templates/python/InstrId.tablepyi.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/rust/instr_category_enum.tablers.template` & `rabbitizer-1.7.5/tables/templates/rust/instr_category_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/rust/instr_id_enum.tablers.template` & `rabbitizer-1.7.5/tables/templates/rust/instr_id_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/rust/instr_suffix_enum.tablers.template` & `rabbitizer-1.7.5/tables/templates/rust/instr_suffix_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/rust/operand_type_enum.tablers.template` & `rabbitizer-1.7.5/tables/templates/rust/operand_type_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/templates/rust/registers_enum.tablers.template` & `rabbitizer-1.7.5/tables/templates/rust/registers_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tools/c_table_gen.sh` & `rabbitizer-1.7.5/tables/tools/c_table_gen.sh`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.4/tables/tools/pyi_table_gen.sh` & `rabbitizer-1.7.5/tables/tools/pyi_table_gen.sh`

 * *Files identical despite different names*

