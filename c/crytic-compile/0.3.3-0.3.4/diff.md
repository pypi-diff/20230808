# Comparing `tmp/crytic-compile-0.3.3.tar.gz` & `tmp/crytic-compile-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crytic-compile-0.3.3.tar", last modified: Thu Jul  6 15:45:04 2023, max compression
+gzip compressed data, was "crytic-compile-0.3.4.tar", last modified: Tue Aug  8 14:10:15 2023, max compression
```

## Comparing `crytic-compile-0.3.3.tar` & `crytic-compile-0.3.4.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/compilation_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    23517 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/crytic_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile/cryticparser/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/cryticparser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15605 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/cryticparser/cryticparser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/cryticparser/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.605070 crytic-compile-0.3.3/crytic_compile/platform/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/abstract_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/all_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/all_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/archive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8496 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/brownie.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/buidler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8641 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/dapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10118 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/embark.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8281 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/etherlime.py
--rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/etherscan.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/foundry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12036 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/hardhat.py
--rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/solc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/solc_standard_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/standard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18378 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/truffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/vyper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13370 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/platform/waffle.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/source_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/crytic_compile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/name_collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/natspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/npm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/unit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/crytic_compile/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.601070 crytic-compile-0.3.3/crytic_compile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 15:45:04.000000 crytic-compile-0.3.3/crytic_compile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:45:04.609070 crytic-compile-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-06 15:44:51.000000 crytic-compile-0.3.3/tests/test_zip_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.278584 crytic-compile-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-08 14:10:15.278584 crytic-compile-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.274584 crytic-compile-0.3.4/crytic_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/compilation_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.274584 crytic-compile-0.3.4/crytic_compile/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/crytic_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.274584 crytic-compile-0.3.4/crytic_compile/cryticparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/cryticparser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15605 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/cryticparser/cryticparser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/cryticparser/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.278584 crytic-compile-0.3.4/crytic_compile/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/abstract_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/all_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/all_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8496 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/brownie.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/buidler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8641 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/dapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10118 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/embark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8281 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/etherlime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19301 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/etherscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/foundry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12036 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/hardhat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29584 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/solc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/solc_standard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18378 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/truffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/vyper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13370 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/platform/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/source_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.278584 crytic-compile-0.3.4/crytic_compile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/name_collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/npm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/crytic_compile/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.274584 crytic-compile-0.3.4/crytic_compile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-08 14:10:15.000000 crytic-compile-0.3.4/crytic_compile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 14:10:15.000000 crytic-compile-0.3.4/crytic_compile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:10:15.000000 crytic-compile-0.3.4/crytic_compile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 14:10:15.000000 crytic-compile-0.3.4/crytic_compile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 14:10:15.000000 crytic-compile-0.3.4/crytic_compile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 14:10:15.000000 crytic-compile-0.3.4/crytic_compile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:10:15.278584 crytic-compile-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:10:15.278584 crytic-compile-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/tests/test_library_linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-08-08 14:10:06.000000 crytic-compile-0.3.4/tests/test_zip_archive.py
```

### Comparing `crytic-compile-0.3.3/LICENSE` & `crytic-compile-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/PKG-INFO` & `crytic-compile-0.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.3
+Version: 0.3.4
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -16,47 +16,65 @@
 # Crytic-compile
 [![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/crytic-compile/ci.yml?branch=master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
 [![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 [![PyPI version](https://badge.fury.io/py/crytic-compile.svg)](https://badge.fury.io/py/crytic-compile)
 
 Library to help smart contract compilation. It includes support for:
 - Direct solc compilation
+- [Foundry](https://github.com/foundry-rs/foundry/)
+- [Hardhat](https://github.com/nomiclabs/hardhat)
 - [Brownie](https://github.com/iamdefinitelyahuman/brownie)
 - [Buidler](https://github.com/nomiclabs/buidler)
 - [Dapp](https://dapp.tools/dapp/)
 - [Embark](https://embark.status.im/)
 - [Etherlime](https://github.com/LimeChain/etherlime)
 - [Etherscan](https://etherscan.io/) (including several alt-chain explorers and testnets)
-- [Foundry](https://github.com/foundry-rs/foundry/)
-- [Hardhat](https://github.com/nomiclabs/hardhat)
 - [Truffle](https://truffleframework.com/)
 - [Waffle](https://github.com/EthWorks/Waffle)
 
+To force compilation with a specific framework, use the `--compile-force-framework` flag. For example, to force compilation with Hardhat:
+
+```shell
+crytic-compile . --compile-force-framework hardhat
+```
+
 See the [Configuration](https://github.com/crytic/crytic-compile/wiki/Configuration) documentation for advanced usages.
 
 The plugin is used in Trail of Bits tools, including:
 - [Slither](https://github.com/crytic/slither)
 - [Echidna](https://github.com/crytic/echidna)
 - [Manticore](https://github.com/trailofbits/manticore/)
 - [evm-cfg-builder](https://github.com/crytic/evm_cfg_builder)
 
 
 ## Installation
 
-```bash
+```shell
 pip3 install crytic-compile
 ```
 
 ## Usage
 
-### Standalone
-```bash
+In the root directory of your project e.g. same directory as `hardhat.config.js` or `foundry.toml`, run:
+
+```shell
 crytic-compile .
 ```
 
 Crytic-compile will generate `crytic-export/contracts.json` containing the AST/ABI and bytecodes of the contracts.
 
 Run `crytic-compile --help` for more options.
 
+## Library Linking
+
+If your project uses [libraries](https://docs.soliditylang.org/en/latest/contracts.html#libraries) with external functions, they can be linked to their deployed address with the `--compile-libraries` flag. For example, if you have a library `SafeMath` deployed at `0xff`, you can link it with:
+
+
+```shell
+crytic-compile . --compile-libraries "(SafeMath, 0xff)"
+```
+
+If you are fuzzing with Echidna or Medusa, follow this [tutorial on linking libraries](https://secure-contracts.com/program-analysis/echidna/advanced/working-with-libraries.html?highlight=library#linking-libraries).
+
 ### As a library
 
 See the [library documentation](https://github.com/crytic/crytic-compile/wiki/Library-Documentation).
```

### Comparing `crytic-compile-0.3.3/crytic_compile/__main__.py` & `crytic-compile-0.3.4/crytic_compile/__main__.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/compilation_unit.py` & `crytic-compile-0.3.4/crytic_compile/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/compiler/compiler.py` & `crytic-compile-0.3.4/crytic_compile/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/crytic_compile.py` & `crytic-compile-0.3.4/crytic_compile/crytic_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,21 +59,22 @@
     return any(platform.is_supported(target) for platform in platforms) or target.endswith(".zip")
 
 
 def _extract_libraries(libraries_str: Optional[str]) -> Optional[Dict[str, int]]:
 
     if not libraries_str:
         return None
-
-    pattern = r"\((?P<name>\w+),\s*(?P<value1>0x[0-9a-fA-F]{2})\),?"
+    # Extract tuple like (libname1, 0x00)
+    pattern = r"\((?P<name>\w+),\s*(?P<value1>0x[0-9a-fA-F]{2,40})\),?"
     matches = re.findall(pattern, libraries_str)
 
     if not matches:
-        logging.info(f"Libraries {libraries_str} could not be parsed")
-        return None
+        raise ValueError(
+            f"Invalid library linking directive\nGot:\n{libraries_str}\nExpected format:\n(libname1, 0x00),(libname2, 0x02)"
+        )
 
     ret: Dict[str, int] = {}
     for key, value in matches:
         ret[key] = int(value, 16) if value.startswith("0x") else int(value)
     return ret
```

### Comparing `crytic-compile-0.3.3/crytic_compile/cryticparser/cryticparser.py` & `crytic-compile-0.3.4/crytic_compile/cryticparser/cryticparser.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/cryticparser/defaults.py` & `crytic-compile-0.3.4/crytic_compile/cryticparser/defaults.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/abstract_platform.py` & `crytic-compile-0.3.4/crytic_compile/platform/abstract_platform.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/all_platforms.py` & `crytic-compile-0.3.4/crytic_compile/platform/all_platforms.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/archive.py` & `crytic-compile-0.3.4/crytic_compile/platform/archive.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/brownie.py` & `crytic-compile-0.3.4/crytic_compile/platform/brownie.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/buidler.py` & `crytic-compile-0.3.4/crytic_compile/platform/buidler.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/dapp.py` & `crytic-compile-0.3.4/crytic_compile/platform/dapp.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/embark.py` & `crytic-compile-0.3.4/crytic_compile/platform/embark.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/etherlime.py` & `crytic-compile-0.3.4/crytic_compile/platform/etherlime.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/etherscan.py` & `crytic-compile-0.3.4/crytic_compile/platform/etherscan.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,14 +295,18 @@
                 LOGGER.error("Etherscan API rate limit exceeded")
                 raise InvalidCompilation("Etherscan API rate limit exceeded")
 
             if "message" not in info:
                 LOGGER.error("Incorrect etherscan request")
                 raise InvalidCompilation("Incorrect etherscan request " + etherscan_url)
 
+            if not info["message"].startswith("OK") and "Invalid API Key" in info["result"]:
+                LOGGER.error("Invalid etherscan API Key")
+                raise InvalidCompilation("Invalid etherscan API Key: " + etherscan_url)
+
             if not info["message"].startswith("OK"):
                 LOGGER.error("Contract has no public source code")
                 raise InvalidCompilation("Contract has no public source code: " + etherscan_url)
 
             if "result" not in info:
                 LOGGER.error("Contract has no public source code")
                 raise InvalidCompilation("Contract has no public source code: " + etherscan_url)
```

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/foundry.py` & `crytic-compile-0.3.4/crytic_compile/platform/foundry.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/hardhat.py` & `crytic-compile-0.3.4/crytic_compile/platform/hardhat.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/solc.py` & `crytic-compile-0.3.4/crytic_compile/platform/solc.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,32 +30,34 @@
 
 LOGGER = logging.getLogger("CryticCompile")
 
 
 def _build_contract_data(compilation_unit: "CompilationUnit") -> Dict:
     contracts = {}
 
-    libraries = compilation_unit.crytic_compile.libraries
+    libraries_to_update = compilation_unit.crytic_compile.libraries
 
     for filename, source_unit in compilation_unit.source_units.items():
         for contract_name in source_unit.contracts_names:
+            libraries = source_unit.libraries_names_and_patterns(contract_name)
             abi = str(source_unit.abi(contract_name))
             abi = abi.replace("'", '"')
             abi = abi.replace("True", "true")
             abi = abi.replace("False", "false")
             abi = abi.replace(" ", "")
             exported_name = combine_filename_name(filename.absolute, contract_name)
             contracts[exported_name] = {
                 "srcmap": ";".join(source_unit.srcmap_init(contract_name)),
                 "srcmap-runtime": ";".join(source_unit.srcmap_runtime(contract_name)),
                 "abi": abi,
-                "bin": source_unit.bytecode_init(contract_name, libraries),
-                "bin-runtime": source_unit.bytecode_runtime(contract_name, libraries),
+                "bin": source_unit.bytecode_init(contract_name, libraries_to_update),
+                "bin-runtime": source_unit.bytecode_runtime(contract_name, libraries_to_update),
                 "userdoc": source_unit.natspec[contract_name].userdoc.export(),
                 "devdoc": source_unit.natspec[contract_name].devdoc.export(),
+                "libraries": dict(libraries) if libraries else {},
             }
     return contracts
 
 
 def export_to_solc_from_compilation_unit(
     compilation_unit: "CompilationUnit", key: str, export_dir: str
 ) -> Optional[str]:
@@ -515,24 +517,29 @@
         solc_args_ = [("--" + x).split(" ", 1) for x in solc_args if x]
         # Flat the list of list
         solc_args = [item.strip() for sublist in solc_args_ for item in sublist if item]
         cmd += solc_args
 
     additional_kwargs: Dict = {"cwd": working_dir} if working_dir else {}
     if not compiler_version.version in [f"0.4.{x}" for x in range(0, 11)]:
-        # Add . as default allowed path
+        # Add --allow-paths argument, if it isn't already specified
+        # We allow the CWD as well as the directory that contains the file
         if "--allow-paths" not in cmd:
             file_dir_start = os.path.normpath(os.path.dirname(filename))
+            # Paths in the --allow-paths arg can't contain commas, since this is the delimeter
+            # Try using absolute path; if it contains a comma, try using relative path instead
             file_dir = os.path.abspath(file_dir_start)
             if "," in file_dir:
                 try:
                     file_dir = os.path.relpath(file_dir_start)
                 except ValueError:
+                    # relpath can fail if, for example, we're on Windows and the directory is on a different drive than CWD
                     pass
 
+            # Even the relative path might have a comma in it, so we want to make sure first
             if "," not in file_dir:
                 cmd += ["--allow-paths", ".," + file_dir]
             else:
                 LOGGER.warning(
                     "Solc filepath contains a comma; omitting the --allow-paths argument. This may result in failed imports.\n"
                 )
```

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/solc_standard_json.py` & `crytic-compile-0.3.4/crytic_compile/platform/solc_standard_json.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/standard.py` & `crytic-compile-0.3.4/crytic_compile/platform/standard.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/truffle.py` & `crytic-compile-0.3.4/crytic_compile/platform/truffle.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/types.py` & `crytic-compile-0.3.4/crytic_compile/platform/types.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/vyper.py` & `crytic-compile-0.3.4/crytic_compile/platform/vyper.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/platform/waffle.py` & `crytic-compile-0.3.4/crytic_compile/platform/waffle.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/source_unit.py` & `crytic-compile-0.3.4/crytic_compile/source_unit.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/utils/naming.py` & `crytic-compile-0.3.4/crytic_compile/utils/naming.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/utils/natspec.py` & `crytic-compile-0.3.4/crytic_compile/utils/natspec.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/utils/npm.py` & `crytic-compile-0.3.4/crytic_compile/utils/npm.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/utils/subprocess.py` & `crytic-compile-0.3.4/crytic_compile/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/utils/unit_tests.py` & `crytic-compile-0.3.4/crytic_compile/utils/unit_tests.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile/utils/zip.py` & `crytic-compile-0.3.4/crytic_compile/utils/zip.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/crytic_compile.egg-info/PKG-INFO` & `crytic-compile-0.3.4/crytic_compile.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.3
+Version: 0.3.4
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -16,47 +16,65 @@
 # Crytic-compile
 [![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/crytic-compile/ci.yml?branch=master)](https://github.com/crytic/crytic-compile/actions?query=workflow%3ACI)
 [![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 [![PyPI version](https://badge.fury.io/py/crytic-compile.svg)](https://badge.fury.io/py/crytic-compile)
 
 Library to help smart contract compilation. It includes support for:
 - Direct solc compilation
+- [Foundry](https://github.com/foundry-rs/foundry/)
+- [Hardhat](https://github.com/nomiclabs/hardhat)
 - [Brownie](https://github.com/iamdefinitelyahuman/brownie)
 - [Buidler](https://github.com/nomiclabs/buidler)
 - [Dapp](https://dapp.tools/dapp/)
 - [Embark](https://embark.status.im/)
 - [Etherlime](https://github.com/LimeChain/etherlime)
 - [Etherscan](https://etherscan.io/) (including several alt-chain explorers and testnets)
-- [Foundry](https://github.com/foundry-rs/foundry/)
-- [Hardhat](https://github.com/nomiclabs/hardhat)
 - [Truffle](https://truffleframework.com/)
 - [Waffle](https://github.com/EthWorks/Waffle)
 
+To force compilation with a specific framework, use the `--compile-force-framework` flag. For example, to force compilation with Hardhat:
+
+```shell
+crytic-compile . --compile-force-framework hardhat
+```
+
 See the [Configuration](https://github.com/crytic/crytic-compile/wiki/Configuration) documentation for advanced usages.
 
 The plugin is used in Trail of Bits tools, including:
 - [Slither](https://github.com/crytic/slither)
 - [Echidna](https://github.com/crytic/echidna)
 - [Manticore](https://github.com/trailofbits/manticore/)
 - [evm-cfg-builder](https://github.com/crytic/evm_cfg_builder)
 
 
 ## Installation
 
-```bash
+```shell
 pip3 install crytic-compile
 ```
 
 ## Usage
 
-### Standalone
-```bash
+In the root directory of your project e.g. same directory as `hardhat.config.js` or `foundry.toml`, run:
+
+```shell
 crytic-compile .
 ```
 
 Crytic-compile will generate `crytic-export/contracts.json` containing the AST/ABI and bytecodes of the contracts.
 
 Run `crytic-compile --help` for more options.
 
+## Library Linking
+
+If your project uses [libraries](https://docs.soliditylang.org/en/latest/contracts.html#libraries) with external functions, they can be linked to their deployed address with the `--compile-libraries` flag. For example, if you have a library `SafeMath` deployed at `0xff`, you can link it with:
+
+
+```shell
+crytic-compile . --compile-libraries "(SafeMath, 0xff)"
+```
+
+If you are fuzzing with Echidna or Medusa, follow this [tutorial on linking libraries](https://secure-contracts.com/program-analysis/echidna/advanced/working-with-libraries.html?highlight=library#linking-libraries).
+
 ### As a library
 
 See the [library documentation](https://github.com/crytic/crytic-compile/wiki/Library-Documentation).
```

### Comparing `crytic-compile-0.3.3/crytic_compile.egg-info/SOURCES.txt` & `crytic-compile-0.3.4/crytic_compile.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,9 +44,10 @@
 crytic_compile/utils/name_collision.py
 crytic_compile/utils/naming.py
 crytic_compile/utils/natspec.py
 crytic_compile/utils/npm.py
 crytic_compile/utils/subprocess.py
 crytic_compile/utils/unit_tests.py
 crytic_compile/utils/zip.py
+tests/test_library_linking.py
 tests/test_metadata.py
 tests/test_zip_archive.py
```

### Comparing `crytic-compile-0.3.3/pyproject.toml` & `crytic-compile-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/setup.py` & `crytic-compile-0.3.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 setup(
     name="crytic-compile",
     description="Util to facilitate smart contracts compilation.",
     url="https://github.com/crytic/crytic-compile",
     author="Trail of Bits",
-    version="0.3.3",
+    version="0.3.4",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=["pycryptodome>=3.4.6", "cbor2", "solc-select>=v1.0.4"],
     extras_require={
         "test": [
             "pytest",
             "pytest-cov",
```

### Comparing `crytic-compile-0.3.3/tests/test_metadata.py` & `crytic-compile-0.3.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.3/tests/test_zip_archive.py` & `crytic-compile-0.3.4/tests/test_zip_archive.py`

 * *Files identical despite different names*

