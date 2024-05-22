# Comparing `tmp/rabbitizer-1.9.4.tar.gz` & `tmp/rabbitizer-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.9.4.tar", last modified: Mon Mar 18 19:42:16 2024, max compression
+gzip compressed data, was "rabbitizer-1.9.5.tar", last modified: Wed Apr  3 16:15:48 2024, max compression
```

## Comparing `rabbitizer-1.9.4.tar` & `rabbitizer-1.9.5.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.223318 rabbitizer-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-18 19:42:16.223318 rabbitizer-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.183318 rabbitizer-1.9.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.187318 rabbitizer-1.9.4/docs/r3000gte/
--rw-r--r--   0 runner    (1001) docker     (127)    38205 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/docs/r3000gte/gte_macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    72630 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/docs/r3000gte/gte_macros_volatile.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.187318 rabbitizer-1.9.4/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.187318 rabbitizer-1.9.4/include/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/analysis/RabbitizerLoPairingInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/analysis/RabbitizerRegistersTracker.h
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/analysis/RabbitizerTrackedRegisterState.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.187318 rabbitizer-1.9.4/include/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/common/RabbitizerConfig.h
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/common/RabbitizerVersion.h
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/common/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.191318 rabbitizer-1.9.4/include/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/Abi_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/AccessType_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrCategory_Names_array.h
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrCategory_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)   114440 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrDescriptor_Descriptors_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrIdType_Names_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrIdType_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)    35751 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrId_Names_array.h
--rw-r--r--   0 runner    (1001) docker     (127)    26827 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrId_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/InstrSuffix_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/OperandType_enum.h
--rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/OperandType_function_declarations.h
--rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/RegisterDescriptor_Descriptors_arrays.h
--rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/Registers_Names_arrays.h
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/Registers_enums.h
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/generated/instrOpercandCallbacks_array.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.195318 rabbitizer-1.9.4/include/instructions/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerAccessType.h
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstrCategory.h
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstrDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstrId.h
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstrIdType.h
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstrSuffix.h
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstruction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstructionR3000GTE.h
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstructionR5900.h
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerInstructionRsp.h
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerOperandType.h
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerRegister.h
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/instructions/RabbitizerRegisterDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/include/rabbitizer.h
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.199318 rabbitizer-1.9.4/rabbitizer/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/Abi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/AccessType.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/Config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/Enum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/InstrCategory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/InstrId.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/InstrIdType.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/LoPairingInfo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/OperandType.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/RegCop1N32.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/RegCop1N64.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/RegCop1O32.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/RegGprN32.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/RegGprO32.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/RegistersTracker.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/TrackedRegisterState.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/TrinaryValue.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/Utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.199318 rabbitizer-1.9.4/rabbitizer/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/enums_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/enums_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_Abi.c
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_AccessType.c
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_InstrId.c
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_InstrIdType.c
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_TrinaryValue.c
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_type_Enum.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.199318 rabbitizer-1.9.4/rabbitizer/enums/registers/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_global_config.c
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_macro_utilities.h
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_module.c
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_module.h
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_submodule_Utils.c
--rw-r--r--   0 runner    (1001) docker     (127)    29838 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_type_Instruction.c
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_type_LoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_type_RegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/rabbitizer/rabbitizer_type_TrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.223318 rabbitizer-1.9.4/rabbitizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-18 19:42:16.000000 rabbitizer-1.9.4/rabbitizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-03-18 19:42:16.000000 rabbitizer-1.9.4/rabbitizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 19:42:16.000000 rabbitizer-1.9.4/rabbitizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-18 19:42:16.000000 rabbitizer-1.9.4/rabbitizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 19:42:16.223318 rabbitizer-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.183318 rabbitizer-1.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.203318 rabbitizer-1.9.4/src/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/analysis/RabbitizerLoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (127)    13674 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/analysis/RabbitizerRegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/analysis/RabbitizerTrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.203318 rabbitizer-1.9.4/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/common/RabbitizerConfig.c
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/common/RabbitizerVersion.c
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/common/Utils.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.203318 rabbitizer-1.9.4/src/instructions/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (127)    22078 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstrDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstrId.c
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstrIdType.c
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstrSuffix.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.203318 rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
--rw-r--r--   0 runner    (1001) docker     (127)    19909 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.203318 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionCpu/
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.203318 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR3000GTE/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.203318 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR5900/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
--rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.207318 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionRsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerRegister.c
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/src/instructions/RabbitizerRegisterDescriptor.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.207318 rabbitizer-1.9.4/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.207318 rabbitizer-1.9.4/tables/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/Abi.inc
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/AccessType.inc
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/InstrCategory.inc
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/InstrIdType.inc
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/InstrIds.inc
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/InstrSuffix.inc
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/OperandTypes.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.207318 rabbitizer-1.9.4/tables/tables/instr_id/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.207318 rabbitizer-1.9.4/tables/tables/instr_id/cpu/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1.inc
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_normal.inc
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.211318 rabbitizer-1.9.4/tables/tables/instr_id/r3000gte/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.211318 rabbitizer-1.9.4/tables/tables/instr_id/r5900/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc
--rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2_special1.inc
--rw-r--r--   0 runner    (1001) docker     (127)    17390 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2_special2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi.inc
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_0.inc
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_1.inc
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_3.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_normal.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.211318 rabbitizer-1.9.4/tables/tables/instr_id/rsp/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_cop2_vu.inc
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_normal.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_normal_swc2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.211318 rabbitizer-1.9.4/tables/tables/instr_id_types/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id_types/InstrIdType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id_types/InstrIdType_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id_types/InstrIdType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/instr_id_types/InstrIdType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.215318 rabbitizer-1.9.4/tables/tables/operands/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/operands/RabbitizerOperandType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/operands/RabbitizerOperandType_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/operands/RabbitizerOperandType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/operands/RabbitizerOperandType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.215318 rabbitizer-1.9.4/tables/tables/registers/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop0.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1Control.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1N32.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1N64.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1O32.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_GprN32.inc
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_GprO32.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_R5900VF.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_R5900VI.inc
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspCop0.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspCop2.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspGpr.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspVector.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.187318 rabbitizer-1.9.4/tables/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.219318 rabbitizer-1.9.4/tables/templates/c/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/Abi_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/AccessType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrCategory_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrCategory_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrDescriptor_Descriptors_array.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrIdType_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrIdType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrId_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrId_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/InstrSuffix_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/OperandType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/OperandType_function_declarations.table.template
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/Registers_Names_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/Registers_enums.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/c/instrOpercandCallbacks_array.table.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.219318 rabbitizer-1.9.4/tables/templates/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/cplusplus/AccessType_enum_class.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/cplusplus/InstrIdType_enum_class.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/cplusplus/OperandType_enum_class.table.template
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/cplusplus/Registers_enum_classes.table.template
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/cplusplus/UniqueId_enum_class.table.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.219318 rabbitizer-1.9.4/tables/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/Abi.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/AccessType.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/InstrCategory.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/InstrId.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/InstrIdType.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/OperandType.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/RegCop1N32.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/RegCop1N64.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/RegCop1O32.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/RegGprN32.tablepyi.template
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/python/RegGprO32.tablepyi.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.223318 rabbitizer-1.9.4/tables/templates/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/abi_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/access_type_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/instr_category_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/instr_id_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/instr_id_type_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/instr_suffix_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/operand_type_enum.tablers.template
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/templates/rust/registers_enum.tablers.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:42:16.223318 rabbitizer-1.9.4/tables/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      757 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tools/c_table_gen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tools/pyi_table_gen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      461 2024-03-18 19:42:11.000000 rabbitizer-1.9.4/tables/tools/rs_table_gen.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.856718 rabbitizer-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-03 16:15:48.856718 rabbitizer-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.816717 rabbitizer-1.9.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.820717 rabbitizer-1.9.5/docs/r3000gte/
+-rw-r--r--   0 runner    (1001) docker     (127)    38205 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/docs/r3000gte/gte_macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72630 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/docs/r3000gte/gte_macros_volatile.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.820717 rabbitizer-1.9.5/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.824717 rabbitizer-1.9.5/include/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/analysis/RabbitizerLoPairingInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/analysis/RabbitizerRegistersTracker.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/analysis/RabbitizerTrackedRegisterState.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.824717 rabbitizer-1.9.5/include/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/common/RabbitizerConfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/common/RabbitizerVersion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/common/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.824717 rabbitizer-1.9.5/include/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/Abi_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/AccessType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrCategory_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrCategory_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)   114478 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrDescriptor_Descriptors_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrIdType_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrIdType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35751 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrId_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26827 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrId_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/InstrSuffix_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/OperandType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/OperandType_function_declarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/RegisterDescriptor_Descriptors_arrays.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/Registers_Names_arrays.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/Registers_enums.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/generated/instrOpercandCallbacks_array.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.828718 rabbitizer-1.9.5/include/instructions/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerAccessType.h
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstrCategory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstrDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstrId.h
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstrIdType.h
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstrSuffix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstruction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstructionR3000GTE.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstructionR5900.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerInstructionRsp.h
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerOperandType.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerRegister.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/instructions/RabbitizerRegisterDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/include/rabbitizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.832718 rabbitizer-1.9.5/rabbitizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/Abi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/AccessType.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/Config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/Enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/InstrCategory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/InstrId.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/InstrIdType.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/LoPairingInfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/OperandType.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/RegCop1N32.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/RegCop1N64.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/RegCop1O32.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/RegGprN32.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/RegGprO32.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/RegistersTracker.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/TrackedRegisterState.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/TrinaryValue.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/Utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.836717 rabbitizer-1.9.5/rabbitizer/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/enums_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/enums_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_Abi.c
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_AccessType.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_InstrId.c
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_InstrIdType.c
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_TrinaryValue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_type_Enum.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.836717 rabbitizer-1.9.5/rabbitizer/enums/registers/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_global_config.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_macro_utilities.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_module.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_submodule_Utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)    29838 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_type_Instruction.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_type_LoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_type_RegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/rabbitizer/rabbitizer_type_TrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.856718 rabbitizer-1.9.5/rabbitizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-03 16:15:48.000000 rabbitizer-1.9.5/rabbitizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-03 16:15:48.000000 rabbitizer-1.9.5/rabbitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:15:48.000000 rabbitizer-1.9.5/rabbitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 16:15:48.000000 rabbitizer-1.9.5/rabbitizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:15:48.856718 rabbitizer-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.816717 rabbitizer-1.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.836717 rabbitizer-1.9.5/src/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/analysis/RabbitizerLoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13674 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/analysis/RabbitizerRegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/analysis/RabbitizerTrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.836717 rabbitizer-1.9.5/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/common/RabbitizerConfig.c
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/common/RabbitizerVersion.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/common/Utils.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.836717 rabbitizer-1.9.5/src/instructions/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22078 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstrDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstrId.c
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstrIdType.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstrSuffix.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19909 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionCpu/
+-rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR3000GTE/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR5900/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20353 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionRsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerRegister.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/src/instructions/RabbitizerRegisterDescriptor.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/Abi.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/AccessType.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/InstrCategory.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/InstrIdType.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/InstrIds.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/InstrSuffix.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/OperandTypes.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.840718 rabbitizer-1.9.5/tables/tables/instr_id/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.844718 rabbitizer-1.9.5/tables/tables/instr_id/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.844718 rabbitizer-1.9.5/tables/tables/instr_id/r3000gte/
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.848718 rabbitizer-1.9.5/tables/tables/instr_id/r5900/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2_special1.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    17390 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2_special2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_0.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_1.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_3.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.848718 rabbitizer-1.9.5/tables/tables/instr_id/rsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_cop2_vu.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_normal_swc2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.848718 rabbitizer-1.9.5/tables/tables/instr_id_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id_types/InstrIdType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id_types/InstrIdType_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id_types/InstrIdType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/instr_id_types/InstrIdType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.848718 rabbitizer-1.9.5/tables/tables/operands/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/operands/RabbitizerOperandType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/operands/RabbitizerOperandType_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/operands/RabbitizerOperandType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/operands/RabbitizerOperandType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.852718 rabbitizer-1.9.5/tables/tables/registers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1Control.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1N32.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1N64.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1O32.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_GprN32.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_GprO32.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_R5900VF.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_R5900VI.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspCop0.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspCop2.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspGpr.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspVector.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.820717 rabbitizer-1.9.5/tables/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.852718 rabbitizer-1.9.5/tables/templates/c/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/Abi_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/AccessType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrCategory_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrCategory_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrDescriptor_Descriptors_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrIdType_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrIdType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrId_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrId_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/InstrSuffix_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/OperandType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/OperandType_function_declarations.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/Registers_Names_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/Registers_enums.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/c/instrOpercandCallbacks_array.table.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.852718 rabbitizer-1.9.5/tables/templates/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/cplusplus/AccessType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/cplusplus/InstrIdType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/cplusplus/OperandType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/cplusplus/Registers_enum_classes.table.template
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/cplusplus/UniqueId_enum_class.table.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.856718 rabbitizer-1.9.5/tables/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/Abi.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/AccessType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/InstrCategory.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/InstrId.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/InstrIdType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/OperandType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/RegCop1N32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/RegCop1N64.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/RegCop1O32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/RegGprN32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/python/RegGprO32.tablepyi.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.856718 rabbitizer-1.9.5/tables/templates/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/abi_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/access_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/instr_category_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/instr_id_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/instr_id_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/instr_suffix_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/operand_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/templates/rust/registers_enum.tablers.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:48.856718 rabbitizer-1.9.5/tables/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      757 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tools/c_table_gen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tools/pyi_table_gen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      461 2024-04-03 16:15:45.000000 rabbitizer-1.9.5/tables/tools/rs_table_gen.sh
```

### Comparing `rabbitizer-1.9.4/LICENSE` & `rabbitizer-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/PKG-INFO` & `rabbitizer-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.9.4
+Version: 1.9.5
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -70,15 +70,15 @@
 python3 -m pip install -U rabbitizer
 ```
 
 If you use a `requirements.txt` file in your repository, then you can add this
 library with the following line:
 
 ```txt
-rabbitizer>=1.9.4,<2.0.0
+rabbitizer>=1.9.5,<2.0.0
 ```
 
 ### Development version
 
 The unstable development version is located at the
 [develop](https://github.com/Decompollaborate/rabbitizer/tree/develop)
 branch. PRs should be made into that branch instead of the main one.
@@ -103,15 +103,15 @@
 ```bash
 cargo add rabbitizer
 ```
 
 Or you can add it manually to your `Cargo.toml`:
 
 ```toml
-rabbitizer = "1.9.4"
+rabbitizer = "1.9.5"
 ```
 
 See this crate at <https://crates.io/crates/rabbitizer>.
 
 ## References
 
 - MIPS CPU:
```

### Comparing `rabbitizer-1.9.4/README.md` & `rabbitizer-1.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 python3 -m pip install -U rabbitizer
 ```
 
 If you use a `requirements.txt` file in your repository, then you can add this
 library with the following line:
 
 ```txt
-rabbitizer>=1.9.4,<2.0.0
+rabbitizer>=1.9.5,<2.0.0
 ```
 
 ### Development version
 
 The unstable development version is located at the
 [develop](https://github.com/Decompollaborate/rabbitizer/tree/develop)
 branch. PRs should be made into that branch instead of the main one.
@@ -92,15 +92,15 @@
 ```bash
 cargo add rabbitizer
 ```
 
 Or you can add it manually to your `Cargo.toml`:
 
 ```toml
-rabbitizer = "1.9.4"
+rabbitizer = "1.9.5"
 ```
 
 See this crate at <https://crates.io/crates/rabbitizer>.
 
 ## References
 
 - MIPS CPU:
```

### Comparing `rabbitizer-1.9.4/docs/r3000gte/gte_macros.h` & `rabbitizer-1.9.5/docs/r3000gte/gte_macros.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/docs/r3000gte/gte_macros_volatile.h` & `rabbitizer-1.9.5/docs/r3000gte/gte_macros_volatile.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/analysis/RabbitizerLoPairingInfo.h` & `rabbitizer-1.9.5/include/analysis/RabbitizerLoPairingInfo.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/analysis/RabbitizerRegistersTracker.h` & `rabbitizer-1.9.5/include/analysis/RabbitizerRegistersTracker.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/analysis/RabbitizerTrackedRegisterState.h` & `rabbitizer-1.9.5/include/analysis/RabbitizerTrackedRegisterState.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/common/RabbitizerConfig.h` & `rabbitizer-1.9.5/include/common/RabbitizerConfig.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/common/RabbitizerVersion.h` & `rabbitizer-1.9.5/include/common/RabbitizerVersion.h`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 extern "C" {
 #endif
 
 
 // Header version
 #define RAB_VERSION_MAJOR 1
 #define RAB_VERSION_MINOR 9
-#define RAB_VERSION_PATCH 4
+#define RAB_VERSION_PATCH 5
 
 #define RAB_VERSION_STR RAB_STRINGIFY(RAB_VERSION_MAJOR) "." RAB_STRINGIFY(RAB_VERSION_MINOR) "." RAB_STRINGIFY(RAB_VERSION_PATCH)
 
 #define RAB_VERSION_AUTHOR "Decompollaborate"
 
 
 // Compiled library version
```

### Comparing `rabbitizer-1.9.4/include/common/Utils.h` & `rabbitizer-1.9.5/include/common/Utils.h`

 * *Files 15% similar despite different names*

```diff
@@ -80,39 +80,49 @@
 
 #define BITREPACK(fullword, v, s, w) ((SHIFTR((fullword), (s)+(w), 32-((s)+(w))) << ((s)+(w))) | SHIFTL((v), (s), (w)) | MASK((fullword), (s)))
 #define BITREPACK_RIGHT(fullword, v, s, w) (SHIFTL((v), (s), (w)) | MASK((fullword), (s)))
 
 #define RABUTILS_BUFFER_ADVANCE(buffer, totalSize, expression) \
     do {                                                       \
         size_t __tempSize = (size_t)(expression);              \
-        (buffer) += __tempSize;                                \
+        if ((buffer) != NULL) {                                \
+            (buffer) += __tempSize;                            \
+        }                                                      \
         (totalSize) += __tempSize;                             \
     } while (0)
 
 #define RABUTILS_BUFFER_WRITE_CHAR(buffer, totalSize, character) \
     do {                                                         \
-        *(buffer) = (character);                                 \
+        if ((buffer) != NULL) {                                  \
+            *(buffer) = (character);                             \
+        }                                                        \
         RABUTILS_BUFFER_ADVANCE(buffer, totalSize, 1);           \
     } while (0)
 
 #define RABUTILS_BUFFER_SPRINTF(buffer, totalSize, format, ...) \
     do {                                                        \
-        int _len = sprintf(buffer, format, __VA_ARGS__);        \
+        int _len;                                               \
+        if (buffer != NULL) {                                   \
+            _len = sprintf(buffer, format, __VA_ARGS__);        \
+        } else {                                                \
+            _len = snprintf(NULL, 0, format, __VA_ARGS__);      \
+        }                                                       \
         assert(_len > 0);                                       \
         RABUTILS_BUFFER_ADVANCE(buffer, totalSize, _len);       \
     } while (0)
 
 #define RABUTILS_BUFFER_CPY(buffer, totalSize, string)         \
     do {                                                       \
         size_t _tempSize = strlen(string);                     \
-        memcpy(buffer, string, _tempSize);                     \
+        if ((buffer) != NULL) {                                \
+            memcpy(buffer, string, _tempSize);                 \
+        }                                                      \
         RABUTILS_BUFFER_ADVANCE(buffer, totalSize, _tempSize); \
     } while (0)
 
-
 CONST NODISCARD
 int32_t RabbitizerUtils_From2Complement(uint32_t number, int bits);
 NON_NULL(1)
 size_t RabbitizerUtils_CharFill(char *dst, int count, char fillchar);
 NON_NULL(1, 3)
 size_t RabbitizerUtils_escapeString(char *dst, size_t dstSize, const char *src, size_t srcSize);
```

### Comparing `rabbitizer-1.9.4/include/generated/InstrDescriptor_Descriptors_array.h` & `rabbitizer-1.9.5/include/generated/InstrDescriptor_Descriptors_array.h`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
     [RABBITIZER_INSTR_ID_rsp_or] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_rsp_xor] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_rsp_nor] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_rsp_slt] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_rsp_sltu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_rsp_break] = { .operands={RAB_OPERAND_cpu_code}, .instrType=RABBITIZER_INSTR_TYPE_R },
     [RABBITIZER_INSTR_ID_rsp_nop] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R, .isPseudo=true },
-    [RABBITIZER_INSTR_ID_rsp_move] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_rsp_move] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .maybeIsMove=true, .isPseudo=true },
     [RABBITIZER_INSTR_ID_rsp_not] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
     [RABBITIZER_INSTR_ID_rsp_neg] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .notEmittedByCompilers=true, .modifiesRd=true, .readsRt=true, .isPseudo=true },
     [RABBITIZER_INSTR_ID_rsp_negu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true, .isPseudo=true },
     [RABBITIZER_INSTR_ID_rsp_bltz] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
     [RABBITIZER_INSTR_ID_rsp_bgez] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
     [RABBITIZER_INSTR_ID_rsp_bltzal] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true, .doesLink=true },
     [RABBITIZER_INSTR_ID_rsp_bgezal] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true, .notEmittedByCompilers=true, .doesLink=true },
@@ -527,15 +527,15 @@
     [RABBITIZER_INSTR_ID_r5900_pceqb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_padduw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_psubuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_pextuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_padduh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_psubuh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_pextuh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-    [RABBITIZER_INSTR_ID_r5900_paddub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true, .maybeIsMove=true },
     [RABBITIZER_INSTR_ID_r5900_psubub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_pextub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_qfsrv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_pmaddw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_psllvw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_psrlvw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_r5900_pmsubw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
```

### Comparing `rabbitizer-1.9.4/include/generated/InstrIdType_Names_array.h` & `rabbitizer-1.9.5/include/generated/InstrIdType_Names_array.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/InstrIdType_enum.h` & `rabbitizer-1.9.5/include/generated/InstrIdType_enum.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/InstrId_Names_array.h` & `rabbitizer-1.9.5/include/generated/InstrId_Names_array.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/InstrId_enum.h` & `rabbitizer-1.9.5/include/generated/InstrId_enum.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/OperandType_enum.h` & `rabbitizer-1.9.5/include/generated/OperandType_enum.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/OperandType_function_declarations.h` & `rabbitizer-1.9.5/include/generated/OperandType_function_declarations.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/RegisterDescriptor_Descriptors_arrays.h` & `rabbitizer-1.9.5/include/generated/RegisterDescriptor_Descriptors_arrays.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/Registers_Names_arrays.h` & `rabbitizer-1.9.5/include/generated/Registers_Names_arrays.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/Registers_enums.h` & `rabbitizer-1.9.5/include/generated/Registers_enums.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/generated/instrOpercandCallbacks_array.h` & `rabbitizer-1.9.5/include/generated/instrOpercandCallbacks_array.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerInstrDescriptor.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerInstrDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerInstrId.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerInstrId.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerInstrSuffix.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerInstrSuffix.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerInstruction.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerInstruction.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerInstructionR3000GTE.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerInstructionR3000GTE.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerInstructionR5900.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerInstructionR5900.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerInstructionRsp.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerInstructionRsp.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerOperandType.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerOperandType.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerRegister.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerRegister.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/instructions/RabbitizerRegisterDescriptor.h` & `rabbitizer-1.9.5/include/instructions/RabbitizerRegisterDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/include/rabbitizer.h` & `rabbitizer-1.9.5/include/rabbitizer.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/pyproject.toml` & `rabbitizer-1.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: © 2022-2024 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "rabbitizer"
 # Version should be synced with include/common/RabbitizerVersion.h
-version = "1.9.4"
+version = "1.9.5"
 description = "MIPS instruction decoder"
 # license = "MIT"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name="Anghelo Carvajal", email="angheloalf95@gmail.com" },
 ]
```

### Comparing `rabbitizer-1.9.4/rabbitizer/Config.pyi` & `rabbitizer-1.9.5/rabbitizer/Config.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/Enum.pyi` & `rabbitizer-1.9.5/rabbitizer/Enum.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/InstrId.pyi` & `rabbitizer-1.9.5/rabbitizer/InstrId.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/InstrIdType.pyi` & `rabbitizer-1.9.5/rabbitizer/InstrIdType.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/OperandType.pyi` & `rabbitizer-1.9.5/rabbitizer/OperandType.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/RegCop1N32.pyi` & `rabbitizer-1.9.5/rabbitizer/RegCop1N32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/RegCop1N64.pyi` & `rabbitizer-1.9.5/rabbitizer/RegCop1N64.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/RegCop1O32.pyi` & `rabbitizer-1.9.5/rabbitizer/RegCop1O32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/RegGprN32.pyi` & `rabbitizer-1.9.5/rabbitizer/RegGprN32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/RegGprO32.pyi` & `rabbitizer-1.9.5/rabbitizer/RegGprO32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/RegistersTracker.pyi` & `rabbitizer-1.9.5/rabbitizer/RegistersTracker.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/__init__.pyi` & `rabbitizer-1.9.5/rabbitizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/enums_utils.c` & `rabbitizer-1.9.5/rabbitizer/enums/enums_utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/enums_utils.h` & `rabbitizer-1.9.5/rabbitizer/enums/enums_utils.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_Abi.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_Abi.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_AccessType.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_AccessType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_InstrCategory.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_InstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_InstrId.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_InstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_InstrIdType.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_InstrIdType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_OperandType.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_enum_TrinaryValue.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_enum_TrinaryValue.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/rabbitizer_type_Enum.c` & `rabbitizer-1.9.5/rabbitizer/enums/rabbitizer_type_Enum.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c` & `rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c` & `rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c` & `rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c` & `rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c` & `rabbitizer-1.9.5/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer.pyi` & `rabbitizer-1.9.5/rabbitizer/rabbitizer.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_global_config.c` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_global_config.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_macro_utilities.h` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_macro_utilities.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_module.c` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_module.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_module.h` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_module.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_submodule_Utils.c` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_submodule_Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_type_Instruction.c` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_type_Instruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_type_LoPairingInfo.c` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_type_LoPairingInfo.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_type_RegistersTracker.c` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_type_RegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer/rabbitizer_type_TrackedRegisterState.c` & `rabbitizer-1.9.5/rabbitizer/rabbitizer_type_TrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/rabbitizer.egg-info/PKG-INFO` & `rabbitizer-1.9.5/rabbitizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.9.4
+Version: 1.9.5
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -70,15 +70,15 @@
 python3 -m pip install -U rabbitizer
 ```
 
 If you use a `requirements.txt` file in your repository, then you can add this
 library with the following line:
 
 ```txt
-rabbitizer>=1.9.4,<2.0.0
+rabbitizer>=1.9.5,<2.0.0
 ```
 
 ### Development version
 
 The unstable development version is located at the
 [develop](https://github.com/Decompollaborate/rabbitizer/tree/develop)
 branch. PRs should be made into that branch instead of the main one.
@@ -103,15 +103,15 @@
 ```bash
 cargo add rabbitizer
 ```
 
 Or you can add it manually to your `Cargo.toml`:
 
 ```toml
-rabbitizer = "1.9.4"
+rabbitizer = "1.9.5"
 ```
 
 See this crate at <https://crates.io/crates/rabbitizer>.
 
 ## References
 
 - MIPS CPU:
```

### Comparing `rabbitizer-1.9.4/rabbitizer.egg-info/SOURCES.txt` & `rabbitizer-1.9.5/rabbitizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/setup.py` & `rabbitizer-1.9.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 extraCompileArgs = ["-std=c11", "-Wall", "-g",]
 if platform.system() == "Linux":
     extraCompileArgs += ["-Os", "-Wextra",]
     extraCompileArgs += ["-Werror=vla", "-Werror=switch", "-Werror=implicit-fallthrough", "-Werror=unused-function", "-Werror=unused-parameter", "-Werror=shadow", "-Werror=switch"]
     extraCompileArgs += ["-Werror=implicit-function-declaration", "-Werror=incompatible-pointer-types"]
     extraCompileArgs += ["-Werror"]
+    extraCompileArgs += ["-Wno-nonnull-compare"]
 
 setup(
     ext_modules=[
         Extension(
             name="rabbitizer",
             sources=sourcesList,
             include_dirs=["include", "rabbitizer", "tables"],
```

### Comparing `rabbitizer-1.9.4/src/analysis/RabbitizerRegistersTracker.c` & `rabbitizer-1.9.5/src/analysis/RabbitizerRegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/analysis/RabbitizerTrackedRegisterState.c` & `rabbitizer-1.9.5/src/analysis/RabbitizerTrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/common/RabbitizerConfig.c` & `rabbitizer-1.9.5/src/common/RabbitizerConfig.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/common/Utils.c` & `rabbitizer-1.9.5/src/common/Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstrCategory.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstrCategory.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstrDescriptor.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstrDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstrId.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstrSuffix.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstrSuffix.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c`

 * *Files 14% similar despite different names*

```diff
@@ -6,31 +6,23 @@
 #include <assert.h>
 #include <stdlib.h>
 
 #include "generated/instrOpercandCallbacks_array.h"
 
 size_t RabbitizerOperandType_getBufferSize(RabbitizerOperandType operand, const RabbitizerInstruction *instr,
                                            size_t immOverrideLength) {
-    char *auxBuffer = calloc(immOverrideLength * 2 + 2, sizeof(char));
-    char *immOverride = calloc(immOverrideLength + 2, sizeof(char));
     OperandCallback callback;
-    size_t size;
 
     assert(operand > RAB_OPERAND_ALL_INVALID);
     assert(operand < RAB_OPERAND_ALL_MAX);
 
     callback = instrOpercandCallbacks[operand];
     assert(callback != NULL);
 
-    size = callback(instr, auxBuffer, immOverride, immOverrideLength);
-
-    free(auxBuffer);
-    free(immOverride);
-
-    return size;
+    return callback(instr, NULL, NULL, immOverrideLength);
 }
 
 size_t RabbitizerInstruction_getSizeForBufferOperandsDisasm(const RabbitizerInstruction *self,
                                                             size_t immOverrideLength) {
     size_t totalSize = 0;
 
     for (size_t i = 0;
```

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c`

 * *Files 2% similar despite different names*

```diff
@@ -191,28 +191,36 @@
     return totalSize;
 }
 
 size_t RabbitizerOperandType_process_cpu_label(const RabbitizerInstruction *self, char *dst, const char *immOverride,
                                                size_t immOverrideLength) {
     size_t totalSize = 0;
 
+    if ((dst == NULL) && (immOverrideLength > 0)) {
+        return immOverrideLength;
+    }
+
     if ((immOverride != NULL) && (immOverrideLength > 0)) {
         memcpy(dst, immOverride, immOverrideLength);
         return immOverrideLength;
     }
 
     RABUTILS_BUFFER_SPRINTF(dst, totalSize, "func_%06X", RabbitizerInstruction_getInstrIndexAsVram(self));
     return totalSize;
 }
 
 size_t RabbitizerOperandType_process_cpu_immediate(const RabbitizerInstruction *self, char *dst,
                                                    const char *immOverride, size_t immOverrideLength) {
     size_t totalSize = 0;
     int32_t number;
 
+    if ((dst == NULL) && (immOverrideLength > 0)) {
+        return immOverrideLength;
+    }
+
     if ((immOverride != NULL) && (immOverrideLength > 0)) {
         memcpy(dst, immOverride, immOverrideLength);
         return immOverrideLength;
     }
 
     number = RabbitizerInstruction_getProcessedImmediate(self);
     if (RabbitizerConfig_Cfg.misc.omit0XOnSmallImm) {
@@ -237,14 +245,18 @@
     return totalSize;
 }
 
 size_t RabbitizerOperandType_process_cpu_branch_target_label(const RabbitizerInstruction *self, char *dst,
                                                              const char *immOverride, size_t immOverrideLength) {
     size_t totalSize = 0;
 
+    if ((dst == NULL) && (immOverrideLength > 0)) {
+        return immOverrideLength;
+    }
+
     if ((immOverride != NULL) && (immOverrideLength > 0)) {
         memcpy(dst, immOverride, immOverrideLength);
         return immOverrideLength;
     }
 
     RABUTILS_BUFFER_CPY(dst, totalSize, ". + 4 + (");
     RABUTILS_BUFFER_ADVANCE(dst, totalSize, RabbitizerOperandType_process_cpu_immediate(self, dst, NULL, 0));
```

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c`

 * *Files 1% similar despite different names*

```diff
@@ -488,14 +488,18 @@
 }
 
 size_t RabbitizerOperandType_process_r5900_immediate5(const RabbitizerInstruction *self, char *dst,
                                                       const char *immOverride, size_t immOverrideLength) {
     size_t totalSize = 0;
     int32_t number;
 
+    if ((dst == NULL) && (immOverrideLength > 0)) {
+        return immOverrideLength;
+    }
+
     if ((immOverride != NULL) && (immOverrideLength > 0)) {
         memcpy(dst, immOverride, immOverrideLength);
         return immOverrideLength;
     }
 
     number = RAB_INSTR_R5900_GET_imm5(self);
     if (RabbitizerConfig_Cfg.misc.omit0XOnSmallImm) {
@@ -521,14 +525,18 @@
 }
 
 size_t RabbitizerOperandType_process_r5900_immediate15(const RabbitizerInstruction *self, char *dst,
                                                        const char *immOverride, size_t immOverrideLength) {
     size_t totalSize = 0;
     int32_t number;
 
+    if ((dst == NULL) && (immOverrideLength > 0)) {
+        return immOverrideLength;
+    }
+
     if ((immOverride != NULL) && (immOverrideLength > 0)) {
         memcpy(dst, immOverride, immOverrideLength);
         return immOverrideLength;
     }
 
     number = RAB_INSTR_R5900_GET_imm15(self) * 8;
     if (RabbitizerConfig_Cfg.misc.omit0XOnSmallImm) {
```

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerRegister.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerRegister.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/src/instructions/RabbitizerRegisterDescriptor.c` & `rabbitizer-1.9.5/src/instructions/RabbitizerRegisterDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/Makefile` & `rabbitizer-1.9.5/tables/Makefile`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_cpu.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_r5900.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/RabbitizerInstrId_rsp.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/RabbitizerInstrId_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop0.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_cop2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_normal.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_regimm.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/cpu/cpu_special.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/cpu/cpu_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2_special1.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2_special1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_cop2_special2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_cop2_special2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_0.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_1.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_1.inc`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
     ) // Parallel EXTend Upper from Halfword
 
     RABBITIZER_DEF_INSTR_ID(
         r5900, 0x18, paddub,
         .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
         .modifiesRd=true,
         .readsRs=true,
-        .readsRt=true
+        .readsRt=true,
+        .maybeIsMove=true
     ) // Parallel ADD Unsigned saturation Byte
     RABBITIZER_DEF_INSTR_ID(
         r5900, 0x19, psubub,
         .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
         .modifiesRd=true,
         .readsRs=true,
         .readsRt=true
```

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_mmi_3.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_mmi_3.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_normal.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_regimm.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/r5900/r5900_special.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/r5900/r5900_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_cop0.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_cop2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_cop2_vu.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_cop2_vu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_normal.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_normal_swc2.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_normal_swc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_regimm.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id/rsp/rsp_special.inc` & `rabbitizer-1.9.5/tables/tables/instr_id/rsp/rsp_special.inc`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
     // OP rd, rs
     RABBITIZER_DEF_INSTR_ID(
         rsp, -0x25, move,
         .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs},
         .instrType=RABBITIZER_INSTR_TYPE_R,
         .modifiesRd=true,
         .readsRs=true,
+        .maybeIsMove=true,
         .isPseudo=true
     ) // Move
     RABBITIZER_DEF_INSTR_ID(
         rsp, -0x27, not,
         .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs},
         .instrType=RABBITIZER_INSTR_TYPE_R,
         .modifiesRd=true,
```

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id_types/InstrIdType_cpu.inc` & `rabbitizer-1.9.5/tables/tables/instr_id_types/InstrIdType_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id_types/InstrIdType_r5900.inc` & `rabbitizer-1.9.5/tables/tables/instr_id_types/InstrIdType_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/instr_id_types/InstrIdType_rsp.inc` & `rabbitizer-1.9.5/tables/tables/instr_id_types/InstrIdType_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/operands/RabbitizerOperandType_cpu.inc` & `rabbitizer-1.9.5/tables/tables/operands/RabbitizerOperandType_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/operands/RabbitizerOperandType_r5900.inc` & `rabbitizer-1.9.5/tables/tables/operands/RabbitizerOperandType_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/operands/RabbitizerOperandType_rsp.inc` & `rabbitizer-1.9.5/tables/tables/operands/RabbitizerOperandType_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop0.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1Control.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1N32.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1N32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1N64.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1N64.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop1O32.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop1O32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_Cop2.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_Cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_GprN32.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_GprN32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_GprO32.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_GprO32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_R5900VF.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_R5900VF.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_R5900VI.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_R5900VI.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspCop0.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspCop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspCop2.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspCop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspGpr.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspGpr.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tables/registers/RabbitizerRegister_RspVector.inc` & `rabbitizer-1.9.5/tables/tables/registers/RabbitizerRegister_RspVector.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/c/InstrDescriptor_Descriptors_array.table.template` & `rabbitizer-1.9.5/tables/templates/c/InstrDescriptor_Descriptors_array.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/c/InstrId_enum.table.template` & `rabbitizer-1.9.5/tables/templates/c/InstrId_enum.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template` & `rabbitizer-1.9.5/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/c/Registers_Names_arrays.table.template` & `rabbitizer-1.9.5/tables/templates/c/Registers_Names_arrays.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/c/Registers_enums.table.template` & `rabbitizer-1.9.5/tables/templates/c/Registers_enums.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/cplusplus/Registers_enum_classes.table.template` & `rabbitizer-1.9.5/tables/templates/cplusplus/Registers_enum_classes.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/python/InstrId.tablepyi.template` & `rabbitizer-1.9.5/tables/templates/python/InstrId.tablepyi.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/rust/instr_category_enum.tablers.template` & `rabbitizer-1.9.5/tables/templates/rust/instr_category_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/rust/instr_id_enum.tablers.template` & `rabbitizer-1.9.5/tables/templates/rust/instr_id_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/rust/instr_suffix_enum.tablers.template` & `rabbitizer-1.9.5/tables/templates/rust/instr_suffix_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/rust/operand_type_enum.tablers.template` & `rabbitizer-1.9.5/tables/templates/rust/operand_type_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/templates/rust/registers_enum.tablers.template` & `rabbitizer-1.9.5/tables/templates/rust/registers_enum.tablers.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tools/c_table_gen.sh` & `rabbitizer-1.9.5/tables/tools/c_table_gen.sh`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.9.4/tables/tools/pyi_table_gen.sh` & `rabbitizer-1.9.5/tables/tools/pyi_table_gen.sh`

 * *Files identical despite different names*

