# Comparing `tmp/rz_bindings-0.5.1.tar.gz` & `tmp/rz_bindings-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rz_bindings-0.5.1.tar", last modified: Tue Mar  7 20:24:50 2023, max compression
+gzip compressed data, was "rz_bindings-0.6.0.tar", last modified: Tue Aug  8 07:51:16 2023, max compression
```

## Comparing `rz_bindings-0.5.1.tar` & `rz_bindings-0.6.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0       34 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/.clang-format
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/.github/workflows/release.yml
--rw-r--r--   0        0        0       27 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/.gitignore
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/.reuse/dep5
--rw-r--r--   0        0        0     7652 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/LICENSE
--rw-r--r--   0        0        0    10280 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    42098 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/LICENSES/LGPL-3.0-only.txt
--rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/LICENSES/LLVM-exception.txt
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/README.md
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cibw_before_all.sh
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/CMakeLists.txt
--rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/CutterRzBindings.cpp
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/CutterRzBindings.h
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/Python.h
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/PythonConsole.cpp
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/PythonConsole.h
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/PythonConsole.ui
--rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/PythonConsoleWriter.cpp
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/PythonConsoleWriter.h
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/cutter/util.h
--rw-r--r--   0        0        0      132 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/doc/README.md
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/doc/bin.md
--rw-r--r--   0        0        0     6310 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/doc/bin_plugin.md
--rw-r--r--   0        0        0     5928 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/doc/cmd.md
--rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/doc/core.md
--rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/doc/intro.md
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/examples/1-rz_core.py
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/examples/2a-rz_bin_plugin.py
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/examples/2b-rz_bin_plugin.py
--rw-r--r--   0        0        0     3284 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/examples/3-cle_bin_plugin.py
--rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/examples/4a-rz_cmd.py
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/examples/4b-rz_cmd.py
--rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/meson.build
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/meson_options.txt
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/mypy.ini
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/plugin/meson.build
--rw-r--r--   0        0        0     7355 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/plugin/plugin.c
--rw-r--r--   0        0        0      188 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/pylintrc
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/README.md
--rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/binding_class.py
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/binding_director.py
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/binding_enum.py
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/binding_func.py
--rw-r--r--   0        0        0     4336 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/binding_generic.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/binding_generic_specializations.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/binding_typemap.py
--rw-r--r--   0        0        0    13078 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/bindings.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/clang/__init__.py
--rw-r--r--   0        0        0   126904 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/clang/cindex.py
--rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/clang/cindex.pyi
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/clang/enumerations.py
--rw-r--r--   0        0        0     6921 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/cparser_header.py
--rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/cparser_types.py
--rw-r--r--   0        0        0    16530 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/generator_sphinx.py
--rw-r--r--   0        0        0    14384 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/generator_swig.py
--rw-r--r--   0        0        0    12614 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/lint.py
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/main.py
--rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/snippets_swig/README.md
--rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/snippets_swig/cmd_director.i
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/snippets_swig/iterators.py
--rw-r--r--   0        0        0     1183 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/snippets_swig/prologue.i
--rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/snippets_swig/register_command.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/snippets_swig/register_swig_command.cpp
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/src/writer.py
--rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 rz_bindings-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       34 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/.clang-format
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       27 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/.reuse/dep5
+-rw-r--r--   0        0        0     7652 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10280 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    42098 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/LICENSES/LGPL-3.0-only.txt
+-rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/LICENSES/LLVM-exception.txt
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/README.md
+-rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cibw_before_all.sh
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/CMakeLists.txt
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/CutterRzBindings.cpp
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/CutterRzBindings.h
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/Python.h
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/PythonConsole.cpp
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/PythonConsole.h
+-rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/PythonConsole.ui
+-rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/PythonConsoleWriter.cpp
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/PythonConsoleWriter.h
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/cutter/util.h
+-rw-r--r--   0        0        0      132 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/doc/README.md
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/doc/bin.md
+-rw-r--r--   0        0        0     6310 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/doc/bin_plugin.md
+-rw-r--r--   0        0        0     5928 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/doc/cmd.md
+-rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/doc/core.md
+-rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/doc/intro.md
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/examples/1-rz_core.py
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/examples/2a-rz_bin_plugin.py
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/examples/2b-rz_bin_plugin.py
+-rw-r--r--   0        0        0     3284 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/examples/3-cle_bin_plugin.py
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/examples/4a-rz_cmd.py
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/examples/4b-rz_cmd.py
+-rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/meson.build
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/meson_options.txt
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/mypy.ini
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/plugin/meson.build
+-rw-r--r--   0        0        0     7355 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/plugin/plugin.c
+-rw-r--r--   0        0        0      188 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/pylintrc
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/README.md
+-rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/binding_class.py
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/binding_director.py
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/binding_enum.py
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/binding_func.py
+-rw-r--r--   0        0        0     4336 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/binding_generic.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/binding_generic_specializations.py
+-rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/binding_typemap.py
+-rw-r--r--   0        0        0    12435 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/bindings.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/clang/__init__.py
+-rw-r--r--   0        0        0   126904 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/clang/cindex.py
+-rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/clang/cindex.pyi
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/clang/enumerations.py
+-rw-r--r--   0        0        0     6921 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/cparser_header.py
+-rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/cparser_types.py
+-rw-r--r--   0        0        0    16530 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/generator_sphinx.py
+-rw-r--r--   0        0        0    14384 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/generator_swig.py
+-rw-r--r--   0        0        0    12614 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/lint.py
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/main.py
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/snippets_swig/README.md
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/snippets_swig/cmd_director.i
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/snippets_swig/iterators.py
+-rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/snippets_swig/prologue.i
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/snippets_swig/register_command.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/snippets_swig/register_swig_command.cpp
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/src/writer.py
+-rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 rz_bindings-0.6.0/PKG-INFO
```

### Comparing `rz_bindings-0.5.1/.github/workflows/ci.yml` & `rz_bindings-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/.github/workflows/lint.yml` & `rz_bindings-0.6.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/.github/workflows/release.yml` & `rz_bindings-0.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/.reuse/dep5` & `rz_bindings-0.6.0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/LICENSE` & `rz_bindings-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/LICENSES/Apache-2.0.txt` & `rz_bindings-0.6.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/LICENSES/LGPL-3.0-only.txt` & `rz_bindings-0.6.0/LICENSES/LGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/LICENSES/LLVM-exception.txt` & `rz_bindings-0.6.0/LICENSES/LLVM-exception.txt`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/README.md` & `rz_bindings-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/CMakeLists.txt` & `rz_bindings-0.6.0/cutter/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/CutterRzBindings.cpp` & `rz_bindings-0.6.0/cutter/CutterRzBindings.cpp`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/CutterRzBindings.h` & `rz_bindings-0.6.0/cutter/CutterRzBindings.h`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/Python.h` & `rz_bindings-0.6.0/cutter/Python.h`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/PythonConsole.cpp` & `rz_bindings-0.6.0/cutter/PythonConsole.cpp`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/PythonConsole.h` & `rz_bindings-0.6.0/cutter/PythonConsole.h`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/PythonConsole.ui` & `rz_bindings-0.6.0/cutter/PythonConsole.ui`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/cutter/PythonConsoleWriter.cpp` & `rz_bindings-0.6.0/cutter/PythonConsoleWriter.cpp`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/doc/bin.md` & `rz_bindings-0.6.0/doc/bin.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/doc/bin_plugin.md` & `rz_bindings-0.6.0/doc/bin_plugin.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/doc/cmd.md` & `rz_bindings-0.6.0/doc/cmd.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/doc/core.md` & `rz_bindings-0.6.0/doc/core.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/doc/intro.md` & `rz_bindings-0.6.0/doc/intro.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/examples/1-rz_core.py` & `rz_bindings-0.6.0/examples/1-rz_core.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/examples/2a-rz_bin_plugin.py` & `rz_bindings-0.6.0/examples/2a-rz_bin_plugin.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/examples/2b-rz_bin_plugin.py` & `rz_bindings-0.6.0/examples/2b-rz_bin_plugin.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/examples/3-cle_bin_plugin.py` & `rz_bindings-0.6.0/examples/3-cle_bin_plugin.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/examples/4a-rz_cmd.py` & `rz_bindings-0.6.0/examples/4a-rz_cmd.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/examples/4b-rz_cmd.py` & `rz_bindings-0.6.0/examples/4b-rz_cmd.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/meson.build` & `rz_bindings-0.6.0/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('rz-bindgen', 'c', 'cpp',
-  version: '0.5.1',
+  version: '0.6.0',
   license: 'LGPL3',
   meson_version: '>=0.53.0',
   default_options: ['python.install_env=auto'])
 
 pymod = import('python')
 fs = import('fs')
 py = pymod.find_installation()
@@ -17,15 +17,15 @@
 target_sphinx = targets.contains('sphinx')
 
 doxygen_path = get_option('doxygen_path')
 
 if clang_path == ''
   llvm = dependency('llvm', required: false)
   if llvm.found()
-    clang_path = llvm.get_variable(configtool: 'libdir', default_value: 'none')
+    clang_path = llvm.get_variable(cmake: 'LLVM_LIBRARY_DIRS', configtool: 'libdir', default_value: 'none')
   elif build_machine.system() == 'darwin'
     clang_path = '/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/'
   elif build_machine.system() == 'windows'
     clang_path = import('fs').parent(find_program('clang.exe').full_path())
   else
     clang_path = '/usr/lib/'
   endif
@@ -151,7 +151,8 @@
     build_by_default: true
   )
 endif
 
 if get_option('plugin').enabled()
   subdir('plugin')
 endif
+
```

### Comparing `rz_bindings-0.5.1/plugin/meson.build` & `rz_bindings-0.6.0/plugin/meson.build`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/plugin/plugin.c` & `rz_bindings-0.6.0/plugin/plugin.c`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/README.md` & `rz_bindings-0.6.0/src/README.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/binding_class.py` & `rz_bindings-0.6.0/src/binding_class.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/binding_director.py` & `rz_bindings-0.6.0/src/binding_director.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/binding_enum.py` & `rz_bindings-0.6.0/src/binding_enum.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/binding_func.py` & `rz_bindings-0.6.0/src/binding_func.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/binding_generic.py` & `rz_bindings-0.6.0/src/binding_generic.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/binding_generic_specializations.py` & `rz_bindings-0.6.0/src/binding_generic_specializations.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/bindings.py` & `rz_bindings-0.6.0/src/bindings.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import concurrent.futures
 
 from cparser_header import HeaderBuilder, Header
 from binding_class import Class
 from binding_director import Director
 from binding_enum import Enum, MacroEnum
 from binding_generic import Generic
-from binding_typemap import buffer_len_typemap, const_buffer_len_typemap
 
 HeaderFunc = Callable[[Header], None]
 threaded_headers: OrderedDict[str, HeaderFunc] = OrderedDict()
 
 
 def threaded_header(name: str) -> Callable[[HeaderFunc], None]:
     """
@@ -150,15 +149,15 @@
     """
     analysis_h.ignore("rz_analysis_version")
 
     rz_analysis = Class(
         analysis_h,
         typedef="RzAnalysis",
         ignore_fields={"leaddrs"},
-        rename_fields={"type_links": "_type_links"},
+        rename_fields={},
     )
 
     rz_analysis_function = Class(analysis_h, typedef="RzAnalysisFunction")
     rz_analysis_function.add_method("rz_analysis_function_delete", rename="delete_self")
     rz_analysis_function.add_prefixed_methods("rz_analysis_function_")
 
     rz_analysis.add_method("rz_analysis_reflines_get", rename="get_reflines")
@@ -217,35 +216,15 @@
 
 @threaded_header("rz_util/rz_buf.h")
 def bind_buf(buf_h: Header) -> None:
     """
     RzBuf
     """
     rz_buf = Class(buf_h, typedef="RzBuffer")
-
-    # const ut8 *buffer, ut64 len
-    for name in [
-        "append_bytes",
-        "prepend_bytes",
-        "set_bytes",
-        "insert_bytes",
-        "write",
-        "write_at",
-    ]:
-        rz_buf.add_method(
-            f"rz_buf_{name}",
-            rename=name,
-            typemaps=[const_buffer_len_typemap],
-        )
-
-    # ut8 *buffer, ut64 len
-    rz_buf.add_method("rz_buf_read", rename="read", typemaps=[buffer_len_typemap])
-    rz_buf.add_method("rz_buf_read_at", rename="read_at", typemaps=[buffer_len_typemap])
-
-    rz_buf.add_method("rz_buf_seek", rename="seek")
+    rz_buf.add_prefixed_methods("rz_buf_")
 
     MacroEnum(buf_h, "RZ_BUF_SET", "RZ_BUF_CUR", "RZ_BUF_END")
 
 
 @threaded_header("rz_cmd.h")
 def bind_cmd(cmd_h: Header) -> None:
     """
```

### Comparing `rz_bindings-0.5.1/src/clang/__init__.py` & `rz_bindings-0.6.0/src/clang/__init__.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/clang/cindex.py` & `rz_bindings-0.6.0/src/clang/cindex.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/clang/cindex.pyi` & `rz_bindings-0.6.0/src/clang/cindex.pyi`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/clang/enumerations.py` & `rz_bindings-0.6.0/src/clang/enumerations.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/cparser_header.py` & `rz_bindings-0.6.0/src/cparser_header.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/cparser_types.py` & `rz_bindings-0.6.0/src/cparser_types.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/generator_sphinx.py` & `rz_bindings-0.6.0/src/generator_sphinx.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/generator_swig.py` & `rz_bindings-0.6.0/src/generator_swig.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/lint.py` & `rz_bindings-0.6.0/src/lint.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/main.py` & `rz_bindings-0.6.0/src/main.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/snippets_swig/README.md` & `rz_bindings-0.6.0/src/snippets_swig/README.md`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/snippets_swig/cmd_director.i` & `rz_bindings-0.6.0/src/snippets_swig/cmd_director.i`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/snippets_swig/iterators.py` & `rz_bindings-0.6.0/src/snippets_swig/iterators.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/snippets_swig/register_command.py` & `rz_bindings-0.6.0/src/snippets_swig/register_command.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/snippets_swig/register_swig_command.cpp` & `rz_bindings-0.6.0/src/snippets_swig/register_swig_command.cpp`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/src/writer.py` & `rz_bindings-0.6.0/src/writer.py`

 * *Files identical despite different names*

### Comparing `rz_bindings-0.5.1/PKG-INFO` & `rz_bindings-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rz-bindings
-Version: 0.5.1
+Version: 0.6.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # rz-bindgen
 
 rz-bindgen parses Rizin header files using libclang to generate SWIG .i binding files
```

