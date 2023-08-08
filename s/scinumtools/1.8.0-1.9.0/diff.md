# Comparing `tmp/scinumtools-1.8.0.tar.gz` & `tmp/scinumtools-1.9.0.tar.gz`

## Comparing `scinumtools-1.8.0.tar` & `scinumtools-1.9.0.tar`

### file list

```diff
@@ -1,89 +1,88 @@
--rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 scinumtools-1.8.0/build_doc.sh
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-1.8.0/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.8.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-1.8.0/.github/workflows/static.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/make.bat
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/conf.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/data.rst
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/index.rst
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/introduction.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/math.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/phys.rst
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/stats.rst
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/structs.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/modules.rst
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.data.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.math.rst
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.math.solver.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.phys.rst
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.phys.units.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.rst
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.stats.rst
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 scinumtools-1.8.0/docs/source/api/scinumtools.structs.rst
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/BaseUnitsClass.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/DimensionsClass.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/FractionClass.py
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/UnitClass.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/structs/ProgressBar.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scinumtools-1.8.0/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/cached_data.npy
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/pyproject.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/requirements.txt
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/test_stats.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/test_struct.py
--rw-r--r--   0        0        0    12551 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/test_units.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.8.0/tests/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.8.0/.gitignore
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scinumtools-1.8.0/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 scinumtools-1.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 scinumtools-1.9.0/build_doc.sh
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-1.9.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.9.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-1.9.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/make.bat
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/cached_function.rst
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/image_thumbnails.rst
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/introduction.rst
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/quantity.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.data.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.math.rst
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.math.solver.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.phys.rst
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.phys.units.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.rst
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.stats.rst
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 scinumtools-1.9.0/docs/source/api/scinumtools.structs.rst
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/data/DataPlotGridClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/data/NormalizeDataClass.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/BaseUnitsClass.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/DimensionsClass.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/FractionClass.py
+-rw-r--r--   0        0        0    13842 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/UnitClass.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/structs/ProgressBar.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scinumtools-1.9.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/cached_data.npy
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/requirements.txt
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/test_stats.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/test_struct.py
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/test_units.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.9.0/tests/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.9.0/.gitignore
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scinumtools-1.9.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 scinumtools-1.9.0/PKG-INFO
```

### Comparing `scinumtools-1.8.0/.github/workflows/python-publish.yml` & `scinumtools-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/.github/workflows/static.yml` & `scinumtools-1.9.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/Makefile` & `scinumtools-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/make.bat` & `scinumtools-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/source/conf.py` & `scinumtools-1.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/source/index.rst` & `scinumtools-1.9.0/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 =======================================
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    introduction
-   data
-   math
-   phys
-   stats
-   structs
+   cached_function
+   image_thumbnails
+   quantity
    api/modules
    
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `scinumtools-1.8.0/docs/source/introduction.rst` & `scinumtools-1.9.0/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/source/api/scinumtools.data.rst` & `scinumtools-1.9.0/docs/source/api/scinumtools.data.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/source/api/scinumtools.math.solver.rst` & `scinumtools-1.9.0/docs/source/api/scinumtools.math.solver.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/source/api/scinumtools.phys.units.rst` & `scinumtools-1.9.0/docs/source/api/scinumtools.phys.units.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/docs/source/api/scinumtools.structs.rst` & `scinumtools-1.9.0/docs/source/api/scinumtools.structs.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/__init__.py` & `scinumtools-1.9.0/src/scinumtools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import scinumtools.structs
 import scinumtools.stats
 import scinumtools.data
 import scinumtools.phys
 
 from scinumtools.data.CachingClass import CachedFunction
-from scinumtools.data.PlottingClass import NormalizeData, DataPlotGrid
+from scinumtools.data.NormalizeDataClass import NormalizeData
+from scinumtools.data.DataPlotGridClass import DataPlotGrid
 from scinumtools.data.ImageClass import ThumbnailImage
 
 from scinumtools.math.solver.SolverClass import ExpressionSolver
 from scinumtools.math.solver.AtomClass import AtomBase
 from scinumtools.math.solver.OperatorClass import *
 
 from scinumtools.phys.units.QuantityClass import Quantity
-from scinumtools.phys.units.UnitClass import Unit, Constant
+from scinumtools.phys.units.UnitClass import Unit, Constant, NaN
 from scinumtools.phys.units.DimensionsClass import Dimensions
 from scinumtools.phys.units.FractionClass import Fraction
 from scinumtools.phys.units.BaseUnitsClass import BaseUnits
 from scinumtools.phys.units.QuantityClass  import Quantity as quant
 from scinumtools.phys.units.UnitClass import Unit as unit
 from scinumtools.phys.units.UnitClass import Constant as const
+from scinumtools.phys.units.UnitClass import NaN as nan
 
 from scinumtools.stats.StopwatchClass import Stopwatch
 
 from scinumtools.structs.CollectorClass import ListCollector, ArrayCollector
 from scinumtools.structs.ParameterClass import ParameterList, ParameterDict
 from scinumtools.structs.ProgressBar import ProgressBar
```

### Comparing `scinumtools-1.8.0/src/scinumtools/data/CachingClass.py` & `scinumtools-1.9.0/src/scinumtools/data/CachingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/data/ImageClass.py` & `scinumtools-1.9.0/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/data/PlottingClass.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from matplotlib.colors import Normalize, LogNorm
 from dataclasses import dataclass
 import numpy as np
-from typing import Union
 
 from ..structs import ArrayCollector
 
 @dataclass
 class Ranges:
     """ Dataclass that contains data ranges
     """
@@ -102,43 +101,43 @@
         """ Return logarithmic norm from ranges
         """
         return LogNorm(
             vmin=np.log10(np.nanmin(self._collector.zminpos)), 
             vmax=np.log10(np.nanmax(self._collector.zmax))
         )
 
-class DataPlotGrid:
-    data: Union[list,dict]
-    ndata: int
-    ncols: int
-    nrows: int
-    figsize: tuple
-
-    def __init__(self, data: Union[list,dict], ncols:int=2, axsize:tuple=(4,2)):
-        self.data = data
-        self.ndata = len(data)
-        self.ncols = ncols
-        self.nrows = int(np.ceil(self.ndata/self.ncols))
-        self.figsize = (self.ncols*axsize[0], self.nrows*axsize[1])
-
-    def items(self, missing:bool=None, transpose:bool=False):
-        if missing:
-            for i in range(self.ndata, self.ncols*self.nrows):
-                if transpose:
-                    yield (i,int(i%self.nrows),int(i/self.nrows))
-                else:
-                    yield (i,int(i/self.ncols),int(i%self.ncols))
-        else:
-            if isinstance(self.data, list):
-                for i,d in enumerate(self.data):
-                    if transpose:
-                        yield (i,int(i%self.nrows),int(i/self.nrows),d)
-                    else:
-                        yield (i,int(i/self.ncols),int(i%self.ncols),d)
-            elif isinstance(self.data, dict):
-                for i,(k,v) in enumerate(self.data.items()):
-                    if transpose:
-                        yield (i,int(i%self.nrows),int(i/self.nrows),k,v)
-                    else:
-                        yield (i,int(i/self.ncols),int(i%self.ncols),k,v)
-            else:
-                raise Exception('Wrong data type:', self.data)
+def ListToGrid(data, ncols, missing=None, transpose=False):
+    """
+    Enumerate given data with an index and row/column number specified by number of columns
+
+    :param list data: Any iterable data, e.g. list, array
+    :param int ncols: Number of grid columns
+    :param bool missing: List only missing grid points
+    :param bool transpose: Transpose grid layout from horizontal to vertical arrangement
+    """
+    ndata = len(data)
+    nrows = int(np.ceil(ndata/ncols))
+    if missing:
+        for i in range(ndata, ncols*nrows):
+            yield (i,int(i%nrows),int(i/nrows)) if transpose else (i,int(i/ncols),int(i%ncols))
+    else:
+        for i,d in enumerate(data):
+            yield (i,int(i%nrows),int(i/nrows),d) if transpose else (i,int(i/ncols),int(i%ncols),d)
+    
+def DictToGrid(data, ncols, missing=None, transpose=False):
+    """
+    Enumerate given data with an index and row/column number specified by number of columns
+
+    :param dict data: A Python dictionary with keys and values
+    :param int ncols: Number of grid columns
+    :param bool missing: List only missing grid points
+    :param bool transpose: Transpose grid layout from horizontal to vertical arrangement
+    """
+    ndata = len(data)
+    nrows = int(np.ceil(ndata/ncols))
+    if missing:
+        for i in range(ndata, ncols*nrows):
+            yield (i,int(i%nrows),int(i/nrows)) if transpose else (i,int(i/ncols),int(i%ncols))
+    else:
+        for i,(k,v) in enumerate(data.items()):
+            yield (i,int(i%nrows),int(i/nrows),k,v) if transpose else (i,int(i/ncols),int(i%ncols),k,v)
+
```

### Comparing `scinumtools-1.8.0/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.9.0/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.9.0/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.9.0/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.9.0/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.9.0/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.9.0/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/units/BaseUnitsClass.py` & `scinumtools-1.9.0/src/scinumtools/phys/units/BaseUnitsClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         units = []
         for unit,exp in self.baseunits.items():
             symbol = unit.replace(self.symbol,'')
             if exp.num==1 and exp.den==1:
                 units.append(symbol)
             else:
                 units.append(f"{symbol}{exp}")
-        return "*".join(units)
+        if units:
+            return "*".join(units)
+        else:
+            return None
     
     def value(self):
         baseunits = {}
         for unit,exp in self.baseunits.items():
             baseunits[unit] = exp.value()
         return baseunits
```

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/units/DimensionsClass.py` & `scinumtools-1.9.0/src/scinumtools/phys/units/DimensionsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/units/FractionClass.py` & `scinumtools-1.9.0/src/scinumtools/phys/units/FractionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.9.0/src/scinumtools/phys/units/QuantityClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             self, magnitude:float,
             dimensions: Union[str,list,np.ndarray,Dimensions,dict,BaseUnits] = None,
             baseunits: Union[dict,BaseUnits] = None
     ):
         # Initialize settings
         self.unitlist = ParameterDict(['magnitude','dimensions','definition','name'], UnitStandard)
         self.prefixes = ParameterDict(['magnitude','dimensions','definition','name'], UnitPrefixes)
+        # Set magnitude
         if isinstance(magnitude, (int,float)):
             self.magnitude = float(magnitude)
         elif isinstance(magnitude, list):
             self.magnitude = np.array(magnitude, dtype=float)
         elif isinstance(magnitude, np.ndarray):
             self.magnitude = magnitude.astype(float)
         else:
@@ -44,16 +45,19 @@
             self.dimensions = Dimensions()
             self.baseunits = BaseUnits()
         elif isinstance(dimensions, (str, dict, BaseUnits)):
             if isinstance(dimensions, dict):
                 dimensions = BaseUnits(dimensions).expression()
             elif isinstance(dimensions, BaseUnits):
                 dimensions = dimensions.expression()
-            with ExpressionSolver(self._atom_parser, [OperatorPar,OperatorMul,OperatorTruediv]) as es:
-                unit = es.solve(dimensions)
+            if dimensions is None:
+                unit = Quantity(1)
+            else:
+                with ExpressionSolver(self._atom_parser, [OperatorPar,OperatorMul,OperatorTruediv]) as es:
+                    unit = es.solve(dimensions)
             self.magnitude *= unit.magnitude
             self.dimensions = unit.dimensions
             self.baseunits = unit.baseunits
         elif isinstance(dimensions, Quantity):
             self.magnitude *= dimensions.magnitude
             self.dimensions = dimensions.dimensions
             self.baseunits = dimensions.baseunits
@@ -278,21 +282,25 @@
             magnitude = magnitude**exp
             dimensions = [dim*exp for dim in dimensions]
             baseunits = {unitid: exp}            
         else:
             baseunits = {unitid: 1}
         return Quantity(magnitude, dimensions, baseunits)
     
-    def value(self, expression=None):
+    def value(self, expression=None, dtype=None):
         if expression:
-            return self.to(expression).value()
+            value = self.to(expression).value()
         elif expr:=self.baseunits.expression():
-            return (self/Quantity(1, expr)).magnitude
+            value = (self/Quantity(1, expr)).magnitude
+        else:
+            value = self.magnitude
+        if dtype:
+            return value.astype(dtype) if isinstance(value, np.ndarray) else dtype(value)
         else:
-            return self.magnitude
+            return value
 
     def units(self):
         return self.baseunits.expression()
 
     def to(self, units: Union[str,list,np.ndarray,Dimensions,dict,BaseUnits]):
         unit1 = self
         unit2 = Quantity(1,units)
@@ -335,7 +343,19 @@
 @implements(np.absolute)
 def absolute(a, **kwargs):
     return Quantity(np.absolute(a.value()), a.baseunits)
 
 @implements(np.abs)
 def abs(a, **kwargs):
     return Quantity(np.abs(a.value()), a.baseunits)
+
+@implements(np.round)
+def round(a, **kwargs):
+    return Quantity(np.round(a.value()), a.baseunits)
+
+@implements(np.floor)
+def round(a, **kwargs):
+    return Quantity(np.floor(a.value()), a.baseunits)
+
+@implements(np.ceil)
+def round(a, **kwargs):
+    return Quantity(np.ceil(a.value()), a.baseunits)
```

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/units/UnitClass.py` & `scinumtools-1.9.0/src/scinumtools/phys/units/UnitClass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 from .UnitList import UnitStandard
 from .QuantityClass import Quantity
 
 class Unit:
     
     def __enter__(self):
         return self
@@ -30,7 +32,16 @@
         if unit:
             return Quantity(1,f"[{str(unit)}]")
         else:
             return object.__new__(cls)
     
     def __getattr__(self, unit):
         return Quantity(1,f"[{str(unit)}]")
+
+class NaN:
+
+    def __new__(cls, unit=None):
+        if unit:
+            return Quantity(np.nan,str(unit))
+        else:
+            return Quantity(np.nan)
+
```

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.9.0/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.9.0/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.9.0/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.9.0/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.9.0/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/src/scinumtools/structs/ProgressBar.py` & `scinumtools-1.9.0/src/scinumtools/structs/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/cached_data.npy` & `scinumtools-1.9.0/tests/cached_data.npy`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/pyproject.toml` & `scinumtools-1.9.0/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/test_data.py` & `scinumtools-1.9.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/test_math.py` & `scinumtools-1.9.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/test_stats.py` & `scinumtools-1.9.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/test_struct.py` & `scinumtools-1.9.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/test_units.py` & `scinumtools-1.9.0/tests/test_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 from scinumtools.structs import ParameterDict
 from scinumtools.phys.units.UnitList import UnitStandard, UnitPrefixes
 from scinumtools.phys.units import *
 
 def test_quantity():
     
-    assert str(Quantity(123e2))         == "Quantity(1.230e+04)"
+    assert str(Quantity(123e2))          == "Quantity(1.230e+04)"
     q = Quantity(123e2, 'km/s')
     assert str(q) == "Quantity(1.230e+04 km*s-1)"
-    assert str(q.value())               == "12300.0"
-    assert str(q.value('m/s'))          == "12300000.0"
-    assert str(q.value({'m':1,'s':-1})) == "12300000.0"
-    assert str(q.units())               == "km*s-1"
+    assert str(q.value())                == "12300.0"
+    assert str(q.value('m/s'))           == "12300000.0"
+    assert str(q.value('m/s',dtype=int)) == "12300000"
+    assert str(q.value({'m':1,'s':-1}))  == "12300000.0"
+    assert str(q.units())                == "km*s-1"
     
     result = "Quantity(1.230e+04 m*s2:3)"
     assert str(Quantity(123e2, [1,0,(2,3),0,0,0,0,0] ))    == result
     assert str(Quantity(123e2, Dimensions(m=1, s=(2,3)) )) == result
 
     result = "Quantity(1.230e+04 J2*kg2:3)"
     assert str(Quantity(123e2, {'J': 2, 'kg':(2,3)} )) == result
@@ -191,14 +192,18 @@
     assert str(Quantity(3, 'km').to(Dimensions(m=1)))     == result
     assert str(Quantity(3, 'km').to({'m':1}))             == result
     assert str(Quantity(3, 'km').to(BaseUnits({'m':1})))  == result
     assert str(Quantity(3, 'km').to(Unit().m))            == result
 
     # reset base units if dimensions are all zero
     assert str(Quantity(3, 'kg*m2/s2')/Quantity(2, 'J')) == "Quantity(1.500e+00)"
+
+    # arithmetics of dimensionless quantities
+    q = Quantity(34)
+    assert str(q-1) == "Quantity(3.300e+01)"
     
 def test_array_arithmetics():
 
     # Test basic arithmetics
     q = Quantity([2,3,4], 'm')
     assert str(q) == "Quantity([2. 3. 4.] m)"
     q += Quantity(2, 'm')
@@ -221,15 +226,16 @@
     assert str(q) == "Quantity([1.024e+03 5.905e+04 1.049e+06] m10)"
 
     # Test unit conversion on arrays
     assert str(Quantity([1,2,3], 'm').to('km')) == "Quantity([0.001 0.002 0.003] km)"
 
     # Array slicing
     q = Quantity([1,2,3], 'm')
-    assert str(q[:2]) == "Quantity([1. 2.] m)"
+    assert str(q[:2])              == "Quantity([1. 2.] m)"
+    assert str(q.value(dtype=int)) == "[1 2 3]"
     
 def test_numpy():
     
     # Test numpy functions
     assert str(np.sqrt(Quantity(4, 'm2')))             == "Quantity(2.000e+00 m)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm2')))    == "Quantity([2. 3. 4.] m)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm3')))    == "Quantity([2. 3. 4.] m3:2)"
@@ -247,15 +253,18 @@
     assert str(np.linspace(0,Quantity(20,'m'),3))      == "Quantity([ 0. 10. 20.] m)"
     assert str(np.linspace(Quantity(10,'m'),Quantity(0.03,'km'),3))  == "Quantity([10. 20. 30.] m)"
     assert str(np.absolute(Quantity(-3,'m')))          == "Quantity(3.000e+00 m)"
     assert str(np.linspace(0,Quantity(23,'km'),3))     == "Quantity([ 0.  11.5 23. ] km)"
     assert str(np.logspace(1,Quantity(3,'m'),3))       == "Quantity([  10.  100. 1000.] m)"
     assert str(np.absolute(Quantity(-3,'m')))          == "Quantity(3.000e+00 m)"
     assert str(np.abs(Quantity(-3,'m')))               == "Quantity(3.000e+00 m)"
-
+    assert str(np.round(Quantity(2.3,'m')))            == "Quantity(2.000e+00 m)"
+    assert str(np.floor(Quantity(2.3,'m')))            == "Quantity(2.000e+00 m)"
+    assert str(np.ceil(Quantity(2.3,'m')))             == "Quantity(3.000e+00 m)"
+    
 def test_operation_sides():
     
     p = Quantity([2,3,4], 'm')
     q = Quantity([5,6,7], 'm')
     assert p+q == q+p
     assert p-q == -(q-p)
     assert q*2 == 2*q
@@ -290,7 +299,12 @@
     assert str(Quantity(2300,'Cel').to('kK'))     == "Quantity(2.573e+00 kK)"
     
 def test_inversion():
 
     assert str(Quantity(23, 'Hz').to('s'))        == "Quantity(4.348e-02 s)"
     assert str(Quantity(34, 'Ohm').to('S'))       == "Quantity(2.941e-02 S)"
     assert str(Quantity(102, 'J').to('erg-1'))    == "Quantity(9.804e-10 erg-1)"
+
+def test_nan():
+
+    assert str(NaN()) == "Quantity(nan)"
+    assert str(NaN('cm')) == "Quantity(nan cm)"
```

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/data/ImageClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.9.0/tests/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.9.0/tests/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/tests/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.9.0/tests/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/.gitignore` & `scinumtools-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.8.0/pyproject.toml` & `scinumtools-1.9.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.8.0"
+version = "1.9.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.8.0/PKG-INFO` & `scinumtools-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.8.0
+Version: 1.9.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

