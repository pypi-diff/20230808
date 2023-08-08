# Comparing `tmp/pyhtml2md-1.4.3.tar.gz` & `tmp/pyhtml2md-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml2md-1.4.3.tar", last modified: Fri May 26 09:38:42 2023, max compression
+gzip compressed data, was "pyhtml2md-1.4.4.tar", last modified: Tue Aug  8 09:23:40 2023, max compression
```

## Comparing `pyhtml2md-1.4.3.tar` & `pyhtml2md-1.4.4.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.373189 pyhtml2md-1.4.3/include/
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/include/html2md.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.373189 pyhtml2md-1.4.3/pyhtml2md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-26 09:38:42.000000 pyhtml2md-1.4.3/pyhtml2md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-26 09:38:42.000000 pyhtml2md-1.4.3/pyhtml2md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:38:42.000000 pyhtml2md-1.4.3/pyhtml2md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:38:42.000000 pyhtml2md-1.4.3/pyhtml2md.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 09:38:42.000000 pyhtml2md-1.4.3/pyhtml2md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:38:42.000000 pyhtml2md-1.4.3/pyhtml2md.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.373189 pyhtml2md-1.4.3/python/
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/python/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/python/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.377189 pyhtml2md-1.4.3/python/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.373189 pyhtml2md-1.4.3/python/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.377189 pyhtml2md-1.4.3/python/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.377189 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28518 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    53462 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    48364 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/python/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    31450 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79416 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126708 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/python/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/python/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-26 09:38:15.000000 pyhtml2md-1.4.3/python/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/src/html2md.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:38:42.381189 pyhtml2md-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/tests/test_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 09:38:13.000000 pyhtml2md-1.4.3/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.744027 pyhtml2md-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-08-08 09:23:40.744027 pyhtml2md-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.732027 pyhtml2md-1.4.4/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/include/html2md.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.732027 pyhtml2md-1.4.4/pyhtml2md.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-08-08 09:23:40.000000 pyhtml2md-1.4.4/pyhtml2md.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-08 09:23:40.000000 pyhtml2md-1.4.4/pyhtml2md.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:23:40.000000 pyhtml2md-1.4.4/pyhtml2md.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:23:40.000000 pyhtml2md-1.4.4/pyhtml2md.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 09:23:40.000000 pyhtml2md-1.4.4/pyhtml2md.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 09:23:40.000000 pyhtml2md-1.4.4/pyhtml2md.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.732027 pyhtml2md-1.4.4/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/python/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/python/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.732027 pyhtml2md-1.4.4/python/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.728027 pyhtml2md-1.4.4/python/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.740028 pyhtml2md-1.4.4/python/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.740028 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28518 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53759 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48364 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.740028 pyhtml2md-1.4.4/python/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32135 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79725 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126706 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    98078 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.740028 pyhtml2md-1.4.4/python/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.744027 pyhtml2md-1.4.4/python/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-08 09:23:26.000000 pyhtml2md-1.4.4/python/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:23:40.744027 pyhtml2md-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.744027 pyhtml2md-1.4.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/src/html2md.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:23:40.744027 pyhtml2md-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/tests/test_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 09:23:24.000000 pyhtml2md-1.4.4/tests/test_basic.py
```

### Comparing `pyhtml2md-1.4.3/CMakeLists.txt` & `pyhtml2md-1.4.4/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 cmake_minimum_required(VERSION 3.8)
-project(html2md VERSION 1.4.3
-                LANGUAGES CXX)
+project(html2md VERSION 1.4.4 LANGUAGES CXX)
 
 set(PROJECT_HOMEPAGE_URL "https://tim-gromeyer.github.io/html2md/")
 set(html2md_HOMEPAGE_URL "${PROJECT_HOMEPAGE_URL}")
 
 set(PROJECT_DESCRIPTION "Transform your HTML into clean, easy-to-read markdown with html2md")
 set(html2md_DESCRIPTION "${PROJECT_DESCRIPTION}")
```

### Comparing `pyhtml2md-1.4.3/COPYING` & `pyhtml2md-1.4.4/COPYING`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/PKG-INFO` & `pyhtml2md-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtml2md
-Version: 1.4.3
+Version: 1.4.4
 Summary: Transform your HTML into clean, easy-to-read markdown with pyhtml2md.
 Home-page: https://github.com/tim-gromeyer/html2md
 Author: Tim Gromeyer
 Author-email: sakul8826@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `pyhtml2md-1.4.3/README.md` & `pyhtml2md-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/include/html2md.h` & `pyhtml2md-1.4.4/include/html2md.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/pyhtml2md.egg-info/PKG-INFO` & `pyhtml2md-1.4.4/pyhtml2md.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtml2md
-Version: 1.4.3
+Version: 1.4.4
 Summary: Transform your HTML into clean, easy-to-read markdown with pyhtml2md.
 Home-page: https://github.com/tim-gromeyer/html2md
 Author: Tim Gromeyer
 Author-email: sakul8826@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `pyhtml2md-1.4.3/pyhtml2md.egg-info/SOURCES.txt` & `pyhtml2md-1.4.4/pyhtml2md.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 python/pybind11/include/pybind11/detail/class.h
 python/pybind11/include/pybind11/detail/common.h
 python/pybind11/include/pybind11/detail/descr.h
 python/pybind11/include/pybind11/detail/init.h
 python/pybind11/include/pybind11/detail/internals.h
 python/pybind11/include/pybind11/detail/type_caster_base.h
 python/pybind11/include/pybind11/detail/typeid.h
+python/pybind11/include/pybind11/eigen/common.h
 python/pybind11/include/pybind11/eigen/matrix.h
 python/pybind11/include/pybind11/eigen/tensor.h
 python/pybind11/include/pybind11/stl/filesystem.h
 python/pybind11/tools/FindCatch.cmake
 python/pybind11/tools/FindEigen3.cmake
 python/pybind11/tools/FindPythonLibsNew.cmake
 python/pybind11/tools/JoinPaths.cmake
```

### Comparing `pyhtml2md-1.4.3/pyproject.toml` & `pyhtml2md-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/README.md` & `pyhtml2md-1.4.4/python/README.md`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/bindings.cpp` & `pyhtml2md-1.4.4/python/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/CMakeLists.txt` & `pyhtml2md-1.4.4/python/pybind11/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     include/pybind11/buffer_info.h
     include/pybind11/cast.h
     include/pybind11/chrono.h
     include/pybind11/common.h
     include/pybind11/complex.h
     include/pybind11/options.h
     include/pybind11/eigen.h
+    include/pybind11/eigen/common.h
     include/pybind11/eigen/matrix.h
     include/pybind11/eigen/tensor.h
     include/pybind11/embed.h
     include/pybind11/eval.h
     include/pybind11/gil.h
     include/pybind11/iostream.h
     include/pybind11/functional.h
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/LICENSE` & `pyhtml2md-1.4.4/python/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/attr.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/buffer_info.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/buffer_info.h`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     std::vector<ssize_t> strides(ndim, itemsize);
     for (size_t i = 1; i < ndim; ++i) {
         strides[i] = strides[i - 1] * shape[i - 1];
     }
     return strides;
 }
 
+template <typename T, typename SFINAE = void>
+struct compare_buffer_info;
+
 PYBIND11_NAMESPACE_END(detail)
 
 /// Information record describing a Python buffer object
 struct buffer_info {
     void *ptr = nullptr;          // Pointer to the underlying storage
     ssize_t itemsize = 0;         // Size of individual items in bytes
     ssize_t size = 0;             // Total number of entries
@@ -146,14 +149,25 @@
             delete m_view;
         }
     }
 
     Py_buffer *view() const { return m_view; }
     Py_buffer *&view() { return m_view; }
 
+    /* True if the buffer item type is equivalent to `T`. */
+    // To define "equivalent" by example:
+    // `buffer_info::item_type_is_equivalent_to<int>(b)` and
+    // `buffer_info::item_type_is_equivalent_to<long>(b)` may both be true
+    // on some platforms, but `int` and `unsigned` will never be equivalent.
+    // For the ground truth, please inspect `detail::compare_buffer_info<>`.
+    template <typename T>
+    bool item_type_is_equivalent_to() const {
+        return detail::compare_buffer_info<T>::compare(*this);
+    }
+
 private:
     struct private_ctr_tag {};
 
     buffer_info(private_ctr_tag,
                 void *ptr,
                 ssize_t itemsize,
                 const std::string &format,
@@ -166,17 +180,18 @@
 
     Py_buffer *m_view = nullptr;
     bool ownview = false;
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename T, typename SFINAE = void>
+template <typename T, typename SFINAE>
 struct compare_buffer_info {
     static bool compare(const buffer_info &b) {
+        // NOLINTNEXTLINE(bugprone-sizeof-expression) Needed for `PyObject *`
         return b.format == format_descriptor<T>::format() && b.itemsize == (ssize_t) sizeof(T);
     }
 };
 
 template <typename T>
 struct compare_buffer_info<T, detail::enable_if_t<std::is_integral<T>::value>> {
     static bool compare(const buffer_info &b) {
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/cast.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/chrono.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/complex.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/class.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/common.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/common.h`

 * *Files 0% similar despite different names*

```diff
@@ -1021,14 +1021,23 @@
     assert(!PyErr_Occurred());
     throw std::runtime_error(reason);
 }
 
 template <typename T, typename SFINAE = void>
 struct format_descriptor {};
 
+template <typename T>
+struct format_descriptor<
+    T,
+    detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value>> {
+    static constexpr const char c = 'O';
+    static constexpr const char value[2] = {c, '\0'};
+    static std::string format() { return std::string(1, c); }
+};
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Returns the index of the given type in the type char array below, and in the list in numpy.h
 // The order here is: bool; 8 ints ((signed,unsigned)x(8,16,32,64)bits); float,double,long double;
 // complex float,double,long double.  Note that the long double types only participate when long
 // double is actually longer than double (it isn't under MSVC).
 // NB: not only the string below but also complex.h and numpy.h rely on this order.
 template <typename T, typename SFINAE = void>
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/descr.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/init.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/internals.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/type_caster_base.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/detail/typeid.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/eigen/matrix.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/eigen/matrix.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "../numpy.h"
+#include "common.h"
 
 /* HINT: To suppress warnings originating from the Eigen headers, use -isystem.
    See also:
        https://stackoverflow.com/questions/2579576/i-dir-vs-isystem-dir
        https://stackoverflow.com/questions/1741816/isystem-for-ms-visual-studio-c-compiler
 */
 PYBIND11_WARNING_PUSH
@@ -283,14 +284,16 @@
 }
 
 // Type caster for regular, dense matrix types (e.g. MatrixXd), but not maps/refs/etc. of dense
 // types.
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_dense_plain<Type>::value>> {
     using Scalar = typename Type::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using props = EigenProps<Type>;
 
     bool load(handle src, bool convert) {
         // If we're in no-convert mode, only load if given an array of the correct type
         if (!convert && !isinstance<array_t<Scalar>>(src)) {
             return false;
         }
@@ -401,14 +404,17 @@
 private:
     Type value;
 };
 
 // Base class for casting reference/map/block/etc. objects back to python.
 template <typename MapType>
 struct eigen_map_caster {
+    static_assert(!std::is_pointer<typename MapType::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
+
 private:
     using props = EigenProps<MapType>;
 
 public:
     // Directly referencing a ref/map's data is a bit dangerous (whatever the map/ref points to has
     // to stay around), but we'll allow it under the assumption that you know what you're doing
     // (and have an appropriate keep_alive in place).  We return a numpy array pointing directly at
@@ -453,14 +459,16 @@
     Eigen::Ref<PlainObjectType, 0, StrideType>,
     enable_if_t<is_eigen_dense_map<Eigen::Ref<PlainObjectType, 0, StrideType>>::value>>
     : public eigen_map_caster<Eigen::Ref<PlainObjectType, 0, StrideType>> {
 private:
     using Type = Eigen::Ref<PlainObjectType, 0, StrideType>;
     using props = EigenProps<Type>;
     using Scalar = typename props::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using MapType = Eigen::Map<PlainObjectType, 0, StrideType>;
     using Array
         = array_t<Scalar,
                   array::forcecast
                       | ((props::row_major ? props::inner_stride : props::outer_stride) == 1
                              ? array::c_style
                          : (props::row_major ? props::outer_stride : props::inner_stride) == 1
@@ -600,14 +608,17 @@
 
 // type_caster for special matrix types (e.g. DiagonalMatrix), which are EigenBase, but not
 // EigenDense (i.e. they don't have a data(), at least not with the usual matrix layout).
 // load() is not supported, but we can cast them into the python domain by first copying to a
 // regular Eigen::Matrix, then casting that.
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_other<Type>::value>> {
+    static_assert(!std::is_pointer<typename Type::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
+
 protected:
     using Matrix
         = Eigen::Matrix<typename Type::Scalar, Type::RowsAtCompileTime, Type::ColsAtCompileTime>;
     using props = EigenProps<Matrix>;
 
 public:
     static handle cast(const Type &src, return_value_policy /* policy */, handle /* parent */) {
@@ -628,14 +639,16 @@
     template <typename>
     using cast_op_type = Type;
 };
 
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_sparse<Type>::value>> {
     using Scalar = typename Type::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using StorageIndex = remove_reference_t<decltype(*std::declval<Type>().outerIndexPtr())>;
     using Index = typename Type::Index;
     static constexpr bool rowMajor = Type::IsRowMajor;
 
     bool load(handle src, bool) {
         if (!src) {
             return false;
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/eigen/tensor.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/eigen/tensor.h`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "../numpy.h"
+#include "common.h"
 
 #if defined(__GNUC__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
 static_assert(__GNUC__ > 5, "Eigen Tensor support in pybind11 requires GCC > 5.0");
 #endif
 
 // Disable warnings for Eigen
 PYBIND11_WARNING_PUSH
@@ -160,14 +161,16 @@
     return result;
 }
 
 PYBIND11_WARNING_POP
 
 template <typename Type>
 struct type_caster<Type, typename eigen_tensor_helper<Type>::ValidType> {
+    static_assert(!std::is_pointer<typename Type::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using Helper = eigen_tensor_helper<Type>;
     static constexpr auto temp_name = get_tensor_descriptor<Type, false>::value;
     PYBIND11_TYPE_CASTER(Type, temp_name);
 
     bool load(handle src, bool convert) {
         if (!convert) {
             if (!isinstance<array>(src)) {
@@ -355,14 +358,16 @@
 struct get_storage_pointer_type<MapType, void_t<typename MapType::PointerArgType>> {
     using SPT = typename MapType::PointerArgType;
 };
 
 template <typename Type, int Options>
 struct type_caster<Eigen::TensorMap<Type, Options>,
                    typename eigen_tensor_helper<remove_cv_t<Type>>::ValidType> {
+    static_assert(!std::is_pointer<typename Type::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using MapType = Eigen::TensorMap<Type, Options>;
     using Helper = eigen_tensor_helper<remove_cv_t<Type>>;
 
     bool load(handle src, bool /*convert*/) {
         // Note that we have a lot more checks here as we want to make sure to avoid copies
         if (!isinstance<array>(src)) {
             return false;
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/embed.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/eval.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/functional.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/gil.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/iostream.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/numpy.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/numpy.h`

 * *Files 2% similar despite different names*

```diff
@@ -560,14 +560,16 @@
         args["names"] = std::move(names);
         args["formats"] = std::move(formats);
         args["offsets"] = std::move(offsets);
         args["itemsize"] = pybind11::int_(itemsize);
         m_ptr = from_args(args).release().ptr();
     }
 
+    /// Return dtype for the given typenum (one of the NPY_TYPES).
+    /// https://numpy.org/devdocs/reference/c-api/array.html#c.PyArray_DescrFromType
     explicit dtype(int typenum)
         : object(detail::npy_api::get().PyArray_DescrFromType_(typenum), stolen_t{}) {
         if (m_ptr == nullptr) {
             throw error_already_set();
         }
     }
 
@@ -1279,20 +1281,24 @@
                                              npy_api::NPY_CFLOAT_,
                                              npy_api::NPY_CDOUBLE_,
                                              npy_api::NPY_CLONGDOUBLE_};
 
 public:
     static constexpr int value = values[detail::is_fmt_numeric<T>::index];
 
-    static pybind11::dtype dtype() {
-        if (auto *ptr = npy_api::get().PyArray_DescrFromType_(value)) {
-            return reinterpret_steal<pybind11::dtype>(ptr);
-        }
-        pybind11_fail("Unsupported buffer format!");
-    }
+    static pybind11::dtype dtype() { return pybind11::dtype(/*typenum*/ value); }
+};
+
+template <typename T>
+struct npy_format_descriptor<T, enable_if_t<is_same_ignoring_cvref<T, PyObject *>::value>> {
+    static constexpr auto name = const_name("object");
+
+    static constexpr int value = npy_api::NPY_OBJECT_;
+
+    static pybind11::dtype dtype() { return pybind11::dtype(/*typenum*/ value); }
 };
 
 #define PYBIND11_DECL_CHAR_FMT                                                                    \
     static constexpr auto name = const_name("S") + const_name<N>();                               \
     static pybind11::dtype dtype() {                                                              \
         return pybind11::dtype(std::string("S") + std::to_string(N));                             \
     }
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/operators.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/options.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/pybind11.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/pybind11.h`

 * *Files 0% similar despite different names*

```diff
@@ -504,16 +504,16 @@
             std::memset(rec->def, 0, sizeof(PyMethodDef));
             rec->def->ml_name = rec->name;
             rec->def->ml_meth
                 = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*)()>(dispatcher));
             rec->def->ml_flags = METH_VARARGS | METH_KEYWORDS;
 
             capsule rec_capsule(unique_rec.release(),
+                                detail::get_function_record_capsule_name(),
                                 [](void *ptr) { destruct((detail::function_record *) ptr); });
-            rec_capsule.set_name(detail::get_function_record_capsule_name());
             guarded_strdup.release();
 
             object scope_module;
             if (rec->scope) {
                 if (hasattr(rec->scope, "__module__")) {
                     scope_module = rec->scope.attr("__module__");
                 } else if (hasattr(rec->scope, "__name__")) {
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/pytypes.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/pytypes.h`

 * *Files 2% similar despite different names*

```diff
@@ -467,66 +467,86 @@
         return reinterpret_cast<PyTypeObject *>(obj)->tp_name;
     }
     return Py_TYPE(obj)->tp_name;
 }
 
 std::string error_string();
 
+// The code in this struct is very unusual, to minimize the chances of
+// masking bugs (elsewhere) by errors during the error handling (here).
+// This is meant to be a lifeline for troubleshooting long-running processes
+// that crash under conditions that are virtually impossible to reproduce.
+// Low-level implementation alternatives are preferred to higher-level ones
+// that might raise cascading exceptions. Last-ditch-kind-of attempts are made
+// to report as much of the original error as possible, even if there are
+// secondary issues obtaining some of the details.
 struct error_fetch_and_normalize {
-    // Immediate normalization is long-established behavior (starting with
-    // https://github.com/pybind/pybind11/commit/135ba8deafb8bf64a15b24d1513899eb600e2011
-    // from Sep 2016) and safest. Normalization could be deferred, but this could mask
-    // errors elsewhere, the performance gain is very minor in typical situations
-    // (usually the dominant bottleneck is EH unwinding), and the implementation here
-    // would be more complex.
+    // This comment only applies to Python <= 3.11:
+    //     Immediate normalization is long-established behavior (starting with
+    //     https://github.com/pybind/pybind11/commit/135ba8deafb8bf64a15b24d1513899eb600e2011
+    //     from Sep 2016) and safest. Normalization could be deferred, but this could mask
+    //     errors elsewhere, the performance gain is very minor in typical situations
+    //     (usually the dominant bottleneck is EH unwinding), and the implementation here
+    //     would be more complex.
+    // Starting with Python 3.12, PyErr_Fetch() normalizes exceptions immediately.
+    // Any errors during normalization are tracked under __notes__.
     explicit error_fetch_and_normalize(const char *called) {
         PyErr_Fetch(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
         if (!m_type) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " called while "
                             "Python error indicator not set.");
         }
         const char *exc_type_name_orig = detail::obj_class_name(m_type.ptr());
         if (exc_type_name_orig == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to obtain the name "
                             "of the original active exception type.");
         }
         m_lazy_error_string = exc_type_name_orig;
+#if PY_VERSION_HEX >= 0x030C0000
+        // The presence of __notes__ is likely due to exception normalization
+        // errors, although that is not necessarily true, therefore insert a
+        // hint only:
+        if (PyObject_HasAttrString(m_value.ptr(), "__notes__")) {
+            m_lazy_error_string += "[WITH __notes__]";
+        }
+#else
         // PyErr_NormalizeException() may change the exception type if there are cascading
         // failures. This can potentially be extremely confusing.
         PyErr_NormalizeException(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
         if (m_type.ptr() == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to normalize the "
                             "active exception.");
         }
         const char *exc_type_name_norm = detail::obj_class_name(m_type.ptr());
         if (exc_type_name_norm == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to obtain the name "
                             "of the normalized active exception type.");
         }
-#if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x07030a00
+#    if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x07030a00
         // This behavior runs the risk of masking errors in the error handling, but avoids a
         // conflict with PyPy, which relies on the normalization here to change OSError to
         // FileNotFoundError (https://github.com/pybind/pybind11/issues/4075).
         m_lazy_error_string = exc_type_name_norm;
-#else
+#    else
         if (exc_type_name_norm != m_lazy_error_string) {
             std::string msg = std::string(called)
                               + ": MISMATCH of original and normalized "
                                 "active exception types: ";
             msg += "ORIGINAL ";
             msg += m_lazy_error_string;
             msg += " REPLACED BY ";
             msg += exc_type_name_norm;
             msg += ": " + format_value_and_trace();
             pybind11_fail(msg);
         }
+#    endif
 #endif
     }
 
     error_fetch_and_normalize(const error_fetch_and_normalize &) = delete;
     error_fetch_and_normalize(error_fetch_and_normalize &&) = delete;
 
     std::string format_value_and_trace() const {
@@ -554,14 +574,48 @@
                         message_error_string = detail::error_string();
                         result = message_unavailable_exc;
                     } else {
                         result = std::string(buffer, static_cast<std::size_t>(length));
                     }
                 }
             }
+#if PY_VERSION_HEX >= 0x030B0000
+            auto notes
+                = reinterpret_steal<object>(PyObject_GetAttrString(m_value.ptr(), "__notes__"));
+            if (!notes) {
+                PyErr_Clear(); // No notes is good news.
+            } else {
+                auto len_notes = PyList_Size(notes.ptr());
+                if (len_notes < 0) {
+                    result += "\nFAILURE obtaining len(__notes__): " + detail::error_string();
+                } else {
+                    result += "\n__notes__ (len=" + std::to_string(len_notes) + "):";
+                    for (ssize_t i = 0; i < len_notes; i++) {
+                        PyObject *note = PyList_GET_ITEM(notes.ptr(), i);
+                        auto note_bytes = reinterpret_steal<object>(
+                            PyUnicode_AsEncodedString(note, "utf-8", "backslashreplace"));
+                        if (!note_bytes) {
+                            result += "\nFAILURE obtaining __notes__[" + std::to_string(i)
+                                      + "]: " + detail::error_string();
+                        } else {
+                            char *buffer = nullptr;
+                            Py_ssize_t length = 0;
+                            if (PyBytes_AsStringAndSize(note_bytes.ptr(), &buffer, &length)
+                                == -1) {
+                                result += "\nFAILURE formatting __notes__[" + std::to_string(i)
+                                          + "]: " + detail::error_string();
+                            } else {
+                                result += '\n';
+                                result += std::string(buffer, static_cast<std::size_t>(length));
+                            }
+                        }
+                    }
+                }
+            }
+#endif
         } else {
             result = "<MESSAGE UNAVAILABLE>";
         }
         if (result.empty()) {
             result = "<EMPTY MESSAGE>";
         }
 
@@ -1867,36 +1921,21 @@
     capsule(const void *value, PyCapsule_Destructor destructor)
         : object(PyCapsule_New(const_cast<void *>(value), nullptr, destructor), stolen_t{}) {
         if (!m_ptr) {
             throw error_already_set();
         }
     }
 
+    /// Capsule name is nullptr.
     capsule(const void *value, void (*destructor)(void *)) {
-        m_ptr = PyCapsule_New(const_cast<void *>(value), nullptr, [](PyObject *o) {
-            // guard if destructor called while err indicator is set
-            error_scope error_guard;
-            auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
-            if (destructor == nullptr && PyErr_Occurred()) {
-                throw error_already_set();
-            }
-            const char *name = get_name_in_error_scope(o);
-            void *ptr = PyCapsule_GetPointer(o, name);
-            if (ptr == nullptr) {
-                throw error_already_set();
-            }
-
-            if (destructor != nullptr) {
-                destructor(ptr);
-            }
-        });
+        initialize_with_void_ptr_destructor(value, nullptr, destructor);
+    }
 
-        if (!m_ptr || PyCapsule_SetContext(m_ptr, reinterpret_cast<void *>(destructor)) != 0) {
-            throw error_already_set();
-        }
+    capsule(const void *value, const char *name, void (*destructor)(void *)) {
+        initialize_with_void_ptr_destructor(value, name, destructor);
     }
 
     explicit capsule(void (*destructor)()) {
         m_ptr = PyCapsule_New(reinterpret_cast<void *>(destructor), nullptr, [](PyObject *o) {
             const char *name = get_name_in_error_scope(o);
             auto destructor = reinterpret_cast<void (*)()>(PyCapsule_GetPointer(o, name));
             if (destructor == nullptr) {
@@ -1956,14 +1995,40 @@
         if ((name == nullptr) && PyErr_Occurred()) {
             // write out and consume error raised by call to PyCapsule_GetName
             PyErr_WriteUnraisable(o);
         }
 
         return name;
     }
+
+    void initialize_with_void_ptr_destructor(const void *value,
+                                             const char *name,
+                                             void (*destructor)(void *)) {
+        m_ptr = PyCapsule_New(const_cast<void *>(value), name, [](PyObject *o) {
+            // guard if destructor called while err indicator is set
+            error_scope error_guard;
+            auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
+            if (destructor == nullptr && PyErr_Occurred()) {
+                throw error_already_set();
+            }
+            const char *name = get_name_in_error_scope(o);
+            void *ptr = PyCapsule_GetPointer(o, name);
+            if (ptr == nullptr) {
+                throw error_already_set();
+            }
+
+            if (destructor != nullptr) {
+                destructor(ptr);
+            }
+        });
+
+        if (!m_ptr || PyCapsule_SetContext(m_ptr, reinterpret_cast<void *>(destructor)) != 0) {
+            throw error_already_set();
+        }
+    }
 };
 
 class tuple : public object {
 public:
     PYBIND11_OBJECT_CVT(tuple, object, PyTuple_Check, PySequence_Tuple)
     template <typename SzType = ssize_t,
               detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/stl/filesystem.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/stl.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/stl.h`

 * *Files 2% similar despite different names*

```diff
@@ -269,19 +269,19 @@
             }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
     PYBIND11_TYPE_CASTER(ArrayType,
-                         const_name("List[") + value_conv::name
+                         const_name<Resizable>(const_name(""), const_name("Annotated["))
+                             + const_name("List[") + value_conv::name + const_name("]")
                              + const_name<Resizable>(const_name(""),
-                                                     const_name("[") + const_name<Size>()
-                                                         + const_name("]"))
-                             + const_name("]"));
+                                                     const_name(", FixedSize(")
+                                                         + const_name<Size>() + const_name(")]")));
 };
 
 template <typename Type, size_t Size>
 struct type_caster<std::array<Type, Size>>
     : array_caster<std::array<Type, Size>, Type, false, Size> {};
 
 template <typename Type>
```

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/stl_bind.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `pyhtml2md-1.4.4/python/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/FindCatch.cmake` & `pyhtml2md-1.4.4/python/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/FindEigen3.cmake` & `pyhtml2md-1.4.4/python/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/FindPythonLibsNew.cmake` & `pyhtml2md-1.4.4/python/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/JoinPaths.cmake` & `pyhtml2md-1.4.4/python/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/check-style.sh` & `pyhtml2md-1.4.4/python/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/cmake_uninstall.cmake.in` & `pyhtml2md-1.4.4/python/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pyhtml2md-1.4.4/python/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/libsize.py` & `pyhtml2md-1.4.4/python/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/make_changelog.py` & `pyhtml2md-1.4.4/python/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/pybind11Common.cmake` & `pyhtml2md-1.4.4/python/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/pybind11Config.cmake.in` & `pyhtml2md-1.4.4/python/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/pybind11NewTools.cmake` & `pyhtml2md-1.4.4/python/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/pybind11Tools.cmake` & `pyhtml2md-1.4.4/python/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/setup_global.py.in` & `pyhtml2md-1.4.4/python/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/python/pybind11/tools/setup_main.py.in` & `pyhtml2md-1.4.4/python/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyhtml2md-1.4.3/setup.py` & `pyhtml2md-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         # Set Python_EXECUTABLE instead if you use PYBIND11_FINDPYTHON
         # EXAMPLE_VERSION_INFO shows you how to pass a value into the C++ code
         # from Python.
         cmake_args = [
             f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={extdir}{os.sep}",
             f"-DPYTHON_EXECUTABLE={sys.executable}",
             f"-DCMAKE_BUILD_TYPE={cfg}",  # not used on MSVC, but no harm
-            f"-DPYTHON_BINDINGS=ON",
+            "-DPYTHON_BINDINGS=ON",
         ]
         build_args = []
         # Adding CMake arguments set as environment variable
         # (needed e.g. to build for ARM OSx on conda-forge)
         if "CMAKE_ARGS" in os.environ:
             cmake_args += [item for item in os.environ["CMAKE_ARGS"].split(" ") if item]
 
@@ -126,15 +126,15 @@
         )
 
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyhtml2md",
-    version="1.4.3",
+    version="1.4.4",
     author="Tim Gromeyer",
     author_email="sakul8826@gmail.com",
     description="Transform your HTML into clean, easy-to-read markdown with pyhtml2md.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tim-gromeyer/html2md",
     ext_modules=[CMakeExtension("pyhtml2md")],
```

### Comparing `pyhtml2md-1.4.3/src/html2md.cpp` & `pyhtml2md-1.4.4/src/html2md.cpp`

 * *Files identical despite different names*

