# Comparing `tmp/simuran-23.2.0.tar.gz` & `tmp/simuran-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simuran-23.2.0.tar", last modified: Mon Feb 13 11:02:27 2023, max compression
+gzip compressed data, was "simuran-23.8.0.tar", last modified: Tue Aug  8 11:44:49 2023, max compression
```

## Comparing `simuran-23.2.0.tar` & `simuran-23.8.0.tar`

### file list

```diff
@@ -1,68 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.602686 simuran-23.2.0/
--rw-rw-rw-   0        0        0    35823 2020-03-18 15:08:46.000000 simuran-23.2.0/LICENSE
--rw-rw-rw-   0        0        0     5478 2023-02-13 11:02:27.603686 simuran-23.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4344 2023-01-17 12:37:59.000000 simuran-23.2.0/README.md
--rw-rw-rw-   0        0        0      499 2023-01-17 10:13:34.000000 simuran-23.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1620 2023-02-13 11:02:27.608687 simuran-23.2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-01-17 10:13:34.000000 simuran-23.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:26.880687 simuran-23.2.0/simuran/
--rw-rw-rw-   0        0        0     1403 2023-01-17 13:05:12.000000 simuran-23.2.0/simuran/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.144685 simuran-23.2.0/simuran/analysis/
--rw-rw-rw-   0        0        0      122 2021-03-31 14:10:15.000000 simuran-23.2.0/simuran/analysis/__init__.py
--rw-rw-rw-   0        0        0     6014 2023-01-17 10:14:17.000000 simuran-23.2.0/simuran/analysis/analysis_handler.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.177686 simuran-23.2.0/simuran/analysis/custom/
--rw-rw-rw-   0        0        0       57 2022-05-09 10:19:11.000000 simuran-23.2.0/simuran/analysis/custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.234686 simuran-23.2.0/simuran/bridges/
--rw-rw-rw-   0        0        0       43 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/bridges/__init__.py
--rw-rw-rw-   0        0        0     5037 2023-02-07 09:38:32.000000 simuran-23.2.0/simuran/bridges/allen_vbn_bridge.py
--rw-rw-rw-   0        0        0     2985 2023-02-07 09:37:19.000000 simuran-23.2.0/simuran/bridges/ibl_wide_bridge.py
--rw-rw-rw-   0        0        0     4421 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/bridges/mne_bridge.py
--rw-rw-rw-   0        0        0     1339 2023-02-10 11:57:30.000000 simuran-23.2.0/simuran/bridges/neo_bridge.py
--rw-rw-rw-   0        0        0      762 2023-01-17 10:14:17.000000 simuran-23.2.0/simuran/bridges/neurochat_bridge.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.393687 simuran-23.2.0/simuran/loaders/
--rw-rw-rw-   0        0        0       56 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/loaders/__init__.py
--rw-rw-rw-   0        0        0     7351 2023-02-01 11:33:25.000000 simuran-23.2.0/simuran/loaders/allen_loader.py
--rw-rw-rw-   0        0        0     4233 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/loaders/base_loader.py
--rw-rw-rw-   0        0        0     3117 2023-01-30 11:28:35.000000 simuran-23.2.0/simuran/loaders/loader_list.py
--rw-rw-rw-   0        0        0    15921 2023-01-17 10:14:17.000000 simuran-23.2.0/simuran/loaders/neurochat_loader.py
--rw-rw-rw-   0        0        0     1813 2023-01-19 16:31:09.000000 simuran-23.2.0/simuran/loaders/nwb_loader.py
--rw-rw-rw-   0        0        0     6024 2023-02-10 11:13:19.000000 simuran-23.2.0/simuran/loaders/one_loader.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.403685 simuran-23.2.0/simuran/plot/
--rw-rw-rw-   0        0        0       52 2023-01-20 16:01:10.000000 simuran-23.2.0/simuran/plot/__init__.py
--rw-rw-rw-   0        0        0     5077 2023-01-20 15:58:46.000000 simuran-23.2.0/simuran/plot/base_plot.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.405686 simuran-23.2.0/simuran/plot/custom/
--rw-rw-rw-   0        0        0       57 2022-05-18 16:46:56.000000 simuran-23.2.0/simuran/plot/custom/__init__.py
--rw-rw-rw-   0        0        0     3966 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/plot/figure.py
--rw-rw-rw-   0        0        0     2350 2023-01-27 18:03:55.000000 simuran-23.2.0/simuran/plot/unit.py
--rw-rw-rw-   0        0        0     3977 2023-01-24 17:31:50.000000 simuran-23.2.0/simuran/recording.py
--rw-rw-rw-   0        0        0     8622 2023-02-01 14:05:31.000000 simuran-23.2.0/simuran/recording_container.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.412686 simuran-23.2.0/simuran/ui/
--rw-rw-rw-   0        0        0       54 2022-05-09 10:19:11.000000 simuran-23.2.0/simuran/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.419688 simuran-23.2.0/simuran/ui/custom/
--rw-rw-rw-   0        0        0       44 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/ui/custom/__init__.py
--rw-rw-rw-   0        0        0     7253 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/ui/custom/example_node.py
--rw-rw-rw-   0        0        0     8603 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/ui/node.py
--rw-rw-rw-   0        0        0    12897 2023-01-17 10:13:35.000000 simuran-23.2.0/simuran/ui/simuran_ui.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:26.949687 simuran-23.2.0/simuran.egg-info/
--rw-rw-rw-   0        0        0     5478 2023-02-13 11:02:26.000000 simuran-23.2.0/simuran.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1460 2023-02-13 11:02:26.000000 simuran-23.2.0/simuran.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 11:02:26.000000 simuran-23.2.0/simuran.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-02-13 11:02:26.000000 simuran-23.2.0/simuran.egg-info/entry_points.txt
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.022686 simuran-23.2.0/simuran.egg-info/large_test_resources/
--rw-rw-rw-   0        0        0     1242 2020-04-28 15:59:44.000000 simuran-23.2.0/simuran.egg-info/large_test_resources/CanCSR7_muscimol.lnk
--rw-rw-rw-   0        0        0        2 2022-07-11 16:26:09.000000 simuran-23.2.0/simuran.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      255 2023-02-13 11:02:26.000000 simuran-23.2.0/simuran.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-13 11:02:26.000000 simuran-23.2.0/simuran.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-13 11:02:27.599687 simuran-23.2.0/tests/
--rw-rw-rw-   0        0        0     1123 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_analysis.py
--rw-rw-rw-   0        0        0     1662 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_base_class.py
--rw-rw-rw-   0        0        0     2066 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_base_container.py
--rw-rw-rw-   0        0        0      461 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_loaders.py
--rw-rw-rw-   0        0        0     1534 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_logging.py
--rw-rw-rw-   0        0        0     3244 2023-01-17 10:14:17.000000 simuran-23.2.0/tests/test_neurochat.py
--rw-rw-rw-   0        0        0     1246 2023-01-17 13:11:51.000000 simuran-23.2.0/tests/test_nwb.py
--rw-rw-rw-   0        0        0     1133 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_parameters.py
--rw-rw-rw-   0        0        0      576 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_plot.py
--rw-rw-rw-   0        0        0     1093 2023-01-17 10:13:35.000000 simuran-23.2.0/tests/test_recording.py
--rw-rw-rw-   0        0        0     2667 2023-01-19 13:22:37.000000 simuran-23.2.0/tests/test_recording_container.py
--rw-rw-rw-   0        0        0     3834 2023-01-17 10:14:17.000000 simuran-23.2.0/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.483770 simuran-23.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 11:44:39.000000 simuran-23.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-08 11:44:49.483770 simuran-23.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-08-08 11:44:39.000000 simuran-23.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-08 11:44:39.000000 simuran-23.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-08 11:44:49.483770 simuran-23.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 11:44:39.000000 simuran-23.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.475770 simuran-23.8.0/simuran/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.475770 simuran-23.8.0/simuran/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/analysis/analysis_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/analysis/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.475770 simuran-23.8.0/simuran/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/bridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/bridges/allen_vbn_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/bridges/ibl_wide_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/bridges/mne_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/bridges/neo_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/bridges/neurochat_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.475770 simuran-23.8.0/simuran/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/core/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/core/base_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/core/base_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/core/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/core/param_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.479770 simuran-23.8.0/simuran/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/loaders/allen_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/loaders/base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/loaders/loader_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/loaders/neurochat_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/loaders/nwb_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/loaders/one_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.479770 simuran-23.8.0/simuran/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/plot/base_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/plot/figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/plot/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/plot/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/recording_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.479770 simuran-23.8.0/simuran/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/node_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/node_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.479770 simuran-23.8.0/simuran/ui/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/nodes/lfp_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/nodes/python_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/nodes/recording_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-08-08 11:44:39.000000 simuran-23.8.0/simuran/ui/simuran_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.475770 simuran-23.8.0/simuran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-08 11:44:49.000000 simuran-23.8.0/simuran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-08 11:44:49.000000 simuran-23.8.0/simuran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:44:49.000000 simuran-23.8.0/simuran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-08 11:44:49.000000 simuran-23.8.0/simuran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:44:49.000000 simuran-23.8.0/simuran.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-08 11:44:49.000000 simuran-23.8.0/simuran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 11:44:49.000000 simuran-23.8.0/simuran.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:44:49.483770 simuran-23.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_base_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_neurochat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_nwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_recording_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-08 11:44:39.000000 simuran-23.8.0/tests/test_signals.py
```

### Comparing `simuran-23.2.0/LICENSE` & `simuran-23.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `simuran-23.2.0/PKG-INFO` & `simuran-23.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,118 @@
-Metadata-Version: 2.1
-Name: simuran
-Version: 23.2.0
-Summary: Simultaneous Multi-region Analysis supported with a network style
-Home-page: https://github.com/seankmartin/SIMURAN
-Download-URL: https://github.com/seankmartin/SIMURAN
-Author: Sean K. Martin
-Author-email: martins7@tcd.ie
-License: GNU GPL
-Project-URL: Bug Tracker, https://github.com/seankmartin/SIMURAN/issues
-Project-URL: Documentation, https://simuran.readthedocs.io
-Keywords: neuroscience,network,gui,api
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: neurochat
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
-# SIMURAN
-
-[![Documentation Status](https://readthedocs.org/projects/simuran/badge/?version=latest)](https://simuran.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.com/seankmartin/SIMURAN.svg?branch=master)](https://app.travis-ci.com/github/seankmartin/SIMURAN)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=seankmartin_SIMURAN&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=seankmartin_SIMURAN)
-[![codecov](https://codecov.io/gh/seankmartin/SIMURAN/branch/main/graph/badge.svg?token=F67OEU0PF2)](https://codecov.io/gh/seankmartin/SIMURAN)
-[![Maintainability](https://api.codeclimate.com/v1/badges/97aa79ac8f356de695d5/maintainability)](https://codeclimate.com/github/seankmartin/SIMURAN/maintainability)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-
-![Demo of UI](demo.gif)
-
-Simultaneous Multi-Region Analysis.
-
-## Installation
-
-```Bash
-git clone https://github.com/seankmartin/SIMURAN
-cd SIMURAN
-pip install ".[neurochat]"
-```
-
-## OS specific setup
-
-### MAC OS
-
-- To use the UI, you will need to perform at least the following. brew install libpng
-- It is possible you may also need the MAC command line developer tools, but perhaps not.
-- To use doit on MAC, you will need the developer tools.
-
-## Objective
-
-Currently, this can facilitate batch processing of many neural recordings in an easy to handle way.
-Firstly, create a table which describes all of your recordings.
-Then you can filter out specific recordings which match certain criteria.
-A recording container stores these recordings which match these criteria, and provides some bridges between common neuroscience packages to facilate loading / analysing in different formats and with different packages
-
-Here, the main object is to setup Recordings (containing all information relevant to an experiment, or part of an experiment) and RecordingContainers, which are a series of Recordings.
-
-For instance, RecordingContainer could represent all t-maze running speed, spikes, etc. and associated metadata, while a Recording is an individual t-maze session.
-This can then support easy extraction of subcontainers, such as, all trials which were successful in mice expressing a particular gene - in a simple filtering method with Pandas style.
-
-Finally, these RecordingContainers can be used to facilitate batch processing of data, and establishing workflows for processing the data.
-
-### GUI - WORK IN PROGRESS
-
-Here, the focus is mostly on the Recording level, but multiple recordings can be bundled as blocks.
-
-Recordings are loaded and processed via Nodes which are established through the UI and run in a digraph fashion.
-
-## Using custom analysis code
-
-SIMURAN can use any code that is on the Python path. The easiest way to manage this is to either:
-
-1. Fork SIMURAN and place your custom analysis code in the SIMURAN package under the directory labelled custom.
-2. Place your code on path separately, such as by creating a `setup.py` file for your code, or a `pyproject.toml` file for installation.
-3. If you place python code and/or a file with the `.pth` extension in a directory named analysis in the same directory that batch_config_path is in, this `.pth` file will be automatically processed and its contents placed on path. If this option is chosen, it is recommended to store the analysis functions directly so that anyone can run the code without modification.
-4. See [examples](https://github.com/seankmartin/neuro-tools/tree/master/SIMURAN).
-
-## Inspiration
-
-1. [GitHub - seankmartin/NeuroChaT: Analysis toolset with GUI for Neuroscience](https://github.com/seankmartin/NeuroChaT)
-2. [SpikeInterface · GitHub](https://github.com/SpikeInterface)
-3. [GitHub - seankmartin/NeuroChaT_API_Scripts: A set of python neuroscience scripts which rely on the NeuroChaT API](https://github.com/seankmartin/NeuroChaT_API_Scripts)
-4. [GitHub - mne-tools/mne-python: MNE: Magnetoencephalography (MEG) and Electroencephalography (EEG) in Python](https://github.com/mne-tools/mne-python/)
-5. [Sumatra - NeuralEnsemble](http://neuralensemble.org/sumatra/)
+Metadata-Version: 2.1
+Name: simuran
+Version: 23.8.0
+Summary: Simultaneous Multi-region Analysis supported with a network style
+Home-page: https://github.com/seankmartin/SIMURAN
+Download-URL: https://github.com/seankmartin/SIMURAN
+Author: Sean K. Martin
+Author-email: martins7@tcd.ie
+License: GNU GPL
+Project-URL: Bug Tracker, https://github.com/seankmartin/SIMURAN/issues
+Project-URL: Documentation, https://simuran.readthedocs.io
+Keywords: neuroscience,network,gui,api
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: neurochat
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
+# Simuran
+
+[![Documentation Status](https://readthedocs.org/projects/simuran/badge/?version=latest)](https://simuran.readthedocs.io/en/latest/?badge=latest)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=seankmartin_SIMURAN&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=seankmartin_SIMURAN)
+[![codecov](https://codecov.io/gh/seankmartin/SIMURAN/branch/main/graph/badge.svg?token=F67OEU0PF2)](https://codecov.io/gh/seankmartin/SIMURAN)
+[![Maintainability](https://api.codeclimate.com/v1/badges/97aa79ac8f356de695d5/maintainability)](https://codeclimate.com/github/seankmartin/SIMURAN/maintainability)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+![Demo of UI](images/demo.gif)
+
+To see more details than in the README, our [read the docs](https://simuran.readthedocs.io/en/latest/) site, or the PhD thesis of Sean K. Martin.
+
+## Installation
+
+```console
+pip install simuran
+```
+
+### MAC OS
+
+- To use the UI, you will need to perform at least the following - `brew install libpng`.
+- It is possible you may also need the MAC command line developer tools.
+
+## Usage
+
+### Objective
+
+Simuran can help facilitate batch processing of many neural recordings in an easy to handle way.
+
+The main objects to setup are Recordings (containing all information relevant to an experiment, or part of an experiment) and RecordingContainers, which are a series of Recordings.
+For instance, a RecordingContainer could represent all t-maze running speed, spikes, etc. and associated metadata, while a Recording is an individual t-maze session.
+This can then support easy extraction of subcontainers, such as, all trials which were successful in mice expressing a particular gene.
+
+### API
+
+The API is built around the Recording and RecordingContainer classes, for instance, one way to load an NWB file is as follows:
+
+```python
+import simuran
+
+recording = simuran.Recording(
+    source_file=PATH_TO_NWB, loader=simuran.loader("NWB"))
+recording.load()
+recording.inspect() # See what was loaded
+```
+
+The Recording class is designed to be as flexible as possible, and can be used to load any data, as long as a loader is provided.
+The loader is a class which takes a Recording object and loads the data into it.
+Other modules include the analysis module, which allows multi-processing of analysis functions, and the base module, which contains the base classes for the API.
+The plot module contains plotting functions for general use, and also some simple figure handling (auto garbage collection, etc.).
+Finally, the bridge module contains Bridge class definitions, which are used to allow interoperability between different software tools and data formats in neuroscience.
+
+### GUI - Visual node based editor
+
+Here, the focus is mostly on the Recording level, but multiple recordings can be bundled as blocks.
+
+Recordings are loaded and processed via Nodes which are established through the UI and run in a digraph fashion.
+The UI is built using dearpygui, and supports a subset of the API via nodes, which can be expanded upon.
+
+![Demo of UI still](images/Demo2.PNG)
+
+### Examples
+
+Some examples are provided in the examples folder.
+
+## Contributing
+
+Contributions are welcome, and any issues can be raised on the github page. Please feel free to reach out to me if you have any questions.
+
+## License
+
+Simuran is distributed under the GPL-3.0 License.
+
+## Inspiration
+
+1. [NeuroChaT: Analysis toolset with GUI for Neuroscience](https://github.com/seankmartin/NeuroChaT)
+2. [SpikeInterface · GitHub](https://github.com/SpikeInterface)
+3. [A set of python neuroscience scripts which rely on the NeuroChaT API](https://github.com/seankmartin/NeuroChaT_API_Scripts)
+4. [MNE: Magnetoencephalography (MEG) and Electroencephalography (EEG) in Python](https://github.com/mne-tools/mne-python/)
+5. [Sumatra - NeuralEnsemble](http://neuralensemble.org/sumatra/)
+6. [Snakemake](https://snakemake.readthedocs.io/en/stable/)
+
+## Update coverage
+
+```console
+pytest .
+codecov -t ba31944a-6070-401e-a731-1bd2f92a5e55
+```
```

### Comparing `simuran-23.2.0/simuran/__init__.py` & `simuran-23.8.0/simuran/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-"""
-Package for multi-region analysis.
-
-To get started, a good place can be to check the supported
-data loaders, and the installed loaders:
-simuran.supported_loaders(), simuran.installed_loaders()
-
-A general flow might be something like:
-
-recording = simuran.Recording()
-recording.loader = simuran.loader("NWB")
-recording.attrs["source_file"] = PATH_TO_NWB
-recording.parse_metadata()
-recording.load()
-recording.inspect()
-"""
-from rich import inspect
-from typing import Union, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from pathlib import Path
-
-from .analysis.analysis_handler import AnalysisHandler
-from .core.base_class import BaseSimuran, NoLoader
-from .core.base_container import GenericContainer
-from .core.base_signal import BaseSignal, Eeg
-from .core.log_handler import log_exception, set_only_log_to_file
-from .core.param_handler import ParamHandler
-from .loaders.loader_list import (
-    loader_from_string,
-    supported_loaders,
-    installed_loaders,
-)
-from .plot.base_plot import despine, save_simuran_plot, set_plot_style, setup_ax
-from .plot.figure import SimuranFigure
-from .recording import Recording
-from .recording_container import RecordingContainer
-
-loader = loader_from_string
-
-
-def config_from_file(filename: Union[str, "Path"]) -> ParamHandler:
-    """Return a configuration from a filename."""
-    return ParamHandler(source_file=filename)
+"""
+Package for multi-region analysis.
+
+To get started, a good place can be to check the supported
+data loaders, and the installed loaders:
+simuran.supported_loaders(), simuran.installed_loaders()
+
+A general flow might be something like:
+
+recording = simuran.Recording()
+recording.loader = simuran.loader("NWB")
+recording.attrs["source_file"] = PATH_TO_NWB
+recording.parse_metadata()
+recording.load()
+recording.inspect()
+"""
+from rich import inspect
+from typing import Union, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+from .analysis.analysis_handler import AnalysisHandler
+from .core.base_class import BaseSimuran, NoLoader
+from .core.base_container import GenericContainer
+from .core.base_signal import BaseSignal, Eeg
+from .core.log_handler import log_exception, set_only_log_to_file
+from .core.param_handler import ParamHandler
+from .loaders.loader_list import (
+    loader_from_string,
+    supported_loaders,
+    installed_loaders,
+)
+from .plot.base_plot import despine, save_simuran_plot, set_plot_style, setup_ax
+from .plot.figure import SimuranFigure
+from .recording import Recording
+from .recording_container import RecordingContainer
+from .ui.node_factories import register_node_factory
+from skm_pyutils.table import df_from_file, df_to_file
+
+loader = loader_from_string
+
+
+def config_from_file(filename: Union[str, "Path"]) -> ParamHandler:
+    """Return a configuration from a filename."""
+    return ParamHandler(source_file=filename)
+
+
+load_config = config_from_file
+load_table = df_from_file
+save_table = df_to_file
```

### Comparing `simuran-23.2.0/simuran/analysis/analysis_handler.py` & `simuran-23.8.0/simuran/analysis/analysis_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,188 +1,185 @@
-"""This module provides functionality for performing large batch analysis."""
-
-import logging
-from dataclasses import dataclass, field
-
-import pandas as pd
-from indexed import IndexedOrderedDict
-from simuran.core.log_handler import log_exception
-from skm_pyutils.table import df_to_file
-from tqdm import tqdm
-from tqdm.notebook import tqdm as tqdm_notebook
-
-
-@dataclass
-class AnalysisHandler(object):
-    """
-    Hold functions to run and the parameters to use for them.
-
-    Attributes
-    ----------
-    fns_to_run : list of functions
-        The functions to run
-    fn_param_list : list of tuples
-        The arguments to pass to these functions.
-        The arguments are passed in order, so these are positional.
-    fn_kwargs_list : list of dicts
-        Keyword arguments to pass to the functions to run.
-    results : indexed.IndexedOrderedDict
-        The results of the function calls
-    verbose : bool
-        Whether to print more information while running the functions.
-    handle_errors : bool
-        Whether to handle errors during runtime of underlying functions,
-        or to crash on error.
-
-    Parameters
-    ----------
-    verbose : bool, optional
-        Sets the value of the verbose attribute, defaults to False.
-    handle_errors : bool, optional
-        Sets the value of the handle_errors attribute, defaults to False.
-
-    """
-
-    fns_to_run: list = field(default_factory=list)
-    fn_params_list: list = field(default_factory=list)
-    fn_kwargs_list: list = field(default_factory=list)
-    results: IndexedOrderedDict = field(default_factory=IndexedOrderedDict)
-    verbose: bool = False
-    handle_errors: bool = False
-    _was_error: bool = field(repr=False, default=False)
-
-    def run_all(self, pbar=False):
-        """Alias for run_all_fns."""
-        self.run_all_fns(pbar)
-
-    def run_all_fns(self, pbar=False):
-        """
-        Run all of the established functions.
-
-        Parameters
-        ----------
-        pbar : string or bool, optional
-            Whether to have a progress bar. Options are
-            False (default) no progress bar.
-            True a tdqm progress bat
-            "notebook" a progress for notebooks
-
-        Returns
-        -------
-        None
-
-        """
-        self._was_error = False
-        pbar_ = None
-        if pbar is True:
-            pbar_ = tqdm(range(len(self.fns_to_run)))
-        elif pbar == "notebook":
-            pbar_ = tqdm_notebook(range(len(self.fns_to_run)))  # pragma no cover
-
-        if pbar_ is not None:
-            for i in pbar_:
-                fn = self.fns_to_run[i]
-                fn_params = self.fn_params_list[i]
-                fn_kwargs = self.fn_kwargs_list[i]
-                self._run_fn(fn, *fn_params, **fn_kwargs)
-        else:
-            fn_zipped = zip(self.fns_to_run, self.fn_params_list, self.fn_kwargs_list)
-            for (fn, fn_params, fn_kwargs) in fn_zipped:
-                self._run_fn(fn, *fn_params, **fn_kwargs)
-        if self._was_error:
-            logging.warning("A handled error occurred while running analysis")
-        self._was_error = False
-
-    def reset(self):
-        """Reset this object, clearing results and function list."""
-        self.fns_to_run = []
-        self.fn_params_list = []
-        self.fn_kwargs_list = []
-        self.results = IndexedOrderedDict()
-
-    def add_fn(self, fn, *args, **kwargs):
-        """
-        Add the function fn to the list with the given args and kwargs.
-
-        Parameters
-        ----------
-        fn : function
-            The function to add.
-        *args : positional arguments
-            The positional arguments to run the function with.
-        **kwargs : keyword arguments
-            The keyword arguments to run the function with.
-
-        Returns
-        -------
-        None
-
-        """
-        self.fns_to_run.append(fn)
-        self.fn_params_list.append(args)
-        self.fn_kwargs_list.append(kwargs)
-
-    def save_results_to_table(self, filename=None, columns=None, from_dict=True):
-        """
-        Dump analysis results to file with pickle.
-
-        Parameters
-        ----------
-        filename : str or Path
-            The output path.
-
-        Returns
-        -------
-        Dataframe
-            The resulting dataframe
-
-        """
-        if from_dict:
-            df = pd.DataFrame.from_dict(self.results, orient="index", columns=columns)
-        else:
-            df = pd.DataFrame(self.results)
-
-        if filename is not None:
-            df_to_file(df, filename)
-
-        return df
-
-    def _run_fn(self, fn, *args, **kwargs):
-        """
-        Run the function with *args and **kwargs, not usually publicly called.
-
-        Pass simuran_save_result as a keyword argument to control
-        if the result of the function is saved or not.
-
-        Parameters
-        ----------
-        fn : function
-            The function to run.
-
-        Returns
-        -------
-        object
-            The return value of the function
-
-        """
-        if self.verbose:
-            print(f"Running {fn} with params {args} kwargs {kwargs}")
-        if self.handle_errors:
-            try:
-                result = fn(*args, **kwargs)
-            except BaseException as e:
-                log_exception(
-                    e, f"Running {fn.__name__} with args {args} and kwargs {kwargs}"
-                )
-                self._was_error = True
-                result = "SIMURAN-ERROR"
-        else:
-            result = fn(*args, **kwargs)
-        ctr = 1
-        save_result = kwargs.get("simuran_save_result", True)
-        save_name = str(fn.__name__)
-        if save_result:
-            while save_name in self.results.keys():
-                save_name = f"{str(fn.__name__)}_{ctr}"
-                ctr = ctr + 1
-            self.results[save_name] = result
-        return result
+"""This module provides functionality for performing large batch analysis."""
+
+import logging
+from dataclasses import dataclass, field
+import pickle
+from typing import Union, Optional, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+import pandas as pd
+from indexed import IndexedOrderedDict
+from skm_pyutils.table import df_to_file
+from mpire import WorkerPool
+
+
+@dataclass
+class AnalysisHandler(object):
+    """
+    Hold functions to run and the parameters to use for them.
+
+    Attributes
+    ----------
+    fns_to_run : list of functions
+        The functions to run
+    fn_param_list : list of tuples
+        The arguments to pass to these functions.
+        The arguments are passed in order, so these are positional.
+    fn_kwargs_list : list of dicts
+        Keyword arguments to pass to the functions to run.
+    results : indexed.IndexedOrderedDict
+        The results of the function calls
+    verbose : bool
+        Whether to print more information while running the functions.
+    handle_errors : bool
+        Whether to handle errors during runtime of underlying functions,
+        or to crash on error.
+
+    Parameters
+    ----------
+    verbose : bool, optional
+        Sets the value of the verbose attribute, defaults to False.
+    handle_errors : bool, optional
+        Sets the value of the handle_errors attribute, defaults to False.
+
+    """
+
+    fns_to_run: list = field(default_factory=list)
+    fn_params_list: list = field(default_factory=list)
+    verbose: bool = False
+    handle_errors: bool = False
+    pickle_path: Optional[Union[str, "Path"]] = "simuran_analysis.pkl"
+    results: IndexedOrderedDict = field(default_factory=IndexedOrderedDict, init=False)
+    _was_error: bool = field(repr=False, default=False)
+
+    def run(
+        self,
+        pbar: bool = False,
+        n_jobs: int = 1,
+        save_every: int = 0,
+        force_mp: bool = False,
+    ):
+        """
+        Run all of the established functions.
+
+        Parameters
+        ----------
+        pbar : string or bool, optional
+            Whether to have a progress bar. Options are
+            False (default) no progress bar.
+            True a tdqm progress bat
+            "notebook" a progress for notebooks
+        n_jobs : int, optional
+            The number of jobs to run in parallel, by default 1
+            Uses mpire.WorkerPool along with a mapping.
+            For more complex multiprocessing, directly use mpire.WorkerPool.
+        save_every : int, optional
+            Save the results to a pickle file every n jobs, by default 0
+            If 0, then no saving occurs.
+        force_mp : bool, optional
+            Force multiprocessing, by default False
+
+        Returns
+        -------
+        None
+
+        """
+        results = []
+        self._was_error = False
+        for fn_, args_ in zip(self.fns_to_run, self.fn_params_list):
+            if n_jobs == 1 and not force_mp:
+                for arg_tuple in args_:
+                    kwargs = {}
+                    args = []
+                    for val in arg_tuple:
+                        if isinstance(val, dict):
+                            kwargs.update(val)
+                        else:
+                            args.append(val)
+                    result = fn_(*args, **kwargs)
+                    self._handle_result(fn_, result)
+                    if save_every > 0 and len(self.results) % save_every == 0:
+                        self.save_results_to_pickle()
+                    results.append(result)
+            else:
+                with WorkerPool(n_jobs=n_jobs) as pool:
+                    for result in pool.imap(fn_, args_, progress_bar=pbar):
+                        self._handle_result(fn_, result)
+                        if save_every > 0 and len(self.results) % save_every == 0:
+                            self.save_results_to_pickle()
+                        results.append(result)
+
+        if self._was_error:
+            logging.warning("A handled error occurred while running analysis")
+        self._was_error = False
+        return results
+
+    def reset(self):
+        """Reset this object, clearing results and function list."""
+        self.fns_to_run = []
+        self.fn_params_list = []
+        self.fn_kwargs_list = []
+        self.results = IndexedOrderedDict()
+
+    def add_analysis(self, fn, args):
+        """
+        Add the function fn to the list with the given args and kwargs.
+
+        Parameters
+        ----------
+        fn : function
+            The function to add.
+        args : positional arguments
+            The list of arguments to run the function with.
+            See https://slimmer-ai.github.io/mpire/usage/map/map.html
+            For more information on how arguments are handled.
+
+        Returns
+        -------
+        None
+
+        """
+        self.fns_to_run.append(fn)
+        self.fn_params_list.append(args)
+
+    def save_results_to_table(self, filename=None, columns=None, from_dict=True):
+        """
+        Dump analysis results to csv file.
+
+        Parameters
+        ----------
+        filename : str or Path
+            The output path.
+
+        Returns
+        -------
+        Dataframe
+            The resulting dataframe
+
+        """
+        if from_dict:
+            df = pd.DataFrame.from_dict(self.results, orient="index", columns=columns)
+        else:
+            df = pd.DataFrame(self.results)
+
+        if filename is not None:
+            df_to_file(df, filename)
+
+        return df
+
+    def save_results_to_pickle(self):
+        with open(self.pickle_path, "wb") as f:
+            pickle.dump(self.results, f)
+
+    def load_results_from_pickle(self):
+        with open(self.pickle_path, "rb") as f:
+            self.results = pickle.load(f)
+
+    def _handle_result(self, fn_, result):
+        ctr = 1
+        save_name = str(fn_.__name__)
+        while save_name in self.results.keys():
+            save_name = f"{str(fn_.__name__)}_{ctr}"
+            ctr = ctr + 1
+        self.results[save_name] = result
```

### Comparing `simuran-23.2.0/simuran/bridges/neo_bridge.py` & `simuran-23.8.0/simuran/bridges/neo_bridge.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-from typing import Union, Dict, List
-import numpy as np
-from neo.core import SpikeTrain
-import quantities
-
-
-def convert_spikes_to_train(
-    spikes: Union[Dict[str, np.ndarray], List[np.ndarray]],
-    units: quantities.Quantity = quantities.s,
-    custom_t_stop: float = None,
-    **kwargs
-) -> List["SpikeTrain"]:
-    """
-    Convert a list of spike times or dict of spike times to list of SpikeTrain.
-
-    Parameters
-    ----------
-    spikes: list or dict of spike times
-        The times can be lists or np.ndarray
-    units: quantities.Quantity
-        The time unit.
-    custom_t_stop: float
-        The t_stop to use for all SpikeTrain objects.
-    kwargs: dict
-        Additional arguments to pass to neo.SpikeTrain.
-
-    Returns
-    -------
-    list
-        list of neo.SpikeTrain objects
-
-    """
-    l = []
-    if hasattr(spikes, "values"):
-        to_iter = spikes.values()
-    else:
-        to_iter = spikes
-    if custom_t_stop is not None:
-        max_ = custom_t_stop
-    else:
-        max_ = 0
-        for v in to_iter:
-            if len(v) == 0:
-                continue
-            max_temp = max(v)
-            if max_temp > max_:
-                max_ = max_temp
-    for v in to_iter:
-        l.append(SpikeTrain(v, units=units, t_stop=max_, **kwargs))
-
-    return l
+from typing import Union, Dict, List
+from dataclasses import dataclass, field
+import numpy as np
+from neo.core import SpikeTrain
+import quantities
+
+
+@dataclass
+class NeoBridge(object):
+    """A class to bridge between other tools and Neo"""
+
+    @staticmethod
+    def convert_spikes(
+        spikes: Union[Dict[str, np.ndarray], List[np.ndarray]],
+        units: quantities.Quantity = quantities.s,
+        custom_t_stop: float = None,
+        **kwargs
+    ) -> List["SpikeTrain"]:
+        """
+        Convert a list of spike times or dict of spike times to list of SpikeTrain.
+
+        Parameters
+        ----------
+        spikes: list or dict of spike times
+            The times can be lists or np.ndarray
+        units: quantities.Quantity
+            The time unit.
+        custom_t_stop: float
+            The t_stop to use for all SpikeTrain objects.
+        kwargs: dict
+            Additional arguments to pass to neo.SpikeTrain.
+
+        Returns
+        -------
+        list
+            list of neo.SpikeTrain objects
+
+        """
+        l = []
+        if hasattr(spikes, "values"):
+            to_iter = spikes.values()
+        else:
+            to_iter = spikes
+        if custom_t_stop is not None:
+            max_ = custom_t_stop
+        else:
+            max_ = 0
+            for v in to_iter:
+                if len(v) == 0:
+                    continue
+                max_temp = max(v)
+                if max_temp > max_:
+                    max_ = max_temp
+        for v in to_iter:
+            l.append(SpikeTrain(v, units=units, t_stop=max_, **kwargs))
+
+        return l
```

### Comparing `simuran-23.2.0/simuran/bridges/neurochat_bridge.py` & `simuran-23.8.0/simuran/bridges/neurochat_bridge.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import TYPE_CHECKING
-
-import numpy as np
-from neurochat.nc_lfp import NLfp
-
-if TYPE_CHECKING:
-    from simuran.core.base_signal import BaseSignal
-
-
-def signal_to_neurochat(signal: "BaseSignal") -> "NLfp":
-    """Convert BaseSignal to NeuroChaT NLfp object."""
-
-    if signal.data is not None and type(signal.data) == NLfp:
-        return signal.data
-
-    lfp = NLfp()
-    lfp.set_channel_id(signal.channel)
-    signal.fill_timestamps()
-    lfp._timestamp = np.array(signal.timestamps)
-    # Neurochat assumes mV signal
-    lfp._samples = np.array(signal.samples) * signal.conversion * 1000
-    lfp._record_info["Sampling rate"] = signal.sampling_rate
-    lfp._record_info["No of samples"] = len(signal.samples)
-    return lfp
+from typing import TYPE_CHECKING
+
+import numpy as np
+from neurochat.nc_lfp import NLfp
+
+if TYPE_CHECKING:
+    from simuran.core.base_signal import BaseSignal
+
+
+def signal_to_neurochat(signal: "BaseSignal") -> "NLfp":
+    """Convert BaseSignal to NeuroChaT NLfp object."""
+
+    if signal.data is not None and type(signal.data) == NLfp:
+        return signal.data
+
+    lfp = NLfp()
+    lfp.set_channel_id(signal.channel)
+    signal.fill_timestamps()
+    lfp._timestamp = np.array(signal.timestamps)
+    # Neurochat assumes mV signal
+    lfp._samples = np.array(signal.samples) * signal.conversion * 1000
+    lfp._record_info["Sampling rate"] = signal.sampling_rate
+    lfp._record_info["No of samples"] = len(signal.samples)
+    return lfp
```

### Comparing `simuran-23.2.0/simuran/loaders/allen_loader.py` & `simuran-23.8.0/simuran/loaders/allen_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,215 +1,232 @@
-from pathlib import Path
-from dataclasses import dataclass, field
-from os.path import isfile, splitext
-from pathlib import Path
-from typing import Type, Union, Optional, TYPE_CHECKING
-
-from allensdk.brain_observatory.behavior.behavior_project_cache.project_cache_base import (
-    ProjectCacheBase,
-)
-from allensdk.brain_observatory.behavior.behavior_project_cache import (
-    VisualBehaviorOphysProjectCache,
-    VisualBehaviorNeuropixelsProjectCache,
-)
-import pandas as pd
-
-from simuran.loaders.base_loader import MetadataLoader
-from simuran.recording import Recording
-
-if TYPE_CHECKING:
-    from pandas import DataFrame
-
-
-@dataclass
-class BaseAllenLoader(MetadataLoader):
-    cache_class_type: Type[ProjectCacheBase]
-    cache_directory: Union[str, Path]
-    manifest: Optional[str]
-    cache: Optional["ProjectCacheBase"] = None
-
-    def create_s3_cache(self):
-        """Create an instance of the cache class for s3."""
-        self.cache = self.cache_class_type.from_s3_cache(cache_dir=self.cache_directory)
-        if self.manifest is not None:
-            self.cache.load_manifest(self.manifest)
-
-    def create_local_cache(self):
-        """Create an instance of the cache class for local data only."""
-        self.cache = self.cache_class_type.from_local_cache(self.cache_directory)
-        if self.manifest is not None:
-            self.cache.load_manifest(self.manifest)
-
-    def path_to_nwb(self, recording: "Recording") -> str:
-        """Return the path to the nwb file for a given recording."""
-        name_dict = self._map_class_to_values()
-        t, session_name = name_dict["t"], name_dict["session_name"]
-        id_ = name_dict["id"]
-        manifest_file = self.cache.current_manifest()
-        manifest_version = splitext(manifest_file)[0].split("_")[-1][1:]
-        id_ = recording.attrs[id_]
-
-        path_start = (
-            Path(self.cache.fetch_api.cache._cache_dir)
-            / f"visual-behavior-{t}-{manifest_version}"
-            / session_name
-        )
-        if session_name == "behavior_ecephys_sessions":
-            return path_start / str(id_) / f"{session_name[9:-1]}_{id_}.nwb"
-        else:
-            return path_start / f"{session_name[:-1]}_{id_}.nwb"
-
-    def parse_metadata(self, recording: "Recording") -> None:
-        """
-        Parse the information into the recording object.
-
-        In this case, pulls out some information from the
-        session table about this recording.
-
-        Parameters
-        ----------
-        recording: simuran.Recording
-            The recording object to parse into.
-
-        Returns
-        -------
-        None
-
-        """
-        recording.source_file = self.path_to_nwb(recording)
-        recording.attrs["downloaded"] = isfile(recording.source_file)
-        recording.attrs["id_name"] = self._map_class_to_values()["id"]
-
-    def load_recording(self, recording: "Recording") -> "Recording":
-        """Load a recording into memory using AllenSDK."""
-        t = self._map_class_to_values()
-        experiment_id = recording.attrs[t["id"]]
-        try:
-            if t["unique"] == 1:
-                experiment = self.cache.get_behavior_ophys_experiment(experiment_id)
-            elif t["unique"] == 2:
-                experiment = self.cache.get_ecephys_session(
-                    ecephys_session_id=experiment_id
-                )
-        except FileNotFoundError:
-            fpath = self.path_to_nwb(recording)
-            print(f"Please download {fpath} before trying to load it.")
-            return recording
-        recording.data = experiment
-        return recording
-
-    def get_units(self) -> "DataFrame":
-        all_units = self.cache.get_unit_table()
-        channels = self.cache.get_channel_table()
-        merged_units = all_units.merge(
-            channels,
-            left_on="ecephys_channel_id",
-            right_index=True,
-            suffixes=(None, "_y"),
-        )
-        return merged_units
-
-    def get_sessions_table(self) -> "DataFrame":
-        allen_sessions = self.cache.get_ecephys_session_table()
-        allen_sessions = allen_sessions.dropna(subset=["file_id"])
-        return allen_sessions
-
-    def _map_class_to_values(self):
-        name_dict = {}
-        if self.cache_class_type.__name__ == "VisualBehaviorOphysProjectCache":
-            name_dict["session_name"] = "behavior_ophys_experiments"
-            name_dict["t"] = "ophys"
-            name_dict["id"] = "ophys_experiment_id"
-            name_dict["unique"] = 1
-        elif self.cache_class_type.__name__ == "VisualBehaviorNeuropixelsProjectCache":
-            if (self.manifest is not None) and ("0.4.0" in self.manifest):
-                name_dict["session_name"] = "behavior_ecephys_sessions"
-            else:
-                name_dict["session_name"] = "ecephys_sessions"
-            name_dict["t"] = "neuropixels"
-            name_dict["id"] = "ecephys_session_id"
-            name_dict["unique"] = 2
-        else:
-            raise ValueError(f"Unsupported cache type {self.cache_class_type.__name__}")
-
-        return name_dict
-
-
-@dataclass
-class AllenOphysLoader(BaseAllenLoader):
-    """
-    Load AIS ophys data VBO from a cache.
-
-    Attributes
-    ----------
-    cache : VisualBehaviorOphysProjectCache
-        The AIS ophys cache to load data from.
-
-    Parameters
-    ----------
-    cache_directory : str
-        Where to store the cached data.
-    manifest : str
-        The name of the .json manifest file to use (version).
-    local : bool
-        If true, instantiate a local cache over
-
-    """
-
-    cache: Optional["VisualBehaviorOphysProjectCache"] = None
-    cache_class_type: Type[ProjectCacheBase] = field(
-        repr=False, init=False, default=VisualBehaviorOphysProjectCache
-    )
-    local: bool = False
-
-    def __post_init__(self):
-        if self.cache is not None:
-            return
-        if self.local:
-            self.create_local_cache()
-        else:
-            self.create_s3_cache()
-
-
-@dataclass
-class AllenVisualBehaviorLoader(BaseAllenLoader):
-    """
-    Load AIS VBN dataset.
-
-    Attributes
-    ----------
-    cache : VisualBehaviorOphysProjectCache
-        The AIS ophys cache to load data from.
-
-    Parameters
-    ----------
-    cache_directory : str
-        Where to store the cached data.
-    manifest : str
-        The name of the .json manifest file to use (version).
-    local : bool
-        If true, instantiate a local cache over
-    """
-
-    cache: Optional["VisualBehaviorNeuropixelsProjectCache"] = None
-    cache_class_type: Type[ProjectCacheBase] = field(
-        repr=False, init=False, default=VisualBehaviorNeuropixelsProjectCache
-    )
-    local: bool = False
-
-    def __post_init__(self):
-        if self.cache is not None:
-            return
-        if self.local:
-            self.create_local_cache()
-        else:
-            self.create_s3_cache()
-
-    def get_all_units(self):
-        all_units = self.cache.get_unit_table()
-        channels = self.cache.get_channel_table()
-        return all_units.merge(
-            channels,
-            left_on="ecephys_channel_id",
-            right_index=True,
-            suffixes=(None, "_y"),
-        )
+from pathlib import Path
+from dataclasses import dataclass, field
+from os.path import isfile, splitext
+from pathlib import Path
+from typing import Type, Union, Optional, TYPE_CHECKING
+
+from allensdk.brain_observatory.behavior.behavior_project_cache.project_cache_base import (
+    ProjectCacheBase,
+)
+from allensdk.brain_observatory.behavior.behavior_project_cache import (
+    VisualBehaviorOphysProjectCache,
+    VisualBehaviorNeuropixelsProjectCache,
+)
+import pandas as pd
+
+from simuran.loaders.base_loader import MetadataLoader
+from simuran.recording import Recording
+
+if TYPE_CHECKING:
+    from pandas import DataFrame
+
+
+@dataclass
+class BaseAllenLoader(MetadataLoader):
+    cache_class_type: Type[ProjectCacheBase]
+    cache_directory: Union[str, Path]
+    manifest: Optional[str] = None
+    cache: Optional["ProjectCacheBase"] = None
+
+    def create_s3_cache(self):
+        """Create an instance of the cache class for s3."""
+        self.cache = self.cache_class_type.from_s3_cache(cache_dir=self.cache_directory)
+        if self.manifest is not None:
+            self.cache.load_manifest(self.manifest)
+
+    def create_local_cache(self):
+        """Create an instance of the cache class for local data only."""
+        self.cache = self.cache_class_type.from_local_cache(self.cache_directory)
+        if self.manifest is not None:
+            self.cache.load_manifest(self.manifest)
+
+    def path_to_nwb(
+        self, recording: Optional["Recording"] = None, session_id: Optional[int] = None
+    ) -> str:
+        """Return the path to the nwb file for a given recording."""
+        name_dict = self._map_class_to_values()
+        t, session_name = name_dict["t"], name_dict["session_name"]
+        manifest_file = self.cache.current_manifest()
+        manifest_version = splitext(manifest_file)[0].split("_")[-1][1:]
+        if session_id is not None:
+            id_ = session_id
+        elif recording is not None:
+            id_ = name_dict["id"]
+            id_ = recording.attrs[id_]
+        else:
+            raise ValueError("Must provide either recording or session_id")
+
+        path_start = (
+            Path(self.cache.fetch_api.cache._cache_dir)
+            / f"visual-behavior-{t}-{manifest_version}"
+            / session_name
+        )
+        if session_name == "behavior_ecephys_sessions":
+            return path_start / str(id_) / f"{session_name[9:-1]}_{id_}.nwb"
+        else:
+            return path_start / f"{session_name[:-1]}_{id_}.nwb"
+
+    def parse_metadata(self, recording: "Recording") -> None:
+        """
+        Parse the information into the recording object.
+
+        In this case, pulls out some information from the
+        session table about this recording.
+
+        Parameters
+        ----------
+        recording: simuran.Recording
+            The recording object to parse into.
+
+        Returns
+        -------
+        None
+
+        """
+        recording.source_file = self.path_to_nwb(recording)
+        recording.attrs["downloaded"] = isfile(recording.source_file)
+        recording.attrs["id_name"] = self._map_class_to_values()["id"]
+
+    def load_recording(self, recording: "Recording") -> "Recording":
+        """Load a recording into memory using AllenSDK."""
+        t = self._map_class_to_values()
+        experiment_id = recording.attrs[t["id"]]
+        try:
+            if t["unique"] == 1:
+                experiment = self.cache.get_behavior_ophys_experiment(experiment_id)
+            elif t["unique"] == 2:
+                experiment = self.cache.get_ecephys_session(
+                    ecephys_session_id=experiment_id
+                )
+        except FileNotFoundError:
+            fpath = self.path_to_nwb(recording)
+            print(f"Please download {fpath} before trying to load it.")
+            return recording
+        recording.data = experiment
+        return recording
+
+    def get_units(self) -> "DataFrame":
+        all_units = self.cache.get_unit_table()
+        channels = self.cache.get_channel_table()
+        merged_units = all_units.merge(
+            channels,
+            left_on="ecephys_channel_id",
+            right_index=True,
+            suffixes=(None, "_y"),
+        )
+        return merged_units
+
+    def get_sessions_table(self) -> "DataFrame":
+        allen_sessions = self.cache.get_ecephys_session_table()
+        allen_sessions = allen_sessions.dropna(subset=["file_id"])
+        return allen_sessions
+
+    def _map_class_to_values(self):
+        name_dict = {}
+        if self.cache_class_type.__name__ == "VisualBehaviorOphysProjectCache":
+            name_dict["session_name"] = "behavior_ophys_experiments"
+            name_dict["t"] = "ophys"
+            name_dict["id"] = "ophys_experiment_id"
+            name_dict["unique"] = 1
+        elif self.cache_class_type.__name__ == "VisualBehaviorNeuropixelsProjectCache":
+            if (self.manifest is not None) and ("0.4.0" in self.manifest):
+                name_dict["session_name"] = "behavior_ecephys_sessions"
+            else:
+                name_dict["session_name"] = "ecephys_sessions"
+            name_dict["t"] = "neuropixels"
+            name_dict["id"] = "ecephys_session_id"
+            name_dict["unique"] = 2
+        else:
+            raise ValueError(f"Unsupported cache type {self.cache_class_type.__name__}")
+
+        return name_dict
+
+
+@dataclass
+class AllenOphysLoader(BaseAllenLoader):
+    """
+    Load AIS ophys data VBO from a cache.
+
+    Attributes
+    ----------
+    cache : VisualBehaviorOphysProjectCache
+        The AIS ophys cache to load data from.
+
+    Parameters
+    ----------
+    cache_directory : str
+        Where to store the cached data.
+    manifest : str
+        The name of the .json manifest file to use (version).
+    local : bool
+        If true, instantiate a local cache over
+
+    """
+
+    cache: Optional["VisualBehaviorOphysProjectCache"] = None
+    cache_class_type: Type[ProjectCacheBase] = field(
+        repr=False, init=False, default=VisualBehaviorOphysProjectCache
+    )
+    local: bool = False
+
+    def __post_init__(self):
+        if self.cache is not None:
+            return
+        if self.local:
+            self.create_local_cache()
+        else:
+            self.create_s3_cache()
+
+
+@dataclass
+class AllenVisualBehaviorLoader(BaseAllenLoader):
+    """
+    Load AIS VBN dataset.
+
+    Attributes
+    ----------
+    cache : VisualBehaviorOphysProjectCache
+        The AIS ophys cache to load data from.
+
+    Parameters
+    ----------
+    cache_directory : str
+        Where to store the cached data.
+    manifest : str
+        The name of the .json manifest file to use (version).
+    local : bool
+        If true, instantiate a local cache over
+    """
+
+    cache: Optional["VisualBehaviorNeuropixelsProjectCache"] = None
+    cache_class_type: Type[ProjectCacheBase] = field(
+        repr=False, init=False, default=VisualBehaviorNeuropixelsProjectCache
+    )
+    local: bool = False
+
+    def __post_init__(self):
+        if self.cache is not None:
+            return
+        if self.local:
+            self.create_local_cache()
+        else:
+            self.create_s3_cache()
+
+    def get_all_units(self):
+        all_units = self.cache.get_unit_table()
+        channels = self.cache.get_channel_table()
+        return all_units.merge(
+            channels,
+            left_on="ecephys_channel_id",
+            right_index=True,
+            suffixes=(None, "_y"),
+        )
+
+    def download_data(self, session_id: Optional[int] = None):
+        if session_id is None:
+            sessions = self.get_sessions_table()
+            for session_id, row in sessions.iterrows():
+                if not self.path_to_nwb(session_id=session_id).exists():
+                    self.cache.get_ecephys_session(ecephys_session_id=session_id)
+        else:
+            if not self.path_to_nwb(session_id=session_id).exists():
+                self.cache.get_ecephys_session(ecephys_session_id=session_id)
```

### Comparing `simuran-23.2.0/simuran/loaders/neurochat_loader.py` & `simuran-23.8.0/simuran/loaders/neurochat_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,404 +1,416 @@
-"""This module handles interfacing with NeuroChaT."""
-import datetime
-import logging
-import os
-from collections.abc import Iterable
-from copy import deepcopy
-from pathlib import Path
-from typing import TYPE_CHECKING
-
-import numpy as np
-from dateutil.tz import tzlocal
-from neurochat.nc_lfp import NLfp
-from neurochat.nc_spatial import NSpatial
-from neurochat.nc_spike import NSpike
-from simuran.core.base_class import NoLoader
-from simuran.core.base_signal import BaseSignal
-from simuran.core.param_handler import ParamHandler
-from simuran.loaders.base_loader import MetadataLoader
-from skm_pyutils.path import get_all_files_in_dir
-from skm_pyutils.table import list_to_df
-from tqdm import tqdm
-
-if TYPE_CHECKING:
-    from simuran.recording import Recording
-
-module_logger = logging.getLogger("simuran.loaders")
-
-
-class NCLoader(MetadataLoader):
-    """
-    Load data compatible with the NeuroChaT package.
-
-    Parameters
-    ----------
-    system : str
-        The system to load, default is "Axona".
-
-    Kwargs and defaults
-    -------------------
-    pos_extension : (".txt", ".pos")
-    clu_extension : ".clu.X"
-    sig_channels : None
-    unit_groups : None
-    stm_extension : ".stm"
-    lfp_extension : ".eeg"
-    cluster_extension : ".cut"
-    """
-
-    def __init__(self, system="Axona", **kwargs):
-        self.system = system
-        self.loader_kwargs = kwargs
-
-    def load_recording(self, recording):
-        def add_mapping_info(recording):
-            mapping = recording.attrs.get("mapping")
-            if not hasattr(mapping, "items"):
-                return
-            for first_key, map_sub in mapping.items():
-                if map_sub is None:
-                    recording.attrs[first_key] = None
-                    continue
-                if (
-                    first_key not in ["signals", "spatial", "units"]
-                    or first_key not in recording.data
-                ):
-                    continue
-                for key, value in map_sub.items():
-                    if isinstance(value, list):
-                        for i in range(len(recording.data[first_key])):
-                            setattr(recording.data[first_key][i], key, value[i])
-                    else:
-                        recording.attrs[f"{first_key}_{key}"] = value
-
-        source_files = recording.attrs["source_files"]
-        if recording.data is None:
-            recording.data = {}
-        recording.last_loaded_source = recording.source_file
-        if (
-            source_files.get("Signal", None) is not None
-            and "Signal" in recording.available_data
-        ):
-            recording.data["signals"] = [
-                self.load_signal(fname) for fname in source_files["Signal"]
-            ]
-
-        if (
-            source_files.get("Spike", None) is not None
-            and "Spike" in recording.available_data
-        ):
-            if source_files["Spike"] is not None:
-                recording.data["units"] = []
-                for spike_f, clust_f in zip(
-                    source_files["Spike"], source_files["Cluster"]
-                ):
-                    if clust_f is not None:
-                        unit = self.load_single_unit(spike_f)
-                    else:
-                        unit = NoLoader(source_file=spike_f)
-                        unit.available_units = None
-                    recording.data["units"].append(unit)
-        if (
-            source_files.get("Spatial", None) is not None
-            and "Spatial" in recording.available_data
-        ):
-            recording.data["spatial"] = self.load_spatial(source_files["Spatial"])
-
-        add_mapping_info(recording)
-
-    def parse_metadata(self, recording: "Recording") -> None:
-        if "source_file" in recording.attrs:
-            source_file = Path(recording.attrs["source_file"])
-        elif "directory" in recording.attrs:
-            source_file = (
-                Path(recording.attrs["directory"]) / recording.attrs["filename"]
-            )
-        else:
-            source_file = recording.source_file
-        recording.source_file = source_file
-        recording.attrs["source_files"] = self.auto_fname_extraction(
-            recording.source_file
-        )[0]
-        recording.available_data = list(recording.attrs["source_files"].keys())
-        if "mapping" in recording.attrs:
-            ph = ParamHandler(source_file=recording.attrs["mapping"], name="mapping")
-            recording.attrs["mapping_file"] = recording.attrs["mapping"]
-            recording.attrs["mapping"] = ph
-        if "datetime" in recording.attrs:
-            recording.datetime = datetime.datetime.strptime(
-                recording.attrs["datetime"], "%Y-%m-%d %H:%M:%S"
-            )
-            recording.datetime = recording.datetime.replace(tzinfo=tzlocal())
-
-    def load_signal(self, *args, **kwargs):
-        """
-        Call the NeuroChaT NLfp.load method.
-
-        Returns
-        -------
-        dict
-            The keys of this dictionary are saved as attributes
-            in simuran.signal.BaseSignal.load()
-        """
-        self.signal = NLfp()
-        self.signal.load(*args, self.system)
-        obj = BaseSignal()
-        obj.data = self.signal
-        obj.timestamps = self.signal.get_timestamp()
-        obj.samples = self.signal.get_samples()
-        obj.conversion = 0.001
-        obj.date = self.signal.get_date()
-        obj.time = self.signal.get_time()
-        obj.channel = self.signal.get_channel_id()
-        obj.sampling_rate = self.signal.get_sampling_rate()
-        obj.source_file = args[0]
-        obj.last_loaded_source = args[0]
-        return obj
-
-    def load_spatial(self, *args, **kwargs):
-        """
-        Call the NeuroChaT NSpatial.load method.
-
-        Returns
-        -------
-        dict
-            The keys of this dictionary are saved as attributes
-            in simuran.single_unit.SingleUnit.load()
-        """
-        self.spatial = NSpatial()
-        self.spatial.load(*args, self.system)
-        obj = NoLoader()
-        obj.data = self.spatial
-        obj.date = self.spatial.get_date()
-        obj.timestamps = self.spatial.get_time()
-        obj.speed = self.spatial.get_speed()
-        obj.position = (self.spatial.get_pos_x(), self.spatial.get_pos_y())
-        obj.direction = self.spatial.get_direction()
-        obj.source_file = args[0]
-        obj.last_loaded_source = args[0]
-        return obj
-
-    def load_single_unit(self, *args, **kwargs):
-        """
-        Call the NeuroChaT NSpike.load method.
-
-        Returns
-        -------
-        dict
-            The keys of this dictionary are saved as attributes
-            in simuran.spatial.Spatial.load()
-
-        """
-        self.single_unit = NSpike()
-        self.single_unit.load(*args, self.system)
-        obj = NoLoader()
-        waveforms = deepcopy(self.single_unit.get_waveform())
-        for chan, val in waveforms.items():
-            waveforms[chan] = val
-        obj.data = self.single_unit
-        obj.timestamps = self.single_unit.get_timestamp()
-        obj.unit_tags = self.single_unit.get_unit_tags()
-        obj.waveforms = waveforms
-        obj.date = self.single_unit.get_date()
-        obj.time = self.single_unit.get_time()
-        obj.available_units = self.single_unit.get_unit_list()
-        obj.source_file = args[0]
-        obj.last_loaded_source = args[0]
-        obj.tag = int(Path(args[0]).suffix[1:])
-        return obj
-
-    def auto_fname_extraction(self, base, **kwargs):
-        """
-        Extract all filenames relevant to the recording from base.
-
-        Parameters
-        ----------
-        base : str
-            Where to start looking from.
-            For Axona, this should be a .set file,
-            or a directory containing exactly one .set file
-
-        Returns
-        -------
-        fnames : dict
-            A dictionary listing the filenames involved in loading.
-        base : str
-            The base file name, in Axona this is a .set file.
-
-        """
-        # Currently only implemented for Axona systems
-        error_on_missing = kwargs.get("enforce_data", True)
-
-        if self.system == "Axona":
-
-            # Find the set file if a directory is passed
-            if os.path.isdir(base):
-                set_files = get_all_files_in_dir(base, ext="set")
-                if len(set_files) == 0:
-                    module_logger.warning(
-                        "No set files found in {}, skipping".format(base)
-                    )
-                    return None, None
-                elif len(set_files) > 1:
-                    raise ValueError(
-                        "Found more than one set file, found {}".format(len(set_files))
-                    )
-                base = set_files[0]
-            elif not os.path.isfile(base):
-                raise ValueError("{} is not a file or directory".format(base))
-
-            joined_params = {
-                "system": self.system,
-            }
-            joined_params.update(self.loader_kwargs)
-            joined_params.update(**kwargs)
-            cluster_extension = joined_params.get("cluster_extension", ".cut")
-            clu_extension = joined_params.get("clu_extension", ".clu.X")
-            pos_extension = joined_params.get("pos_extension", (".txt", ".pos"))
-            lfp_extension = joined_params.get("lfp_extension", ".eeg")  # eeg or egf
-            stm_extension = joined_params.get("stm_extension", ".stm")
-            tet_groups = joined_params.get("unit_groups", None)
-            channels = joined_params.get("sig_channels", None)
-
-            filename = os.path.splitext(base)[0]
-            base_filename = os.path.splitext(os.path.basename(base))[0]
-
-            # Extract the tetrode and cluster data
-            spike_names_all = []
-            cluster_names_all = []
-            if tet_groups is None:
-                tet_groups = [
-                    x for x in range(0, 64) if os.path.exists(filename + "." + str(x))
-                ]
-            if channels is None:
-                channels = [
-                    x
-                    for x in range(2, 256)
-                    if os.path.exists(filename + lfp_extension + str(x))
-                ]
-                if os.path.exists(filename + lfp_extension):
-                    channels = [1] + channels
-            for tetrode in tet_groups:
-                spike_name = filename + "." + str(tetrode)
-                if not os.path.isfile(spike_name):
-                    e_msg = "Axona data is not available for {}".format(spike_name)
-                    if error_on_missing:
-                        raise ValueError(e_msg)
-                    else:
-                        logging.warning(e_msg)
-                        return None, base
-
-                spike_names_all.append(spike_name)
-
-                cut_name = filename + "_" + str(tetrode) + cluster_extension
-                clu_name = filename + clu_extension[:-1] + str(tetrode)
-                if os.path.isfile(cut_name):
-                    cluster_name = cut_name
-                elif os.path.isfile(clu_name):
-                    cluster_name = clu_name
-                else:
-                    cluster_name = None
-                cluster_names_all.append(cluster_name)
-
-            # Extract the positional data
-            output_list = [None, None]
-            for i, ext in enumerate([pos_extension, stm_extension]):
-                if isinstance(ext, Iterable) and not isinstance(ext, str):
-                    for ext_ in ext:
-                        filename_ = self._grab_stim_pos_files(base, base_filename, ext_)
-                        if filename_ is not None:
-                            output_list[i] = filename_
-                            break
-                else:
-                    output_list[i] = self._grab_stim_pos_files(base, base_filename, ext)
-            spatial_name, stim_name = output_list
-
-            base_sig_name = filename + lfp_extension
-            signal_names = []
-            for c in channels:
-                if c != 1:
-                    if os.path.exists(base_sig_name + str(c)):
-                        signal_names.append(base_sig_name + str(c))
-                    else:
-                        e_msg = "{} does not exist".format(base_sig_name + str(c))
-                        if error_on_missing:
-                            raise ValueError(e_msg)
-                        else:
-                            logging.warning(e_msg)
-                            return None, base
-                else:
-                    if os.path.exists(base_sig_name):
-                        signal_names.append(base_sig_name)
-                    else:
-                        e_msg = "{} does not exist".format(base_sig_name)
-                        if error_on_missing:
-                            raise ValueError(e_msg)
-                        else:
-                            logging.warning(e_msg)
-                            return None, base
-
-            file_locs = {
-                "Spike": spike_names_all,
-                "Cluster": cluster_names_all,
-                "Spatial": spatial_name,
-                "Signal": signal_names,
-                "Stimulation": stim_name,
-            }
-            return file_locs, base
-        else:
-            raise ValueError("auto_fname_extraction only implemented for Axona")
-
-    def _grab_stim_pos_files(self, base, base_filename, ext):
-        for fname in get_all_files_in_dir(
-            os.path.dirname(base),
-            ext=ext,
-            return_absolute=False,
-            case_sensitive_ext=True,
-        ):
-            if ext == ".txt":
-                if fname[: len(base_filename) + 1] == f"{base_filename}_":
-                    name = os.path.join(os.path.dirname(base), fname)
-                    return name
-            elif fname[: len(base_filename)] == base_filename:
-                name = os.path.join(os.path.dirname(base), fname)
-                return name
-
-    def index_files(self, folder, **kwargs):
-        """Find all available neurochat files in the given folder"""
-        if self.system != "Axona":
-            raise ValueError("auto_fname_extraction only implemented for Axona")
-        set_files = []
-        root_folders = []
-        times = []
-        durations = []
-        module_logger.info("Finding all .set files...")
-        files = get_all_files_in_dir(
-            folder,
-            ext=".set",
-            recursive=True,
-            return_absolute=True,
-            case_sensitive_ext=True,
-        )
-        module_logger.info(f"Found {len(files)} set files")
-
-        for fname in tqdm(files, desc="Processing files"):
-            set_files.append(os.path.basename(fname))
-            root_folders.append(os.path.normpath(os.path.dirname(fname)))
-            with open(fname) as f:
-                f.readline()
-                t = f.readline()[-9:-1]
-                try:
-                    int(t[:2])
-                    times.append(t)
-                    f.readline()
-                    f.readline()
-                    durations.append(int(f.readline()[-11:-1].strip()))
-                except Exception:
-                    if len(times) != len(set_files):
-                        times.append(np.nan)
-                    if len(durations) != len(set_files):
-                        durations.append(np.nan)
-
-        headers = ["directory", "filename", "time", "duration"]
-        in_list = [root_folders, set_files, times, durations]
-        return list_to_df(in_list, transpose=True, headers=headers)
+"""This module handles interfacing with NeuroChaT."""
+import datetime
+import logging
+import os
+from collections.abc import Iterable
+from copy import deepcopy
+from pathlib import Path
+from typing import TYPE_CHECKING
+
+import numpy as np
+from dateutil.tz import tzlocal
+from neurochat.nc_lfp import NLfp
+from neurochat.nc_spatial import NSpatial
+from neurochat.nc_spike import NSpike
+from simuran.core.base_class import NoLoader
+from simuran.core.base_signal import BaseSignal
+from simuran.core.param_handler import ParamHandler
+from simuran.loaders.base_loader import MetadataLoader
+from skm_pyutils.path import get_all_files_in_dir
+from skm_pyutils.table import list_to_df
+from tqdm import tqdm
+
+if TYPE_CHECKING:
+    from simuran.recording import Recording
+
+module_logger = logging.getLogger("simuran.loaders")
+
+
+class NeurochatLoader(MetadataLoader):
+    """
+    Load data compatible with the NeuroChaT package.
+
+    Parameters
+    ----------
+    system : str
+        The system to load, default is "Axona".
+
+    Kwargs and defaults
+    -------------------
+    pos_extension : (".txt", ".pos")
+    clu_extension : ".clu.X"
+    sig_channels : None
+    unit_groups : None
+    stm_extension : ".stm"
+    lfp_extension : ".eeg"
+    cluster_extension : ".cut"
+    """
+
+    def __init__(self, system="Axona", **kwargs):
+        self.system = system
+        self.loader_kwargs = kwargs
+
+    def load_recording(self, recording):
+        def add_mapping_info(recording):
+            mapping = recording.attrs.get("mapping")
+            if not hasattr(mapping, "items"):
+                return
+            for first_key, map_sub in mapping.items():
+                if map_sub is None:
+                    recording.attrs[first_key] = None
+                    continue
+                if (
+                    first_key not in ["signals", "spatial", "units"]
+                    or first_key not in recording.data
+                ):
+                    continue
+                for key, value in map_sub.items():
+                    if isinstance(value, list):
+                        for i in range(len(recording.data[first_key])):
+                            setattr(recording.data[first_key][i], key, value[i])
+                    else:
+                        recording.attrs[f"{first_key}_{key}"] = value
+
+        source_files = recording.attrs["source_files"]
+        if recording.data is None:
+            recording.data = {}
+        recording.last_loaded_source = recording.source_file
+        if (
+            source_files.get("Signal", None) is not None
+            and "Signal" in recording.available_data
+        ):
+            recording.data["signals"] = [
+                self.load_signal(fname) for fname in source_files["Signal"]
+            ]
+
+        if (
+            source_files.get("Spike", None) is not None
+            and "Spike" in recording.available_data
+        ):
+            if source_files["Spike"] is not None:
+                recording.data["units"] = []
+                for spike_f, clust_f in zip(
+                    source_files["Spike"], source_files["Cluster"]
+                ):
+                    if clust_f is not None:
+                        unit = self.load_single_unit(spike_f)
+                    else:
+                        unit = NoLoader(source_file=spike_f)
+                        unit.available_units = None
+                    recording.data["units"].append(unit)
+        if (
+            source_files.get("Spatial", None) is not None
+            and "Spatial" in recording.available_data
+        ):
+            recording.data["spatial"] = self.load_spatial(source_files["Spatial"])
+
+        add_mapping_info(recording)
+
+    def parse_metadata(self, recording: "Recording") -> None:
+        if "source_file" in recording.attrs:
+            source_file = Path(recording.attrs["source_file"])
+        elif "directory" in recording.attrs:
+            source_file = (
+                Path(recording.attrs["directory"]) / recording.attrs["filename"]
+            )
+        else:
+            source_file = recording.source_file
+        recording.source_file = source_file
+        recording.attrs["source_files"] = self.auto_fname_extraction(
+            recording.source_file
+        )[0]
+        recording.available_data = list(recording.attrs["source_files"].keys())
+        if "mapping" in recording.attrs:
+            ph = ParamHandler(source_file=recording.attrs["mapping"], name="mapping")
+            recording.attrs["mapping_file"] = recording.attrs["mapping"]
+            recording.attrs["mapping"] = ph
+        if "datetime" in recording.attrs:
+            recording.datetime = datetime.datetime.strptime(
+                recording.attrs["datetime"], "%Y-%m-%d %H:%M:%S"
+            )
+            recording.datetime = recording.datetime.replace(tzinfo=tzlocal())
+
+    def load_signal(self, *args, **kwargs):
+        """
+        Call the NeuroChaT NLfp.load method.
+
+        Returns
+        -------
+        dict
+            The keys of this dictionary are saved as attributes
+            in simuran.signal.BaseSignal.load()
+        """
+        self.signal = NLfp()
+        obj = BaseSignal()
+        try:
+            self.signal.load(*args, self.system)
+        except Exception as e:
+            module_logger.warning(f"Failed to load signal with NeuroChaT due to {e}, skipping")
+            return obj
+        obj.data = self.signal
+        obj.timestamps = self.signal.get_timestamp()
+        obj.samples = self.signal.get_samples()
+        obj.conversion = 0.001
+        obj.date = self.signal.get_date()
+        obj.time = self.signal.get_time()
+        obj.channel = self.signal.get_channel_id()
+        obj.sampling_rate = self.signal.get_sampling_rate()
+        obj.source_file = args[0]
+        obj.last_loaded_source = args[0]
+        return obj
+
+    def load_spatial(self, *args, **kwargs):
+        """
+        Call the NeuroChaT NSpatial.load method.
+
+        Returns
+        -------
+        dict
+            The keys of this dictionary are saved as attributes
+            in simuran.single_unit.SingleUnit.load()
+        """
+        self.spatial = NSpatial()
+        self.spatial.load(*args, self.system)
+        obj = NoLoader()
+        obj.data = self.spatial
+        obj.date = self.spatial.get_date()
+        obj.timestamps = self.spatial.get_time()
+        obj.speed = self.spatial.get_speed()
+        obj.position = (self.spatial.get_pos_x(), self.spatial.get_pos_y())
+        obj.direction = self.spatial.get_direction()
+        obj.source_file = args[0]
+        obj.last_loaded_source = args[0]
+        return obj
+
+    def load_single_unit(self, *args, **kwargs):
+        """
+        Call the NeuroChaT NSpike.load method.
+
+        Returns
+        -------
+        dict
+            The keys of this dictionary are saved as attributes
+            in simuran.spatial.Spatial.load()
+
+        """
+        self.single_unit = NSpike()
+        self.single_unit.load(*args, self.system)
+        obj = NoLoader()
+        waveforms = deepcopy(self.single_unit.get_waveform())
+        for chan, val in waveforms.items():
+            waveforms[chan] = val
+        obj.data = self.single_unit
+        obj.timestamps = self.single_unit.get_timestamp()
+        obj.unit_tags = self.single_unit.get_unit_tags()
+        obj.waveforms = waveforms
+        obj.date = self.single_unit.get_date()
+        obj.time = self.single_unit.get_time()
+        obj.available_units = self.single_unit.get_unit_list()
+        obj.source_file = args[0]
+        obj.last_loaded_source = args[0]
+        obj.tag = int(Path(args[0]).suffix[1:])
+        return obj
+
+    def auto_fname_extraction(self, base, **kwargs):
+        """
+        Extract all filenames relevant to the recording from base.
+
+        Parameters
+        ----------
+        base : str
+            Where to start looking from.
+            For Axona, this should be a .set file,
+            or a directory containing exactly one .set file
+
+        Returns
+        -------
+        fnames : dict
+            A dictionary listing the filenames involved in loading.
+        base : str
+            The base file name, in Axona this is a .set file.
+
+        """
+        # Currently only implemented for Axona systems
+        error_on_missing = kwargs.get("enforce_data", True)
+
+        if self.system == "Axona":
+
+            # Find the set file if a directory is passed
+            if os.path.isdir(base):
+                set_files = get_all_files_in_dir(base, ext="set")
+                if len(set_files) == 0:
+                    module_logger.warning(
+                        "No set files found in {}, skipping".format(base)
+                    )
+                    return None, None
+                elif len(set_files) > 1:
+                    raise ValueError(
+                        "Found more than one set file, found {}".format(len(set_files))
+                    )
+                base = set_files[0]
+            elif not os.path.isfile(base):
+                raise ValueError("{} is not a file or directory".format(base))
+
+            joined_params = {
+                "system": self.system,
+            }
+            joined_params.update(self.loader_kwargs)
+            joined_params.update(**kwargs)
+            cluster_extension = joined_params.get("cluster_extension", ".cut")
+            clu_extension = joined_params.get("clu_extension", ".clu.X")
+            pos_extension = joined_params.get("pos_extension", (".txt", ".pos"))
+            lfp_extension = joined_params.get("lfp_extension", ".eeg")  # eeg or egf
+            stm_extension = joined_params.get("stm_extension", ".stm")
+            tet_groups = joined_params.get("unit_groups", None)
+            channels = joined_params.get("sig_channels", None)
+
+            filename = os.path.splitext(base)[0]
+            base_filename = os.path.splitext(os.path.basename(base))[0]
+
+            # Extract the tetrode and cluster data
+            spike_names_all = []
+            cluster_names_all = []
+            if tet_groups is None:
+                tet_groups = [
+                    x for x in range(0, 64) if os.path.exists(filename + "." + str(x))
+                ]
+            if channels is None:
+                channels = [
+                    x
+                    for x in range(2, 256)
+                    if os.path.exists(filename + lfp_extension + str(x))
+                ]
+                if os.path.exists(filename + lfp_extension):
+                    channels = [1] + channels
+            for tetrode in tet_groups:
+                spike_name = filename + "." + str(tetrode)
+                if not os.path.isfile(spike_name):
+                    e_msg = "Axona data is not available for {}".format(spike_name)
+                    if error_on_missing:
+                        raise ValueError(e_msg)
+                    else:
+                        logging.warning(e_msg)
+                        return None, base
+
+                spike_names_all.append(spike_name)
+
+                cut_name = filename + "_" + str(tetrode) + cluster_extension
+                clu_name = filename + clu_extension[:-1] + str(tetrode)
+                if os.path.isfile(cut_name):
+                    cluster_name = cut_name
+                elif os.path.isfile(clu_name):
+                    cluster_name = clu_name
+                else:
+                    cluster_name = None
+                cluster_names_all.append(cluster_name)
+
+            # Extract the positional data
+            output_list = [None, None]
+            for i, ext in enumerate([pos_extension, stm_extension]):
+                if isinstance(ext, Iterable) and not isinstance(ext, str):
+                    for ext_ in ext:
+                        filename_ = self._grab_stim_pos_files(base, base_filename, ext_)
+                        if filename_ is not None:
+                            output_list[i] = filename_
+                            break
+                else:
+                    output_list[i] = self._grab_stim_pos_files(base, base_filename, ext)
+            spatial_name, stim_name = output_list
+
+            base_sig_name = filename + lfp_extension
+            signal_names = []
+            for c in channels:
+                if c != 1:
+                    if os.path.exists(base_sig_name + str(c)):
+                        signal_names.append(base_sig_name + str(c))
+                    else:
+                        e_msg = "{} does not exist".format(base_sig_name + str(c))
+                        if error_on_missing:
+                            raise ValueError(e_msg)
+                        else:
+                            logging.warning(e_msg)
+                            return None, base
+                else:
+                    if os.path.exists(base_sig_name):
+                        signal_names.append(base_sig_name)
+                    else:
+                        e_msg = "{} does not exist".format(base_sig_name)
+                        if error_on_missing:
+                            raise ValueError(e_msg)
+                        else:
+                            logging.warning(e_msg)
+                            return None, base
+
+            file_locs = {
+                "Spike": spike_names_all,
+                "Cluster": cluster_names_all,
+                "Spatial": spatial_name,
+                "Signal": signal_names,
+                "Stimulation": stim_name,
+            }
+            return file_locs, base
+        else:
+            raise ValueError("auto_fname_extraction only implemented for Axona")
+
+    def _grab_stim_pos_files(self, base, base_filename, ext):
+        for fname in get_all_files_in_dir(
+            os.path.dirname(base),
+            ext=ext,
+            return_absolute=False,
+            case_sensitive_ext=True,
+        ):
+            if ext == ".txt":
+                if fname[: len(base_filename) + 1] == f"{base_filename}_":
+                    name = os.path.join(os.path.dirname(base), fname)
+                    return name
+            elif fname[: len(base_filename)] == base_filename:
+                name = os.path.join(os.path.dirname(base), fname)
+                return name
+
+    def index_files(self, folder, **kwargs):
+        """Find all available neurochat files in the given folder"""
+        if self.system != "Axona":
+            raise ValueError("auto_fname_extraction only implemented for Axona")
+        set_files = []
+        root_folders = []
+        times = []
+        durations = []
+        dates = []
+        comments = []
+        module_logger.info("Finding all .set files...")
+        files = get_all_files_in_dir(
+            str(folder),
+            ext=".set",
+            recursive=True,
+            return_absolute=True,
+            case_sensitive_ext=True,
+        )
+        module_logger.info(f"Found {len(files)} set files")
+
+        for fname in tqdm(files, desc="Processing files"):
+            set_files.append(os.path.basename(fname))
+            root_folders.append(os.path.normpath(os.path.dirname(fname)))
+            with open(fname) as f:
+                d = f.readline()
+                dates.append(d.split(" ", 1)[1].strip())
+                t = f.readline()[-9:-1]
+                try:
+                    int(t[:2])
+                    times.append(t)
+                except ValueError:
+                    times.append(np.nan)
+                f.readline()
+                comment = f.readline()
+                try:
+                    comments.append(comment.split(" ", 1)[1].strip())
+                except IndexError:
+                    comments.append("")
+                duration = f.readline()
+                try:
+                    durations.append(int(float(duration.split(" ", 1)[1].strip())))
+                except Exception:
+                    durations.append(np.nan)
+
+        headers = ["directory", "filename", "date", "time", "duration", "comments"]
+        in_list = [root_folders, set_files, dates, times, durations, comments]
+        return list_to_df(in_list, transpose=True, headers=headers)
```

### Comparing `simuran-23.2.0/simuran/loaders/nwb_loader.py` & `simuran-23.8.0/simuran/loaders/nwb_loader.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from dataclasses import dataclass
-from typing import TYPE_CHECKING
-
-import pynwb
-from simuran.loaders.base_loader import MetadataLoader
-
-if TYPE_CHECKING:
-    from simuran.recording import Recording
-
-
-@dataclass
-class NWBLoader(MetadataLoader):
-    """
-    Load NWB data.
-
-    Attributes
-    ----------
-    mode : str
-        The mode to open the file in, by default "r"
-        But "a" and "w" are other options for example.
-
-    """
-
-    mode: str = "r"
-
-    def parse_metadata(self, recording: "Recording") -> None:
-        options = ["nwb_file", "source_file"]
-        for option in options:
-            if option in recording.attrs:
-                recording.source_file = recording.attrs[option]
-                break
-        else:
-            raise ValueError(
-                f"Please provide one of {options} as metadata for NWB parsing"
-            )
-
-    def load_recording(self, recording) -> "Recording":
-        try:
-            load_namespaces = True if self.mode == "r" else False
-            nwb_io = pynwb.NWBHDF5IO(
-                recording.source_file, self.mode, load_namespaces=load_namespaces
-            )
-        except OSError as e:
-            print(f"{recording.source_file} is not a valid NWB file")
-            raise (e)
-        except TypeError as e:
-            print(f"{recording.source_file} is not a valid type for NWB file")
-            raise (e)
-        recording.data = nwb_io.read()
-        recording._nwb_io = nwb_io
-
-    def unload(self, recording: "Recording") -> None:
-        if hasattr(recording, "_nwb_io"):
-            try:
-                recording._nwb_io.close()
-            except TypeError:
-                delattr(recording, "_nwb_io")
-            else:
-                delattr(recording, "_nwb_io")
+from dataclasses import dataclass
+from typing import TYPE_CHECKING
+
+import pynwb
+from simuran.loaders.base_loader import MetadataLoader
+
+if TYPE_CHECKING:
+    from simuran.recording import Recording
+
+
+@dataclass
+class NWBLoader(MetadataLoader):
+    """
+    Load NWB data.
+
+    Attributes
+    ----------
+    mode : str
+        The mode to open the file in, by default "r"
+        But "a" and "w" are other options for example.
+
+    """
+
+    mode: str = "r"
+
+    def parse_metadata(self, recording: "Recording") -> None:
+        options = ["nwb_file", "source_file"]
+        for option in options:
+            if option in recording.attrs:
+                recording.source_file = recording.attrs[option]
+                break
+        else:
+            raise ValueError(
+                f"Please provide one of {options} as metadata for NWB parsing"
+            )
+
+    def load_recording(self, recording) -> "Recording":
+        try:
+            load_namespaces = True if self.mode == "r" else False
+            nwb_io = pynwb.NWBHDF5IO(
+                recording.source_file, self.mode, load_namespaces=load_namespaces
+            )
+        except OSError as e:
+            print(f"{recording.source_file} is not a valid NWB file")
+            raise (e)
+        except TypeError as e:
+            print(f"{recording.source_file} is not a valid type for NWB file")
+            raise (e)
+        recording.data = nwb_io.read()
+        recording._nwb_io = nwb_io
+
+    def unload(self, recording: "Recording") -> None:
+        if hasattr(recording, "_nwb_io"):
+            try:
+                recording._nwb_io.close()
+            except TypeError:
+                delattr(recording, "_nwb_io")
+            else:
+                delattr(recording, "_nwb_io")
```

### Comparing `simuran-23.2.0/simuran/loaders/one_loader.py` & `simuran-23.8.0/simuran/loaders/one_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,180 @@
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Optional, Union
-from pathlib import Path
-
-from one.api import ONE
-import one
-from brainbox.io.one import SpikeSortingLoader
-from ibllib.atlas import AllenAtlas
-import pandas as pd
-
-from simuran.loaders.base_loader import MetadataLoader
-
-if TYPE_CHECKING:
-    from simuran import Recording
-    from pandas import DataFrame
-
-
-@dataclass
-class OneAlyxLoader(MetadataLoader):
-    """
-    Load One alyx data from online/cache.
-
-    Attributes
-    ----------
-    one : ONE
-        The ONE alyx instance
-    atlas : AllenAtlas
-        The allen brain atlas to use to associate data with.
-    cache_directory : str
-        The path to the directory to store data in.
-
-    """
-
-    one: Optional["ONE"] = None
-    atlas: Optional["AllenAtlas"] = None
-    cache_directory: Optional[Union[str, "Path"]] = None
-    mode: str = "auto"
-
-    def __post_init__(self):
-        if self.one is None:
-            self.create_cache()
-
-    def create_cache(self):
-        one_instance = ONE(
-            base_url="https://openalyx.internationalbrainlab.org",
-            password="international",
-            silent=True,
-            cache_dir=self.cache_directory,
-            mode=self.mode,
-        )
-        param_file_location = one.params.iopar.getfile(one.params._PAR_ID_STR)
-        p = Path(param_file_location) / ".caches"
-        p.unlink(missing_ok=True)
-        one.params.CACHE_DIR_DEFAULT = self.cache_directory
-        one.params.setup(silent=True)
-        self.one = one_instance
-        if self.atlas is None:
-            self.atlas = AllenAtlas()
-        self.sessions = self.one.alyx.rest("insertions", "list")
-        self._probe_dict = {}
-        for s in self.sessions:
-            self._probe_dict.setdefault(s["session"], []).append(s["id"])
-
-    def find_eid(self, lab, subject, details=True):
-        return self.one.search(lab=lab, subject=subject, details=details)
-
-    def describe_dataset(self, eid: str):
-        return self.one.list_datasets(eid=eid, collection="alf", details=True)
-
-    def get_sessions_table(self) -> "DataFrame":
-        return pd.DataFrame([s for s in self.sessions])
-
-    def load_recording(self, recording: "Recording") -> "Recording":
-        id_ = recording.attrs.get("session")
-        if id_ is None:
-            id_ = recording.attrs.get("experiment_id")
-        if id_ is None:
-            raise KeyError("No session or experiment_id set in recording.attrs")
-        exclude = recording.attrs.get("data_to_exclude", ["full_details", "motion"])
-        recording.data = self._download_data(id_, exclude=exclude)
-        recording.attrs["quality_control"] = recording.data.pop("quality_control")
-        recording.attrs["extended_quality_control"] = recording.data.pop(
-            "extended_quality_control"
-        )
-        return recording
-
-    def summarise(self, recording: "Recording") -> "Recording":
-        out_dict = {}
-        for key, value in recording.data.items():
-            out_dict[key] = type(value)
-
-        pass_ = recording.attrs["quality_control"]
-
-        output_str = (
-            f"This dataset is a {pass_} and is summarised as follows:\n"
-            + f"It contains the following data keys and data types {out_dict}\n"
-        )
-
-        out_dict = {}
-        for key, value in recording.data.items():
-            if hasattr(value, "keys"):
-                out_dict[key] = [k for k in value.keys()]
-            elif hasattr(value, "columns"):
-                out_dict[key] = value.columns
-            else:
-                out_dict[key] = f"of type {type(value)}"
-
-        for key, value in out_dict.items():
-            output_str += f"The {key} is {value}\n"
-
-        output_str += f"\nThe full quality control is {recording.attrs['extended_quality_control']}"
-
-        print(output_str)
-        return output_str
-
-    def _download_data(self, eid, exclude=[]):
-        session_data = [
-            "trials",
-            "wheels",
-            "wheelMoves",
-            "licks",
-        ]
-        if not "camera" in exclude:
-            session_data += ["leftCamera", "bodyCamera", "rightCamera"]
-
-        if not "motion" in exclude:
-            session_data += [
-                "leftROIMotionEnergy",
-                "bodyROIMotionEnergy",
-                "rightROIMotionEnergy",
-            ]
-
-        return_dict = {}
-        for sd in session_data:
-            try:
-                return_dict[sd] = self.one.load_object(eid, sd, collection="alf")
-            except Exception:
-                continue
-
-        for pid in self._probe_dict[eid]:
-            name = self.one.alyx.rest("insertions", "list", id=pid)[0]["name"]
-            return_dict[f"{name}"] = self._get_probe_data(pid)
-
-        if not "full_details" in exclude:
-            return_dict["full_details"] = self.one.get_details(eid, full=True)
-            return_dict["quality_control"] = return_dict["full_details"]["qc"]
-            return_dict["extended_quality_control"] = return_dict["full_details"][
-                "extended_qc"
-            ]
-        else:
-            full = self.one.get_details(eid, full=True)
-            return_dict["quality_control"] = full["qc"]
-            return_dict["extended_quality_control"] = full["extended_qc"]
-        return return_dict
-
-    def _get_probe_data(self, pid):
-        # Alternatively, one can instantiate the spike sorting loader using the session unique identifier eid and the probe name pname
-        sl = SpikeSortingLoader(pid=pid, one=self.one, atlas=self.atlas)
-        spikes, clusters, channels = sl.load_spike_sorting()
-        clusters = sl.merge_clusters(spikes, clusters, channels)
-        clusters_df = pd.DataFrame(clusters)
-
-        # Filter to only have good units as per data release
-        # return clusters_df.loc[clusters["label"] == 1]
-
-        return spikes, clusters_df
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Optional, Union
+from pathlib import Path
+
+from one.api import ONE
+import one
+from brainbox.io.one import SpikeSortingLoader
+from ibllib.atlas import AllenAtlas
+import requests
+import pandas as pd
+
+from simuran.loaders.base_loader import MetadataLoader
+
+if TYPE_CHECKING:
+    from simuran import Recording
+    from pandas import DataFrame
+
+
+@dataclass
+class OneAlyxLoader(MetadataLoader):
+    """
+    Load One alyx data from online/cache.
+
+    Attributes
+    ----------
+    one : ONE
+        The ONE alyx instance
+    atlas : AllenAtlas
+        The allen brain atlas to use to associate data with.
+    cache_directory : str
+        The path to the directory to store data in.
+
+    """
+
+    one: Optional["ONE"] = None
+    atlas: Optional["AllenAtlas"] = None
+    cache_directory: Optional[Union[str, "Path"]] = None
+    mode: str = "auto"
+
+    def __post_init__(self):
+        if self.one is None:
+            self.create_cache()
+
+    def create_cache(self):
+        try:
+            one_instance = ONE(
+                base_url="https://openalyx.internationalbrainlab.org",
+                password="international",
+                silent=True,
+                cache_dir=self.cache_directory,
+                mode=self.mode,
+            )
+        except (requests.exceptions.ConnectionError, requests.exceptions.HTTPError):
+            one_instance = ONE(
+                silent=True,
+                cache_dir=self.cache_directory,
+                mode="local",
+            )
+        param_file_location = one.params.iopar.getfile(one.params._PAR_ID_STR)
+        p = Path(param_file_location) / ".caches"
+        p.unlink(missing_ok=True)
+        one.params.CACHE_DIR_DEFAULT = self.cache_directory
+        one.params.setup(silent=True)
+        self.one = one_instance
+        if self.atlas is None:
+            self.atlas = AllenAtlas()
+        self.sessions = self.one.alyx.rest("insertions", "list")
+        self._probe_dict = {}
+        for s in self.sessions:
+            self._probe_dict.setdefault(s["session"], []).append(s["id"])
+
+    def find_eid(self, lab, subject, details=True):
+        return self.one.search(lab=lab, subject=subject, details=details)
+
+    def describe_dataset(self, eid: str):
+        return self.one.list_datasets(eid=eid, collection="alf", details=True)
+
+    def get_sessions_table(self) -> "DataFrame":
+        all_insertions = pd.DataFrame([s for s in self.sessions])
+        return all_insertions.drop_duplicates(subset=["session"])
+
+    def parse_metadata(self, recording: "Recording") -> None:
+        id_ = recording.attrs.get("session")
+        if id_ is None:
+            id_ = recording.attrs.get("experiment_id")
+        if id_ is None:
+            raise KeyError("No session or experiment_id set in recording.attrs")
+        recording.source_file = id_
+
+    def load_recording(self, recording: "Recording") -> "Recording":
+        exclude = recording.attrs.get("data_to_exclude", ["full_details", "motion"])
+        recording.data = self._download_data(recording.source_file, exclude=exclude)
+        recording.attrs["quality_control"] = recording.data.pop("quality_control")
+        recording.attrs["extended_quality_control"] = recording.data.pop(
+            "extended_quality_control"
+        )
+        return recording
+
+    def summarise(self, recording: "Recording") -> "Recording":
+        out_dict = {}
+        for key, value in recording.data.items():
+            out_dict[key] = type(value)
+
+        pass_ = recording.attrs["quality_control"]
+
+        output_str = (
+            f"This dataset is a {pass_} and is summarised as follows:\n"
+            + f"It contains the following data keys and data types {out_dict}\n"
+        )
+
+        out_dict = {}
+        for key, value in recording.data.items():
+            if hasattr(value, "keys"):
+                out_dict[key] = [k for k in value.keys()]
+            elif hasattr(value, "columns"):
+                out_dict[key] = value.columns
+            else:
+                out_dict[key] = f"of type {type(value)}"
+
+        for key, value in out_dict.items():
+            output_str += f"The {key} is {value}\n"
+
+        output_str += f"\nThe full quality control is {recording.attrs['extended_quality_control']}"
+
+        print(output_str)
+        return output_str
+
+    def _download_data(self, eid, exclude=[]):
+        if self.one.offline:
+            raise ValueError("Cannot download data when in offline mode")
+        session_data = [
+            "trials",
+            "wheels",
+            "wheelMoves",
+            "licks",
+        ]
+        if not "camera" in exclude:
+            session_data += ["leftCamera", "bodyCamera", "rightCamera"]
+
+        if not "motion" in exclude:
+            session_data += [
+                "leftROIMotionEnergy",
+                "bodyROIMotionEnergy",
+                "rightROIMotionEnergy",
+            ]
+
+        return_dict = {}
+        for sd in session_data:
+            try:
+                return_dict[sd] = self.one.load_object(eid, sd, collection="alf")
+            except Exception:
+                continue
+
+        for pid in self._probe_dict[eid]:
+            name = self.one.alyx.rest("insertions", "list", id=pid)[0]["name"]
+            return_dict[f"{name}"] = self._get_probe_data(pid)
+
+        if not "full_details" in exclude:
+            return_dict["full_details"] = self.one.get_details(eid, full=True)
+            return_dict["quality_control"] = return_dict["full_details"]["qc"]
+            return_dict["extended_quality_control"] = return_dict["full_details"][
+                "extended_qc"
+            ]
+        else:
+            full = self.one.get_details(eid, full=True)
+            return_dict["quality_control"] = full["qc"]
+            return_dict["extended_quality_control"] = full["extended_qc"]
+        return return_dict
+
+    def _get_probe_data(self, pid):
+        # Alternatively, one can instantiate the spike sorting loader using the session unique identifier eid and the probe name pname
+        sl = SpikeSortingLoader(pid=pid, one=self.one, atlas=self.atlas)
+        spikes, clusters, channels = sl.load_spike_sorting()
+        clusters = sl.merge_clusters(spikes, clusters, channels)
+        clusters_df = pd.DataFrame(clusters)
+
+        # Filter to only have good units as per data release
+        # return clusters_df.loc[clusters["label"] == 1]
+
+        return spikes, clusters_df
```

### Comparing `simuran-23.2.0/simuran/plot/base_plot.py` & `simuran-23.8.0/simuran/plot/base_plot.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-"""This module provides functions to interface with matplotlib."""
-
-import os
-from copy import copy
-
-from typing import TYPE_CHECKING
-import matplotlib.pyplot as plt
-import seaborn as sns
-import skm_pyutils.path
-
-if TYPE_CHECKING:
-    import matplotlib
-
-
-def setup_ax(ax=None, default={}, **kwargs) -> "matplotlib.axes.Axes":
-    """
-    Set up an axis object with default parameters that can be overridden.
-
-    In this way, a function can set default for the usual things that should
-    be plotted (e.g. plot axis labels), but keyword arguments can overwrite
-    any of these.
-
-    Parameters
-    ----------
-    ax : matplotlib.axes.Axes
-        The axis object to set up.
-    default : dict
-        Parameters to use for setting up the axis if not overridden.
-        Can contain any of the keys that can be keyword arguments
-
-    Keyword arguments
-    -----------------
-    xlabel : str
-        What to label the x-axis
-    ylabel : str
-        What to label the y-axis with
-    xticks : array like
-        x ticks
-    xticklabels : array like
-        Labels for the x- ticks
-    yticks : array like
-        y ticks
-    yticklabels : array like
-        Labels for the y- ticks
-    xrotate : float
-        The amount to rotate the x labels by
-    yrotate : float
-        The amount to rotate the y labels by
-    labelsize : float
-        The text size of the labels
-
-    Returns
-    -------
-    ax
-
-    """
-    if ax is None:
-        fig, ax = plt.subplots()
-    default = copy(default)
-    for key, value in kwargs.items():
-        default[key] = value
-    ax.set_xlabel(default.get("xlabel", None))
-    ax.set_ylabel(default.get("ylabel", None))
-    ax.set_title(default.get("title", None))
-    if "xticks" in default:
-        ax.set_xticks(default.get("xticks"))
-    if "xticklabels" in default:
-        ax.set_xticklabels(default.get("xticklabels"))
-    if "yticks" in default:
-        ax.set_yticks(default.get("yticks"))
-    if "yticklabels" in default:
-        ax.set_yticklabels(default.get("yticklabels"))
-    if "xrotate" in default:
-        plt.setp(
-            ax.get_xticklabels(),
-            rotation=default["xrotate"],
-            ha="right",
-            rotation_mode="anchor",
-        )
-    if "yrotate" in default:
-        plt.setp(
-            ax.get_yticklabels(),
-            rotation=default["yrotate"],
-            ha="right",
-            rotation_mode="anchor",
-        )
-    if "labelsize" in default:
-        ax.tick_params(labelsize=default["labelsize"])
-    return ax
-
-
-def save_simuran_plot(fig, save_location, **kwargs):
-    """
-    Save a figure using some default settings.
-
-    By default saves both a raster image (bitmap e.g. PNG, JPG)
-    and a vector image (e.g. PDF, SVG).
-    This can be disabled by setting format to None for the raster
-    and vector_format to none for the vector
-
-    Parameters
-    ----------
-    fig : matplotlib.figure.Figure
-        The figure to save
-    save_location : str
-        Where to save the figure to
-
-    Keyword arguments
-    -----------------
-    dpi : int
-        The dots per inch of the output, by default 400
-    bbox_inches : str or val
-        The size of the bounding box, by default "tight"
-    pad_inches : str or val
-        The size of the padding, by default 0.1
-    verbose : bool
-        Whether to print more information, by default False
-    out_format : str
-        The format to save the output to, by default None,
-        which just uses the extension that is on save_location
-
-    Returns
-    -------
-    str
-        The locations saved to
-
-    """
-    dpi = kwargs.get("dpi", 400)
-    bbox_inches = kwargs.get("bbox_inches", "tight")
-    pad_inches = kwargs.get("pad_inches", 0.1)
-    verbose = kwargs.get("verbose", False)
-    save_locations = []
-
-    raster_info = ["raster", "format", "png"]
-    vector_info = ["vector", "vector_format", "pdf"]
-
-    for info in [raster_info, vector_info]:
-        name, key, default = info
-        final_path = get_plot_location(save_location, kwargs.get(key, default))
-        if verbose:
-            print(f"Saving {name} image to {final_path}")
-
-        skm_pyutils.path.make_path_if_not_exists(final_path)
-        fig.savefig(final_path, dpi=dpi, bbox_inches=bbox_inches, pad_inches=pad_inches)
-        save_locations.append(final_path)
-
-    return save_locations
-
-
-def get_plot_location(save_location, out_format):
-    if out_format is not None:
-        save_location = f"{os.path.splitext(save_location)[0]}.{out_format}"
-        dirname, basename = os.path.split(save_location)
-        return os.path.join(dirname, out_format, basename)
-
-
-def despine():
-    """Despine the current plot with trimming."""
-    sns.despine(offset=0, trim=True)
-
-
-def set_plot_style(palette="dark"):
-    """Set the seaborn palette and style."""
-    sns.set_palette(palette)
-    sns.set_context(
-        "paper",
-        font_scale=1.4,
-        rc={"lines.linewidth": 3.2},
-    )
+"""This module provides functions to interface with matplotlib."""
+
+import os
+from copy import copy
+
+from typing import TYPE_CHECKING
+import matplotlib.pyplot as plt
+import seaborn as sns
+import skm_pyutils.path
+
+if TYPE_CHECKING:
+    import matplotlib
+
+
+def setup_ax(ax=None, default={}, **kwargs) -> "matplotlib.axes.Axes":
+    """
+    Set up an axis object with default parameters that can be overridden.
+
+    In this way, a function can set default for the usual things that should
+    be plotted (e.g. plot axis labels), but keyword arguments can overwrite
+    any of these.
+
+    Parameters
+    ----------
+    ax : matplotlib.axes.Axes
+        The axis object to set up.
+    default : dict
+        Parameters to use for setting up the axis if not overridden.
+        Can contain any of the keys that can be keyword arguments
+
+    Keyword arguments
+    -----------------
+    xlabel : str
+        What to label the x-axis
+    ylabel : str
+        What to label the y-axis with
+    xticks : array like
+        x ticks
+    xticklabels : array like
+        Labels for the x- ticks
+    yticks : array like
+        y ticks
+    yticklabels : array like
+        Labels for the y- ticks
+    xrotate : float
+        The amount to rotate the x labels by
+    yrotate : float
+        The amount to rotate the y labels by
+    labelsize : float
+        The text size of the labels
+
+    Returns
+    -------
+    ax
+
+    """
+    if ax is None:
+        fig, ax = plt.subplots()
+    default = copy(default)
+    for key, value in kwargs.items():
+        default[key] = value
+    ax.set_xlabel(default.get("xlabel", None))
+    ax.set_ylabel(default.get("ylabel", None))
+    ax.set_title(default.get("title", None))
+    if "xticks" in default:
+        ax.set_xticks(default.get("xticks"))
+    if "xticklabels" in default:
+        ax.set_xticklabels(default.get("xticklabels"))
+    if "yticks" in default:
+        ax.set_yticks(default.get("yticks"))
+    if "yticklabels" in default:
+        ax.set_yticklabels(default.get("yticklabels"))
+    if "xrotate" in default:
+        plt.setp(
+            ax.get_xticklabels(),
+            rotation=default["xrotate"],
+            ha="right",
+            rotation_mode="anchor",
+        )
+    if "yrotate" in default:
+        plt.setp(
+            ax.get_yticklabels(),
+            rotation=default["yrotate"],
+            ha="right",
+            rotation_mode="anchor",
+        )
+    if "labelsize" in default:
+        ax.tick_params(labelsize=default["labelsize"])
+    return ax
+
+
+def save_simuran_plot(fig, save_location, **kwargs):
+    """
+    Save a figure using some default settings.
+
+    By default saves both a raster image (bitmap e.g. PNG, JPG)
+    and a vector image (e.g. PDF, SVG).
+    This can be disabled by setting format to None for the raster
+    and vector_format to none for the vector
+
+    Parameters
+    ----------
+    fig : matplotlib.figure.Figure
+        The figure to save
+    save_location : str
+        Where to save the figure to
+
+    Keyword arguments
+    -----------------
+    dpi : int
+        The dots per inch of the output, by default 400
+    bbox_inches : str or val
+        The size of the bounding box, by default "tight"
+    pad_inches : str or val
+        The size of the padding, by default 0.1
+    verbose : bool
+        Whether to print more information, by default False
+    out_format : str
+        The format to save the output to, by default None,
+        which just uses the extension that is on save_location
+
+    Returns
+    -------
+    str
+        The locations saved to
+
+    """
+    dpi = kwargs.get("dpi", 400)
+    bbox_inches = kwargs.get("bbox_inches", "tight")
+    pad_inches = kwargs.get("pad_inches", 0.1)
+    verbose = kwargs.get("verbose", False)
+    save_locations = []
+
+    raster_info = ["raster", "format", "png"]
+    vector_info = ["vector", "vector_format", "pdf"]
+
+    for info in [raster_info, vector_info]:
+        name, key, default = info
+        final_path = get_plot_location(save_location, kwargs.get(key, default))
+        if verbose:
+            print(f"Saving {name} image to {final_path}")
+
+        skm_pyutils.path.make_path_if_not_exists(final_path)
+        fig.savefig(final_path, dpi=dpi, bbox_inches=bbox_inches, pad_inches=pad_inches)
+        save_locations.append(final_path)
+
+    return save_locations
+
+
+def get_plot_location(save_location, out_format):
+    if out_format is not None:
+        save_location = f"{os.path.splitext(save_location)[0]}.{out_format}"
+        dirname, basename = os.path.split(save_location)
+        return os.path.join(dirname, out_format, basename)
+
+
+def despine():
+    """Despine the current plot with trimming."""
+    sns.despine(offset=0, trim=True)
+
+
+def set_plot_style(palette="dark"):
+    """Set the seaborn palette and style."""
+    sns.set_palette(palette)
+    sns.set_context(
+        "paper",
+        font_scale=1.4,
+        rc={"lines.linewidth": 3.2},
+    )
```

### Comparing `simuran-23.2.0/simuran/plot/figure.py` & `simuran-23.8.0/simuran/plot/figure.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-"""Holds a custom figure class."""
-import logging
-import os
-
-import matplotlib.pyplot as plt
-from simuran.plot.base_plot import save_simuran_plot, get_plot_location
-
-module_logger = logging.getLogger("simuran.plot.figure")
-
-
-class SimuranFigure(object):
-    """
-    A custom figure class that holds a figure and filename.
-
-    It also has helper methods, and support for saving only when ready.
-
-    Attributes
-    ----------
-    figure : matplotlib.figure.Figure
-        The underlying figure object.
-    filename : str
-        The filename that the figure will be saved to.
-    kwargs : dict
-        Extra keyword arguments used for saving.
-    done : bool
-        Whether this figure is ready to save or not.
-    closed : bool
-        Whether the underlying mpl figure has been closed.
-    """
-
-    def __init__(self, figure=None, filename=None, done=False, **kwargs):
-        """Holds a figure as well as a filename."""
-        self.figure = figure
-        self.filename = filename
-        self._output_filenames = {}
-        self.kwargs = kwargs
-        if "fig" in self.kwargs:
-            self.figure = self.kwargs.pop("fig")
-        if "name" in self.kwargs:
-            self.filename = self.kwargs.pop("name")
-        self.done = done
-        self.closed = False
-
-    def __del__(self):
-        """On deletion, closes the underlying figure."""
-        self.close()
-
-    @property
-    def output_filenames(self):
-        """Get the filenames that will be saved to."""
-        self._output_filenames = {}
-
-        self._output_filenames["raster"] = get_plot_location(
-            self.filename, self.kwargs.get("format", "png")
-        )
-        self._output_filenames["vector"] = get_plot_location(
-            self.filename, self.kwargs.get("vector_format", "pdf")
-        )
-
-        return self._output_filenames
-
-    @output_filenames.setter
-    def output_filenames(self, value):
-        self._output_filenames = value
-
-    def update_kwargs(self, **kwargs):
-        """Update self.kwargs."""
-        for key, val in kwargs.items():
-            self.kwargs[key] = val
-
-    def savefig(self, filename=None, **kwargs):
-        """
-        Call simuran.plot.base_plot.save_simuran_plot to save this figure.
-
-        The underlying figure object is saved to filename,
-        and any kwargs are passed to simuran.plot.base_plot.save_simuran_plot
-
-        Parameters
-        ----------
-        filename : str, optional
-            Overrides self.filename if passed.
-        kwargs : keyword arguments
-            simuran.plot.base_plot.save_simuran_plot for support kwargs
-
-        Returns
-        -------
-        None
-
-        """
-        if filename is None:
-            filename = self.filename
-        keyword_args = self.kwargs.copy()
-        for key, val in kwargs.items():
-            keyword_args[key] = val
-        save_simuran_plot(self.figure, filename, **keyword_args)
-
-    def save(self, filename=None, **kwargs):
-        """Alias for savefig."""
-        self.savefig(filename, **kwargs)
-
-    def close(self):
-        """Close the underlying figure if not closed."""
-        if self.closed:
-            return
-        self.closed = True
-        if self.figure is None:
-            return
-        try:
-            plt.close(self.figure)
-        except BaseException:
-            if hasattr(self.figure, "close"):
-                self.figure.close()
-            elif hasattr(self.figure, "_close"):
-                self.figure._close(None)
-            else:
-                if self.filename is None:
-                    module_logger.warning("Unable to close figure")
-                else:
-                    module_logger.warning(f"Unable to close {self.filename}")
-                self.closed = False
-
-    def isdone(self):
-        """Return if this figure is ready for saving."""
-        return self.done or self.closed
+"""Holds a custom figure class."""
+import logging
+import os
+
+import matplotlib.pyplot as plt
+from simuran.plot.base_plot import save_simuran_plot, get_plot_location
+
+module_logger = logging.getLogger("simuran.plot.figure")
+
+
+class SimuranFigure(object):
+    """
+    A custom figure class that holds a figure and filename.
+
+    It also has helper methods, and support for saving only when ready.
+
+    Attributes
+    ----------
+    figure : matplotlib.figure.Figure
+        The underlying figure object.
+    filename : str
+        The filename that the figure will be saved to.
+    kwargs : dict
+        Extra keyword arguments used for saving.
+    done : bool
+        Whether this figure is ready to save or not.
+    closed : bool
+        Whether the underlying mpl figure has been closed.
+    """
+
+    def __init__(self, figure=None, filename=None, done=False, **kwargs):
+        """Holds a figure as well as a filename."""
+        self.figure = figure
+        self.filename = filename
+        self._output_filenames = {}
+        self.kwargs = kwargs
+        if "fig" in self.kwargs:
+            self.figure = self.kwargs.pop("fig")
+        if "name" in self.kwargs:
+            self.filename = self.kwargs.pop("name")
+        self.done = done
+        self.closed = False
+
+    def __del__(self):
+        """On deletion, closes the underlying figure."""
+        self.close()
+
+    @property
+    def output_filenames(self):
+        """Get the filenames that will be saved to."""
+        self._output_filenames = {}
+
+        self._output_filenames["raster"] = get_plot_location(
+            self.filename, self.kwargs.get("format", "png")
+        )
+        self._output_filenames["vector"] = get_plot_location(
+            self.filename, self.kwargs.get("vector_format", "pdf")
+        )
+
+        return self._output_filenames
+
+    @output_filenames.setter
+    def output_filenames(self, value):
+        self._output_filenames = value
+
+    def update_kwargs(self, **kwargs):
+        """Update self.kwargs."""
+        for key, val in kwargs.items():
+            self.kwargs[key] = val
+
+    def savefig(self, filename=None, **kwargs):
+        """
+        Call simuran.plot.base_plot.save_simuran_plot to save this figure.
+
+        The underlying figure object is saved to filename,
+        and any kwargs are passed to simuran.plot.base_plot.save_simuran_plot
+
+        Parameters
+        ----------
+        filename : str, optional
+            Overrides self.filename if passed.
+        kwargs : keyword arguments
+            simuran.plot.base_plot.save_simuran_plot for support kwargs
+
+        Returns
+        -------
+        None
+
+        """
+        if filename is None:
+            filename = self.filename
+        keyword_args = self.kwargs.copy()
+        for key, val in kwargs.items():
+            keyword_args[key] = val
+        save_simuran_plot(self.figure, filename, **keyword_args)
+
+    def save(self, filename=None, **kwargs):
+        """Alias for savefig."""
+        self.savefig(filename, **kwargs)
+
+    def close(self):
+        """Close the underlying figure if not closed."""
+        if self.closed:
+            return
+        self.closed = True
+        if self.figure is None:
+            return
+        try:
+            plt.close(self.figure)
+        except BaseException:
+            if hasattr(self.figure, "close"):
+                self.figure.close()
+            elif hasattr(self.figure, "_close"):
+                self.figure._close(None)
+            else:
+                if self.filename is None:
+                    module_logger.warning("Unable to close figure")
+                else:
+                    module_logger.warning(f"Unable to close {self.filename}")
+                self.closed = False
+
+    def isdone(self):
+        """Return if this figure is ready for saving."""
+        return self.done or self.closed
```

### Comparing `simuran-23.2.0/simuran/plot/unit.py` & `simuran-23.8.0/simuran/plot/unit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,67 @@
-import seaborn as sns
-from typing import TYPE_CHECKING, List, Dict, Optional, Union
-import matplotlib.pyplot as plt
-from pathlib import Path
-
-if TYPE_CHECKING:
-    from pandas import DataFrame
-
-from simuran.plot.base_plot import set_plot_style, despine
-from simuran.plot.figure import SimuranFigure
-
-
-def plot_unit_properties(
-    units_table: "DataFrame",
-    properties: List[str],
-    log_scale: List[bool],
-    output_directory: Union[Path, str],
-    region_dict: Optional[Dict[str, str]] = None,
-    structure_name: str = "structure_acronym",
-    split_regions: bool = False,
-):
-    set_plot_style()
-
-    def match_region(region):
-        for k, v in region_dict.items():
-            if region in v:
-                return k
-        return "Other"
-
-    if split_regions:
-        units_table["Structure"] = units_table[structure_name].apply(match_region)
-    for prop, log in zip(properties, log_scale):
-        fig, ax = plt.subplots()
-        hue = "Structure" if split_regions else None
-        sns.kdeplot(
-            data=units_table, x=prop, log_scale=log, hue=hue, ax=ax, common_norm=False
-        )
-        despine()
-
-        fig = SimuranFigure(fig)
-        fig.save(Path(output_directory) / f"{prop}_distribution")
-
-
-def get_brain_regions_units(units, n=20):
-    return units["structure_acronym"].value_counts()[:n].index.tolist()
-
-
-color_dict = {
-    "cortex": "#08858C",
-    "thalamus": "#FC6B6F",
-    "hippocampus": "#7ED04B",
-    "midbrain": "#FC9DFE",
-}
-
-
-def ccf_unit_plot(session_units_channels):
-    from matplotlib import pyplot as plt
-
-    fig = plt.figure()
-    fig.set_size_inches([14, 8])
-    ax = fig.add_subplot(111, projection="3d")
-
-    def plot_probe_coords(probe_group):
-        ax.scatter(
-            probe_group["left_right_ccf_coordinate"],
-            probe_group["anterior_posterior_ccf_coordinate"],
-            -probe_group[
-                "dorsal_ventral_ccf_coordinate"
-            ],  # reverse the z coord so that down is into the brain
-        )
-        return probe_group["probe_id"].values[0]
-
-    probe_ids = session_units_channels.groupby("probe_id").apply(plot_probe_coords)
-
-    ax.set_zlabel("D/V")
-    ax.set_xlabel("Left/Right")
-    ax.set_ylabel("A/P")
-    ax.legend(probe_ids)
-    ax.view_init(elev=55, azim=70)
+import seaborn as sns
+from typing import TYPE_CHECKING, List, Dict, Optional, Union
+import matplotlib.pyplot as plt
+from pathlib import Path
+
+if TYPE_CHECKING:
+    from pandas import DataFrame
+
+from simuran.plot.base_plot import set_plot_style, despine
+from simuran.plot.figure import SimuranFigure
+
+
+def plot_unit_properties(
+    units_table: "DataFrame",
+    properties: List[str],
+    log_scale: List[bool],
+    output_directory: Union[Path, str],
+    region_dict: Optional[Dict[str, str]] = None,
+    structure_name: str = "structure_acronym",
+    split_regions: bool = False,
+):
+    set_plot_style()
+
+    def match_region(region):
+        for k, v in region_dict.items():
+            if region in v:
+                return k
+        return "Other"
+
+    if split_regions:
+        units_table["Structure"] = units_table[structure_name].apply(match_region)
+    for prop, log in zip(properties, log_scale):
+        fig, ax = plt.subplots()
+        hue = "Structure" if split_regions else None
+        sns.kdeplot(
+            data=units_table, x=prop, log_scale=log, hue=hue, ax=ax, common_norm=False
+        )
+        despine()
+
+        fig = SimuranFigure(fig)
+        fig.save(Path(output_directory) / f"{prop}_distribution")
+
+
+def ccf_unit_plot(session_units_channels):
+    from matplotlib import pyplot as plt
+
+    fig = plt.figure()
+    fig.set_size_inches([14, 8])
+    ax = fig.add_subplot(111, projection="3d")
+
+    def plot_probe_coords(probe_group):
+        ax.scatter(
+            probe_group["left_right_ccf_coordinate"],
+            probe_group["anterior_posterior_ccf_coordinate"],
+            -probe_group[
+                "dorsal_ventral_ccf_coordinate"
+            ],  # reverse the z coord so that down is into the brain
+        )
+        return probe_group["probe_id"].values[0]
+
+    probe_ids = session_units_channels.groupby("probe_id").apply(plot_probe_coords)
+
+    ax.set_zlabel("D/V")
+    ax.set_xlabel("Left/Right")
+    ax.set_ylabel("A/P")
+    ax.legend(probe_ids)
+    ax.view_init(elev=55, azim=70)
```

### Comparing `simuran-23.2.0/simuran/recording.py` & `simuran-23.8.0/simuran/recording.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,114 +1,119 @@
-"""This module holds single experiment related information."""
-from dataclasses import dataclass, field
-from pathlib import Path
-
-import numpy as np
-
-from simuran.core.base_class import BaseSimuran
-
-
-@dataclass
-class Recording(BaseSimuran):
-    """
-    Describe a full recording session and holds data.
-
-    This holds single unit information, spatial information,
-    EEG information, stimulation information, and
-    event information.
-
-    Note that anything you want to store on this object that
-    has not been accounted for in attributes, then this can
-    be stored on self.info
-
-    Attributes
-    ----------
-    attrs: dict or ParamHandler
-        Fixed information about this object, e.g. model or session type.
-    datetime : datetime.datetime
-        The date associated with this object, e.g. recording date.
-    tag : str
-        An optional tag to describe the object.
-        Default "untagged"
-    loader : simuran.loader.BaseLoader
-        A loader object that is used to load this object.
-        The relationship between the loader and this object
-        is established in self.load()
-    source_file : str
-        The path to the source file for this object.
-        For instance, an NWB file or an online URL.
-    last_loaded_source : str
-        The path to the last file this object was loaded from.
-    data : Any
-        When this object is loaded, complex variables can be stored in data.
-        For instance, an xarray object could be set as the data.
-        Generally speaking it is where the large (in terms of memory) objects
-        are stored after loading.
-    results : dict
-        A dictionary of results.
-    available_data : list[str]
-        A list of the available data on this recording as a string description.
-        E.g. ["spatial:running_speed", "ophys:deltaf/f", "behaviour:lick_times"]
-        This can be used in functions explicitly by following types, such
-        as those in pynwb, or simply as a helpful flag when debugging/analysing etc.
-
-    See also
-    --------
-    simuran.base_class.BaseSimuran
-
-    """
-
-    available_data: list = field(default_factory=list)
-
-    def load(self):
-        """Load each available attribute."""
-        super().load()
-        self.loader.load_recording(self)
-
-    def parse_metadata(self):
-        """Parse the metadata."""
-        self.loader.parse_metadata(self)
-
-    def parse_table_row(self, table, index):
-        """Parse the table row."""
-        self.loader.parse_table_row(table, index, self)
-
-    def get_name_for_save(self, rel_dir=None):
-        """
-        Get the name of the recording for saving purposes.
-
-        This is very useful when plotting.
-        For example, if the recording is in foo/bar/foo/pie.py
-        Then passing rel_dir as foo, would return the name as
-        bar--foo--pie
-
-        Parameters
-        ----------
-        rel_dir, str, optional
-            The directory to take the path relative to, default is None.
-            If None, it returns the full path with os.sep replaced by --
-            and with no extension.
-
-        Returns
-        -------
-        str
-            The name for saving, it has no extension and os.sep replaced by --
-
-        """
-        path_sf = Path(self.source_file)
-        if rel_dir is None:
-            return "--".join(path_sf.with_suffix("").parts)
-        name_up_to_rel = path_sf.relative_to(rel_dir).with_suffix("")
-        return "--".join(name_up_to_rel.parts)
-
-    def summarise(self) -> str:
-        if self.loader is None:
-            raise RuntimeError("Please set a loader before summarising")
-        if hasattr(self.loader, "summarise"):
-            return self.loader.summarise(self)
-        else:
-            raise NotImplementedError(
-                "Please implement a summarise method on the selected loader"
-            )
-
-    def __del__(self):
-        self.unload()
+"""This module holds single experiment related information."""
+from dataclasses import dataclass, field
+from pathlib import Path
+
+import numpy as np
+
+from simuran.core.base_class import BaseSimuran
+
+
+@dataclass
+class Recording(BaseSimuran):
+    """
+    Describe a full recording session and holds data.
+
+    This holds single unit information, spatial information,
+    EEG information, stimulation information, and
+    event information.
+
+    Note that anything you want to store on this object that
+    has not been accounted for in attributes, then this can
+    be stored on self.info
+
+    Attributes
+    ----------
+    attrs: dict or ParamHandler
+        Fixed information about this object, e.g. model or session type.
+    datetime : datetime.datetime
+        The date associated with this object, e.g. recording date.
+    tag : str
+        An optional tag to describe the object.
+        Default "untagged"
+    loader : simuran.loader.BaseLoader
+        A loader object that is used to load this object.
+        The relationship between the loader and this object
+        is established in self.load()
+    source_file : str
+        The path to the source file for this object.
+        For instance, an NWB file or an online URL.
+    last_loaded_source : str
+        The path to the last file this object was loaded from.
+    data : Any
+        When this object is loaded, complex variables can be stored in data.
+        For instance, an xarray object could be set as the data.
+        Generally speaking it is where the large (in terms of memory) objects
+        are stored after loading.
+    results : dict
+        A dictionary of results.
+    available_data : list[str]
+        A list of the available data on this recording as a string description.
+        E.g. ["spatial:running_speed", "ophys:deltaf/f", "behaviour:lick_times"]
+        This can be used in functions explicitly by following types, such
+        as those in pynwb, or simply as a helpful flag when debugging/analysing etc.
+
+    See also
+    --------
+    simuran.base_class.BaseSimuran
+
+    """
+
+    available_data: list = field(default_factory=list)
+
+    def load(self):
+        """Load each available attribute."""
+        super().load()
+        self.loader.load_recording(self)
+
+    def parse_metadata(self):
+        """Parse the metadata."""
+        self.loader.parse_metadata(self)
+
+    def parse_table_row(self, table, index):
+        """Parse the table row."""
+        self.loader.parse_table_row(table, index, self)
+
+    def get_name_for_save(self, rel_dir=None):
+        """
+        Get the name of the recording for saving purposes.
+
+        This is very useful when plotting.
+        For example, if the recording is in foo/bar/foo/pie.py
+        Then passing rel_dir as foo, would return the name as
+        bar--foo--pie
+
+        Parameters
+        ----------
+        rel_dir, str, optional
+            The directory to take the path relative to, default is None.
+            If None, it returns the full path with os.sep replaced by --
+            and with no extension.
+
+        Returns
+        -------
+        str
+            The name for saving, it has no extension and os.sep replaced by --
+
+        """
+        if self.source_file is None:
+            raise RuntimeError("Please set a source file before getting a name")
+        path_sf = Path(self.source_file)
+        if rel_dir is None:
+            return "--".join(path_sf.with_suffix("").parts)
+        try:
+            name_up_to_rel = path_sf.relative_to(rel_dir).with_suffix("")
+            return "--".join(name_up_to_rel.parts)
+        except Exception:
+            return "--".join(path_sf.with_suffix("").parts)
+
+    def summarise(self) -> str:
+        if self.loader is None:
+            raise RuntimeError("Please set a loader before summarising")
+        if hasattr(self.loader, "summarise"):
+            return self.loader.summarise(self)
+        else:
+            raise NotImplementedError(
+                "Please implement a summarise method on the selected loader"
+            )
+
+    def __del__(self):
+        self.unload()
```

### Comparing `simuran-23.2.0/simuran/recording_container.py` & `simuran-23.8.0/simuran/recording_container.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,272 +1,309 @@
-"""This module provides a container for multiple recording objects."""
-from __future__ import annotations
-
-import copy
-import os
-from collections.abc import Iterable as abcIterable
-from dataclasses import dataclass, field
-import logging
-from pathlib import Path
-import pickle
-from typing import TYPE_CHECKING, Iterable, Optional, Union, overload, List, Tuple, Any
-from skm_pyutils.table import df_to_file
-import gc
-
-import pandas as pd
-
-from simuran.core.base_container import GenericContainer
-from simuran.recording import Recording
-
-if TYPE_CHECKING:
-    from simuran.loaders.base_loader import BaseLoader
-
-module_logger = logging.getLogger("simuran.recording_container")
-
-
-@dataclass
-class RecordingContainer(GenericContainer):
-    """
-    A class to hold recording objects.
-
-    Attributes
-    ----------
-    load_on_fly : bool
-        Should information be loaded at the start in bulk, or as needed.
-    last_loaded : simuran.recording.Recording
-        A reference to the last used recording.
-    _last_loaded_idx : int
-        The index of the last loaded recording.
-    attrs : dict
-        Dictionary of metadata.
-    invalid_recording_locations : list of int
-        Index of recordings that could not be set up.
-    table : Dataframe
-        A table which describes each recording in the container.
-        For example, each row could contain metadata about the session,
-        and a path to a source NWB file to load the data for that session.
-
-    """
-
-    load_on_fly: bool = True
-    last_loaded: "Recording" = field(default_factory=Recording)
-    attrs: dict = field(default_factory=dict)
-    invalid_recording_locations: list = field(default_factory=list)
-    table: "pd.DataFrame" = field(default_factory=pd.DataFrame)
-    _last_loaded_idx: int = field(repr=False, init=False, default=-1)
-
-    @classmethod
-    def from_table(
-        cls,
-        table: "pd.DataFrame",
-        loader: Union["BaseLoader", Iterable["BaseLoader"]],
-        load_on_fly: bool = True,
-    ) -> RecordingContainer:
-        """
-        Create a Recording container from a pandas dataframe.
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The dataframe to load from.
-        loader : BaseLoader or iterable of BaseLoader
-            The loader to use for all recordings if one passed
-            Otherwise a different loader to use for each recording.
-        load_on_fly : bool, optional
-            Whether to load the data for the recording container on the fly.
-            Defaults to True (best for memory usage).
-
-        Returns
-        -------
-        simuran.RecordingContainer
-
-        """
-        rc = cls(load_on_fly=load_on_fly)
-        rc.table = table
-
-        for i in range(len(table)):
-            loader_ = loader[i] if isinstance(loader, abcIterable) else loader
-            recording = Recording()
-            module_logger.debug(f"Parsing information from table for row {i}")
-            loader_.parse_table_row(table, i, recording)
-            rc.append(recording)
-
-        return rc
-
-    def load(self) -> None:
-        ...
-        """Load all recordings."""
-
-    @overload
-    def load(self, idx: int) -> "Recording":
-        ...
-        """Load recording at index idx and return it."""
-
-    def load(self, idx: Optional[int] = None, force_reload=False) -> "Recording":
-        """
-        Get the item at the specified index, and load it if not already loaded.
-
-        Parameters
-        ----------
-        idx : int
-            The index of the the item to retrieve.
-        force_reload : bool
-            Whether to force reload if loading on the fly.
-
-        Returns
-        -------
-        simuran.recording.Recording
-            The recording at the specified index.
-
-        """
-        if idx is None:
-            if self.load_on_fly:
-                raise RuntimeError("Can't bulk load when load_on_fly=True")
-            for r in self:
-                r.load()
-            return
-        if self.load_on_fly:
-            if self._last_loaded_idx != idx or force_reload:
-                del self.last_loaded
-                gc.collect()
-                self.last_loaded = copy.copy(self[idx])
-                self.last_loaded.load()
-                self._last_loaded_idx = idx
-            return self.last_loaded
-        else:
-            self[idx].load()
-            return self[idx]
-
-    def get_results(self, idx=None):
-        """
-        Get the results stored on the objects in the container.
-
-        Parameters
-        ----------
-        idx : int, optional
-            If passed, the index of the item to get the results for, by default None.
-
-        Returns
-        -------
-        list of dict, or dict
-            If idx is None, a list of dictionaries, else a single dictionary.
-
-        """
-        return [item.results for item in self] if idx is None else self[idx].results
-
-    def find_recording_with_source(self, source_file) -> Union[int, List]:
-        """
-        Return the index of the recording in the container with the given source file.
-
-        Parameters
-        ----------
-        source_file : str
-            The source file to search for.
-
-        Returns
-        -------
-        int, list, or None
-            The index of the recording in the container.
-            or a list of indices of the recordings if multiple
-            matches are found.
-            or None if the source file is not found.
-
-        """
-        locations = []
-        for i, recording in enumerate(self):
-            compare = recording.source_file[-len(source_file) :]
-            if os.path.normpath(source_file) == os.path.normpath(compare):
-                locations.append(i)
-        return locations[0] if len(locations) == 1 else locations
-
-    def find_recording_by_attribute(self, key: str, value: Any) -> Recording:
-        """
-        Return the recording(s) with self.attrs[key] matching value.
-
-        Parameters
-        ----------
-        key : str
-            The attribute to match by.
-        value : Any
-            The value to match by.
-
-        Returns
-        -------
-        Recording
-            The matched recording (first match)
-        """
-        for recording in self:
-            if recording.attrs[key] == value:
-                return recording
-        raise ValueError(
-            f"No recording with key {key} matching {value}, values are {[r.attrs[key] for r in self.container]}"
-        )
-
-    def load_iter(self):
-        """Iterator through the container that loads data on item retrieval."""
-        return RecordingContainerLoadIterator(self)
-
-    def dump(self, filename, results_only=True):
-        """
-        Dump recording_container to file with pickle.
-
-        Parameters
-        ----------
-        filename : str or Path
-            The output path.
-        results_only : bool, optional
-            Only save the results
-
-        Returns
-        -------
-        None
-
-        """
-        to_dump = self.get_results() if results_only else self
-        with open(filename, "wb") as outfile:
-            pickle.dump(to_dump, outfile)
-
-    def save_results_to_table(self, filename=None):
-        """
-        Dump recording_container results to file with pandas.
-
-        Parameters
-        ----------
-        filename : str or Path
-            The output path.
-
-        Returns
-        -------
-        Dataframe
-            The resulting dataframe
-
-        """
-        results = self.get_results()
-        for res_dict, item in zip(results, self):
-            sfile = item.source_file
-            if sfile is not None:
-                sfile = Path(sfile)
-                res_dict.setdefault("Directory", sfile.parent)
-                res_dict.setdefault("Filename", sfile.name)
-        df = pd.DataFrame.from_dict(results)
-
-        if filename is not None:
-            df_to_file(df, filename)
-
-        return df
-
-
-class RecordingContainerLoadIterator(object):
-    """An iterator for loading recording container on the fly."""
-
-    def __init__(self, recording_container: "RecordingContainer"):
-        self.recording_container = recording_container
-        self.current = -1
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        self.current += 1
-        if self.current < len(self.recording_container):
-            return self.recording_container.load(self.current)
-        raise StopIteration
+"""This module provides a container for multiple recording objects."""
+from __future__ import annotations
+
+import copy
+import os
+from collections.abc import Iterable as abcIterable
+from dataclasses import dataclass, field
+import logging
+from pathlib import Path
+import pickle
+from typing import TYPE_CHECKING, Iterable, Optional, Union, overload, List, Tuple, Any
+from skm_pyutils.table import df_to_file
+import gc
+
+import pandas as pd
+
+from simuran.core.base_container import GenericContainer
+from simuran.recording import Recording
+
+if TYPE_CHECKING:
+    from simuran.loaders.base_loader import BaseLoader
+
+module_logger = logging.getLogger("simuran.recording_container")
+
+
+@dataclass
+class RecordingContainer(GenericContainer):
+    """
+    A class to hold recording objects.
+
+    Attributes
+    ----------
+    load_on_fly : bool
+        Should information be loaded at the start in bulk, or as needed.
+    last_loaded : simuran.recording.Recording
+        A reference to the last used recording.
+    _last_loaded_idx : int
+        The index of the last loaded recording.
+    attrs : dict
+        Dictionary of metadata.
+    invalid_recording_locations : list of int
+        Index of recordings that could not be set up.
+    table : Dataframe
+        A table which describes each recording in the container.
+        For example, each row could contain metadata about the session,
+        and a path to a source NWB file to load the data for that session.
+
+    """
+
+    load_on_fly: bool = True
+    last_loaded: "Recording" = field(default_factory=Recording)
+    attrs: dict = field(default_factory=dict)
+    invalid_recording_locations: list = field(default_factory=list)
+    table: "pd.DataFrame" = field(default_factory=pd.DataFrame)
+    _last_loaded_idx: int = field(repr=False, init=False, default=-1)
+
+    @classmethod
+    def from_table(
+        cls,
+        table: "pd.DataFrame",
+        loader: Union["BaseLoader", Iterable["BaseLoader"]],
+        load_on_fly: bool = True,
+    ) -> RecordingContainer:
+        """
+        Create a Recording container from a pandas dataframe.
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The dataframe to load from.
+        loader : BaseLoader or iterable of BaseLoader
+            The loader to use for all recordings if one passed
+            Otherwise a different loader to use for each recording.
+        load_on_fly : bool, optional
+            Whether to load the data for the recording container on the fly.
+            Defaults to True (best for memory usage).
+
+        Returns
+        -------
+        simuran.RecordingContainer
+
+        """
+        rc = cls(load_on_fly=load_on_fly)
+        rc._setup_from_table(table, loader)
+        return rc
+
+    def load(self) -> None:
+        ...
+        """Load all recordings."""
+
+    @overload
+    def load(self, idx: int) -> "Recording":
+        ...
+        """Load recording at index idx and return it."""
+
+    def load(self, idx: Optional[int] = None, force_reload=False) -> "Recording":
+        """
+        Get the item at the specified index, and load it if not already loaded.
+
+        Parameters
+        ----------
+        idx : int
+            The index of the the item to retrieve.
+        force_reload : bool
+            Whether to force reload if loading on the fly.
+
+        Returns
+        -------
+        simuran.recording.Recording
+            The recording at the specified index.
+
+        """
+        if idx is None:
+            if self.load_on_fly:
+                raise RuntimeError("Can't bulk load when load_on_fly=True")
+            for r in self:
+                r.load()
+            return
+        if self.load_on_fly:
+            if self._last_loaded_idx != idx or force_reload:
+                del self.last_loaded
+                gc.collect()
+                self.last_loaded = copy.copy(self[idx])
+                self.last_loaded.load()
+                self._last_loaded_idx = idx
+            return self.last_loaded
+        else:
+            self[idx].load()
+            return self[idx]
+
+    def get_results(self, idx=None):
+        """
+        Get the results stored on the objects in the container.
+
+        Parameters
+        ----------
+        idx : int, optional
+            If passed, the index of the item to get the results for, by default None.
+
+        Returns
+        -------
+        list of dict, or dict
+            If idx is None, a list of dictionaries, else a single dictionary.
+
+        """
+        return [item.results for item in self] if idx is None else self[idx].results
+
+    def find_recording_with_source(self, source_file) -> Union[int, List]:
+        """
+        Return the index of the recording in the container with the given source file.
+
+        Parameters
+        ----------
+        source_file : str
+            The source file to search for.
+
+        Returns
+        -------
+        int, list, or None
+            The index of the recording in the container.
+            or a list of indices of the recordings if multiple
+            matches are found.
+            or None if the source file is not found.
+
+        """
+        locations = []
+        for i, recording in enumerate(self):
+            compare = recording.source_file[-len(source_file) :]
+            if os.path.normpath(source_file) == os.path.normpath(compare):
+                locations.append(i)
+        return locations[0] if len(locations) == 1 else locations
+
+    def find_recording_by_attribute(self, key: str, value: Any) -> Recording:
+        """
+        Return the recording(s) with self.attrs[key] matching value.
+
+        Parameters
+        ----------
+        key : str
+            The attribute to match by.
+        value : Any
+            The value to match by.
+
+        Returns
+        -------
+        Recording
+            The matched recording (first match)
+        """
+        for recording in self:
+            if recording.attrs[key] == value:
+                return recording
+        raise ValueError(
+            f"No recording with key {key} matching {value}, values are {[r.attrs[key] for r in self.container]}"
+        )
+
+    def load_iter(self):
+        """Iterator through the container that loads data on item retrieval."""
+        return RecordingContainerLoadIterator(self)
+
+    def dump(self, filename, results_only=True):
+        """
+        Dump recording_container to file with pickle.
+
+        Parameters
+        ----------
+        filename : str or Path
+            The output path.
+        results_only : bool, optional
+            Only save the results
+
+        Returns
+        -------
+        None
+
+        """
+        to_dump = self.get_results() if results_only else self
+        with open(filename, "wb") as outfile:
+            pickle.dump(to_dump, outfile)
+
+    def save_results_to_table(self, filename=None):
+        """
+        Dump recording_container results to file with pandas.
+
+        Parameters
+        ----------
+        filename : str or Path
+            The output path.
+
+        Returns
+        -------
+        Dataframe
+            The resulting dataframe
+
+        """
+        results = self.get_results()
+        for res_dict, item in zip(results, self):
+            sfile = item.source_file
+            if sfile is not None:
+                sfile = Path(sfile)
+                res_dict.setdefault("Directory", sfile.parent)
+                res_dict.setdefault("Filename", sfile.name)
+        df = pd.DataFrame.from_dict(results)
+
+        if filename is not None:
+            df_to_file(df, filename)
+
+        return df
+
+    def filter_table(
+        self,
+        rows: Union[List[int], slice],
+        loader: Optional[Union["BaseLoader", Iterable["BaseLoader"]]] = None,
+        inplace: bool = False,
+    ) -> RecordingContainer:
+        """
+        Filter the table by rows.
+
+        Parameters
+        ----------
+        rows : list of int or slice
+            The rows to keep.
+        loader : BaseLoader or list of BaseLoader
+            The loader(s) to use to parse the table.
+            If None, it is assumed that the first loader in the
+            container is the correct one.
+        inplace : bool, optional
+            Whether to modify the current container, by default False
+
+        Returns
+        -------
+        RecordingContainer
+            The filtered container.
+
+        """
+        table = self.table.copy().iloc[rows]
+        if loader is None:
+            loader = self[0].loader
+        if inplace:
+            self._setup_from_table(table, loader)
+            return self
+        else:
+            return RecordingContainer.from_table(table, loader)
+
+    def _setup_from_table(self, table, loader) -> None:
+        self.table = table
+
+        for i in range(len(table)):
+            loader_ = loader[i] if isinstance(loader, abcIterable) else loader
+            recording = Recording()
+            module_logger.debug(f"Parsing information from table for row {i}")
+            loader_.parse_table_row(table, i, recording)
+            self.append(recording)
+
+
+class RecordingContainerLoadIterator(object):
+    """An iterator for loading recording container on the fly."""
+
+    def __init__(self, recording_container: "RecordingContainer"):
+        self.recording_container = recording_container
+        self.current = -1
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        self.current += 1
+        if self.current < len(self.recording_container):
+            return self.recording_container.load(self.current)
+        raise StopIteration
```

### Comparing `simuran-23.2.0/simuran/ui/node.py` & `simuran-23.8.0/simuran/ui/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,239 +1,267 @@
-"""
-Handles creating nodes in the UI.
-
-Uses the factory method design pattern.
-"""
-
-from copy import deepcopy
-
-import dearpygui.dearpygui as dpg
-from rich import print
-
-# Should probably convert to abstract
-
-# TODO this needs to be a factory method
-# And then nodes - so node factories make nodes
-
-# TODO abstract
-# TODO remove getter and setter
-class BaseNode(object):
-    def __init__(self, parent, label="Node", tag=None, debug=False):
-        self.tag = dpg.generate_uuid() if tag is None else tag
-        self.label = label
-        self.parent = parent
-        self.attributes = {}
-        self.contents = {}
-        self.debug = debug
-        self.category = None
-
-        # TODO this should hold application state
-        self.state = {}
-
-        self.input_attributes = {}
-        self.output_attributes = {}
-
-        self.plot_paths = None
-
-    def on_connect(self, sender, receiver):
-        # Needs work for context
-        sender_attr = self.get_attribute(sender)
-        receiver_attr = self.get_attribute(receiver)
-
-        if sender_attr is not None:
-            self.output_attributes[f"{sender}--{receiver}"] = receiver
-
-            if self.debug:
-                print(f"{self.tag}: Connected to {receiver} as sender")
-
-        if receiver_attr is not None:
-            self.input_attributes[f"{sender}--{receiver}"] = sender
-
-            if self.debug:
-                print(f"{self.tag}: Connected to {sender} as receiver")
-
-    def on_disconnect(self, sender, receiver):
-        # Needs work for context
-        sender_attr = self.get_attribute(sender)
-        receiver_attr = self.get_attribute(receiver)
-
-        if sender_attr is not None:
-            receiver_attr = self.output_attributes.pop(f"{sender}--{receiver}")
-
-            if self.debug:
-                print(f"{self.tag}: Disconnected from {receiver} as sender")
-
-        if receiver_attr is not None:
-            sender_attr = self.input_attributes.pop(f"{sender}--{receiver}")
-
-            if self.debug:
-                print(f"{self.tag}: Disconnected from {sender} as receiver")
-
-    def create(self, attributes, clicked_callback, tooltip=None, position=None):
-        if position is None:
-            position = []
-        dpg.add_node(
-            label=self.label,
-            parent=self.parent,
-            show=True,
-            pos=position,
-            tag=self.tag,
-            use_internal_label=self.debug,
-        )
-
-        for attribute in attributes:
-            attribute_tag = dpg.generate_uuid()
-            self.attributes[attribute_tag] = attribute
-            contents = attribute.pop("contents", [])
-            attribute_tooltip = attribute.pop("tooltip", None)
-            dpg.add_node_attribute(
-                parent=self.tag,
-                tag=attribute_tag,
-                use_internal_label=self.debug,
-                **attribute,
-            )
-            if attribute_tooltip is not None:
-                tooltip_tag = dpg.generate_uuid()
-                with dpg.tooltip(parent=attribute_tag):
-                    dpg.add_text(default_value=attribute_tooltip, tag=tooltip_tag)
-                attribute["tooltip"] = attribute_tooltip
-                attribute["tooltip_tag"] = tooltip_tag
-            if len(contents) != 0:
-                attribute["contents"] = contents
-
-            for content in contents:
-                type_ = content.pop("type", "TEXT")
-                content_tag = dpg.generate_uuid()
-                if type_ == "INT":
-                    dpg.add_input_int(parent=attribute_tag, tag=content_tag, **content)
-                elif type_ == "FLOAT":
-                    dpg.add_input_float(
-                        parent=attribute_tag, tag=content_tag, **content
-                    )
-                elif type_ == "TEXT":
-                    dpg.add_input_text(parent=attribute_tag, tag=content_tag, **content)
-                    # TODO perhaps a separate menu for selecting files
-                    handler_tag = dpg.generate_uuid()
-                    with dpg.item_handler_registry(tag=handler_tag) as handler:
-                        dpg.add_item_clicked_handler(
-                            button=1,
-                            callback=clicked_callback,
-                            user_data=["content", content["label"], self.tag],
-                        )
-                    dpg.bind_item_handler_registry(content_tag, handler_tag)
-                else:
-                    raise ValueError(
-                        f'Unsupported content type {type_}, options are {("INT", "FLOAT", "TEXT")}'
-                    )
-
-                content["type"] = type_
-                content["parent"] = attribute_tag
-                self.contents[content_tag] = content
-
-        # real version node.tag
-        dpg.add_item_clicked_handler(
-            button=1,
-            callback=clicked_callback,
-            user_data=["node", self.tag],
-            parent="node context handler",
-        )
-        dpg.bind_item_handler_registry(self.tag, "node context handler")
-
-    def process(self, nodes):
-        if self.debug:
-            print(f"Processing {self.tag} -- {self.label}")
-
-    def __str__(self):
-        return f"SIMURAN node with label {self.label}, tag {self.tag} and contains {[self.attribute_tags, self.content_tags]}"
-
-    def get_values(self):
-        return dpg.get_values(list(self.contents.keys()))
-
-    def get_value_of_label(self, label):
-        content_tag, _ = self.get_content_with_label(label)
-        return dpg.get_value(content_tag)
-
-    def get_content_with_label(self, label):
-        return next(
-            (
-                (content_tag, content)
-                for content_tag, content in self.contents.items()
-                if label == content.get("label", "")
-            ),
-            (None, None),
-        )
-
-    def has_attribute(self, tag):
-        return tag in self.attributes.keys()
-
-    def get_attribute(self, tag):
-        return self.attributes[tag] if tag in self.attributes.keys() else None
-
-    def get_owning_attribute(self, content_tag):
-        return self.attributes[self.contents[content_tag]["parent"]]
-
-    def set_source_file(self, fpath, label=None):
-        if label is None:
-            for content_tag, content in self.contents.items():
-                if content.get("label", "").startswith("File"):
-                    break
-        else:
-            content_tag, content = self.get_content_with_label(label)
-        dpg.set_value(content_tag, fpath)
-
-        owning_attribute = self.get_owning_attribute(content_tag)
-        tooltip_tag = owning_attribute["tooltip_tag"]
-        dpg.set_value(tooltip_tag, fpath)
-
-    def get_downstream_nodes(self, nodes):
-        downstream_nodes = []
-        output_attributes = self.output_attributes.values()
-        for _, node in nodes.items():
-            downstream_nodes.extend(
-                node.tag
-                for attribute in output_attributes
-                if node.has_attribute(attribute)
-            )
-
-        return downstream_nodes
-
-
-class NodeFactory(object):
-    def __init__(self, **kwargs):
-        self.node_class = kwargs.get("node_class", BaseNode)
-        self.label = kwargs.get("label", "Custom name")
-        self.category = kwargs.get("category", "default")
-        self.debug = kwargs.get("debug", False)
-        self.attributes = kwargs.get("attributes", [])
-        self.clicked_callback = kwargs.get("clicked_callback", None)
-
-        # Keep track of the ID of created items
-        self.created_nodes = []
-
-    def create(self, editor_id, **kwargs):
-        position = kwargs.get("position", [])
-
-        num_nodes = len(self.created_nodes)
-        new_node_label = self.label
-        if num_nodes > 0:
-            new_node_label = f"{new_node_label} {num_nodes}"
-        new_node = self.node_class(
-            parent=editor_id, label=new_node_label, debug=self.debug
-        )
-        new_node.name = self.label
-        new_node.category = self.category
-        new_node.create(
-            deepcopy(self.attributes), self.clicked_callback, position=position
-        )
-
-        self.created_nodes.append(new_node.tag)
-
-        if self.debug:
-            print(self)
-
-        return new_node
-
-    def __str__(self):
-        return (
-            f"SIMURAN Node Factory with label {self.label},"
-            + f" and attributes {self.attributes}"
-        )
+"""
+Handles creating nodes in the UI.
+
+Uses the factory method design pattern.
+"""
+
+from copy import deepcopy
+import contextlib
+
+import dearpygui.dearpygui as dpg
+from rich import print
+
+
+class BaseNode(object):
+    def __init__(self, parent, label="Node", tag=None, debug=False):
+        self.tag = dpg.generate_uuid() if tag is None else tag
+        self.label = label
+        self.parent = parent
+        self.attributes = {}
+        self.contents = {}
+        self.debug = debug
+        self.category = None
+        self.position = None
+        self.factory_label = None
+        self.internal_id = None
+
+        self.state = {}
+        self.input_attributes = {}
+        self.output_attributes = {}
+
+        self.plot_paths = None
+
+    def on_connect(self, sender, receiver):
+        sender_attr = self.get_attribute(sender)
+        receiver_attr = self.get_attribute(receiver)
+
+        if sender_attr is not None:
+            if self.debug:
+                print(f"{self.tag}: Connected to {receiver} as sender {sender}")
+            self.output_attributes[f"{sender}->{receiver}"] = receiver
+
+        if receiver_attr is not None:
+            if self.debug:
+                print(f"{self.tag}: Connected to {sender} as receiver {receiver}")
+            self.input_attributes[f"{sender}->{receiver}"] = sender
+
+    def on_disconnect(self, sender, receiver):
+        sender_attr = self.get_attribute(sender)
+        receiver_attr = self.get_attribute(receiver)
+
+        if sender_attr is not None:
+            if self.debug:
+                print(f"{self.tag}: Disconnected from {receiver} as sender {sender}")
+            self.output_attributes.pop(f"{sender}->{receiver}")
+
+        if receiver_attr is not None:
+            if self.debug:
+                print(f"{self.tag}: Disconnected from {sender} as receiver {receiver}")
+            self.input_attributes.pop(f"{sender}->{receiver}")
+
+    def create(self, attributes, clicked_callback, position=None):
+        self.position = position
+        if position is None:
+            position = []
+        dpg.add_node(
+            label=self.label,
+            parent=self.parent,
+            show=True,
+            pos=position,
+            tag=self.tag,
+            use_internal_label=self.debug,
+        )
+
+        for attribute in attributes:
+            attribute_tag = dpg.generate_uuid()
+            self.attributes[attribute_tag] = attribute
+            contents = attribute.pop("contents", [])
+            attribute_tooltip = attribute.pop("tooltip", None)
+            dpg.add_node_attribute(
+                parent=self.tag,
+                tag=attribute_tag,
+                use_internal_label=self.debug,
+                **attribute,
+            )
+            if attribute_tooltip is not None:
+                tooltip_tag = dpg.generate_uuid()
+                with dpg.tooltip(parent=attribute_tag):
+                    dpg.add_text(default_value=attribute_tooltip, tag=tooltip_tag)
+                attribute["tooltip"] = attribute_tooltip
+                attribute["tooltip_tag"] = tooltip_tag
+            if len(contents) != 0:
+                attribute["contents"] = contents
+
+            for content in contents:
+                type_ = content.pop("type", "TEXT")
+                content_tag = dpg.generate_uuid()
+                if type_ == "INT":
+                    dpg.add_input_int(parent=attribute_tag, tag=content_tag, **content)
+                elif type_ == "FLOAT":
+                    dpg.add_input_float(
+                        parent=attribute_tag, tag=content_tag, **content
+                    )
+                elif type_ == "TEXT":
+                    dpg.add_input_text(parent=attribute_tag, tag=content_tag, **content)
+                    handler_tag = dpg.generate_uuid()
+                    with dpg.item_handler_registry(tag=handler_tag) as handler:
+                        dpg.add_item_clicked_handler(
+                            button=1,
+                            callback=clicked_callback,
+                            user_data=["content", content["label"], self.tag],
+                        )
+                    dpg.bind_item_handler_registry(content_tag, handler_tag)
+                else:
+                    raise ValueError(
+                        f'Unsupported content type {type_}, options are {("INT", "FLOAT", "TEXT")}'
+                    )
+
+                content["type"] = type_
+                content["parent"] = attribute_tag
+                self.contents[content_tag] = content
+
+        # real version node.tag
+        dpg.add_item_clicked_handler(
+            button=1,
+            callback=clicked_callback,
+            user_data=["node", self.tag],
+            parent="node context handler",
+        )
+        dpg.bind_item_handler_registry(self.tag, "node context handler")
+
+    def process(self, nodes):
+        if self.debug:
+            print(f"Processing {self.tag} -- {self.label}")
+
+    def __str__(self):
+        return f"SIMURAN node with label {self.label}, tag {self.tag} and contains {self.attributes}, {self.contents}"
+
+    def get_values(self):
+        return dpg.get_values(list(self.contents.keys()))
+
+    def get_value_of_label(self, label):
+        content_tag, _ = self.get_content_with_label(label)
+        return dpg.get_value(content_tag)
+
+    def get_content_with_label(self, label):
+        return next(
+            (
+                (content_tag, content)
+                for content_tag, content in self.contents.items()
+                if label == content.get("label", "")
+            ),
+            (None, None),
+        )
+
+    def has_attribute(self, tag):
+        return tag in self.attributes.keys()
+
+    def get_attribute(self, tag):
+        return self.attributes[tag] if tag in self.attributes.keys() else None
+
+    def get_attribute_with_label(self, label):
+        return next(
+            (
+                (attribute_tag, attribute)
+                for attribute_tag, attribute in self.attributes.items()
+                if label == attribute.get("label", "")
+            ),
+            (None, None),
+        )
+
+    def get_owning_attribute(self, content_tag):
+        return self.attributes[self.contents[content_tag]["parent"]]
+
+    def set_source_file(self, fpath, label=None):
+        if label is None:
+            for content_tag, content in self.contents.items():
+                if content.get("label", "").startswith("File"):
+                    break
+        else:
+            content_tag, content = self.get_content_with_label(label)
+        dpg.set_value(content_tag, fpath)
+
+        owning_attribute = self.get_owning_attribute(content_tag)
+        tooltip_tag = owning_attribute["tooltip_tag"]
+        dpg.set_value(tooltip_tag, fpath)
+
+    def get_downstream_nodes(self, nodes):
+        downstream_nodes = []
+        output_attributes = self.output_attributes.values()
+        if self.debug:
+            print(
+                f"Searching for attributes {output_attributes}"
+                f" in nodes with attributes: {[(k, list(node.attributes.keys())) for k, node in nodes.items()]}"
+            )
+        for _, node in nodes.items():
+            downstream_nodes.extend(
+                node.tag
+                for attribute in output_attributes
+                if node.has_attribute(attribute)
+            )
+
+        return downstream_nodes
+
+    def find_matching_input_node(self, reciever_label, nodes):
+        for key, _ in self.input_attributes.items():
+            sender, receiver = key.split("->")
+            with contextlib.suppress(ValueError):
+                sender = int(sender)
+            with contextlib.suppress(ValueError):
+                receiver = int(receiver)
+            attr = self.get_attribute(receiver)
+            if attr["label"] == reciever_label:
+                source_file_tag = sender
+                break
+
+        for node in nodes.values():
+            if node.has_attribute(source_file_tag):
+                input_node = node
+                break
+
+        return input_node
+
+
+class NodeFactory(object):
+    def __init__(self, **kwargs):
+        self.node_class = kwargs.get("node_class", BaseNode)
+        self.label = kwargs.get("label", "Custom name")
+        self.category = kwargs.get("category", "default")
+        self.debug = kwargs.get("debug", False)
+        self.attributes = kwargs.get("attributes", [])
+        self.clicked_callback = kwargs.get("clicked_callback", None)
+
+        # Keep track of the ID of created items
+        self.created_nodes = []
+
+    def create(self, editor_id, **kwargs):
+        position = kwargs.get("position", [])
+
+        num_nodes = len(self.created_nodes)
+        new_node_label = self.label
+        if num_nodes > 0:
+            new_node_label = f"{new_node_label} {num_nodes}"
+        new_node = self.node_class(
+            parent=editor_id,
+            label=new_node_label,
+            debug=self.debug,
+            tag=kwargs.get("tag"),
+        )
+        new_node.name = self.label
+        new_node.category = self.category
+        new_node.create(
+            deepcopy(self.attributes), self.clicked_callback, position=position
+        )
+        new_node.factory_label = self.label
+
+        self.created_nodes.append(new_node.tag)
+
+        if self.debug:
+            print(self)
+
+        return new_node
+
+    def __str__(self):
+        return (
+            f"SIMURAN Node Factory with label {self.label},"
+            + f" and attributes {self.attributes}"
+        )
```

### Comparing `simuran-23.2.0/simuran.egg-info/PKG-INFO` & `simuran-23.8.0/simuran.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,118 @@
-Metadata-Version: 2.1
-Name: simuran
-Version: 23.2.0
-Summary: Simultaneous Multi-region Analysis supported with a network style
-Home-page: https://github.com/seankmartin/SIMURAN
-Download-URL: https://github.com/seankmartin/SIMURAN
-Author: Sean K. Martin
-Author-email: martins7@tcd.ie
-License: GNU GPL
-Project-URL: Bug Tracker, https://github.com/seankmartin/SIMURAN/issues
-Project-URL: Documentation, https://simuran.readthedocs.io
-Keywords: neuroscience,network,gui,api
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: neurochat
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
-# SIMURAN
-
-[![Documentation Status](https://readthedocs.org/projects/simuran/badge/?version=latest)](https://simuran.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.com/seankmartin/SIMURAN.svg?branch=master)](https://app.travis-ci.com/github/seankmartin/SIMURAN)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=seankmartin_SIMURAN&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=seankmartin_SIMURAN)
-[![codecov](https://codecov.io/gh/seankmartin/SIMURAN/branch/main/graph/badge.svg?token=F67OEU0PF2)](https://codecov.io/gh/seankmartin/SIMURAN)
-[![Maintainability](https://api.codeclimate.com/v1/badges/97aa79ac8f356de695d5/maintainability)](https://codeclimate.com/github/seankmartin/SIMURAN/maintainability)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-
-![Demo of UI](demo.gif)
-
-Simultaneous Multi-Region Analysis.
-
-## Installation
-
-```Bash
-git clone https://github.com/seankmartin/SIMURAN
-cd SIMURAN
-pip install ".[neurochat]"
-```
-
-## OS specific setup
-
-### MAC OS
-
-- To use the UI, you will need to perform at least the following. brew install libpng
-- It is possible you may also need the MAC command line developer tools, but perhaps not.
-- To use doit on MAC, you will need the developer tools.
-
-## Objective
-
-Currently, this can facilitate batch processing of many neural recordings in an easy to handle way.
-Firstly, create a table which describes all of your recordings.
-Then you can filter out specific recordings which match certain criteria.
-A recording container stores these recordings which match these criteria, and provides some bridges between common neuroscience packages to facilate loading / analysing in different formats and with different packages
-
-Here, the main object is to setup Recordings (containing all information relevant to an experiment, or part of an experiment) and RecordingContainers, which are a series of Recordings.
-
-For instance, RecordingContainer could represent all t-maze running speed, spikes, etc. and associated metadata, while a Recording is an individual t-maze session.
-This can then support easy extraction of subcontainers, such as, all trials which were successful in mice expressing a particular gene - in a simple filtering method with Pandas style.
-
-Finally, these RecordingContainers can be used to facilitate batch processing of data, and establishing workflows for processing the data.
-
-### GUI - WORK IN PROGRESS
-
-Here, the focus is mostly on the Recording level, but multiple recordings can be bundled as blocks.
-
-Recordings are loaded and processed via Nodes which are established through the UI and run in a digraph fashion.
-
-## Using custom analysis code
-
-SIMURAN can use any code that is on the Python path. The easiest way to manage this is to either:
-
-1. Fork SIMURAN and place your custom analysis code in the SIMURAN package under the directory labelled custom.
-2. Place your code on path separately, such as by creating a `setup.py` file for your code, or a `pyproject.toml` file for installation.
-3. If you place python code and/or a file with the `.pth` extension in a directory named analysis in the same directory that batch_config_path is in, this `.pth` file will be automatically processed and its contents placed on path. If this option is chosen, it is recommended to store the analysis functions directly so that anyone can run the code without modification.
-4. See [examples](https://github.com/seankmartin/neuro-tools/tree/master/SIMURAN).
-
-## Inspiration
-
-1. [GitHub - seankmartin/NeuroChaT: Analysis toolset with GUI for Neuroscience](https://github.com/seankmartin/NeuroChaT)
-2. [SpikeInterface · GitHub](https://github.com/SpikeInterface)
-3. [GitHub - seankmartin/NeuroChaT_API_Scripts: A set of python neuroscience scripts which rely on the NeuroChaT API](https://github.com/seankmartin/NeuroChaT_API_Scripts)
-4. [GitHub - mne-tools/mne-python: MNE: Magnetoencephalography (MEG) and Electroencephalography (EEG) in Python](https://github.com/mne-tools/mne-python/)
-5. [Sumatra - NeuralEnsemble](http://neuralensemble.org/sumatra/)
+Metadata-Version: 2.1
+Name: simuran
+Version: 23.8.0
+Summary: Simultaneous Multi-region Analysis supported with a network style
+Home-page: https://github.com/seankmartin/SIMURAN
+Download-URL: https://github.com/seankmartin/SIMURAN
+Author: Sean K. Martin
+Author-email: martins7@tcd.ie
+License: GNU GPL
+Project-URL: Bug Tracker, https://github.com/seankmartin/SIMURAN/issues
+Project-URL: Documentation, https://simuran.readthedocs.io
+Keywords: neuroscience,network,gui,api
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: neurochat
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
+# Simuran
+
+[![Documentation Status](https://readthedocs.org/projects/simuran/badge/?version=latest)](https://simuran.readthedocs.io/en/latest/?badge=latest)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=seankmartin_SIMURAN&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=seankmartin_SIMURAN)
+[![codecov](https://codecov.io/gh/seankmartin/SIMURAN/branch/main/graph/badge.svg?token=F67OEU0PF2)](https://codecov.io/gh/seankmartin/SIMURAN)
+[![Maintainability](https://api.codeclimate.com/v1/badges/97aa79ac8f356de695d5/maintainability)](https://codeclimate.com/github/seankmartin/SIMURAN/maintainability)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+![Demo of UI](images/demo.gif)
+
+To see more details than in the README, our [read the docs](https://simuran.readthedocs.io/en/latest/) site, or the PhD thesis of Sean K. Martin.
+
+## Installation
+
+```console
+pip install simuran
+```
+
+### MAC OS
+
+- To use the UI, you will need to perform at least the following - `brew install libpng`.
+- It is possible you may also need the MAC command line developer tools.
+
+## Usage
+
+### Objective
+
+Simuran can help facilitate batch processing of many neural recordings in an easy to handle way.
+
+The main objects to setup are Recordings (containing all information relevant to an experiment, or part of an experiment) and RecordingContainers, which are a series of Recordings.
+For instance, a RecordingContainer could represent all t-maze running speed, spikes, etc. and associated metadata, while a Recording is an individual t-maze session.
+This can then support easy extraction of subcontainers, such as, all trials which were successful in mice expressing a particular gene.
+
+### API
+
+The API is built around the Recording and RecordingContainer classes, for instance, one way to load an NWB file is as follows:
+
+```python
+import simuran
+
+recording = simuran.Recording(
+    source_file=PATH_TO_NWB, loader=simuran.loader("NWB"))
+recording.load()
+recording.inspect() # See what was loaded
+```
+
+The Recording class is designed to be as flexible as possible, and can be used to load any data, as long as a loader is provided.
+The loader is a class which takes a Recording object and loads the data into it.
+Other modules include the analysis module, which allows multi-processing of analysis functions, and the base module, which contains the base classes for the API.
+The plot module contains plotting functions for general use, and also some simple figure handling (auto garbage collection, etc.).
+Finally, the bridge module contains Bridge class definitions, which are used to allow interoperability between different software tools and data formats in neuroscience.
+
+### GUI - Visual node based editor
+
+Here, the focus is mostly on the Recording level, but multiple recordings can be bundled as blocks.
+
+Recordings are loaded and processed via Nodes which are established through the UI and run in a digraph fashion.
+The UI is built using dearpygui, and supports a subset of the API via nodes, which can be expanded upon.
+
+![Demo of UI still](images/Demo2.PNG)
+
+### Examples
+
+Some examples are provided in the examples folder.
+
+## Contributing
+
+Contributions are welcome, and any issues can be raised on the github page. Please feel free to reach out to me if you have any questions.
+
+## License
+
+Simuran is distributed under the GPL-3.0 License.
+
+## Inspiration
+
+1. [NeuroChaT: Analysis toolset with GUI for Neuroscience](https://github.com/seankmartin/NeuroChaT)
+2. [SpikeInterface · GitHub](https://github.com/SpikeInterface)
+3. [A set of python neuroscience scripts which rely on the NeuroChaT API](https://github.com/seankmartin/NeuroChaT_API_Scripts)
+4. [MNE: Magnetoencephalography (MEG) and Electroencephalography (EEG) in Python](https://github.com/mne-tools/mne-python/)
+5. [Sumatra - NeuralEnsemble](http://neuralensemble.org/sumatra/)
+6. [Snakemake](https://snakemake.readthedocs.io/en/stable/)
+
+## Update coverage
+
+```console
+pytest .
+codecov -t ba31944a-6070-401e-a731-1bd2f92a5e55
+```
```

### Comparing `simuran-23.2.0/tests/test_base_class.py` & `simuran-23.8.0/tests/test_base_class.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-"""Test BaseSimuran"""
-
-import pytest
-from simuran.core.base_class import BaseSimuran, NoLoader
-from simuran.loaders.base_loader import MetadataLoader
-
-
-class BaseClassToTest(BaseSimuran):
-    """Needed as Base is ABC"""
-
-    def load(self):
-        super().load()
-        self.loader.load_recording(self)
-
-
-def create_test_obj(meta_dict):
-    loader = MetadataLoader()
-    return BaseClassToTest(attrs=meta_dict, loader=loader)
-
-
-def test_raises_loading_exception():
-    base_obj = BaseClassToTest()
-    with pytest.raises(ValueError):
-        base_obj.load()
-
-
-def test_parameter_load():
-    meta_dict = dict((["a", 1], [55, "test_str"]))
-    new_dict = dict((["test / test", 551], ["test_again", [1, 1, "b"]]))
-    base_obj = create_test_obj(meta_dict)
-    assert not base_obj.is_loaded()
-
-    # Loading first time
-    base_obj.load()
-    assert meta_dict == base_obj.attrs
-
-    # Faking this for now, can test properly with a real source file
-    base_obj.last_loaded_source = "meta_dict"
-    base_obj.source_file = "meta_dict"
-    assert base_obj.is_loaded()
-
-    # And a new loading
-    base_obj.source_file = "new_dict"
-    assert not base_obj.is_loaded()
-    base_obj.attrs = new_dict
-
-    base_obj.load()
-    assert new_dict == base_obj.attrs
-
-
-def test_inpsect():
-    d = {"test": "banana"}
-    obj = create_test_obj(d)
-    attrs = obj.get_attrs()
-    assert "attrs" in attrs
-    attrs_and_methods = obj.get_attrs_and_methods()
-    assert "get_attrs_and_methods" in attrs_and_methods
-
-
-def test_no_loader():
-    no_loader = NoLoader()
-    no_loader.load()
-    assert no_loader.is_loaded()
+"""Test BaseSimuran"""
+
+import pytest
+from simuran.core.base_class import BaseSimuran, NoLoader
+from simuran.loaders.base_loader import MetadataLoader
+
+
+class BaseClassToTest(BaseSimuran):
+    """Needed as Base is ABC"""
+
+    def load(self):
+        super().load()
+        self.loader.load_recording(self)
+
+
+def create_test_obj(meta_dict):
+    loader = MetadataLoader()
+    return BaseClassToTest(attrs=meta_dict, loader=loader)
+
+
+def test_raises_loading_exception():
+    base_obj = BaseClassToTest()
+    with pytest.raises(ValueError):
+        base_obj.load()
+
+
+def test_parameter_load():
+    meta_dict = dict((["a", 1], [55, "test_str"]))
+    new_dict = dict((["test / test", 551], ["test_again", [1, 1, "b"]]))
+    base_obj = create_test_obj(meta_dict)
+    assert not base_obj.is_loaded()
+
+    # Loading first time
+    base_obj.load()
+    assert meta_dict == base_obj.attrs
+
+    # Faking this for now, can test properly with a real source file
+    base_obj.last_loaded_source = "meta_dict"
+    base_obj.source_file = "meta_dict"
+    assert base_obj.is_loaded()
+
+    # And a new loading
+    base_obj.source_file = "new_dict"
+    assert not base_obj.is_loaded()
+    base_obj.attrs = new_dict
+
+    base_obj.load()
+    assert new_dict == base_obj.attrs
+
+
+def test_inpsect():
+    d = {"test": "banana"}
+    obj = create_test_obj(d)
+    attrs = obj.get_attrs()
+    assert "attrs" in attrs
+    attrs_and_methods = obj.get_attrs_and_methods()
+    assert "get_attrs_and_methods" in attrs_and_methods
+
+
+def test_no_loader():
+    no_loader = NoLoader()
+    no_loader.load()
+    assert no_loader.is_loaded()
```

### Comparing `simuran-23.2.0/tests/test_base_container.py` & `simuran-23.8.0/tests/test_base_container.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import pytest
-
-from simuran.core.base_class import BaseSimuran
-from simuran.core.base_container import GenericContainer
-
-
-class FakeLoader(BaseSimuran):
-    def load(self):
-        self.data = self.attrs.get("fake", "default")
-
-    def is_loaded(self):
-        return self.data is not None
-
-
-@pytest.mark.parametrize(
-    "num_items, values",
-    [
-        (3, ("apple", "banana", "apple")),
-        (5, (1, "orange", 30, (2, 3), "hi")),
-    ],
-)
-class TestContainerSetup:
-    @pytest.fixture
-    def container(self, values):
-        container_ = GenericContainer()
-        for val in values:
-            new = FakeLoader(dict(fake=val))
-            container_.append(new)
-        container_.load()
-        return container_
-
-    def test_container_create(self, num_items, values, container):
-        assert len(container) == num_items
-
-    def test_container_load(self, num_items, values, container):
-        assert all(c.is_loaded() for c in container)
-
-    def test_container_single_load(self, num_items, values, container):
-        container.append(FakeLoader())
-        item = container.load(num_items)
-        assert item.is_loaded()
-
-    def test_container_group(self, num_items, values, container):
-        test_val = values[0]
-        _, indices = container.group_by_property("data", test_val)
-        group_split = container.split_into_groups("data")
-        matches = [i for i in range(num_items) if values[i] == test_val]
-        assert indices == matches
-        assert group_split[test_val][1] == matches
-
-    def test_container_values(self, num_items, values, container):
-        data = container.get_property("data")
-        assert data == list(values)
-
-        data = container.get_possible_values("data")
-        assert data == set(values)
-
-    def test_container_extend(self, num_items, values, container):
-        container.extend([1, 2, 3])
-        assert len(container) == num_items + 3
-        assert container[-1] == 3
-
-        container[1] = 2
-        assert container[1] == 2
+import pytest
+
+from simuran.core.base_class import BaseSimuran
+from simuran.core.base_container import GenericContainer
+
+
+class FakeLoader(BaseSimuran):
+    def load(self):
+        self.data = self.attrs.get("fake", "default")
+
+    def is_loaded(self):
+        return self.data is not None
+
+
+@pytest.mark.parametrize(
+    "num_items, values",
+    [
+        (3, ("apple", "banana", "apple")),
+        (5, (1, "orange", 30, (2, 3), "hi")),
+    ],
+)
+class TestContainerSetup:
+    @pytest.fixture
+    def container(self, values):
+        container_ = GenericContainer()
+        for val in values:
+            new = FakeLoader(dict(fake=val))
+            container_.append(new)
+        container_.load()
+        return container_
+
+    def test_container_create(self, num_items, values, container):
+        assert len(container) == num_items
+
+    def test_container_load(self, num_items, values, container):
+        assert all(c.is_loaded() for c in container)
+
+    def test_container_single_load(self, num_items, values, container):
+        container.append(FakeLoader())
+        item = container.load(num_items)
+        assert item.is_loaded()
+
+    def test_container_group(self, num_items, values, container):
+        test_val = values[0]
+        _, indices = container.group_by_property("data", test_val)
+        group_split = container.split_into_groups("data")
+        matches = [i for i in range(num_items) if values[i] == test_val]
+        assert indices == matches
+        assert group_split[test_val][1] == matches
+
+    def test_container_values(self, num_items, values, container):
+        data = container.get_property("data")
+        assert data == list(values)
+
+        data = container.get_possible_values("data")
+        assert data == set(values)
+
+    def test_container_extend(self, num_items, values, container):
+        container.extend([1, 2, 3])
+        assert len(container) == num_items + 3
+        assert container[-1] == 3
+
+        container[1] = 2
+        assert container[1] == 2
```

### Comparing `simuran-23.2.0/tests/test_neurochat.py` & `simuran-23.8.0/tests/test_neurochat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import os
-import urllib
-
-import numpy as np
-from neurochat.nc_lfp import NLfp
-from neurochat.nc_spatial import NSpatial
-from neurochat.nc_spike import NSpike
-from simuran.core.param_handler import ParamHandler
-from simuran.loaders.neurochat_loader import NCLoader
-from simuran.recording import Recording
-
-main_dir = os.path.dirname(__file__)[:-len(f"{os.sep}tests")]
-
-
-def fetch_axona_data():
-    base_url = (
-        "https://gin.g-node.org/seankmartin/SIMURAN_Test_Data/raw/master/AxonaData/"
-    )
-    filenames = [
-        "010416b-LS3-50Hz10.V5.ms.2",
-        "010416b-LS3-50Hz10.V5.ms.eeg",
-        "010416b-LS3-50Hz10.V5.ms_2.cut",
-        "010416b-LS3-50Hz10.V5.ms_2.txt",
-        "010416b-LS3-50Hz10.V5.ms.set",
-    ]
-    full_filenames = [
-        os.path.join(main_dir, "tests", "resources", "temp", "axona", f)
-        for f in filenames
-    ]
-    full_urls = [base_url + f for f in filenames]
-
-    for i in range(len(filenames)):
-        if not os.path.isfile(full_filenames[i]):
-            urllib.request.urlretrieve(full_urls[i], full_filenames[i])
-
-    return full_filenames
-
-
-def test_nc_recording_loading(delete=False):
-    main_test_dir = os.path.join(main_dir, "tests", "resources", "temp", "axona")
-    os.makedirs(main_test_dir, exist_ok=True)
-
-    axona_files = fetch_axona_data()
-
-    # Load using SIMURAN auto detection.
-    metadata = ParamHandler(
-        source_file=os.path.join(
-            main_dir, "tests", "resources", "params", "axona_test.py"
-        ),
-        name="mapping",
-    )
-    metadata["source_file"] = axona_files[-1]
-
-    loader = NCLoader(system="Axona", pos_extension=".txt")
-    ex = Recording(attrs=metadata, loader=loader)
-    ex.parse_metadata()
-
-    ex.load()
-
-    ex.data["units"][0].data.set_unit_no(1)
-    # Load using NeuroChaT
-    lfp = NLfp()
-    lfp.set_filename(os.path.join(main_test_dir, "010416b-LS3-50Hz10.V5.ms.eeg"))
-    lfp.load(system="Axona")
-
-    unit = NSpike()
-    unit.set_filename(os.path.join(main_test_dir, "010416b-LS3-50Hz10.V5.ms.2"))
-    unit.load(system="Axona")
-    unit.set_unit_no(1)
-
-    spatial = NSpatial()
-    spatial.set_filename(os.path.join(main_test_dir, "010416b-LS3-50Hz10.V5.ms_2.txt"))
-    spatial.load(system="Axona")
-
-    assert np.all(ex.data["signals"][0].data.get_samples() == lfp.get_samples())
-    assert np.all(ex.data["units"][0].data.get_unit_stamp() == unit.get_unit_stamp())
-    assert np.all(ex.data["units"][0].data.get_unit_tags() == unit.get_unit_tags())
-    assert np.all(ex.data["spatial"].data.get_pos_x() == spatial.get_pos_x())
-
-    ncl = NCLoader()
-    ncl.system = "Axona"
-    loc = os.path.join(main_dir, "tests", "resources", "temp", "axona")
-    file_locs, _ = ncl.auto_fname_extraction(
-        loc,
-        verbose=False,
-        unit_groups=[
-            2,
-        ],
-        sig_channels=[
-            1,
-        ],
-    )
-    clust_locs = [os.path.basename(f) for f in file_locs["Cluster"] if f is not None]
-    assert "010416b-LS3-50Hz10.V5.ms_2.cut" in clust_locs
-
-    if delete:
-        for f in axona_files:
-            os.remove(f)
-
-
-if __name__ == "__main__":
-    test_nc_recording_loading(delete=False)
+import os
+import urllib
+
+import numpy as np
+from neurochat.nc_lfp import NLfp
+from neurochat.nc_spatial import NSpatial
+from neurochat.nc_spike import NSpike
+from simuran.core.param_handler import ParamHandler
+from simuran.loaders.neurochat_loader import NeurochatLoader
+from simuran.recording import Recording
+
+main_dir = os.path.dirname(__file__)[: -len(f"{os.sep}tests")]
+
+
+def fetch_axona_data():
+    base_url = (
+        "https://gin.g-node.org/seankmartin/SIMURAN_Test_Data/raw/master/AxonaData/"
+    )
+    filenames = [
+        "010416b-LS3-50Hz10.V5.ms.2",
+        "010416b-LS3-50Hz10.V5.ms.eeg",
+        "010416b-LS3-50Hz10.V5.ms_2.cut",
+        "010416b-LS3-50Hz10.V5.ms_2.txt",
+        "010416b-LS3-50Hz10.V5.ms.set",
+    ]
+    full_filenames = [
+        os.path.join(main_dir, "tests", "resources", "temp", "axona", f)
+        for f in filenames
+    ]
+    full_urls = [base_url + f for f in filenames]
+
+    for i in range(len(filenames)):
+        if not os.path.isfile(full_filenames[i]):
+            urllib.request.urlretrieve(full_urls[i], full_filenames[i])
+
+    return full_filenames
+
+
+def test_nc_recording_loading(delete=False):
+    main_test_dir = os.path.join(main_dir, "tests", "resources", "temp", "axona")
+    os.makedirs(main_test_dir, exist_ok=True)
+
+    axona_files = fetch_axona_data()
+
+    # Load using SIMURAN auto detection.
+    metadata = ParamHandler(
+        source_file=os.path.join(
+            main_dir, "tests", "resources", "params", "axona_test.py"
+        ),
+        name="mapping",
+    )
+    metadata["source_file"] = axona_files[-1]
+
+    loader = NeurochatLoader(system="Axona", pos_extension=".txt")
+    ex = Recording(attrs=metadata, loader=loader)
+    ex.parse_metadata()
+
+    ex.load()
+
+    ex.data["units"][0].data.set_unit_no(1)
+    # Load using NeuroChaT
+    lfp = NLfp()
+    lfp.set_filename(os.path.join(main_test_dir, "010416b-LS3-50Hz10.V5.ms.eeg"))
+    lfp.load(system="Axona")
+
+    unit = NSpike()
+    unit.set_filename(os.path.join(main_test_dir, "010416b-LS3-50Hz10.V5.ms.2"))
+    unit.load(system="Axona")
+    unit.set_unit_no(1)
+
+    spatial = NSpatial()
+    spatial.set_filename(os.path.join(main_test_dir, "010416b-LS3-50Hz10.V5.ms_2.txt"))
+    spatial.load(system="Axona")
+
+    assert np.all(ex.data["signals"][0].data.get_samples() == lfp.get_samples())
+    assert np.all(ex.data["units"][0].data.get_unit_stamp() == unit.get_unit_stamp())
+    assert np.all(ex.data["units"][0].data.get_unit_tags() == unit.get_unit_tags())
+    assert np.all(ex.data["spatial"].data.get_pos_x() == spatial.get_pos_x())
+
+    ncl = NeurochatLoader()
+    ncl.system = "Axona"
+    loc = os.path.join(main_dir, "tests", "resources", "temp", "axona")
+    file_locs, _ = ncl.auto_fname_extraction(
+        loc,
+        verbose=False,
+        unit_groups=[
+            2,
+        ],
+        sig_channels=[
+            1,
+        ],
+    )
+    clust_locs = [os.path.basename(f) for f in file_locs["Cluster"] if f is not None]
+    assert "010416b-LS3-50Hz10.V5.ms_2.cut" in clust_locs
+
+    if delete:
+        for f in axona_files:
+            os.remove(f)
+
+
+if __name__ == "__main__":
+    test_nc_recording_loading(delete=False)
```

### Comparing `simuran-23.2.0/tests/test_parameters.py` & `simuran-23.8.0/tests/test_parameters.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
-
-import pytest
-from simuran.core.param_handler import ParamHandler
-from simuran import config_from_file
-
-
-@pytest.mark.parametrize("file_type", [(".yaml"), (".json"), (".py")])
-def test_read_write(file_type):
-    params = {"hello_world": "banana", 0: [1, 10, 14.1], "chans": {"1": "b"}}
-    ph_write = ParamHandler(attrs=params)
-    ph_write.write(f"test_simuran_temp{file_type}")
-    ph_read = config_from_file(f"test_simuran_temp{file_type}")
-    assert ph_read.attrs["hello_world"] == "banana"
-    if file_type == ".yaml":
-        assert ph_read[0] == [1, 10, 14.1]
-    else:
-        assert ph_read["0"] == [1, 10, 14.1]
-    assert ph_read["chans"]["1"] == "b"
-    os.remove(f"test_simuran_temp{file_type}")
-
-
-def test_dict_passes():
-    ph = ParamHandler()
-    ph.setdefault("a", "val")
-    assert ph.get("a") == "val"
-    assert ph.get("b", "hi") == "hi"
-    assert len(ph.values()) == 1
-    assert len(ph.keys()) == 1
-    ph.pop("a")
-    assert len(ph.items()) == 0
-    ph["1"] = 100
-    assert "1" in ph
-    assert ph.setdefault("1") == 100
-    ph.clear()
-    assert len(ph) == 0
+import os
+
+import pytest
+from simuran.core.param_handler import ParamHandler
+from simuran import config_from_file
+
+
+@pytest.mark.parametrize("file_type", [(".yaml"), (".json"), (".py")])
+def test_read_write(file_type):
+    params = {"hello_world": "banana", 0: [1, 10, 14.1], "chans": {"1": "b"}}
+    ph_write = ParamHandler(attrs=params)
+    ph_write.write(f"test_simuran_temp{file_type}")
+    ph_read = config_from_file(f"test_simuran_temp{file_type}")
+    assert ph_read.attrs["hello_world"] == "banana"
+    if file_type == ".yaml":
+        assert ph_read[0] == [1, 10, 14.1]
+    else:
+        assert ph_read["0"] == [1, 10, 14.1]
+    assert ph_read["chans"]["1"] == "b"
+    os.remove(f"test_simuran_temp{file_type}")
+
+
+def test_dict_passes():
+    ph = ParamHandler()
+    ph.setdefault("a", "val")
+    assert ph.get("a") == "val"
+    assert ph.get("b", "hi") == "hi"
+    assert len(ph.values()) == 1
+    assert len(ph.keys()) == 1
+    ph.pop("a")
+    assert len(ph.items()) == 0
+    ph["1"] = 100
+    assert "1" in ph
+    assert ph.setdefault("1") == 100
+    ph.clear()
+    assert len(ph) == 0
```

### Comparing `simuran-23.2.0/tests/test_recording.py` & `simuran-23.8.0/tests/test_recording.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import os
-
-from simuran.core.param_handler import ParamHandler
-from simuran.loaders.base_loader import MetadataLoader
-from simuran.recording import Recording
-
-main_dir = os.path.dirname(__file__)[: -len(f"{os.sep}tests")]
-
-
-def test_recording_setup():
-    metadata = ParamHandler(
-        source_file=os.path.join(
-            main_dir, "tests", "resources", "params", "simuran_base_params.py"
-        ),
-        name="mapping",
-    )
-
-    loader = MetadataLoader()
-    ex = Recording(attrs=metadata, loader=loader)
-    loader.parse_metadata(ex)
-    assert ex.attrs["signals"]["region"][0] == "ACC"
-    assert set(ex.available_data) == {
-        "signals",
-        "units",
-        "spatial",
-        "loader",
-        "loader_kwargs",
-    }
-
-
-def test_recording_save_name():
-    source_file = "fake_dir/fake_dir2/fake_name.txt"
-    r = Recording(source_file=source_file)
-
-    name = r.get_name_for_save()
-    assert name == "fake_dir--fake_dir2--fake_name"
-
-    name2 = r.get_name_for_save(rel_dir="fake_dir")
-    assert name2 == "fake_dir2--fake_name"
+import os
+
+from simuran.core.param_handler import ParamHandler
+from simuran.loaders.base_loader import MetadataLoader
+from simuran.recording import Recording
+
+main_dir = os.path.dirname(__file__)[: -len(f"{os.sep}tests")]
+
+
+def test_recording_setup():
+    metadata = ParamHandler(
+        source_file=os.path.join(
+            main_dir, "tests", "resources", "params", "simuran_base_params.py"
+        ),
+        name="mapping",
+    )
+
+    loader = MetadataLoader()
+    ex = Recording(attrs=metadata, loader=loader)
+    loader.parse_metadata(ex)
+    assert ex.attrs["signals"]["region"][0] == "ACC"
+    assert set(ex.available_data) == {
+        "signals",
+        "units",
+        "spatial",
+        "loader",
+        "loader_kwargs",
+    }
+
+
+def test_recording_save_name():
+    source_file = "fake_dir/fake_dir2/fake_name.txt"
+    r = Recording(source_file=source_file)
+
+    name = r.get_name_for_save()
+    assert name == "fake_dir--fake_dir2--fake_name"
+
+    name2 = r.get_name_for_save(rel_dir="fake_dir")
+    assert name2 == "fake_dir2--fake_name"
```

### Comparing `simuran-23.2.0/tests/test_recording_container.py` & `simuran-23.8.0/tests/test_recording_container.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import os
-import pickle
-import pytest
-from simuran.recording_container import RecordingContainer
-from simuran.loaders.base_loader import MetadataLoader
-import pandas as pd
-
-
-class FakeLoader1(MetadataLoader):
-    def load_recording(self, recording):
-        recording.data = "FAKE1"
-
-
-class FakeLoader2(MetadataLoader):
-    def load_recording(self, recording):
-        recording.data = "FAKE2"
-
-
-class TestRecordingContainer(object):
-    @pytest.fixture
-    def rc(self):
-        data = {"r_1": ["t1", 55, 0], "r_2": ["t2", 10, 1]}
-        columns = ["Name", "Peak", "Passed"]
-        table = pd.DataFrame.from_dict(data, orient="index", columns=columns)
-        loaders = [FakeLoader1(), FakeLoader2()]
-
-        return RecordingContainer.from_table(table, loaders)
-
-    def test_recording_container_from_table(self, rc):
-        assert len(rc) == 2
-        assert rc[0].attrs["_index"] == "r_1"
-
-    def test_multiple_loaders(self, rc):
-        assert rc[0].data is None
-        rc.load(0)
-        assert rc.last_loaded.data == "FAKE1"
-        rc.load(1)
-        assert rc.last_loaded.data == "FAKE2"
-
-    def test_bulk_load(self, rc):
-        rc.load_on_fly = False
-        for r in rc:
-            assert not r.is_loaded()
-
-        rc.load()
-        for r in rc:
-            assert r.is_loaded()
-
-        assert [r.data for r in rc] == ["FAKE1", "FAKE2"]
-
-        for r in rc:
-            r.source_file = "BLAH"
-
-        for r in rc:
-            assert not r.is_loaded()
-
-    def test_results(self, rc):
-        results = rc.get_results()
-        assert len(results) == 2
-
-    def test_source_finder(self, rc):
-        rc[0].source_file = "hi"
-        rc[1].source_file = "bye"
-
-        assert rc.find_recording_with_source("hi") == 0
-        assert rc.find_recording_with_source("bye") == 1
-        assert len(rc.find_recording_with_source("hih")) == 0
-
-        rc[1].source_file = "hi"
-        assert rc.find_recording_with_source("hi") == [0, 1]
-
-    def test_load_iter(self, rc):
-        for r in rc.load_iter():
-            assert r.is_loaded()
-
-    def test_rc_dump(self, rc):
-        rc.load_on_fly = False
-        rc.load()
-        rc.dump("test.pkl", results_only=False)
-        with open("test.pkl", "rb") as f:
-            res = pickle.load(f)
-        assert res[0].data == "FAKE1"
-
-        os.remove("test.pkl")
-
-    def test_rc_results_save(self, rc):
-        rc[0].results = {"H": 1, "B": 2}
-        rc[1].results = {"H": 2, "B": 3}
-
-        df = rc.save_results_to_table()
-        assert (df.columns == ["H", "B"]).all()
-        assert df.iloc[0]["H"] == 1
+import os
+import pickle
+import pytest
+from simuran.recording_container import RecordingContainer
+from simuran.loaders.base_loader import MetadataLoader
+import pandas as pd
+
+
+class FakeLoader1(MetadataLoader):
+    def load_recording(self, recording):
+        recording.data = "FAKE1"
+
+
+class FakeLoader2(MetadataLoader):
+    def load_recording(self, recording):
+        recording.data = "FAKE2"
+
+
+class TestRecordingContainer(object):
+    @pytest.fixture
+    def rc(self):
+        data = {"r_1": ["t1", 55, 0], "r_2": ["t2", 10, 1]}
+        columns = ["Name", "Peak", "Passed"]
+        table = pd.DataFrame.from_dict(data, orient="index", columns=columns)
+        loaders = [FakeLoader1(), FakeLoader2()]
+
+        return RecordingContainer.from_table(table, loaders)
+
+    def test_recording_container_from_table(self, rc):
+        assert len(rc) == 2
+        assert rc[0].attrs["_index"] == "r_1"
+
+    def test_multiple_loaders(self, rc):
+        assert rc[0].data is None
+        rc.load(0)
+        assert rc.last_loaded.data == "FAKE1"
+        rc.load(1)
+        assert rc.last_loaded.data == "FAKE2"
+
+    def test_bulk_load(self, rc):
+        rc.load_on_fly = False
+        for r in rc:
+            assert not r.is_loaded()
+
+        rc.load()
+        for r in rc:
+            assert r.is_loaded()
+
+        assert [r.data for r in rc] == ["FAKE1", "FAKE2"]
+
+        for r in rc:
+            r.source_file = "BLAH"
+
+        for r in rc:
+            assert not r.is_loaded()
+
+    def test_results(self, rc):
+        results = rc.get_results()
+        assert len(results) == 2
+
+    def test_source_finder(self, rc):
+        rc[0].source_file = "hi"
+        rc[1].source_file = "bye"
+
+        assert rc.find_recording_with_source("hi") == 0
+        assert rc.find_recording_with_source("bye") == 1
+        assert len(rc.find_recording_with_source("hih")) == 0
+
+        rc[1].source_file = "hi"
+        assert rc.find_recording_with_source("hi") == [0, 1]
+
+    def test_load_iter(self, rc):
+        for r in rc.load_iter():
+            assert r.is_loaded()
+
+    def test_rc_dump(self, rc):
+        rc.load_on_fly = False
+        rc.load()
+        rc.dump("test.pkl", results_only=False)
+        with open("test.pkl", "rb") as f:
+            res = pickle.load(f)
+        assert res[0].data == "FAKE1"
+
+        os.remove("test.pkl")
+
+    def test_rc_results_save(self, rc):
+        rc[0].results = {"H": 1, "B": 2}
+        rc[1].results = {"H": 2, "B": 3}
+
+        df = rc.save_results_to_table()
+        assert (df.columns == ["H", "B"]).all()
+        assert df.iloc[0]["H"] == 1
```

### Comparing `simuran-23.2.0/tests/test_signals.py` & `simuran-23.8.0/tests/test_signals.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,98 @@
-import pytest
-import numpy as np
-
-import mne
-from simuran.core.base_signal import BaseSignal, Eeg
-from simuran.bridges.neurochat_bridge import signal_to_neurochat
-from simuran.bridges.mne_bridge import convert_signals_to_mne, plot_signals
-from simuran.loaders.base_loader import MetadataLoader
-
-from copy import copy
-
-
-class FakeLoader(MetadataLoader):
-    def load_signal(self, source_file):
-        signal = Eeg()
-        signal.fake_data = source_file
-        return signal
-
-
-@pytest.mark.parametrize("array_size, sampling_rate", [(10000, 20)])
-class TestBaseSignal:
-    @pytest.fixture
-    def signal(self, array_size, sampling_rate):
-        np_arr = np.random.random(size=array_size)
-        signal = BaseSignal.from_numpy(np_arr, sampling_rate)
-        signal.samples = list(np_arr)
-        signal.channel = "1"
-        signal.region = "NA"
-        return signal
-
-    def test_from_numpy(self, array_size, sampling_rate, signal):
-        t2 = np.arange(0, array_size / sampling_rate, 1.0 / sampling_rate)
-        assert np.all(np.isclose(signal.timestamps, t2))
-
-    def test_naming(self, signal):
-        assert signal.default_name() == "NA - misc 1"
-
-    def test_to_nc(self, array_size, sampling_rate, signal):
-        lfp = signal_to_neurochat(signal)
-        t2 = np.arange(0, array_size / sampling_rate, 1.0 / sampling_rate)
-        assert lfp.get_channel_id() == "1"
-        assert np.all(np.isclose(lfp._timestamp, t2))
-        assert np.all(np.isclose(signal.samples, lfp.get_samples()))
-        signal.data = lfp
-        lfp2 = signal_to_neurochat(signal)
-        assert np.all(np.isclose(lfp2.get_samples(), lfp.get_samples()))
-
-    def test_range(self, signal, sampling_rate):
-        r_bit = signal.in_range(1, 2)
-        assert np.all(signal.samples[1 * sampling_rate : 2 * sampling_rate] == r_bit)
-        r_bit = signal.in_range(1, 8, 2)
-        assert np.all(
-            signal.samples[1 * sampling_rate : 8 * sampling_rate : 2 * sampling_rate]
-            == r_bit
-        )
-
-    def test_filter(self, signal, sampling_rate):
-        filtered_data = signal.filter(1, 5, inplace=False)
-        filter_by_mne = mne.filter.filter_data(signal.samples, sampling_rate, 1, 5)
-        assert np.all(np.isclose(filtered_data.samples, filter_by_mne))
-        assert np.any(~np.isclose(filtered_data.samples, signal.samples))
-        filtered_data = signal.filter(1, 5, inplace=True)
-        assert np.all(np.isclose(signal.samples, filter_by_mne))
-        assert np.all(signal.filter(None, None).samples == signal.samples)
-
-    def test_start_end(self, signal, array_size, sampling_rate):
-        assert signal.get_start() == 0
-        assert np.isclose(signal.get_end(), (array_size - 1) / sampling_rate)
-        assert signal.get_duration() == signal.get_end()
-
-    def test_convert_to_mne(self, signal):
-        signals = [copy(signal) for _ in range(10)]
-        for i in range(len(signals)):
-            signals[i].channel = i
-        bad_chans = [0]
-        mne_signals = convert_signals_to_mne(
-            signals, ch_names=None, verbose=False, bad_chans=bad_chans
-        )
-        assert np.all(
-            np.isclose(mne_signals.get_data()[0], signal.get_samples_in_volts())
-        )
-
-    def test_plot(self, signal):
-        signals = [copy(signal) for _ in range(10)]
-        for signal_ in signals:
-            signal_.channel_type = "eeg"
-        fig = plot_signals(signals, show=False)
-        assert fig != None
-
-    def test_loading(self, signal):
-        sigcal = BaseSignal()
-        sigcal.loader = FakeLoader()
-        sigcal.source_file = "text.txt"
-        sigcal.load()
-        assert sigcal.fake_data == "text.txt"
-        assert sigcal.is_loaded()
-        assert sigcal.channel_type == "eeg"
+import pytest
+import numpy as np
+
+import mne
+from simuran.core.base_signal import BaseSignal, Eeg
+from simuran.bridges.neurochat_bridge import signal_to_neurochat
+from simuran.bridges.mne_bridge import convert_signals_to_mne
+from simuran.plot.signal import plot_signals
+from simuran.loaders.base_loader import MetadataLoader
+
+from copy import copy
+
+
+class FakeLoader(MetadataLoader):
+    def load_signal(self, source_file):
+        signal = Eeg()
+        signal.fake_data = source_file
+        return signal
+
+
+@pytest.mark.parametrize("array_size, sampling_rate", [(10000, 20)])
+class TestBaseSignal:
+    @pytest.fixture
+    def signal(self, array_size, sampling_rate):
+        np_arr = np.random.random(size=array_size)
+        signal = BaseSignal.from_numpy(np_arr, sampling_rate)
+        signal.samples = list(np_arr)
+        signal.channel = "1"
+        signal.region = "NA"
+        return signal
+
+    def test_from_numpy(self, array_size, sampling_rate, signal):
+        t2 = np.arange(0, array_size / sampling_rate, 1.0 / sampling_rate)
+        assert np.all(np.isclose(signal.timestamps, t2))
+
+    def test_naming(self, signal):
+        assert signal.default_name() == "NA - misc 1"
+
+    def test_to_nc(self, array_size, sampling_rate, signal):
+        lfp = signal_to_neurochat(signal)
+        t2 = np.arange(0, array_size / sampling_rate, 1.0 / sampling_rate)
+        assert lfp.get_channel_id() == "1"
+        assert np.all(np.isclose(lfp._timestamp, t2))
+        assert np.all(np.isclose(signal.samples, lfp.get_samples()))
+        signal.data = lfp
+        lfp2 = signal_to_neurochat(signal)
+        assert np.all(np.isclose(lfp2.get_samples(), lfp.get_samples()))
+
+    def test_range(self, signal, sampling_rate):
+        r_bit = signal.in_range(1, 2)
+        assert np.all(signal.samples[1 * sampling_rate : 2 * sampling_rate] == r_bit)
+        r_bit = signal.in_range(1, 8, 2)
+        assert np.all(
+            signal.samples[1 * sampling_rate : 8 * sampling_rate : 2 * sampling_rate]
+            == r_bit
+        )
+
+    def test_filter(self, signal, sampling_rate):
+        filtered_data = signal.filter(1, 5, inplace=False)
+        filter_by_mne = mne.filter.filter_data(signal.samples, sampling_rate, 1, 5)
+        assert np.all(np.isclose(filtered_data.samples, filter_by_mne))
+        assert np.any(~np.isclose(filtered_data.samples, signal.samples))
+        filtered_data = signal.filter(1, 5, inplace=True)
+        assert np.all(np.isclose(signal.samples, filter_by_mne))
+        assert np.all(signal.filter(None, None).samples == signal.samples)
+
+    def test_start_end(self, signal, array_size, sampling_rate):
+        assert signal.get_start() == 0
+        assert np.isclose(signal.get_end(), (array_size - 1) / sampling_rate)
+        assert signal.get_duration() == signal.get_end()
+
+    def test_convert_to_mne(self, signal):
+        signals = [copy(signal) for _ in range(10)]
+        for i in range(len(signals)):
+            signals[i].channel = i
+        bad_chans = [0]
+        mne_signals = convert_signals_to_mne(
+            signals, ch_names=None, verbose=False, bad_chans=bad_chans
+        )
+        assert np.all(
+            np.isclose(mne_signals.get_data()[0], signal.get_samples_in_volts())
+        )
+
+    def test_plot(self, signal):
+        signals = [copy(signal) for _ in range(10)]
+        for signal_ in signals:
+            signal_.channel_type = "eeg"
+        fig = plot_signals(signals, show=False)
+        assert fig != None
+
+    def test_loading(self, signal):
+        sigcal = BaseSignal()
+        sigcal.loader = FakeLoader()
+        sigcal.source_file = "text.txt"
+        sigcal.load()
+        assert sigcal.fake_data == "text.txt"
+        assert sigcal.is_loaded()
+        assert sigcal.channel_type == "eeg"
```

