# Comparing `tmp/hydrotoolbox-2.0.7.tar.gz` & `tmp/hydrotoolbox-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrotoolbox-2.0.7.tar", last modified: Mon Jul 24 12:03:40 2023, max compression
+gzip compressed data, was "hydrotoolbox-2.0.8.tar", last modified: Tue Aug  8 05:14:47 2023, max compression
```

## Comparing `hydrotoolbox-2.0.7.tar` & `hydrotoolbox-2.0.8.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/
--rw-rw-r--   0 tim       (1000) tim       (1000)      155 2023-06-17 22:11:44.000000 hydrotoolbox-2.0.7/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.383932 hydrotoolbox-2.0.7/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-07-24 05:53:00.000000 hydrotoolbox-2.0.7/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:11:45.000000 hydrotoolbox-2.0.7/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:14.000000 hydrotoolbox-2.0.7/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-07-24 05:53:00.000000 hydrotoolbox-2.0.7/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)       50 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.7/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1051 2022-09-28 02:43:28.000000 hydrotoolbox-2.0.7/BADGES.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1266 2023-07-24 12:03:33.000000 hydrotoolbox-2.0.7/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3187 2021-07-31 11:07:02.000000 hydrotoolbox-2.0.7/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1489 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.7/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     4457 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2997 2023-06-10 05:29:49.000000 hydrotoolbox-2.0.7/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-07-24 12:03:33.000000 hydrotoolbox-2.0.7/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.7/docs/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.7/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     2471 2023-05-13 04:19:38.000000 hydrotoolbox-2.0.7/docs/command_line.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     9636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.7/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      866 2023-06-16 14:57:14.000000 hydrotoolbox-2.0.7/docs/function_summary.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-07-03 12:45:13.000000 hydrotoolbox-2.0.7/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.7/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2022-02-08 03:38:16.000000 hydrotoolbox-2.0.7/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.7/docs/readme.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     2792 2023-07-24 12:03:34.000000 hydrotoolbox-2.0.7/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.7/pytest.ini
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      516 2023-03-01 21:50:53.000000 hydrotoolbox-2.0.7/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.383932 hydrotoolbox-2.0.7/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/
--rw-rw-r--   0 tim       (1000) tim       (1000)      181 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/__init__.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/
--rw-rw-r--   0 tim       (1000) tim       (1000)      172 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3195 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/comparison.py
--rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-01-28 18:17:47.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/example.csv
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/
--rw-rw-r--   0 tim       (1000) tim       (1000)      815 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Boughton.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      578 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/CM.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      597 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Chapman.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      571 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/EWMA.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      871 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Eckhardt.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Fixed.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      799 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Furey.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      877 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/LH.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1581 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Local.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      748 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Slide.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1459 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/UKIH.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      933 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Willems.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      323 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      840 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/five_day.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      542 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/ihacres.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      380 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/strict.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3336 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/param_estimate.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2615 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/separation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2791 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/utils.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    21293 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow_sep.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    82189 2023-03-12 15:02:23.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/hydrotoolbox.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/indices/
--rw-rw-r--   0 tim       (1000) tim       (1000)    56628 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/indices/indices.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      866 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/utils.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4457 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     2366 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       64 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      267 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       13 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/tests/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1017 2022-09-29 03:00:21.000000 hydrotoolbox-2.0.7/tests/BEC_test.sh
--rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-03-11 23:36:08.000000 hydrotoolbox-2.0.7/tests/data.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1123858 2022-02-25 03:11:09.000000 hydrotoolbox-2.0.7/tests/data_02239501.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1231005 2022-09-05 18:15:22.000000 hydrotoolbox-2.0.7/tests/data_boughton.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1248213 2022-09-05 17:47:34.000000 hydrotoolbox-2.0.7/tests/data_chapman.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1180403 2022-09-05 17:47:42.000000 hydrotoolbox-2.0.7/tests/data_cm.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1230240 2022-09-05 17:53:18.000000 hydrotoolbox-2.0.7/tests/data_eckhardt.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1170952 2022-09-05 17:56:40.000000 hydrotoolbox-2.0.7/tests/data_ewma.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1010905 2022-09-05 18:09:12.000000 hydrotoolbox-2.0.7/tests/data_five_day.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1235656 2022-09-05 18:02:10.000000 hydrotoolbox-2.0.7/tests/data_furey.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   928259 2022-09-05 17:53:27.000000 hydrotoolbox-2.0.7/tests/data_ihacres.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1235555 2022-09-05 18:09:03.000000 hydrotoolbox-2.0.7/tests/data_lh.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)      169 2022-04-06 12:39:07.000000 hydrotoolbox-2.0.7/tests/data_percentile_test.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   712817 2022-09-05 18:09:21.000000 hydrotoolbox-2.0.7/tests/data_strict.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1140492 2022-09-05 18:02:36.000000 hydrotoolbox-2.0.7/tests/data_ukih.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   914278 2022-09-05 17:56:48.000000 hydrotoolbox-2.0.7/tests/data_usgs_hysep_fixed.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1060115 2022-09-05 18:02:19.000000 hydrotoolbox-2.0.7/tests/data_usgs_hysep_local.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   913052 2022-09-05 18:02:27.000000 hydrotoolbox-2.0.7/tests/data_usgs_hysep_slide.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1234584 2022-09-05 18:08:54.000000 hydrotoolbox-2.0.7/tests/data_willems.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)    16068 2022-10-09 19:21:06.000000 hydrotoolbox-2.0.7/tests/hydrotoolbox_indices.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     2948 2022-09-29 03:00:20.000000 hydrotoolbox-2.0.7/tests/run_test.sh
--rw-rw-r--   0 tim       (1000) tim       (1000)     2055 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/tests/test_baseflow_sep.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1738 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices.inp
--rw-rw-r--   0 tim       (1000) tim       (1000)     1715 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices_percentile_test.inp
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.165843 hydrotoolbox-2.0.8/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      155 2023-08-02 21:30:08.000000 hydrotoolbox-2.0.8/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.145842 hydrotoolbox-2.0.8/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.145842 hydrotoolbox-2.0.8/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-08-02 21:30:09.000000 hydrotoolbox-2.0.8/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-08-02 21:30:09.000000 hydrotoolbox-2.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:14.000000 hydrotoolbox-2.0.8/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2652 2023-08-08 04:58:02.000000 hydrotoolbox-2.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)       50 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.8/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1051 2022-09-28 02:43:28.000000 hydrotoolbox-2.0.8/BADGES.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1290 2023-08-08 05:14:39.000000 hydrotoolbox-2.0.8/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3187 2021-07-31 11:07:02.000000 hydrotoolbox-2.0.8/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1489 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.8/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4457 2023-08-08 05:14:47.165843 hydrotoolbox-2.0.8/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2997 2023-06-10 05:29:49.000000 hydrotoolbox-2.0.8/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-08-08 05:14:39.000000 hydrotoolbox-2.0.8/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.149842 hydrotoolbox-2.0.8/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.8/docs/Makefile
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.8/docs/authors.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     2471 2023-05-13 04:19:38.000000 hydrotoolbox-2.0.8/docs/command_line.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.8/docs/contributing.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      866 2023-06-16 14:57:14.000000 hydrotoolbox-2.0.8/docs/function_summary.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-07-03 12:45:13.000000 hydrotoolbox-2.0.8/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.8/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2022-02-08 03:38:16.000000 hydrotoolbox-2.0.8/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.8/docs/readme.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2792 2023-08-08 05:14:39.000000 hydrotoolbox-2.0.8/pyproject.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.8/pytest.ini
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-08-08 05:14:47.165843 hydrotoolbox-2.0.8/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      516 2023-03-01 21:50:53.000000 hydrotoolbox-2.0.8/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.145842 hydrotoolbox-2.0.8/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.149842 hydrotoolbox-2.0.8/src/hydrotoolbox/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      181 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/__init__.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.149842 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      172 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3195 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/comparison.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-01-28 18:17:47.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/example.csv
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.149842 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      815 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Boughton.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      578 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/CM.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      597 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Chapman.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      571 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/EWMA.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      871 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Eckhardt.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Fixed.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      799 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Furey.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      877 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/LH.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1662 2023-08-08 04:57:35.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Local.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      748 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Slide.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1459 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/UKIH.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      933 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Willems.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      323 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      840 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/five_day.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      542 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/ihacres.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      380 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/strict.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3336 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/param_estimate.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2615 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/separation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2791 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/utils.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21374 2023-08-08 04:57:35.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow_sep.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    82270 2023-08-08 04:57:36.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/hydrotoolbox.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.149842 hydrotoolbox-2.0.8/src/hydrotoolbox/indices/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    56628 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/indices/indices.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      866 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.8/src/hydrotoolbox/utils.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.149842 hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4457 2023-08-08 05:14:47.000000 hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2366 2023-08-08 05:14:47.000000 hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-08-08 05:14:47.000000 hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       64 2023-08-08 05:14:47.000000 hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      267 2023-08-08 05:14:47.000000 hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       13 2023-08-08 05:14:47.000000 hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-08-08 05:14:47.165843 hydrotoolbox-2.0.8/tests/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1017 2022-09-29 03:00:21.000000 hydrotoolbox-2.0.8/tests/BEC_test.sh
+-rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-03-11 23:36:08.000000 hydrotoolbox-2.0.8/tests/data.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1123858 2022-02-25 03:11:09.000000 hydrotoolbox-2.0.8/tests/data_02239501.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1231005 2022-09-05 18:15:22.000000 hydrotoolbox-2.0.8/tests/data_boughton.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1248213 2022-09-05 17:47:34.000000 hydrotoolbox-2.0.8/tests/data_chapman.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1180403 2022-09-05 17:47:42.000000 hydrotoolbox-2.0.8/tests/data_cm.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1230240 2022-09-05 17:53:18.000000 hydrotoolbox-2.0.8/tests/data_eckhardt.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1170952 2022-09-05 17:56:40.000000 hydrotoolbox-2.0.8/tests/data_ewma.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1010905 2022-09-05 18:09:12.000000 hydrotoolbox-2.0.8/tests/data_five_day.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1235656 2022-09-05 18:02:10.000000 hydrotoolbox-2.0.8/tests/data_furey.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   928259 2022-09-05 17:53:27.000000 hydrotoolbox-2.0.8/tests/data_ihacres.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1235555 2022-09-05 18:09:03.000000 hydrotoolbox-2.0.8/tests/data_lh.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)      169 2022-04-06 12:39:07.000000 hydrotoolbox-2.0.8/tests/data_percentile_test.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   712817 2022-09-05 18:09:21.000000 hydrotoolbox-2.0.8/tests/data_strict.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1140492 2022-09-05 18:02:36.000000 hydrotoolbox-2.0.8/tests/data_ukih.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   914278 2022-09-05 17:56:48.000000 hydrotoolbox-2.0.8/tests/data_usgs_hysep_fixed.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1060115 2022-09-05 18:02:19.000000 hydrotoolbox-2.0.8/tests/data_usgs_hysep_local.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   913052 2022-09-05 18:02:27.000000 hydrotoolbox-2.0.8/tests/data_usgs_hysep_slide.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1234584 2022-09-05 18:08:54.000000 hydrotoolbox-2.0.8/tests/data_willems.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16068 2022-10-09 19:21:06.000000 hydrotoolbox-2.0.8/tests/hydrotoolbox_indices.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2948 2022-09-29 03:00:20.000000 hydrotoolbox-2.0.8/tests/run_test.sh
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2055 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.8/tests/test_baseflow_sep.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1738 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.8/tests/tsproc_hydrologic_indices.inp
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1715 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.8/tests/tsproc_hydrologic_indices_percentile_test.inp
```

### Comparing `hydrotoolbox-2.0.7/.github/workflows/python-package.yml` & `hydrotoolbox-2.0.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/.pre-commit-config.yaml` & `hydrotoolbox-2.0.8/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -74,22 +74,22 @@
 
     - repo: https://github.com/asottile/blacken-docs
       rev: 1.15.0
       hooks:
           - id: blacken-docs
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.9.0
+      rev: v3.10.1
       hooks:
           - id: pyupgrade
 
     - repo: https://github.com/commitizen-tools/commitizen
-      rev: 3.5.3
+      rev: 3.6.0
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.7
+      rev: v1.15.0
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `hydrotoolbox-2.0.7/BADGES.rst` & `hydrotoolbox-2.0.8/BADGES.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/CHANGELOG.md` & `hydrotoolbox-2.0.8/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+## v2.0.8 (2023-08-08)
+
 ## v2.0.7 (2023-07-24)
 
 ## v2.0.6 (2023-04-29)
 
 ## v2.0.5 (2023-02-14)
 
 ### Refactor
```

### Comparing `hydrotoolbox-2.0.7/CONTRIBUTING.rst` & `hydrotoolbox-2.0.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/LICENSE.txt` & `hydrotoolbox-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/PKG-INFO` & `hydrotoolbox-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrotoolbox
-Version: 2.0.7
+Version: 2.0.8
 Summary: Command line script and Python library for analysis of flow time-series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hydrotoolbox/docs/index.html#hydrotoolbox-documentation
 Project-URL: github, https://github.com/timcera/hydrotoolbox
 Project-URL: bitbucket, https://bitbucket.org/timcera/hydrotoolbox/src/main/
 Keywords: time-series,cli-app,hydrology,baseflow,hydrograph-recession,hydrographic
```

### Comparing `hydrotoolbox-2.0.7/README.rst` & `hydrotoolbox-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/docs/Makefile` & `hydrotoolbox-2.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/docs/command_line.rst` & `hydrotoolbox-2.0.8/docs/command_line.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/docs/conf.py` & `hydrotoolbox-2.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/docs/function_summary.rst` & `hydrotoolbox-2.0.8/docs/function_summary.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/docs/make.bat` & `hydrotoolbox-2.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/pyproject.toml` & `hydrotoolbox-2.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "2.0.7"
+version = "2.0.8"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
```

### Comparing `hydrotoolbox-2.0.7/setup.py` & `hydrotoolbox-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/comparison.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/comparison.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/example.csv` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/example.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Boughton.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Boughton.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/CM.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/CM.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Chapman.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Chapman.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/EWMA.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/EWMA.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Eckhardt.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Eckhardt.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Fixed.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Fixed.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Furey.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Furey.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/LH.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/LH.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Local.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import Optional
 
 import numpy as np
-from pydantic import validate_arguments
+
+try:
+    from pydantic import validate_call
+except ImportError:
+    from pydantic import validate_arguments as validate_call
 
 from .UKIH import linear_interpolation
 
 
 def Local(Q, b_LH, area=None, return_exceed=False):
     """Local minimum graphical method from HYSEP program (Sloto & Crouse, 1996)
 
@@ -16,15 +20,15 @@
     idx_turn = Local_turn(Q, hysep_interval(area))
     b = linear_interpolation(Q, idx_turn, return_exceed=return_exceed)
     b[: idx_turn[0]] = b_LH[: idx_turn[0]]
     b[idx_turn[-1] + 1 :] = b_LH[idx_turn[-1] + 1 :]
     return b
 
 
-@validate_arguments
+@validate_call
 def hysep_interval(area: Optional[float] = None) -> int:
     # The duration of surface runoff is calculated from the empirical relation:
     # N=A^0.2, (1) where N is the number of days after which surface runoff ceases,
     # and A is the drainage area in square miles (Linsley and others, 1982, p. 210).
     # The interval 2N* used for hydrograph separations is the odd integer between
     # 3 and 11 nearest to 2N (Pettyjohn and Henning, 1979, p. 31).
     N = 5 if area is None else np.power(0.3861022 * area, 0.2)
```

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Slide.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Slide.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/UKIH.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/UKIH.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Willems.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/Willems.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/five_day.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/five_day.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/ihacres.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/methods/ihacres.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/param_estimate.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/param_estimate.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/separation.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/separation.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/utils.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow/utils.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow_sep.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/baseflow_sep.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 hydrotoolbox recession """
 
 import logging
 import warnings
 
 import numpy as np
 import pandas as pd
-from pydantic import validate_arguments
+
+try:
+    from pydantic import validate_call
+except ImportError:
+    from pydantic import validate_arguments as validate_call
 from toolbox_utils import tsutils
 
 from .baseflow.separation import separation
 
 warnings.filterwarnings("ignore")
 
 tsutils.docstrings[
@@ -616,15 +620,15 @@
         clean=clean,
         source_units=source_units,
         target_units=target_units,
     )
     return bfsep(flow, "local", print_input, area=area)
 
 
-@validate_arguments
+@validate_call
 @tsutils.doc(tsutils.docstrings)
 def ihacres(
     k: float,
     C: float,
     a: float,
     input_ts="-",
     columns=None,
```

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/hydrotoolbox.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/hydrotoolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 import warnings
 from typing import Literal
 
 import numpy as np
 import pandas as pd
 from cltoolbox import Program
 from cltoolbox.rst_text_formatter import RSTHelpFormatter
-from pydantic import validate_arguments
+
+try:
+    from pydantic import validate_call
+except ImportError:
+    from pydantic import validate_arguments as validate_call
 from scipy.signal import find_peaks
 from toolbox_utils import tsutils
 
 from . import baseflow_sep
 from .baseflow.comparison import strict_baseflow
 from .baseflow.param_estimate import recession_coefficient
 from .indices import indices as ind
@@ -2011,15 +2015,15 @@
     tsutils.printiso(
         ans,
         float_format=".3f",
         headers=["Flow", f"Exceedance Time ({under_over} {time_units})"],
     )
 
 
-@validate_arguments
+@validate_call
 def exceedance_time(
     *thresholds,
     input_ts="-",
     delays=0,
     under_over="over",
     time_units: Literal["year", "month", "day", "hour", "min", "sec"] = "day",
     columns=None,
```

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/indices/indices.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/indices/indices.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox/utils.py` & `hydrotoolbox-2.0.8/src/hydrotoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/PKG-INFO` & `hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrotoolbox
-Version: 2.0.7
+Version: 2.0.8
 Summary: Command line script and Python library for analysis of flow time-series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hydrotoolbox/docs/index.html#hydrotoolbox-documentation
 Project-URL: github, https://github.com/timcera/hydrotoolbox
 Project-URL: bitbucket, https://bitbucket.org/timcera/hydrotoolbox/src/main/
 Keywords: time-series,cli-app,hydrology,baseflow,hydrograph-recession,hydrographic
```

### Comparing `hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/SOURCES.txt` & `hydrotoolbox-2.0.8/src/hydrotoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/BEC_test.sh` & `hydrotoolbox-2.0.8/tests/BEC_test.sh`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data.csv` & `hydrotoolbox-2.0.8/tests/data.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_02239501.csv` & `hydrotoolbox-2.0.8/tests/data_02239501.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_boughton.csv` & `hydrotoolbox-2.0.8/tests/data_boughton.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_chapman.csv` & `hydrotoolbox-2.0.8/tests/data_chapman.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_cm.csv` & `hydrotoolbox-2.0.8/tests/data_cm.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_eckhardt.csv` & `hydrotoolbox-2.0.8/tests/data_eckhardt.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_ewma.csv` & `hydrotoolbox-2.0.8/tests/data_ewma.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_five_day.csv` & `hydrotoolbox-2.0.8/tests/data_five_day.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_furey.csv` & `hydrotoolbox-2.0.8/tests/data_furey.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_ihacres.csv` & `hydrotoolbox-2.0.8/tests/data_ihacres.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_lh.csv` & `hydrotoolbox-2.0.8/tests/data_lh.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_strict.csv` & `hydrotoolbox-2.0.8/tests/data_strict.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_ukih.csv` & `hydrotoolbox-2.0.8/tests/data_ukih.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_usgs_hysep_fixed.csv` & `hydrotoolbox-2.0.8/tests/data_usgs_hysep_fixed.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_usgs_hysep_local.csv` & `hydrotoolbox-2.0.8/tests/data_usgs_hysep_local.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_usgs_hysep_slide.csv` & `hydrotoolbox-2.0.8/tests/data_usgs_hysep_slide.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/data_willems.csv` & `hydrotoolbox-2.0.8/tests/data_willems.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/hydrotoolbox_indices.txt` & `hydrotoolbox-2.0.8/tests/hydrotoolbox_indices.txt`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/run_test.sh` & `hydrotoolbox-2.0.8/tests/run_test.sh`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/test_baseflow_sep.py` & `hydrotoolbox-2.0.8/tests/test_baseflow_sep.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices.inp` & `hydrotoolbox-2.0.8/tests/tsproc_hydrologic_indices.inp`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices_percentile_test.inp` & `hydrotoolbox-2.0.8/tests/tsproc_hydrologic_indices_percentile_test.inp`

 * *Files identical despite different names*

