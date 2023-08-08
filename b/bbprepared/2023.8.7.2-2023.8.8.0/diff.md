# Comparing `tmp/bbprepared-2023.8.7.2.tar.gz` & `tmp/bbprepared-2023.8.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbprepared-2023.8.7.2.tar", last modified: Mon Aug  7 17:21:12 2023, max compression
+gzip compressed data, was "bbprepared-2023.8.8.0.tar", last modified: Tue Aug  8 17:49:34 2023, max compression
```

## Comparing `bbprepared-2023.8.7.2.tar` & `bbprepared-2023.8.8.0.tar`

### file list

```diff
@@ -1,79 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.015863 bbprepared-2023.8.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.003863 bbprepared-2023.8.7.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.003863 bbprepared-2023.8.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-07 17:21:12.015863 bbprepared-2023.8.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 17:21:12.015863 bbprepared-2023.8.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.003863 bbprepared-2023.8.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.007863 bbprepared-2023.8.7.2/src/bbprep/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.007863 bbprepared-2023.8.7.2/src/bbprep/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.007863 bbprepared-2023.8.7.2/src/bbprep/_internal/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/ensemble/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.007863 bbprepared-2023.8.7.2/src/bbprep/_internal/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/generators/etkdg.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/generators/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/generators/torsion_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.007863 bbprepared-2023.8.7.2/src/bbprep/_internal/processes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/processes/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/processes/planarfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/processes/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/processes/torsion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/processes/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.011863 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/all_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/binders.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/by_smarts.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/deleters.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/xcomx.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 17:21:11.000000 bbprepared-2023.8.7.2/src/bbprep/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/src/bbprep/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.011863 bbprepared-2023.8.7.2/src/bbprepared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-07 17:21:11.000000 bbprepared-2023.8.7.2/src/bbprepared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-07 17:21:11.000000 bbprepared-2023.8.7.2/src/bbprepared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:21:11.000000 bbprepared-2023.8.7.2/src/bbprepared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-07 17:21:11.000000 bbprepared-2023.8.7.2/src/bbprepared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 17:21:11.000000 bbprepared-2023.8.7.2/src/bbprepared.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.011863 bbprepared-2023.8.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.011863 bbprepared-2023.8.7.2/tests/angle_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/angle_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/angle_test/angle_molecule0_min.mol
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/angle_test/angle_molecule1_min.mol
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/angle_test/angle_molecule2_min.mol
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/angle_test/case_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/angle_test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/angle_test/test_minimiseangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.015863 bbprepared-2023.8.7.2/tests/planarfy_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/case_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule0_min.mol
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule1_min.mol
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule2_min.mol
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule3_min.mol
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/planarfy_test/test_planarfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:21:12.015863 bbprepared-2023.8.7.2/tests/torsion_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/case_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/test_targettorsion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule0_best.mol
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule1_best.mol
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule2_best.mol
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-07 17:20:11.000000 bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule3_best.mol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.587989 bbprepared-2023.8.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.571989 bbprepared-2023.8.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.571989 bbprepared-2023.8.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-08 17:49:34.583989 bbprepared-2023.8.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:49:34.587989 bbprepared-2023.8.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.567988 bbprepared-2023.8.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.571989 bbprepared-2023.8.8.0/src/bbprep/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.571989 bbprepared-2023.8.8.0/src/bbprep/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.571989 bbprepared-2023.8.8.0/src/bbprep/_internal/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/ensemble/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.571989 bbprepared-2023.8.8.0/src/bbprep/_internal/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/generators/etkdg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/generators/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/generators/torsion_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.571989 bbprepared-2023.8.8.0/src/bbprep/_internal/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/modifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/modifiers/distanced_functional_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/modifiers/modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.575989 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/ditopicfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/planarfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/torsion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/processes/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.575989 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/all_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/binders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/by_smarts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/deleters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/notplacers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/xcomx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 17:49:34.000000 bbprepared-2023.8.8.0/src/bbprep/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/src/bbprep/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.575989 bbprepared-2023.8.8.0/src/bbprepared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-08 17:49:34.000000 bbprepared-2023.8.8.0/src/bbprepared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-08 17:49:34.000000 bbprepared-2023.8.8.0/src/bbprepared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:49:34.000000 bbprepared-2023.8.8.0/src/bbprepared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-08 17:49:34.000000 bbprepared-2023.8.8.0/src/bbprepared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 17:49:34.000000 bbprepared-2023.8.8.0/src/bbprepared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.579989 bbprepared-2023.8.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.579989 bbprepared-2023.8.8.0/tests/angle_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/angle_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/angle_test/angle_molecule0_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/angle_test/angle_molecule1_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/angle_test/angle_molecule2_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/angle_test/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/angle_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/angle_test/test_minimiseangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.579989 bbprepared-2023.8.8.0/tests/distanced_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/dist_molecule0_clo.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/dist_molecule0_fur.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/dist_molecule1_clo.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/dist_molecule1_fur.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/dist_molecule2_clo.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/dist_molecule2_fur.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/test_closest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/distanced_test/test_furthest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.583989 bbprepared-2023.8.8.0/tests/ditopic_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/ditopic_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/ditopic_test/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/ditopic_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/ditopic_test/ditopic_molecule0_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/ditopic_test/ditopic_molecule1_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/ditopic_test/ditopic_molecule2_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/ditopic_test/test_ditopicfitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.583989 bbprepared-2023.8.8.0/tests/planarfy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule0_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule1_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule2_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule3_min.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/planarfy_test/test_planarfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:49:34.583989 bbprepared-2023.8.8.0/tests/torsion_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/test_targettorsion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule0_best.mol
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule1_best.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule2_best.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-08 17:48:28.000000 bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule3_best.mol
```

### Comparing `bbprepared-2023.8.7.2/.github/pull_request_template.md` & `bbprepared-2023.8.8.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/.github/workflows/publish_release.yml` & `bbprepared-2023.8.8.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/.github/workflows/tests.yml` & `bbprepared-2023.8.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/.gitignore` & `bbprepared-2023.8.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/LICENSE` & `bbprepared-2023.8.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/PKG-INFO` & `bbprepared-2023.8.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbprepared
-Version: 2023.8.7.2
+Version: 2023.8.8.0
 Maintainer-email: Andrew Tarzia <andrew.tarzia@gmail.com>
 Project-URL: github, https://github.com/andrewtarzia/bbprepared
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `bbprepared-2023.8.7.2/README.md` & `bbprepared-2023.8.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/pyproject.toml` & `bbprepared-2023.8.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/__init__.py` & `bbprepared-2023.8.8.0/src/bbprep/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from bbprep import generators, selectors
 from bbprep._internal.ensemble.ensemble import Conformer, Ensemble
+from bbprep._internal.modifiers.distanced_functional_groups import (
+    ClosestFGs,
+    FurthestFGs,
+)
+from bbprep._internal.modifiers.modifier import Modifier
 from bbprep._internal.processes.angle import MinimiseAngle
+from bbprep._internal.processes.ditopicfitter import DitopicFitter
 from bbprep._internal.processes.planarfy import Planarfy
 from bbprep._internal.processes.process import Process, TargetProcess
 from bbprep._internal.processes.torsion import TargetTorsion
 
 __all__ = [
     "generators",
     "selectors",
     "Ensemble",
+    "DitopicFitter",
     "Conformer",
     "Process",
     "TargetProcess",
     "Planarfy",
     "MinimiseAngle",
     "TargetTorsion",
+    "Modifier",
+    "FurthestFGs",
+    "ClosestFGs",
 ]
```

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/ensemble/ensemble.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/ensemble/ensemble.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/generators/etkdg.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/generators/etkdg.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/generators/torsion_scanner.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/generators/torsion_scanner.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/processes/angle.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/processes/angle.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/processes/planarfy.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/processes/planarfy.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/processes/process.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/processes/process.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/processes/torsion.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/processes/torsion.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/processes/utilities.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/processes/utilities.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/all_selector.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/all_selector.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/by_smarts.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/by_smarts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 import stk
 from rdkit.Chem import AllChem as rdkit
 
 from .selector import Selector
 
 
 class BySmartsSelector(Selector):
@@ -26,7 +28,23 @@
         )
         atoms = []
         for match in matches:
             for idx, atom_id in enumerate(match):
                 if idx in self._selected_indices:
                     atoms.append(atom_id)
         return tuple(atoms)
+
+    def yield_stepwise(
+        self,
+        molecule: stk.BuildingBlock,
+    ) -> typing.Iterator[tuple[int, ...]]:
+        rdkit_mol = molecule.to_rdkit_mol()
+        rdkit.SanitizeMol(rdkit_mol)
+        matches = rdkit_mol.GetSubstructMatches(
+            query=rdkit.MolFromSmarts(self._smarts),
+        )
+        for match in matches:
+            atoms = []
+            for idx, atom_id in enumerate(match):
+                if idx in self._selected_indices:
+                    atoms.append(atom_id)
+            yield tuple(atoms)
```

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/deleters.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/deleters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 import stk
 
 from .selector import Selector
 
 
 class DeletersSelector(Selector):
     """
@@ -21,7 +23,19 @@
 
         atoms = []
         for fg in molecule.get_functional_groups():
             for id_ in fg.get_deleter_ids():  # type: ignore[attr-defined]
                 atoms.append(id_)
 
         return tuple(atoms)
+
+    def yield_stepwise(
+        self,
+        molecule: stk.BuildingBlock,
+    ) -> typing.Iterator[tuple[int, ...]]:
+        assert molecule.get_num_functional_groups() > 0
+
+        for fg in molecule.get_functional_groups():
+            atoms = []
+            for id_ in fg.get_deleter_ids():  # type: ignore[attr-defined]
+                atoms.append(id_)
+            yield tuple(atoms)
```

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/selector.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/selector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 import numpy as np
 import stk
 
 
 class Selector:
     """
     Select atom ids in stk molecules by deleters.
@@ -14,14 +16,30 @@
 
         """
         pass
 
     def select_atoms(self, molecule: stk.BuildingBlock) -> tuple[int, ...]:
         raise NotImplementedError()
 
+    def yield_stepwise(
+        self,
+        molecule: stk.BuildingBlock,
+    ) -> typing.Iterator[tuple[int, ...]]:
+        raise NotImplementedError()
+
     def get_atomic_positions(
         self,
         molecule: stk.BuildingBlock,
     ) -> tuple[np.ndarray, ...]:
         return tuple(
             molecule.get_atomic_positions(atom_ids=self.select_atoms(molecule))
         )
+
+
+class NullSelector(Selector):
+    """
+    Selecter that does nothing.
+
+    """
+
+    def select_atoms(self, molecule: stk.BuildingBlock) -> tuple:
+        return ()
```

### Comparing `bbprepared-2023.8.7.2/src/bbprep/_internal/selectors/xcomx.py` & `bbprepared-2023.8.8.0/src/bbprep/_internal/selectors/xcomx.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/src/bbprep/selectors.py` & `bbprepared-2023.8.8.0/src/bbprep/selectors.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,23 @@
     AllNonHSelector,
     AllSelector,
 )
 from bbprep._internal.selectors.binders import BindersSelector
 from bbprep._internal.selectors.by_id import ByIdSelector
 from bbprep._internal.selectors.by_smarts import BySmartsSelector
 from bbprep._internal.selectors.deleters import DeletersSelector
-from bbprep._internal.selectors.selector import Selector
+from bbprep._internal.selectors.notplacers import NotPlacersSelector
+from bbprep._internal.selectors.selector import NullSelector, Selector
 from bbprep._internal.selectors.xcomx import XCOMXSelector
 
 __all__ = [
     "Selector",
+    "NullSelector",
     "AllSelector",
     "AllNonHSelector",
     "BindersSelector",
     "ByIdSelector",
     "BySmartsSelector",
     "DeletersSelector",
+    "NotPlacersSelector",
     "XCOMXSelector",
 ]
```

### Comparing `bbprepared-2023.8.7.2/src/bbprepared.egg-info/PKG-INFO` & `bbprepared-2023.8.8.0/src/bbprepared.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbprepared
-Version: 2023.8.7.2
+Version: 2023.8.8.0
 Maintainer-email: Andrew Tarzia <andrew.tarzia@gmail.com>
 Project-URL: github, https://github.com/andrewtarzia/bbprepared
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `bbprepared-2023.8.7.2/tests/angle_test/angle_molecule0_min.mol` & `bbprepared-2023.8.8.0/tests/angle_test/angle_molecule0_min.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/angle_test/angle_molecule1_min.mol` & `bbprepared-2023.8.8.0/tests/angle_test/angle_molecule1_min.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/angle_test/angle_molecule2_min.mol` & `bbprepared-2023.8.8.0/tests/angle_test/angle_molecule2_min.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/angle_test/case_data.py` & `bbprepared-2023.8.8.0/tests/angle_test/case_data.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/angle_test/conftest.py` & `bbprepared-2023.8.8.0/tests/angle_test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/angle_test/test_minimiseangle.py` & `bbprepared-2023.8.8.0/tests/angle_test/test_minimiseangle.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/planarfy_test/case_data.py` & `bbprepared-2023.8.8.0/tests/planarfy_test/case_data.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/planarfy_test/conftest.py` & `bbprepared-2023.8.8.0/tests/planarfy_test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule0_min.mol` & `bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule0_min.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule1_min.mol` & `bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule1_min.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule2_min.mol` & `bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule2_min.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/planarfy_test/planar_molecule3_min.mol` & `bbprepared-2023.8.8.0/tests/planarfy_test/planar_molecule3_min.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/planarfy_test/test_planarfy.py` & `bbprepared-2023.8.8.0/tests/planarfy_test/test_planarfy.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/torsion_test/case_data.py` & `bbprepared-2023.8.8.0/tests/torsion_test/case_data.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/torsion_test/conftest.py` & `bbprepared-2023.8.8.0/tests/torsion_test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/torsion_test/test_targettorsion.py` & `bbprepared-2023.8.8.0/tests/torsion_test/test_targettorsion.py`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule0_best.mol` & `bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule0_best.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule1_best.mol` & `bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule1_best.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule2_best.mol` & `bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule2_best.mol`

 * *Files identical despite different names*

### Comparing `bbprepared-2023.8.7.2/tests/torsion_test/torsion_molecule3_best.mol` & `bbprepared-2023.8.8.0/tests/torsion_test/torsion_molecule3_best.mol`

 * *Files identical despite different names*

