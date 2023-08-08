# Comparing `tmp/grav-toolbox-0.2.2.tar.gz` & `tmp/grav-toolbox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grav-toolbox-0.2.2.tar", last modified: Wed Jul 12 11:09:05 2023, max compression
+gzip compressed data, was "grav-toolbox-0.2.3.tar", last modified: Tue Aug  8 14:01:28 2023, max compression
```

## Comparing `grav-toolbox-0.2.2.tar` & `grav-toolbox-0.2.3.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.2.2/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.119650 grav-toolbox-0.2.2/bev_legacy/
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/__init__.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/adjust.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/adjust_reilly1970.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/command_line.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/const.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/drift_mlr.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/init.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/output.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/plots.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/schwaus.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.2.2/bev_legacy/settings.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/bev_legacy/utils.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.123649 grav-toolbox-0.2.2/grav_toolbox.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     7522 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2418 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       59 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-07-12 11:09:05.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.2.2/grav_toolbox.egg-info/zip-safe
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.123649 grav-toolbox-0.2.2/gravtools/
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.123649 grav-toolbox-0.2.2/gravtools/CG5_utils/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/CG5_utils/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32664 2023-06-27 12:10:33.000000 grav-toolbox-0.2.2/gravtools/CG5_utils/cg5_survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/const.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.131649 grav-toolbox-0.2.2/gravtools/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    65336 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_autoselection_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    11546 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_estimation_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_export_results.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_gis_export_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_load_stations.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_new_campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_options.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/dialog_setup_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15540 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/gui/dlg_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1784 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/gui/dlg_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/gui/dlg_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   199887 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_observation_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_correlation_matrix_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_drift_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_obs_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     7493 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_stat_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_results_vg_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_setup_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_station_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.2.2/gravtools/gui/gui_model_survey_table.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.135650 grav-toolbox-0.2.2/gravtools/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    49871 2023-06-27 12:10:33.000000 grav-toolbox-0.2.2/gravtools/models/campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/models/exceptions.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    38608 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/lsm.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    38803 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/lsm_diff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35256 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/lsm_nondiff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.2.2/gravtools/models/misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18698 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/mlr_bev_legacy.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.2.2/gravtools/models/station.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    99702 2023-07-12 11:07:51.000000 grav-toolbox-0.2.2/gravtools/models/survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32396 2023-05-14 14:10:01.000000 grav-toolbox-0.2.2/gravtools/models/vg_lsm.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.135650 grav-toolbox-0.2.2/gravtools/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/scripts/create_correction_time_seriens_from_tsf.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/scripts/load_tfs_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/scripts/run_gui.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    12252 2023-06-27 12:10:33.000000 grav-toolbox-0.2.2/gravtools/settings.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/gravtools/tides/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/tides/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16244 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/tides/correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/gravtools/tides/longman1959.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/tides/tide_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18016 2023-06-07 17:28:21.000000 grav-toolbox-0.2.2/gravtools/tides/tide_data_tfs.py
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.2.2/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)      917 2023-07-12 11:09:05.139649 grav-toolbox-0.2.2/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.685267 grav-toolbox-0.2.3/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6682 2023-08-08 14:01:28.685267 grav-toolbox-0.2.3/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6060 2023-08-08 14:00:57.000000 grav-toolbox-0.2.3/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.661267 grav-toolbox-0.2.3/bev_legacy/
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/__init__.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/adjust.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/adjust_reilly1970.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/command_line.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/const.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/drift_mlr.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/init.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/output.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/plots.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/schwaus.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.2.3/bev_legacy/settings.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/bev_legacy/utils.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.665267 grav-toolbox-0.2.3/grav_toolbox.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6682 2023-08-08 14:01:28.000000 grav-toolbox-0.2.3/grav_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2460 2023-08-08 14:01:28.000000 grav-toolbox-0.2.3/grav_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-08-08 14:01:28.000000 grav-toolbox-0.2.3/grav_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-08-08 14:01:28.000000 grav-toolbox-0.2.3/grav_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       59 2023-08-08 14:01:28.000000 grav-toolbox-0.2.3/grav_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-08-08 14:01:28.000000 grav-toolbox-0.2.3/grav_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.2.3/grav_toolbox.egg-info/zip-safe
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.665267 grav-toolbox-0.2.3/gravtools/
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.669267 grav-toolbox-0.2.3/gravtools/CG5_utils/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/CG5_utils/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35358 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/CG5_utils/cg5_survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/const.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.673267 grav-toolbox-0.2.3/gravtools/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    66060 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1322 2023-08-08 14:00:57.000000 grav-toolbox-0.2.3/gravtools/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_autoselection_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15709 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_estimation_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_export_results.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_gis_export_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_load_stations.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_new_campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_options.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2023-08-08 08:48:33.000000 grav-toolbox-0.2.3/gravtools/gui/dialog_setup_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15613 2023-08-08 14:00:57.000000 grav-toolbox-0.2.3/gravtools/gui/dlg_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1890 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/gui/dlg_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-06-07 17:28:21.000000 grav-toolbox-0.2.3/gravtools/gui/dlg_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   202051 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/gui/gui_misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15404 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_observation_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_results_correlation_matrix_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_results_drift_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_results_obs_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7493 2023-07-12 11:07:51.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_results_stat_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_results_vg_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9633 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_setup_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_station_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.2.3/gravtools/gui/gui_model_survey_table.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.681267 grav-toolbox-0.2.3/gravtools/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3978 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/atmosphere_correction.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    51790 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/models/exceptions.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    40811 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/lsm.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    39099 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/lsm_diff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35552 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/lsm_nondiff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.2.3/gravtools/models/misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    19191 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/mlr_bev_legacy.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.2.3/gravtools/models/station.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   112515 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32692 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/models/vg_lsm.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.681267 grav-toolbox-0.2.3/gravtools/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-06-07 17:28:21.000000 grav-toolbox-0.2.3/gravtools/scripts/create_correction_time_seriens_from_tsf.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-06-07 17:28:21.000000 grav-toolbox-0.2.3/gravtools/scripts/load_tfs_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/scripts/run_gui.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    12623 2023-08-08 14:01:05.000000 grav-toolbox-0.2.3/gravtools/settings.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-08-08 14:01:28.685267 grav-toolbox-0.2.3/gravtools/tides/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/gravtools/tides/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16244 2023-06-07 17:28:21.000000 grav-toolbox-0.2.3/gravtools/tides/correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16019 2023-08-08 14:00:57.000000 grav-toolbox-0.2.3/gravtools/tides/longman1959.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-06-07 17:28:21.000000 grav-toolbox-0.2.3/gravtools/tides/tide_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18016 2023-06-07 17:28:21.000000 grav-toolbox-0.2.3/gravtools/tides/tide_data_tfs.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.2.3/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)      917 2023-08-08 14:01:28.685267 grav-toolbox-0.2.3/setup.cfg
```

### Comparing `grav-toolbox-0.2.2/LICENSE` & `grav-toolbox-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/PKG-INFO` & `grav-toolbox-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,41 +15,38 @@
 Provides-Extra: gis
 License-File: LICENSE
 
 # GravTools
 GravTools is an open source software toolbox for processing relative gravity surveys developed at the Austrian
 Federal Office of Metrology and Surveying (BEV).  
 
-The source code is hosted on github.com: https://github.com/ahellers/GravTools
+ - The source code is hosted on github.com: https://github.com/ahellers/GravTools
+ - The python package is hosted at: https://pypi.org/project/grav-toolbox/
 
 # Installation
 
-## Install python package from pypi.org (Linux shell)
-For installation in a virtual python environment follow these steps: 
-
-1. Create a new virtual environment in the directory "venv": `python3 -n venv env`
-2. Activate the virtual env.: `source env/bin/activate`
-3. Install the GravTools package: `pip install grav-toolbox`
+## Install python package with pip:
+`pip install grav-toolbox`
 
 ### Optional dependency for GIS data export
 GravTools allows to export station- und observation-results to shapefiles for import and analysis in GIS programs.
 To enable these features the optional package "geopandas" needs to be installed by executing:
 `pip install grav-toolbox[gis]`
  
 ## Installation issues on Centos 8:
 * **1. Carry out installation steps describes above** 
 * **2. Install QT5, if required**
   * `sudo yum install qt5-qtbase-devel.x86_64`
   
-## Installation issues on Ubuntu (20.04):
+## Installation issues on Ubuntu 20.04:
 After just installing PyQt5 with pip3 the following error occurred when trying to actually run a PyQt GUI: qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
 This issue was resolved by installing the QT dev tools (Designer, etc.): 
-sudo apt-get install qttools5-dev-tools
+`sudo apt-get install qttools5-dev-tools`
 
-## Test installation with setuptools 
+## Test installation
 In a virtual environment.
 
 * Editable installation with pip: `pip install -e .`
   * Or: `make test_pack`
 * Uninstall: `pip uninstall grav-toolbox`
   * Or: `test_pack_uninstall`
 
@@ -59,63 +56,54 @@
 ## Create a source and binary distribution (sdist and wheel)
 * Set up setup.cfg and pyproject.toml in the project root directory
 * With make and the predefined makefile: `make build`
 * Without make: `python3 -m build`
 
 The created package (wheel and source distribution) is located in the "dist" directory.
 
-## Upload to pypi.org
-
+## Push package to pypi.org
 Define user credentials in /home/.pypirc
 
-* `twine upload --verbose dist/*`
+* `twine upload --verbose dist/*` or
+* `make pypi_push`
 
 
 # Create a stand-alone Windows executable
 For creating a Windows executable (stand-alone application, without python installation) the 
-package "auto-py-to-exe" is used (see: https://pypi.org/project/auto-py-to-exe/). This is a 
+package "auto-py-to-exe" can be used (see: https://pypi.org/project/auto-py-to-exe/). This is a 
 simple graphical user interface (based on the chrome browser) that allows to define all settings 
-for the package "PyInstaller" (see: https://www.pyinstaller.org/). auto-py-to-exe and all 
-required dependencies are listet in this project's requirements.txt file. 
-Creating a Windows executable with the mentioned packages was tested on a Windows 10 computer. 
-On Linux (Ubuntu 16.x) it failed to create an executable file, although no obvious errors occured.
+for the package "PyInstaller" (see: https://www.pyinstaller.org/). 
+
+Creating a Windows executable with auto-py-to-exe was tested on Windows 10. 
 Follow these steps to create an executable on a Windows machine:
 * **1. Install Python3**
   * With installer from https://www.python.org/downloads/windows/
   * Add python3.x to the Windows search path and install pip!
-* **2. Pull the project files from git as described above.**
-* **3. Install virtualenv and create a virtual environment** in CMD
+* **2. Install virtualenv and create a virtual environment** in CMD
   * a. `pip install virtualenv`
   * b. Change to project directory (`cd ..`)
   * c. Create virtual environment: `virtualenv env`
   * d. Activate it: `env\Scripts\activate.bat`
     * Deactivate with `deactivate`
-* **4. Install gravtools: `pip install gravtools-x.x.x.tar.gz`
-    * If a windiws executable should be created install auto-py-to-exe (`pip install auto-py-to-exe`)
-* **5. Try and run the application**
-  * Type `gt` in the command line interface (virtual environmernt must be active)
+* **3. Install gravtools**: `pip install gravtools[gis]`
+* **4. Install auto-py-to-exe**: `pip install auto-py-to-exe`
+* **5. Try to run the GravTools**
+  * Type `gt` in the command line interface (virtual environment must be active)
 * **6. Create exe with auto-py-to-exe**
   * Run the CMD Window as administrator!
   * a. Start auto-py-to-exe in CMD: `auto-py-to-exe`
   * b. Select the script location (select: gravtools/scripts/run_gui.py)
   * c. Select "One File" and "Console based" (in addition to teh GUI a console will appear)
   * d. Start conversion py pressing the big blue button on the GUI bottom
   * e. The exe file will be save at a new "output" directory. Move the file to: "Windows_executables"
- 
-# Comments on requirements.txt file:
-* Two entries can be deleted:
-  * -e git+git@gitlab.com:Heller182/grav.git@fe528c0769502e84a06be67a742032cacfd386df#egg=gravtools
-  * pkg-resources==0.0.0 (created due a bug when using Linux, see: https://stackoverflow.com/questions/39577984/what-is-pkg-resources-0-0-0-in-output-of-pip-freeze-command)
-
 
 # Create HTML documentation with sphinx:
 Sphinx is used to create an API documentation based on docstrings. Run make in the gravtools/doc directory: 
 * `>>>make html_doc`
 
-
 # Guidelines and conventions
 
 ## Code style:
 * Respect the PEP conventions on python coding!
   * PEP 8 -- Style Guide for Python Code: https://www.python.org/dev/peps/pep-0008/
 * The maximum line length is 120 characters
 * Use **type hints**: https://www.python.org/dev/peps/pep-0484/
```

### Comparing `grav-toolbox-0.2.2/README.md` & `grav-toolbox-0.2.3/grav_toolbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,52 @@
+Metadata-Version: 2.1
+Name: grav-toolbox
+Version: 0.2.3
+Summary: Gravity survey utility tools
+Home-page: https://github.com/ahellers/GravTools
+Author: Andreas Hellerschmied
+Author-email: andreas.hellerschmied@bev.gv.at
+License: GNU GPLv3
+Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: gis
+License-File: LICENSE
+
 # GravTools
 GravTools is an open source software toolbox for processing relative gravity surveys developed at the Austrian
 Federal Office of Metrology and Surveying (BEV).  
 
-The source code is hosted on github.com: https://github.com/ahellers/GravTools
+ - The source code is hosted on github.com: https://github.com/ahellers/GravTools
+ - The python package is hosted at: https://pypi.org/project/grav-toolbox/
 
 # Installation
 
-## Install python package from pypi.org (Linux shell)
-For installation in a virtual python environment follow these steps: 
-
-1. Create a new virtual environment in the directory "venv": `python3 -n venv env`
-2. Activate the virtual env.: `source env/bin/activate`
-3. Install the GravTools package: `pip install grav-toolbox`
+## Install python package with pip:
+`pip install grav-toolbox`
 
 ### Optional dependency for GIS data export
 GravTools allows to export station- und observation-results to shapefiles for import and analysis in GIS programs.
 To enable these features the optional package "geopandas" needs to be installed by executing:
 `pip install grav-toolbox[gis]`
  
 ## Installation issues on Centos 8:
 * **1. Carry out installation steps describes above** 
 * **2. Install QT5, if required**
   * `sudo yum install qt5-qtbase-devel.x86_64`
   
-## Installation issues on Ubuntu (20.04):
+## Installation issues on Ubuntu 20.04:
 After just installing PyQt5 with pip3 the following error occurred when trying to actually run a PyQt GUI: qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
 This issue was resolved by installing the QT dev tools (Designer, etc.): 
-sudo apt-get install qttools5-dev-tools
+`sudo apt-get install qttools5-dev-tools`
 
-## Test installation with setuptools 
+## Test installation
 In a virtual environment.
 
 * Editable installation with pip: `pip install -e .`
   * Or: `make test_pack`
 * Uninstall: `pip uninstall grav-toolbox`
   * Or: `test_pack_uninstall`
 
@@ -42,63 +56,54 @@
 ## Create a source and binary distribution (sdist and wheel)
 * Set up setup.cfg and pyproject.toml in the project root directory
 * With make and the predefined makefile: `make build`
 * Without make: `python3 -m build`
 
 The created package (wheel and source distribution) is located in the "dist" directory.
 
-## Upload to pypi.org
-
+## Push package to pypi.org
 Define user credentials in /home/.pypirc
 
-* `twine upload --verbose dist/*`
+* `twine upload --verbose dist/*` or
+* `make pypi_push`
 
 
 # Create a stand-alone Windows executable
 For creating a Windows executable (stand-alone application, without python installation) the 
-package "auto-py-to-exe" is used (see: https://pypi.org/project/auto-py-to-exe/). This is a 
+package "auto-py-to-exe" can be used (see: https://pypi.org/project/auto-py-to-exe/). This is a 
 simple graphical user interface (based on the chrome browser) that allows to define all settings 
-for the package "PyInstaller" (see: https://www.pyinstaller.org/). auto-py-to-exe and all 
-required dependencies are listet in this project's requirements.txt file. 
-Creating a Windows executable with the mentioned packages was tested on a Windows 10 computer. 
-On Linux (Ubuntu 16.x) it failed to create an executable file, although no obvious errors occured.
+for the package "PyInstaller" (see: https://www.pyinstaller.org/). 
+
+Creating a Windows executable with auto-py-to-exe was tested on Windows 10. 
 Follow these steps to create an executable on a Windows machine:
 * **1. Install Python3**
   * With installer from https://www.python.org/downloads/windows/
   * Add python3.x to the Windows search path and install pip!
-* **2. Pull the project files from git as described above.**
-* **3. Install virtualenv and create a virtual environment** in CMD
+* **2. Install virtualenv and create a virtual environment** in CMD
   * a. `pip install virtualenv`
   * b. Change to project directory (`cd ..`)
   * c. Create virtual environment: `virtualenv env`
   * d. Activate it: `env\Scripts\activate.bat`
     * Deactivate with `deactivate`
-* **4. Install gravtools: `pip install gravtools-x.x.x.tar.gz`
-    * If a windiws executable should be created install auto-py-to-exe (`pip install auto-py-to-exe`)
-* **5. Try and run the application**
-  * Type `gt` in the command line interface (virtual environmernt must be active)
+* **3. Install gravtools**: `pip install gravtools[gis]`
+* **4. Install auto-py-to-exe**: `pip install auto-py-to-exe`
+* **5. Try to run the GravTools**
+  * Type `gt` in the command line interface (virtual environment must be active)
 * **6. Create exe with auto-py-to-exe**
   * Run the CMD Window as administrator!
   * a. Start auto-py-to-exe in CMD: `auto-py-to-exe`
   * b. Select the script location (select: gravtools/scripts/run_gui.py)
   * c. Select "One File" and "Console based" (in addition to teh GUI a console will appear)
   * d. Start conversion py pressing the big blue button on the GUI bottom
   * e. The exe file will be save at a new "output" directory. Move the file to: "Windows_executables"
- 
-# Comments on requirements.txt file:
-* Two entries can be deleted:
-  * -e git+git@gitlab.com:Heller182/grav.git@fe528c0769502e84a06be67a742032cacfd386df#egg=gravtools
-  * pkg-resources==0.0.0 (created due a bug when using Linux, see: https://stackoverflow.com/questions/39577984/what-is-pkg-resources-0-0-0-in-output-of-pip-freeze-command)
-
 
 # Create HTML documentation with sphinx:
 Sphinx is used to create an API documentation based on docstrings. Run make in the gravtools/doc directory: 
 * `>>>make html_doc`
 
-
 # Guidelines and conventions
 
 ## Code style:
 * Respect the PEP conventions on python coding!
   * PEP 8 -- Style Guide for Python Code: https://www.python.org/dev/peps/pep-0008/
 * The maximum line length is 120 characters
 * Use **type hints**: https://www.python.org/dev/peps/pep-0484/
```

### Comparing `grav-toolbox-0.2.2/bev_legacy/adjust.py` & `grav-toolbox-0.2.3/bev_legacy/adjust.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/adjust_reilly1970.py` & `grav-toolbox-0.2.3/bev_legacy/adjust_reilly1970.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/command_line.py` & `grav-toolbox-0.2.3/bev_legacy/command_line.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/drift_mlr.py` & `grav-toolbox-0.2.3/bev_legacy/drift_mlr.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/init.py` & `grav-toolbox-0.2.3/bev_legacy/init.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/output.py` & `grav-toolbox-0.2.3/bev_legacy/output.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/plots.py` & `grav-toolbox-0.2.3/bev_legacy/plots.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/schwaus.py` & `grav-toolbox-0.2.3/bev_legacy/schwaus.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/settings.py` & `grav-toolbox-0.2.3/bev_legacy/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/bev_legacy/utils.py` & `grav-toolbox-0.2.3/bev_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/grav_toolbox.egg-info/PKG-INFO` & `grav-toolbox-0.2.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,35 @@
-Metadata-Version: 2.1
-Name: grav-toolbox
-Version: 0.2.2
-Summary: Gravity survey utility tools
-Home-page: https://github.com/ahellers/GravTools
-Author: Andreas Hellerschmied
-Author-email: andreas.hellerschmied@bev.gv.at
-License: GNU GPLv3
-Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: gis
-License-File: LICENSE
-
 # GravTools
 GravTools is an open source software toolbox for processing relative gravity surveys developed at the Austrian
 Federal Office of Metrology and Surveying (BEV).  
 
-The source code is hosted on github.com: https://github.com/ahellers/GravTools
+ - The source code is hosted on github.com: https://github.com/ahellers/GravTools
+ - The python package is hosted at: https://pypi.org/project/grav-toolbox/
 
 # Installation
 
-## Install python package from pypi.org (Linux shell)
-For installation in a virtual python environment follow these steps: 
-
-1. Create a new virtual environment in the directory "venv": `python3 -n venv env`
-2. Activate the virtual env.: `source env/bin/activate`
-3. Install the GravTools package: `pip install grav-toolbox`
+## Install python package with pip:
+`pip install grav-toolbox`
 
 ### Optional dependency for GIS data export
 GravTools allows to export station- und observation-results to shapefiles for import and analysis in GIS programs.
 To enable these features the optional package "geopandas" needs to be installed by executing:
 `pip install grav-toolbox[gis]`
  
 ## Installation issues on Centos 8:
 * **1. Carry out installation steps describes above** 
 * **2. Install QT5, if required**
   * `sudo yum install qt5-qtbase-devel.x86_64`
   
-## Installation issues on Ubuntu (20.04):
+## Installation issues on Ubuntu 20.04:
 After just installing PyQt5 with pip3 the following error occurred when trying to actually run a PyQt GUI: qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
 This issue was resolved by installing the QT dev tools (Designer, etc.): 
-sudo apt-get install qttools5-dev-tools
+`sudo apt-get install qttools5-dev-tools`
 
-## Test installation with setuptools 
+## Test installation
 In a virtual environment.
 
 * Editable installation with pip: `pip install -e .`
   * Or: `make test_pack`
 * Uninstall: `pip uninstall grav-toolbox`
   * Or: `test_pack_uninstall`
 
@@ -59,63 +39,54 @@
 ## Create a source and binary distribution (sdist and wheel)
 * Set up setup.cfg and pyproject.toml in the project root directory
 * With make and the predefined makefile: `make build`
 * Without make: `python3 -m build`
 
 The created package (wheel and source distribution) is located in the "dist" directory.
 
-## Upload to pypi.org
-
+## Push package to pypi.org
 Define user credentials in /home/.pypirc
 
-* `twine upload --verbose dist/*`
+* `twine upload --verbose dist/*` or
+* `make pypi_push`
 
 
 # Create a stand-alone Windows executable
 For creating a Windows executable (stand-alone application, without python installation) the 
-package "auto-py-to-exe" is used (see: https://pypi.org/project/auto-py-to-exe/). This is a 
+package "auto-py-to-exe" can be used (see: https://pypi.org/project/auto-py-to-exe/). This is a 
 simple graphical user interface (based on the chrome browser) that allows to define all settings 
-for the package "PyInstaller" (see: https://www.pyinstaller.org/). auto-py-to-exe and all 
-required dependencies are listet in this project's requirements.txt file. 
-Creating a Windows executable with the mentioned packages was tested on a Windows 10 computer. 
-On Linux (Ubuntu 16.x) it failed to create an executable file, although no obvious errors occured.
+for the package "PyInstaller" (see: https://www.pyinstaller.org/). 
+
+Creating a Windows executable with auto-py-to-exe was tested on Windows 10. 
 Follow these steps to create an executable on a Windows machine:
 * **1. Install Python3**
   * With installer from https://www.python.org/downloads/windows/
   * Add python3.x to the Windows search path and install pip!
-* **2. Pull the project files from git as described above.**
-* **3. Install virtualenv and create a virtual environment** in CMD
+* **2. Install virtualenv and create a virtual environment** in CMD
   * a. `pip install virtualenv`
   * b. Change to project directory (`cd ..`)
   * c. Create virtual environment: `virtualenv env`
   * d. Activate it: `env\Scripts\activate.bat`
     * Deactivate with `deactivate`
-* **4. Install gravtools: `pip install gravtools-x.x.x.tar.gz`
-    * If a windiws executable should be created install auto-py-to-exe (`pip install auto-py-to-exe`)
-* **5. Try and run the application**
-  * Type `gt` in the command line interface (virtual environmernt must be active)
+* **3. Install gravtools**: `pip install gravtools[gis]`
+* **4. Install auto-py-to-exe**: `pip install auto-py-to-exe`
+* **5. Try to run the GravTools**
+  * Type `gt` in the command line interface (virtual environment must be active)
 * **6. Create exe with auto-py-to-exe**
   * Run the CMD Window as administrator!
   * a. Start auto-py-to-exe in CMD: `auto-py-to-exe`
   * b. Select the script location (select: gravtools/scripts/run_gui.py)
   * c. Select "One File" and "Console based" (in addition to teh GUI a console will appear)
   * d. Start conversion py pressing the big blue button on the GUI bottom
   * e. The exe file will be save at a new "output" directory. Move the file to: "Windows_executables"
- 
-# Comments on requirements.txt file:
-* Two entries can be deleted:
-  * -e git+git@gitlab.com:Heller182/grav.git@fe528c0769502e84a06be67a742032cacfd386df#egg=gravtools
-  * pkg-resources==0.0.0 (created due a bug when using Linux, see: https://stackoverflow.com/questions/39577984/what-is-pkg-resources-0-0-0-in-output-of-pip-freeze-command)
-
 
 # Create HTML documentation with sphinx:
 Sphinx is used to create an API documentation based on docstrings. Run make in the gravtools/doc directory: 
 * `>>>make html_doc`
 
-
 # Guidelines and conventions
 
 ## Code style:
 * Respect the PEP conventions on python coding!
   * PEP 8 -- Style Guide for Python Code: https://www.python.org/dev/peps/pep-0008/
 * The maximum line length is 120 characters
 * Use **type hints**: https://www.python.org/dev/peps/pep-0484/
```

### Comparing `grav-toolbox-0.2.2/grav_toolbox.egg-info/SOURCES.txt` & `grav-toolbox-0.2.3/grav_toolbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 gravtools/gui/gui_model_results_obs_table.py
 gravtools/gui/gui_model_results_stat_table.py
 gravtools/gui/gui_model_results_vg_table.py
 gravtools/gui/gui_model_setup_table.py
 gravtools/gui/gui_model_station_table.py
 gravtools/gui/gui_model_survey_table.py
 gravtools/models/__init__.py
+gravtools/models/atmosphere_correction.py
 gravtools/models/campaign.py
 gravtools/models/exceptions.py
 gravtools/models/lsm.py
 gravtools/models/lsm_diff.py
 gravtools/models/lsm_nondiff.py
 gravtools/models/misc.py
 gravtools/models/mlr_bev_legacy.py
```

### Comparing `grav-toolbox-0.2.2/gravtools/CG5_utils/__init__.py` & `grav-toolbox-0.2.3/gravtools/CG5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/CG5_utils/cg5_survey.py` & `grav-toolbox-0.2.3/gravtools/CG5_utils/cg5_survey.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     Attributes
     ----------
     survey_name : str
         Name of gravity survey.
     client : str
         Client of survey.
     operator : str
-        Name of the survey'S operator.
+        Name of the survey's operator.
     long_deg : float
         Geographical longitude at begin of survey [°].
     lat_deg : float
         Geographical latitude at begin of survey [°].
     zone : str
         Timezone of all time records.
     date_time : datetime object
@@ -400,15 +400,15 @@
     survey_parameters : :py:class:`.CG5SurveyParameters`
         Survey Parameter of the Parameters block in the observation file.
     setup_parameters :  :py:class:`.CG5SetupParameters`
         Setup Parameter of the Setup block in the observation file.
     options : :py:class:`.CG5OptionsParameters`
         Instrumental options from the Options block in the observation file.
     obs_df : pandas data frame
-       Contains the actual observation data records.
+       Contains the actual observation data records with the colums defined in `self._OBS_DF_COLUMN_NAMES`.
     """
 
     # Column names of the dataframe containing tha actual observation data:
     _OBS_DF_COLUMN_NAMES = ('lat_deg',  # Latitude [deg] :
                             'lon_deg',  # Longitude [deg]
                             'alt_m',  # Altitude [m]
                             'g_mgal',  # Determined gravity (corrected) [mGal]
@@ -422,14 +422,15 @@
                             'time_str',  # Reference time = mid of setup with duration `duration_sec`) (dropped later)
                             'dec_time_date',
                             'terrain',  # Terrain correction [??]
                             'date',  # Date (dropped later)
                             'station_name',  # Station name : str
                             'dhf_m',  # Distance between instrument top and physical reference point [m]
                             'dhb_m',  # Distance between instrument top and ground [m]
+                            'atm_pres_hpa',  # Measured atmospheric pressure [hPa]
                             'setup_id',  # Unique ID of this observation (=setup)
                             )
                             # obs_epoch : datetime object (added to df later)
 
     # Rename columns: df.rename(columns = {'$b':'B'}, inplace = True)
 
     # Non-numeric columns in the observation dataframe:
@@ -466,19 +467,14 @@
 
         # Read observation file, if a valid filename is available and valid. Otherwise initialize obs_df as None.
         if self.obs_filename:
             self.read_obs_file(obs_filename)
         else:
             self.obs_df = None  # Initialize as None
 
-    # def set_params(self, param_dict):
-    #     for param in param_dict:
-    #         if param in self.PARAM_ATTRIBUTES:
-    #             self.__setattr__("param_" + param, param_dict[param])
-
     def __str__(self):
         if self.obs_df is None:
             return 'Empty CG-5 Survey.'
         else:
             if not self.survey_parameters.survey_name:
                 return 'Unnamed CG-5 Survey with {} observations (file: {}).'.format(len(self.obs_df),
                                                                                      self.obs_filename.split('/')[-1])
@@ -586,81 +582,124 @@
         # ### 3 possibilities: ###
         # Initialize empty dataframe and append observation blocks at each station
         # Warning: Better performance, when preparing the data as list (appending) and then converting to df at once.
         #  See: https://stackoverflow.com/questions/13784192/creating-an-empty-pandas-dataframe-then-filling-it
 
         obs_list = []  # Collect all obs data in this list and then convert to pd dataframe.
 
-        # 1.) Only Station name
-        expr = "\/\s+Note:\s+(?P<station_name>\S+)\s*\n(?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r\n])+)"
-        dhf_m = 0.0
-        dhb_m = 0.0
+        # 1.) Station name & dbh=dhf
+        expr = '\/\tNote:   \t(?P<station_name>\S+)\s+(?P<dh_cm>-?[.0-9]+)\s*[\r?\n](?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r?\n])+)'
         for obs_block in re.finditer(expr, str_obs_file):
             obs_dict = obs_block.groupdict()
             station_name = self.resolve_station_name(obs_dict['station_name'])
+            dhf_m = float(obs_dict['dh_cm']) * 1e-2
+            dhb_m = float(obs_dict['dh_cm']) * 1e-2
+            atm_pres_hpa = None
             lines = obs_dict['obs_data'].splitlines()
             # Create unique ID (= UNIX timestamp of first observation) for each setup on a station:
             #  - To distinguish multiple setups (with multiple observations each) on multiple stations
             time_str = lines[0].split()[-1] + ' ' + lines[0].split()[11]
             setup_id = int(dt.datetime.timestamp(dt.datetime.strptime(time_str, "%Y/%m/%d %H:%M:%S")))
 
             for line in lines:
                 line_items = line.split()
                 line_items.append(station_name)
                 line_items.append(dhf_m)
                 line_items.append(dhb_m)
+                line_items.append(atm_pres_hpa)
                 line_items.append(setup_id)
                 obs_list.append(line_items)
 
-        # 2.) Station name & dbh=dhf
-        expr = "\/\s+Note:\s+(?P<station_name>\S+)\s+(?P<dh_cm>\S+)\s*\n(?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r\n])+)"
+        # 2.) Station name & dbh=dhf & pressure
+        expr = '\/\tNote:   \t(?P<station_name>\S+)\s+(?P<dh_cm>-?[.0-9]+)\s*[\r?\n](?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r?\n])+)\/\tNote:   \t(?P<pres>[0-9]{3,4}[.]{0,1}[0-9]*)'
         for obs_block in re.finditer(expr, str_obs_file):
             obs_dict = obs_block.groupdict()
             station_name = self.resolve_station_name(obs_dict['station_name'])
             dhf_m = float(obs_dict['dh_cm']) * 1e-2
             dhb_m = float(obs_dict['dh_cm']) * 1e-2
+            atm_pres_hpa = float(obs_dict['pres'])
             lines = obs_dict['obs_data'].splitlines()
             # Create unique ID (= UNIX timestamp of first observation) for each setup on a station:
             #  - To distinguish multiple setups (with multiple observations each) on multiple stations
             time_str = lines[0].split()[-1] + ' ' + lines[0].split()[11]
             setup_id = int(dt.datetime.timestamp(dt.datetime.strptime(time_str, "%Y/%m/%d %H:%M:%S")))
 
             for line in lines:
                 line_items = line.split()
                 line_items.append(station_name)
                 line_items.append(dhf_m)
                 line_items.append(dhb_m)
+                line_items.append(atm_pres_hpa)
                 line_items.append(setup_id)
                 obs_list.append(line_items)
 
         # 3.) Station name & dhb & dhf
-        expr = "\/\s+Note:\s+(?P<station_name>\S+)\s+(?P<dhb_cm>\S+)\s+(?P<dhf_cm>\S+)\s*\n(?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r\n])+)"
+        expr = '\/\tNote:   \t(?P<station_name>\S+)\s+(?P<dhb_cm>-?[.0-9]+)\s+(?P<dhf_cm>-?[.0-9]+)\s*[\r?\n](?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r?\n])+)'
+        for obs_block in re.finditer(expr, str_obs_file):
+            obs_dict = obs_block.groupdict()
+
+            station_name = self.resolve_station_name(obs_dict['station_name'])
+            dhf_m = float(obs_dict['dhf_cm']) * 1e-2
+            dhb_m = float(obs_dict['dhb_cm']) * 1e-2
+            atm_pres_hpa = None
+            lines = obs_dict['obs_data'].splitlines()
+            # Create unique ID (= UNIX timestamp of first observation) for each setup on a station:
+            #  - To distinguish multiple setups (with multiple observations each) on multiple stations
+            time_str = lines[0].split()[-1] + ' ' + lines[0].split()[11]
+            setup_id = int(dt.datetime.timestamp(dt.datetime.strptime(time_str, "%Y/%m/%d %H:%M:%S")))
+
+            for line in lines:
+                line_items = line.split()
+                line_items.append(station_name)
+                line_items.append(dhf_m)
+                line_items.append(dhb_m)
+                line_items.append(atm_pres_hpa)
+                line_items.append(setup_id)
+                obs_list.append(line_items)
+
+        # 4.) Station name & dhb & dhf & pressure
+        # expr = "\/\s+Note:\s+(?P<station_name>\S+)\s+(?P<dhb_cm>\S+)\s+(?P<dhf_cm>\S+)\s*\n(?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r\n])+)"
+        expr = '\/\tNote:   \t(?P<station_name>\S+)\s+(?P<dhb_cm>-?[.0-9]+)\s+(?P<dhf_cm>-?[.0-9]+)\s*[\r?\n](?P<obs_data>(?:\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s+\S+\s*[\r?\n])+)\/\tNote:   \t(?P<pres>[0-9]{3,4}[.]{0,1}[0-9]*)'
         for obs_block in re.finditer(expr, str_obs_file):
             obs_dict = obs_block.groupdict()
 
             station_name = self.resolve_station_name(obs_dict['station_name'])
             dhf_m = float(obs_dict['dhf_cm']) * 1e-2
             dhb_m = float(obs_dict['dhb_cm']) * 1e-2
+            atm_pres_hpa = float(obs_dict['pres'])
             lines = obs_dict['obs_data'].splitlines()
             # Create unique ID (= UNIX timestamp of first observation) for each setup on a station:
             #  - To distinguish multiple setups (with multiple observations each) on multiple stations
             time_str = lines[0].split()[-1] + ' ' + lines[0].split()[11]
             setup_id = int(dt.datetime.timestamp(dt.datetime.strptime(time_str, "%Y/%m/%d %H:%M:%S")))
 
             for line in lines:
                 line_items = line.split()
                 line_items.append(station_name)
                 line_items.append(dhf_m)
                 line_items.append(dhb_m)
+                line_items.append(atm_pres_hpa)
                 line_items.append(setup_id)
                 obs_list.append(line_items)
 
         # Create pandas dataframe of prepared list:
         self.obs_df = pd.DataFrame(obs_list, columns=self._OBS_DF_COLUMN_NAMES)
 
+        # Remove duplicates entries that were matched with and without pressure:
+        setup_ids = self.obs_df['setup_id'].unique().tolist()
+        setup_ids_diplicates = []
+        for setup_id in setup_ids:
+            tmp_filter = self.obs_df['setup_id'] == setup_id
+            if (~self.obs_df.loc[tmp_filter, 'atm_pres_hpa'].isna()).any():  # Entries with pressure found
+                setup_ids_diplicates.append(setup_id)
+
+        if setup_ids_diplicates:
+            tmp_filter = ~(self.obs_df['atm_pres_hpa'].isna() & self.obs_df['setup_id'].isin(setup_ids_diplicates))
+            self.obs_df = self.obs_df.loc[tmp_filter].copy(deep=True)
+
         # Convert numeric columns to numeric dtypes:
         cols = self.obs_df.columns.drop(self._OBS_DF_NON_NUMERIC_COLUMNS)
         self.obs_df[cols] = self.obs_df[cols].apply(pd.to_numeric, errors='raise')
         # Sort observations by time and date and reset index:
         self.obs_df.sort_values(by='dec_time_date', inplace=True, ignore_index=True)
         # Convert date and time to datetime objects (aware, if UTC offset is available):
         if self.survey_parameters.date_time is not None:
```

### Comparing `grav-toolbox-0.2.2/gravtools/__init__.py` & `grav-toolbox-0.2.3/gravtools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (andreas.hellerschmied@bev.gv.at)
 """
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://github.com/ahellers/GravTools'
 __pypi_repo__ = 'https://pypi.org/project/grav-toolbox/'
 __email__ = 'andreas.hellerschmied@bev.gv.at'
 __copyright__ = '(c) 2022 Andreas Hellerschmied'
```

### Comparing `grav-toolbox-0.2.2/gravtools/const.py` & `grav-toolbox-0.2.3/gravtools/const.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/MainWindow.py` & `grav-toolbox-0.2.3/gravtools/gui/MainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,21 @@
         self.label_obs_setups_2 = QtWidgets.QLabel(self.groupBox_obs_setups_applied_corrections)
         self.label_obs_setups_2.setObjectName("label_obs_setups_2")
         self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_obs_setups_2)
         self.label_obs_setups_ref_height = QtWidgets.QLabel(self.groupBox_obs_setups_applied_corrections)
         self.label_obs_setups_ref_height.setText("")
         self.label_obs_setups_ref_height.setObjectName("label_obs_setups_ref_height")
         self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.label_obs_setups_ref_height)
+        self.label_obs_setups_3 = QtWidgets.QLabel(self.groupBox_obs_setups_applied_corrections)
+        self.label_obs_setups_3.setObjectName("label_obs_setups_3")
+        self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_obs_setups_3)
+        self.label_obs_setups_atm_pres_corr = QtWidgets.QLabel(self.groupBox_obs_setups_applied_corrections)
+        self.label_obs_setups_atm_pres_corr.setText("")
+        self.label_obs_setups_atm_pres_corr.setObjectName("label_obs_setups_atm_pres_corr")
+        self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.label_obs_setups_atm_pres_corr)
         self.verticalLayout_11.addWidget(self.groupBox_obs_setups_applied_corrections)
         self.tabWidget_observations.addTab(self.tab_observations_setups, "")
         self.verticalLayout_7.addWidget(self.splitter_obs)
         self.tabWidget_Main.addTab(self.tab_main_observations, "")
         self.tab_main_results = QtWidgets.QWidget()
         self.tab_main_results.setToolTipDuration(2)
         self.tab_main_results.setObjectName("tab_main_results")
@@ -697,14 +704,15 @@
         self.groupBox_obs_setups_applied_corrections.setTitle(_translate("MainWindow", "Applied corrections:"))
         self.label_obs_setups_1.setToolTip(_translate("MainWindow", "Type of applied tidal corrections."))
         self.label_obs_setups_1.setText(_translate("MainWindow", "Tidal correction:"))
         self.label_obs_setups_tidal_corr.setToolTip(_translate("MainWindow", "Type of applied tidal corrections."))
         self.label_obs_setups_2.setToolTip(_translate("MainWindow", "Type of the applied reference height reduction."))
         self.label_obs_setups_2.setText(_translate("MainWindow", "Obs. reference height:"))
         self.label_obs_setups_ref_height.setToolTip(_translate("MainWindow", "Type of the applied reference height reduction."))
+        self.label_obs_setups_3.setText(_translate("MainWindow", "Atm. pressure correction: "))
         self.tabWidget_observations.setTabText(self.tabWidget_observations.indexOf(self.tab_observations_setups), _translate("MainWindow", "Setups table"))
         self.tabWidget_Main.setTabText(self.tabWidget_Main.indexOf(self.tab_main_observations), _translate("MainWindow", "Observations"))
         self.groupBox_results_lsm_runs.setTitle(_translate("MainWindow", "LSM runs"))
         self.pushButton_results_delete_lsm_run.setText(_translate("MainWindow", "Delete selected lsm run"))
         self.groupBox_results_data_selection.setTitle(_translate("MainWindow", "Data selection"))
         self.label_2.setText(_translate("MainWindow", "Station"))
         self.comboBox_results_selection_station.setItemText(0, _translate("MainWindow", "All stations"))
```

### Comparing `grav-toolbox-0.2.2/gravtools/gui/__init__.py` & `grav-toolbox-0.2.3/gravtools/gui/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 GravTools - A software toolbox for processing relative gravity surveys
 ======================================================================
 
 The module *gui* represents the graphical user interface of GravTools written with PyQt.
 
 Notes
 -----
-The *.ui files are created using the Qt Designer. The according *.py files are automatically created with the program
-pyuic5 based on the *.ui files and should therefore not be edited!
+
+The .ui files are created using the Qt Designer. The according .py files are automatically created with the program
+pyuic5 based on the .ui files and should therefore not be edited!
 
 License, contact and authorship
 -------------------------------
 
 Copyright (C) 2021  Andreas Hellerschmied
 
 GravTools was developed at Austria's the *Federal Office of Metrology and Surveying (BEV)*.
```

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_about.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_about.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_autoselection_settings.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_autoselection_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_correction_time_series.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_estimation_settings.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_estimation_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_export_results.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_export_results.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_gis_export_settings.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_gis_export_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_load_stations.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_load_stations.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_load_tsf_file.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_load_tsf_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_new_campaign.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_new_campaign.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_options.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_options.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dialog_setup_data.py` & `grav-toolbox-0.2.3/gravtools/gui/dialog_setup_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dlg_correction_time_series.py` & `grav-toolbox-0.2.3/gravtools/gui/dlg_correction_time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from PyQt5.QtWidgets import QDialog, QMessageBox, QTreeWidgetItem
 import pyqtgraph as pg
 
 from gravtools.gui.dialog_correction_time_series import Ui_DialogCorrectionTimeSeries
 from gravtools.gui.dlg_load_tsf_file import DialogLoadTsfFile
 from gravtools import __version__
+from gravtools import settings
 
 # Set splitter stretch:
 _SPLITTER_STRETCH_LEFT = 1
 _SPLITTER_STRETCH_RIGHT = 10
 
 class TimeAxisItem(pg.AxisItem):
     """"Needed to handle the x-axes tags representing date and time.
@@ -37,15 +38,15 @@
 
     Notes
     -----
     The timestamps need to refer to UTC!"
     """
     def tickStrings(self, values, scale, spacing) -> str:
         """Handles the x-axes tags representing date and time."""
-        return [dt.datetime.fromtimestamp(value, tz=pytz.utc) for value in values]
+        return [dt.datetime.fromtimestamp(value, tz=pytz.utc).strftime(settings.Y_TICK_DATETIME_FORMAT) for value in values]
 
 class DialogCorrectionTimeSeries(QDialog, Ui_DialogCorrectionTimeSeries):
     """Dialog for managing time series data for observation corrections."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
```

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dlg_corrections.py` & `grav-toolbox-0.2.3/gravtools/gui/dlg_corrections.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,7 +36,9 @@
 
         # Set up combo box for interpolation method selection and select default method:
         for idx, (method_name, tooltip) in enumerate(settings.SCIPY_INTERP1_INTERPOLATION_METHODS.items()):
             self.comboBox_tides_interpolation_method.addItem(method_name)
             self.comboBox_tides_interpolation_method.setItemData(idx, tooltip, QtCore.Qt.ToolTipRole)
             if method_name == settings.SCIPY_INTERP1_INTERPOLATION_DEFAULT_METHOD:
                 self.comboBox_tides_interpolation_method.setCurrentIndex(idx)
+
+        self.doubleSpinBox_atm_pres_admittance.setValue(settings.ATM_PRES_CORRECTION_ADMITTANCE_DEFAULT)
```

### Comparing `grav-toolbox-0.2.2/gravtools/gui/dlg_load_tsf_file.py` & `grav-toolbox-0.2.3/gravtools/gui/dlg_load_tsf_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_main.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -495,16 +495,14 @@
                 self.set_up_results_drift_view_model()
                 self.set_up_results_vg_view_model()
                 self.update_results_tab(select_latest_item=True)
                 # - Corrections time series dialog:
                 self.dlg_correction_time_series.check_correction_time_series_object(parent=self)
                 self.dlg_correction_time_series.reset_update_gui()
 
-
-
                 self.statusBar().showMessage(
                     f"Previously saved campaign loaded rom pickle file (name: {self.campaign.campaign_name}, "
                     f"output directory: {self.campaign.output_directory})")
                 self.setWindowTitle('GravTools - Campaign: ' + self.campaign.campaign_name)
         else:
             self.statusBar().showMessage(f"No campaign data loaded.")
 
@@ -1885,17 +1883,23 @@
                 self.label_obs_setups_ref_height.setText(f'{self.setup_model.get_ref_heigth_type} ({settings.REFERENCE_HEIGHT_TYPE[self.setup_model.get_ref_heigth_type]})')
             else:
                 self.label_obs_setups_ref_height.setText(f'{self.setup_model.get_ref_heigth_type}')
             if self.setup_model.get_tidal_corr_type in settings.TIDE_CORRECTION_TYPES.keys():
                 self.label_obs_setups_tidal_corr.setText(f'{self.setup_model.get_tidal_corr_type} ({settings.TIDE_CORRECTION_TYPES[self.setup_model.get_tidal_corr_type]})')
             else:
                 self.label_obs_setups_tidal_corr.setText(f'{self.setup_model.get_tidal_corr_type}')
+            if self.setup_model.get_atm_pres_corr_type in settings.ATM_PRES_CORRECTION_TYPES.keys():
+                self.label_obs_setups_atm_pres_corr.setText(f'{self.setup_model.get_atm_pres_corr_type} ({settings.ATM_PRES_CORRECTION_TYPES[self.setup_model.get_atm_pres_corr_type]})')
+            else:
+                self.label_obs_setups_atm_pres_corr.setText(f'{self.setup_model.get_atm_pres_corr_type}')
+
         except KeyError:
             self.label_obs_setups_ref_height.setText('')
             self.label_obs_setups_tidal_corr.setText('')
+            self.label_obs_setups_atm_pres_corr.setText('')
 
     def compute_setup_data_for_campaign(self):
         """Compute setup data for the campaign."""
 
         # Get GUI settings:
         active_obs_only_for_ref_epoch = self.dlg_setup_data.checkBox_drift_ref_epoch_active_obs_only.checkState() == Qt.Checked
         if self.dlg_setup_data.radioButton_variance_weighted_mean.isChecked():
@@ -2469,28 +2473,40 @@
 
                 # Get data:
             if flag_show_reduced_observations:
                 g_mugal = obs_df['g_red_mugal'].astype(float).values
                 sd_g_mugal = obs_df['sd_g_red_mugal'].values
                 corr_tide = obs_df['corr_tide_red_mugal'].values
                 corr_tide_name = self.campaign.surveys[survey_name].red_tide_correction_type
+
+                # try-except scheme to provide downward compatibility for versions < 0.2.3
+                try:
+                    corr_atm_pres_name = self.campaign.surveys[survey_name].red_atm_pres_correction_type
+                except AttributeError:
+                    corr_atm_pres_name = '' # ... won't be plotted in GUI.
+                corr_atm_pres = obs_df['corr_atm_pres_red_mugal'].values
+                if (corr_atm_pres == None).all():
+                    corr_atm_pres_name = ''  # ... won't be plotted in GUI.
+                elif np.isnan(corr_atm_pres).all():
+                    corr_atm_pres_name = ''  # ... won't be plotted in GUI.
                 try:
                     corr_description_str = self.campaign.surveys[survey_name].red_tide_correction_description
                 except AttributeError:
                     pass
                 else:
                     if corr_description_str:
                         corr_tide_name = corr_tide_name + ': ' + corr_description_str
                 ref_height_name = self.campaign.surveys[survey_name].red_reference_height_type
             else:
                 g_mugal = obs_df['g_obs_mugal'].values
                 sd_g_mugal = obs_df['sd_g_obs_mugal'].values
                 corr_tide = obs_df['corr_tide_mugal'].values
                 corr_tide_name = self.campaign.surveys[survey_name].obs_tide_correction_type
                 ref_height_name = self.campaign.surveys[survey_name].obs_reference_height_type
+                corr_atm_pres_name = ''  # ... won't be plotted in GUI.
 
             # Gravity g [µGal]
             # - Plot with marker symbols according to their 'keep_obs' states and connect the 'sigPointsClicked' event.
             self.plot_obs_g.clear()
             self.plot_obs_g.setLabel(axis='left', text=f'g [µGal]')
             self.plot_obs_g.setTitle(f'Observed gravity [µGal]')
             pen = pg.mkPen(color='b')
@@ -2543,16 +2559,22 @@
             self.plot_xy_data(self.plot_obs_tilt, obs_epoch_timestamps, tilt_y, plot_name='Y', color='r', symbol='t',
                               symbol_size=10)
             self.plot_obs_tilt.showGrid(x=True, y=True)
             self.plot_obs_tilt.autoRange()
 
             # Observation corrections [µGal]
             self.plot_obs_corrections.clear()
+            # - Tidal corrections:
             self.plot_xy_data(self.plot_obs_corrections, obs_epoch_timestamps, corr_tide,
                               plot_name=f'tides ({corr_tide_name})', color='b', symbol='o', symbol_size=10)
+            # - Atm. pressure corrections (if available):
+            if corr_atm_pres_name != '' and corr_atm_pres_name != 'no_atm_pres_corr':
+                self.plot_xy_data(self.plot_obs_corrections, obs_epoch_timestamps, corr_atm_pres,
+                                  plot_name=f'atm. pres ({corr_atm_pres_name})', color='r', symbol='o', symbol_size=10)
+
             self.plot_obs_corrections.showGrid(x=True, y=True)
             self.plot_obs_corrections.autoRange()
 
             self.plot_obs_g.autoRange()  # Finally adjust data range to g values!
 
     def plot_xy_data(self, plot_item, x, y, plot_name, color='k', symbol='o', symbol_size=10):
         """Plot XY-data."""
@@ -2868,15 +2890,15 @@
     def on_menu_help_about(self):
         """Launch the about dialog."""
         _ = self.dlg_about.exec()
 
     def on_menu_observations_corrections(self):
         """Launch diaglog to select and apply observation corrections."""
         return_value = self.dlg_corrections.exec()
-        if return_value == QDialog.Accepted:
+        if return_value == QDialog.Accepted and self.campaign:
             try:
                 self.apply_observation_corrections()
             except Exception as e:
                 QMessageBox.critical(self, 'Error!', str(e))
                 self.statusBar().showMessage(f"Error: No observation corrections applied.")
             else:
                 # Load survey from campaign data to observations vie model:
@@ -2898,36 +2920,49 @@
         elif self.dlg_corrections.radioButton_corr_ref_heights_sensor.isChecked():
             target_ref_height = 'sensor_height'
         elif self.dlg_corrections.radioButton_corr_ref_heights_instrument_top.isChecked():
             target_ref_height = 'instrument_top'
         else:
             flag_selection_ok = False
             error_msg = f'Invalid selection of reference height in GUI (observation corrections dialog).'
-            # QMessageBox.critical('Error!', error_msg)
+            QMessageBox.critical('Error!', error_msg)
 
         if self.dlg_corrections.radioButton_corr_tides_no_correction.isChecked():
             target_tide_corr = 'no_tide_corr'
         elif self.dlg_corrections.radioButton_corr_tides_cg5_model.isChecked():
             target_tide_corr = 'cg5_longman1959'
         elif self.dlg_corrections.radioButton_corr_tides_longman1959.isChecked():
             target_tide_corr = 'longman1959'
         elif self.dlg_corrections.radioButton_corr_tides_time_series.isChecked():
             target_tide_corr = 'from_time_series'
             tide_corr_timeseries_interpol_method = self.dlg_corrections.comboBox_tides_interpolation_method.currentText()
         else:
             flag_selection_ok = False
             error_msg = f'Invalid selection of tidal correction in GUI (observation corrections dialog).'
-            # QMessageBox.critical('Error!', error_msg)
+            QMessageBox.critical('Error!', error_msg)
+
+        if self.dlg_corrections.checkBox_corrections_atm_pressure.isChecked():
+            target_atm_pres_corr = 'iso_2533_1975'
+        else:
+            target_atm_pres_corr = 'no_atm_pres_corr'
+
+        atm_pres_admittance = self.dlg_corrections.doubleSpinBox_atm_pres_admittance.value()
 
         if flag_selection_ok:
-            self.campaign.reduce_observations_in_all_surveys(
-                target_ref_height=target_ref_height,
-                target_tide_corr=target_tide_corr,
-                tide_corr_timeseries_interpol_method=tide_corr_timeseries_interpol_method,
-                verbose=IS_VERBOSE)
+            try:
+                self.campaign.reduce_observations_in_all_surveys(
+                    target_ref_height=target_ref_height,
+                    target_tide_corr=target_tide_corr,
+                    target_atm_pres_corr=target_atm_pres_corr,
+                    atm_pres_admittance=atm_pres_admittance,
+                    tide_corr_timeseries_interpol_method=tide_corr_timeseries_interpol_method,
+                    verbose=IS_VERBOSE)
+            except Exception as e:
+                QMessageBox.critical(self, 'Error!', str(e))
+
 
     @pyqtSlot()
     def on_menu_file_new_campaign(self):
         """Launching dialog to create a new campaign."""
         dlg = DialogNewCampaign(old_campaign=self.campaign)
         return_value = dlg.exec()
         if return_value == QDialog.Accepted:
```

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_misc.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_observation_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_observation_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,20 +56,24 @@
         'corr_tide_red_mugal': 1,
         'temp': 1,
         'tiltx': 1,
         'tilty': 1,
         'dhf_m': 3,
         'dhb_m': 3,
         'vg_mugalm': 1,
+        'atm_pres_hpa': 1,
+        'corr_atm_pres_red_mugal': 1,
+        'norm_atm_pres_hpa': 1,
     }
 
     # Columns that will be shown in the table view, if available in the data (Also defines the order of columns):
     # - keys: Actual names of the dataframe columns
     # - items: Header names for the Table View Widget
     _SHOW_COLUMNS_IN_TABLE_DICT = {
+        'keep_obs': 'Ḱeep obs.',
         'station_name': 'Station',
         'setup_id': 'Setup ID',
         'loop_id': 'Loop ID',
         'lon_deg': 'Lon [°]',
         'lat_deg': 'Lat [°]',
         'alt_m': 'h [m]',
         'obs_epoch': 'Epoch UTC',
@@ -83,15 +87,17 @@
         'temp': 'Temp. corr. [?]',
         'tiltx': 'Tilt_x [asec]',
         'tilty': 'Tilt_y [asec]',
         'dhb_m': 'dhb [m]',
         'dhf_m': 'dhf [m]',
         'vg_mugal': 'VG [µGal]',
         'duration_sec': 'Duration [sec]',
-        'keep_obs': 'Ḱeep obs.',
+        'atm_pres_hpa': 'p [hPa]',
+        'norm_atm_pres_hpa': 'pn [hPa]',
+        'corr_atm_pres_red_mugal': 'p corr [µGal]',
     }
     _SHOW_COLUMNS_IN_TABLE = list(_SHOW_COLUMNS_IN_TABLE_DICT.keys())  # Actual list of columns to be shown
 
     # List of columns that are shown in the simple mode of the GUI
     _SHOW_COLUMNS_IN_TABLE_SIMPLE_GUI = [
         'station_name',
         'setup_id',
@@ -105,14 +111,16 @@
         'tiltx',
         'tilty',
         'corr_tide_red_mugal',
         'corr_tide_mugal',
         'vg_mugal',
         'duration_sec',
         'keep_obs',
+        'atm_pres_hpa',
+        'corr_atm_pres_red_mugal',
     ]
 
     def __init__(self, surveys):
         """Initialize the observation table view model.
 
         Parameters
         ----------
```

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_correlation_matrix_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_results_correlation_matrix_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_drift_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_results_drift_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_obs_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_results_obs_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_stat_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_results_stat_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_results_vg_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_results_vg_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_setup_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_setup_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         self._data = None  # Observations (or at subset of them) of the survey with the name `self._data_survey_name`
         self.load_surveys(surveys)
         self._data_survey_name = ''  # Name of the Survey that is currently represented by `self._data`
         self._data_column_names = None
         self.flag_gui_simple_mode = False
         self._reference_height_type = ''
         self._tide_correction_type = ''
+        self._atm_pres_correction_type = ''
 
     def load_surveys(self, surveys):
         """Load observation data (dict of survey objects in the campaign object) to the observation model.
 
         Notes
         -----
         The data is assigned by reference, i.e. all changes in `_surveys` will propagate to the data origin.
@@ -112,14 +113,18 @@
                 self._data_survey_name = survey_name
                 try:
                     self._reference_height_type = self._surveys[survey_name].setup_reference_height_type
                     self._tide_correction_type = self._surveys[survey_name].setup_tide_correction_type
                 except AttributeError:
                     self._reference_height_type = ''
                     self._tide_correction_type = ''
+                try:
+                    self._atm_pres_correction_type = self._surveys[survey_name].setup_atm_pres_correction_type
+                except AttributeError:
+                    self._atm_pres_correction_type = ''
                 self.flag_gui_simple_mode = gui_simple_mode
 
                 # Get list of columns to be depicted via the table model:
                 # - Keep order of items in `self._SHOW_COLUMNS_IN_TABLE`
                 if setup_df is not None:
                     setup_df_columns_set = frozenset(setup_df.columns)
                     table_model_columns = [x for x in self.get_table_columns if x in setup_df_columns_set]
@@ -204,7 +209,12 @@
         """Returns the reference height type of the setup observations."""
         return self._reference_height_type
 
     @property
     def get_tidal_corr_type(self):
         """Returns the tidal corrections applied on the setup observations."""
         return self._tide_correction_type
+
+    @property
+    def get_atm_pres_corr_type(self):
+        """Returns the atmospheric pressure corrections applied on the setup observations."""
+        return self._atm_pres_correction_type
```

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_station_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_station_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/gui/gui_model_survey_table.py` & `grav-toolbox-0.2.3/gravtools/gui/gui_model_survey_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/models/__init__.py` & `grav-toolbox-0.2.3/gravtools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/models/campaign.py` & `grav-toolbox-0.2.3/gravtools/models/campaign.py`

 * *Files 4% similar despite different names*

```diff
@@ -328,16 +328,19 @@
         return len(self.surveys)
 
     @property
     def number_of_stations(self) -> int:
         """int : Returns the number of stations in this campaign."""
         return self.stations.get_number_of_stations
 
-    def reduce_observations_in_all_surveys(self, target_ref_height=None,
+    def reduce_observations_in_all_surveys(self,
+                                           target_ref_height=None,
                                            target_tide_corr=None,
+                                           target_atm_pres_corr=None,
+                                           atm_pres_admittance=None,
                                            tide_corr_timeseries_interpol_method='',
                                            verbose=False):
         """Reduce the observed gravity by applying the specified corrections.
 
         Notes
         -----
         - For this reduction vertical gravity gradients are required. They are obtained from the `Station` object.
@@ -350,14 +353,22 @@
         target_ref_height : string, specifying the target reference height type (default = `None`).
             The target reference height type has to be listed in :py:obj:`gravtools.settings.REFERENCE_HEIGHT_TYPE`.
             Default is `None` indicating that the reference heights of the input data are not changed.
         target_tide_corr : str, specifying the tidal correction type to be applied (default = `None`).
             The target tidal correction type specifies what kind of tidal correction will be applied. Valid types have
             to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`. Default is `None` indicating that the
             tidal corrections are not considered here (tidal corrections are inherited from input data).
+        target_atm_pres_corr : str (default = `None`)
+            Specifying the atmospheric press ure correction type to be applied to all surveys. Valid types to be listed
+            in :py:obj:`gravtools.settings.ATM_PRES_CORRECTION_TYPES`. Default is `None` indicating that the respective
+            corrections of the input data are not changed.
+        atm_pres_admittance : float, optional (default = `None`)
+            Admittance factor for the determination of pressure corrections based on the difference between measured and
+            normal air pressure. If `target_atm_pres_corr` is not None (i.e. atmospheric pressure corrections will be
+            calculated), `atm_pres_admittance` has to be provided too (float). Otherwise, an error is raised.
         tide_corr_timeseries_interpol_method : str, optional (default='')
             Interpolation method used to calculate tidal corrections from time series data. If tidal corrections are
             obtained from other sources or models, this attribute is irrelevant and has to be empty!
         verbose : bool, optional (default=False)
             If True, status messages are printed to the command line.
         """
         if verbose:
@@ -368,14 +379,16 @@
             if target_ref_height is not None:
                 if verbose:
                     print(f' - Get vertical gradients')
                 survey.obs_df_populate_vg_from_stations(self.stations, verbose=verbose)
             survey.reduce_observations(
                 target_ref_height=target_ref_height,
                 target_tide_corr=target_tide_corr,
+                target_atm_pres_corr=target_atm_pres_corr,
+                atm_pres_admittance=atm_pres_admittance,
                 tide_corr_timeseries_interpol_method=tide_corr_timeseries_interpol_method,
                 correction_time_series=self.correction_time_series,
                 verbose=verbose)
 
     def add_stations_from_oesgn_table_file(self, oesgn_filename, is_datum=False, verbose=False):
         """Add station from an OESGN table file.
 
@@ -825,16 +838,39 @@
         -------
         `Campaign` object
         """
         campaign = pd.read_pickle(filename)
         if verbose:
             print(
                 f'Loaded campaign "{campaign.campaign_name}" with {campaign.number_of_stations} station(s) and {campaign.number_of_surveys} survey(s).')
+        campaign.check_survey_data(verbose=verbose)
         return campaign
 
+    def check_survey_data(self, verbose: bool = True):
+        """Check survey data in campaign, correct missing elements or raise an error.
+
+        Parameters
+        ----------
+        verbose : bool, optional (default=False)
+            If `True`, status messages are printed to the command line.
+
+        Returns
+        -------
+        `Campaign` object
+        """
+        for survey_name, survey in self.surveys.items():
+            # Check observation dataframe:
+            is_valid, error_msg = survey.check_obs_df(verbose=verbose)
+            if not is_valid:
+                if verbose:
+                    print('Error: ' + error_msg)
+                raise RuntimeError(error_msg)
+            # Check survey object attributes:
+            survey.init_missing_attributes(verbose=verbose)
+
     def set_output_directory(self, output_directory):
         """Change the campaign's output directory.
 
         Parameters
         ----------
         output_directory : str
             New output directory. The specified directory has to exist on the computer/os!
```

### Comparing `grav-toolbox-0.2.2/gravtools/models/exceptions.py` & `grav-toolbox-0.2.3/gravtools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/models/lsm.py` & `grav-toolbox-0.2.3/gravtools/models/lsm.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 """
 
 import numpy as np
 from scipy import stats
 import datetime as dt
 import pytz
 import copy
+import pandas as pd
 
 # optional imports:
 try:
     import geopandas
 except ImportError:
     _has_geopandas = False
 else:
@@ -241,14 +242,15 @@
                                              f'differential observations!')
                     else:
                         setup_data_dict = {'ref_epoch_delta_t_h': survey.ref_delta_t_dt,
                                            'ref_epoch_delta_t_campaign_h': campaign.ref_delta_t_dt,
                                            'setup_df': survey.setup_df,
                                            'tide_correction_type': survey.setup_tide_correction_type,
                                            'reference_height_type': survey.setup_reference_height_type,
+                                           'atm_pres_correction_type': survey.setup_atm_pres_correction_type,
                                            'setup_calc_method': survey.setup_calc_method,
                                            'setup_obs_list_df': survey.setup_obs_list_df}
                         setups[survey_name] = setup_data_dict
 
         # Check if setup data is available:
         if len(setups) == 0:
             raise AssertionError(f'Setup data of campaign "{campaign.campaign_name}" does not contain observations!')
@@ -591,14 +593,54 @@
         If observations were not aggregated within at least one setup, checking for unique setup IDs makes no sense.
         """
         for survey_name, setup_data in self.setups.items():
             if setup_data['setup_calc_method'] == 'individual_obs':
                 return False
         return True
 
+    @property
+    def survey_info_string(self) -> str:
+        """Returns information on all surveys."""
+        survey_names_list = []
+        num_setups_list = []
+        num_obs_total_list = []
+        num_obs_active_list = []
+        tide_correction_type_list = []
+        reference_height_type_list = []
+        atm_pres_correction_type_list = []
+        setup_calc_method_list = []
+        for survey_name, survey in self.setups.items():
+            survey_names_list.append(survey_name)
+            setup_df = survey['setup_df']
+            num_setups_list.append(len(setup_df))
+            setup_obs_list_df = survey['setup_obs_list_df']
+            num_obs_total_list.append(len(setup_obs_list_df))
+            num_obs_active_list.append(len(setup_obs_list_df.loc[setup_obs_list_df['keep_obs']]))
+            tide_correction_type_list.append(survey['tide_correction_type'])
+            reference_height_type_list.append(survey['reference_height_type'])
+            atm_pres_correction_type_list.append(survey['atm_pres_correction_type'])
+            setup_calc_method_list.append(survey['setup_calc_method'])
+        tmp_df = pd.DataFrame(list(zip(survey_names_list,
+                                       num_setups_list,
+                                       num_obs_total_list,
+                                       num_obs_active_list,
+                                       tide_correction_type_list,
+                                       reference_height_type_list,
+                                       atm_pres_correction_type_list,
+                                       setup_calc_method_list,
+                                       )),
+                          columns=['Survey', '#Setups', '#Obs', '#Active obs', 'Tide correction', 'Ref. height', 'Atm. correction', 'Setup calc. method'])
+        return tmp_df.to_string(index=False)
+
+    # @property
+    # def obs_level_corrections_info_string(self) -> str:
+    #     """Returns information on the applied observation-level corrections."""
+    #     info_str = ''
+    #     return info_str
+
 def bin_redundacy_components(mat_r):
     """Bin redundancy components for easier interpretatzion.
 
     See: Skriptum AG2 (Navratil, TU Wien), p. 70.
     """
     number_obs_r_equal_0 = 0  # No error control: Errors cannot be detected
     number_obs_r_0_to_03 = 0  # Bad error control
@@ -701,7 +743,12 @@
     if chi_crit_lower < test_value < chi_crit_upper:
     # if test_value <= test_value:  # Equ. (2-15) in Caspary (1987)
         chi_test_status = 'Passed'
     else:
         chi_test_status = 'Not passed'
     chi_crit = [chi_crit_lower, chi_crit_upper]
     return chi_crit, test_value, chi_test_status
+
+
+
+
+
```

### Comparing `grav-toolbox-0.2.2/gravtools/models/lsm_diff.py` & `grav-toolbox-0.2.3/gravtools/models/lsm_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,21 +268,30 @@
             tmp_str += f'Scaling factor for datum constraints: {scaling_factor_datum_observations}\n'
             tmp_str += f'Scaling factor for SD of setup observations: {scaling_factor_for_sd_of_observations}\n'
             tmp_str += f'Additive const. to SD of setup obs. [µGal]: {add_const_to_sd_of_observations_mugal}\n'
             tmp_str += f'Noise floor for std. error determination [µGal]: {noise_floor_mugal}\n'
             tmp_str += f'Confidence level Chi-test: {confidence_level_chi_test:4.2f}\n'
             tmp_str += f'Confidence level Tau-test: {confidence_level_tau_test:4.2f}\n'
             tmp_str += f'\n'
-            tmp_str += f'---- Set up and populate matrices ----\n'
+            tmp_str += f'---- Survey infos ----\n'
+            tmp_str += self.survey_info_string
+            tmp_str += f'\n'
+            tmp_str += f'\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # Initialize matrices:
+        if verbose or self.write_log:
+            tmp_str = f'---- Set up and populate matrices ----\n'
+            if verbose:
+                print(tmp_str)
+            if self.write_log:
+                self.log_str += tmp_str
         # => Initialize complete matrices first and then populate them. This is most efficient!
         # - Observation model:
         mat_A0 = np.zeros([number_of_diff_obs, number_of_parameters])  # Model-matrix
         mat_L0 = np.zeros((number_of_diff_obs, 1))
         mat_sig_ll0 = np.zeros(number_of_diff_obs)
         # - Constraints:
         mat_Ac = np.zeros([number_of_datum_stations, number_of_parameters])  # Model-matrix for constraints
@@ -404,15 +413,15 @@
         mat_L = np.vstack((mat_L0, mat_Lc))  # Eq. (16)
         mat_sig_ll = np.diag(np.hstack((mat_sig_ll0, mat_sig_llc)))
         mat_Qll = mat_sig_ll / (sig0_mugal ** 2)
         mat_P = np.linalg.inv(mat_Qll)
 
         if verbose or self.write_log:
             tmp_str = f'\n'
-            tmp_str += f'---- Solve equation system: Results and statistics ----\n'
+            tmp_str += f'---- Results and statistics ----\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # Solve equation system:
         mat_N = mat_A.T @ mat_P @ mat_A  # Normal equation matrix
```

### Comparing `grav-toolbox-0.2.2/gravtools/models/lsm_nondiff.py` & `grav-toolbox-0.2.3/gravtools/models/lsm_nondiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,21 +257,30 @@
             tmp_str += f'Scaling factor for datum constraints: {scaling_factor_datum_observations}\n'
             tmp_str += f'Scaling factor for SD of setup observations: {scaling_factor_for_sd_of_observations}\n'
             tmp_str += f'Additive const. to SD of setup obs. [µGal]: {add_const_to_sd_of_observations_mugal}\n'
             tmp_str += f'Noise floor for std. error determination [µGal]: {noise_floor_mugal}\n'
             tmp_str += f'Confidence level Chi-test: {confidence_level_chi_test:4.2f}\n'
             tmp_str += f'Confidence level Tau-test: {confidence_level_tau_test:4.2f}\n'
             tmp_str += f'\n'
-            tmp_str += f'---- Set up and populate matrices ----\n'
+            tmp_str += f'---- Survey infos ----\n'
+            tmp_str += self.survey_info_string
+            tmp_str += f'\n'
+            tmp_str += f'\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # Initialize matrices:
+        if verbose or self.write_log:
+            tmp_str = f'---- Set up and populate matrices ----\n'
+            if verbose:
+                print(tmp_str)
+            if self.write_log:
+                self.log_str += tmp_str
         # => Initialize complete matrices first and then populate them. This is most efficient!
         # - Observation model:
         mat_A0 = np.zeros([number_of_observations, number_of_parameters])  # Model-matrix
         mat_L0 = np.zeros((number_of_observations, 1))
         mat_sig_ll0 = np.zeros(number_of_observations)
         # - Constraints:
         mat_Ac = np.zeros([number_of_datum_stations, number_of_parameters])  # Model-matrix for constraints
@@ -371,15 +380,15 @@
         mat_L = np.vstack((mat_L0, mat_Lc))  # Eq. (16)
         mat_sig_ll = np.diag(np.hstack((mat_sig_ll0, mat_sig_llc)))
         mat_Qll = mat_sig_ll / (sig0_mugal**2)
         mat_P = np.linalg.inv(mat_Qll)
 
         if verbose or self.write_log:
             tmp_str = f'\n'
-            tmp_str += f'---- Solve equation system: Results and statistics ----\n'
+            tmp_str += f'---- Results and statistics ----\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # Solve equation system:
         mat_N = mat_A.T @ mat_P @ mat_A  # Normal equation matrix
```

### Comparing `grav-toolbox-0.2.2/gravtools/models/misc.py` & `grav-toolbox-0.2.3/gravtools/models/misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/models/mlr_bev_legacy.py` & `grav-toolbox-0.2.3/gravtools/models/mlr_bev_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,18 @@
         Notes
         -----
         Only one drift polynomial is adjusted in the input data! Hence, it might be problematic to use observations
         of multiple surveys that were taken over a longer time period.
         """
 
         # ##### 1.) Initial preparations #####
+        if len(self.setups) > 1:
+            raise RuntimeError(f'The current campaign contains {len(self.setups)} active surveys. The "MLR" method'
+                               f'only supports the adjustment of single surveys. Use a different adjustment method or '
+                               f'adjust all surveys individually.')
 
         # - Observations and parameters:
         all_setups_df = None
         observed_stations = []
         survey_names = []
         number_of_observations = 0
         setup_ids = []
@@ -183,14 +187,18 @@
             tmp_str += f'Number of surveys: {number_of_surveys}\n'
             tmp_str += f'Number of stations: {number_of_stations}\n'
             tmp_str += f'Number of observations: {number_of_observations}\n'
             # tmp_str += f'Number of estimated parameters: {number_of_parameters}\n'  # obsolet
             # tmp_str += f'Number of datum stations: {number_of_datum_stations}\n'  # ????????????????????ß
             # tmp_str += f'Degree of freedom: {number_of_diff_obs - number_of_parameters}\n'  # obsolet
             tmp_str += f'\n'
+            tmp_str += f'---- Survey infos ----\n'
+            tmp_str += self.survey_info_string
+            tmp_str += f'\n'
+            tmp_str += f'\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # Get dataframe with subset of observed stations only:
         filter_tmp = self.stat_df['station_name'].isin(observed_stations)
```

### Comparing `grav-toolbox-0.2.2/gravtools/models/station.py` & `grav-toolbox-0.2.3/gravtools/models/station.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/models/survey.py` & `grav-toolbox-0.2.3/gravtools/models/survey.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 import os
 
 import gravtools.models.lsm_diff
 import gravtools.tides.longman1959
 from gravtools.settings import SURVEY_DATA_SOURCE_TYPES, TIDE_CORRECTION_TYPES, DEFAULT_GRAVIMETER_TYPE_CG5_SURVEY, \
     REFERENCE_HEIGHT_TYPE, BEV_GRAVIMETER_TIDE_CORR_LOOKUP, GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m, \
     GRAVIMETER_SERIAL_NUMBERS, GRAVIMETER_TYPES, GRAVIMETER_SERIAL_NUMBER_TO_ID_LOOKUPTABLE, SETUP_CALC_METHODS, \
-    UNIT_CONVERSION_TO_MUGAL, SETUP_SD_METHODS
+    UNIT_CONVERSION_TO_MUGAL, SETUP_SD_METHODS, ATM_PRES_CORRECTION_TYPES, ATM_PRES_CORRECTION_ADMITTANCE_DEFAULT
 from gravtools.const import VG_DEFAULT
 from gravtools.CG5_utils.cg5_survey import CG5Survey
 from gravtools.models.misc import format_seconds_to_hhmmss
 from gravtools.tides.correction_time_series import convert_to_mugal
+from gravtools.models import atmosphere_correction
 
 
 class Survey:
     """Gravity survey (instrument-independent).
 
     A gravity survey object contains all data that belongs to a single field observation job, carried out under the
     same circumstances (same instrument, measurement area, drift- and datum-point planing, same observer, etc.). A
@@ -88,22 +89,30 @@
         Type of the tidal corrections applied on the observations (gravimeter readings as obtained from the data
         source; column `g_obs_mugal` in `obs_df`). Valid entries have to be listed in
         :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`.
     obs_reference_height_type : str, (default='')
         Reference level type of the observations (gravimeter readings as obtained from the data
         source; column `g_obs_mugal` in `obs_df`). Valid entries have to be listed in
         :py:obj:`gravtools.settings.REFERENCE_HEIGHT_TYPE`.
+    obs_atm_pres_correction_type : str, (default='')
+        Type of atmospheric pressure correction applied on the observations (gravimeter readings as obtained from the
+        data source; column `g_obs_mugal` in `obs_df`). Valid entries have to be listed in
+        :py:obj:`gravtools.settings.ATM_PRES_CORRECTION_TYPES`.
     red_tide_correction_type : str, optional (default='')
         Type of the tidal corrections applied on the reduced observations (column `g_red_mugal` in `obs_df`). Valid
         entries have to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`. `Empty string`, if corrected
         observations are not available.
     red_reference_height_type : str, optional (default='')
         Reference level type of the reduced observations (column `g_red_mugal` in `obs_df`). Valid entries have to be
         listed in :py:obj:`gravtools.settings.REFERENCE_HEIGHT_TYPE`. `Empty string`, if corrected observations are not
         available.
+    red_atm_pres_correction_type : str, (default='')
+        Type of atmospheric pressure correction applied on the reduced (column `g_red_mugal` in `obs_df`). Valid entries
+         have to be listed in :py:obj:`gravtools.settings.ATM_PRES_CORRECTION_TYPES`. `Empty string`, if corrected
+        observations are not available.
     red_tide_correction_description : str, optional (default='')
         Optional description of the tide correction e.g. obtained from time series data. The reduced observations are
         stored in the column `g_red_mugal` and the corrections in column `corr_tide_red_mugal` in `obs_df`. Only
     red_tide_corr_timeseries_interpol_method : str, optional (default='')
         Interpolation method used to calculate tidal corrections from time series data. If tidal corrections are
         obtained from other sources or models, this attribute is irrelevant and has to be empty!
     red_tide_corr_timeseries_creation_dt : `datetime`, optional (default=`None`)
@@ -114,15 +123,19 @@
         Type of the tidal corrections applied on the observations that are used to calculate the setup data in the
         `setup_df` dataframe. Valid entries have to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`.
         `Empty string`, if corrected setup data has not been calculated so far (`setup_df` = None).
     setup_reference_height_type : str, optional (default='')
         Reference height reduction type applied on the observations that are used to calculate the setup data in the
         `setup_df` dataframe. Valid entries have to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`.
         `Empty string`, if corrected setup data has not been calculated so far (`setup_df` = None).
-    setup_calc_method : str, optional (default='')
+    setup_atm_pres_correction_type : str, (default='')
+        Type of atmospheric pressure correction applied on the observations that are used to calculate the setup data in
+        the`setup_df` dataframe. Valid entries have to be listed in
+        :py:obj:`gravtools.settings.ATM_PRES_CORRECTION_TYPES`.`Empty string`, if corrected setup data has not been
+        calculated so far (`setup_df` = None).
         Method for the calculation of setup data. `variance_weighted_mean` implies that setup observations
         (observed gravity, standard deviations and reference time) are calculated by variance weighted mean of the
         individual observations. `individual_obs` implies that the original observations are used as setup data
         without any aggregation.
     setup_sd_method : str, optional (default='')
         Method for the determination of standard deviations (SD) of setup observations. `sd_from_obs_file` implies that
         SD are taken from the observation file. `sd_default_per_obs` and `sd_default_per_setup` imply that the
@@ -166,20 +179,21 @@
             and/or reductions may have been applied already! The reference height type and the applied tidal correction
             have to be concise with the statements in :py:obj:`.Survey.obs_reference_height_type` and
             :py:obj:`.Survey.obs_tide_correction_type`, respectively.
         - sd_g_obs_mugal : float, optional (default=None)
             Standard deviation of `g_obs_mugal`. If `None`, the standard deviation is not available.
         - g_red_mugal : float, optional (default=None)
             Reduced gravity observation. This value is derived from the observed gravimeter reading (`g_obs_mugal`) by
-            applying reductions and corrections, e.g. from analytical models for tidal effects, or by a reduction to a
-            different height level (using the vertical gravity gradient). Take care, that the same  reductions and
-            corrections are not applied more than once! The reference height type and the applied tidal correction
-            have to be concise with the statements in :py:obj:`.Survey.red_reference_height_type` and
-            :py:obj:`.Survey.red_tide_correction_type`, respectively. If `None`, no reductions and/or corrections have
-            been applied so far.
+            applying reductions and corrections, e.g. from analytical models for tidal effects, by a reduction to a
+            different height level (using the vertical gravity gradient), or reduction due to atmospheric pressure
+            variations. Take care, that the same  reductions and corrections are not applied more than once! The
+            reference height type, the applied tidal correction and the applied atmospheric pressure corrections
+            have to be concise with the statements in :py:obj:`.Survey.red_reference_height_type`,
+            :py:obj:`.Survey.red_tide_correction_type` and :py:obj:`.Survey.red_atm_pres_correction_type`, respectively.
+            If `None`, no reductions and/or corrections have been applied so far.
         - sd_g_red_mugal : float, optional (default=None)
             Standard deviation of the reduced gravity reading (`g_red_mugal`). This value is derived from the standard
             deviation of the gravity reading (`sd_g_obs_mugal`) by applying proper error propagation. If `None`, the SD
             of the gravity reading is not available, or no reductions/corrections have been applied so far, or an error
             propagation model is still missing. In general, this value should not be `None`, if `g_red_mugal` is not
             `None`.
         - corr_terrain : float, optional (default=None)
@@ -212,14 +226,20 @@
         - vg_mugalm : float, optional (default=None)
             Vertical gravity gradient at the station [µGal/m], obtained from an external source (e.g. station info
             file). The vertical gradient is required for reducing the observed gravity to different reference heights.
         - corr_tide_red_mugal : float, optional (default=None)
             Tidal correction [µGal] that is applied to `g_red_mugal`.
         - duration_sec : int
             Duration of each observation from the CG-5 observation files. Given in seconds.
+        - atm_pres_hpa : float, optional (default=None)
+            Measured atmospheric pressure in hPa. Used for correcting atmospheric pressure variations.
+        - norm_atm_pres_hpa : float, optional (default=None)
+            Normal atmospheric pressure in hPa. Used for correcting atmospheric pressure variations.
+        - corr_atm_pres_red_mugal : float, optional (default=None)
+            Atmospheric pressurecorrection [µGal] that is applied to `g_red_mugal`.
 
     ref_delta_t_dt : datetime, optional (default=None)
         Reference time for relative times (), e.g. reference time t0 the for drift polynomial adjustment.
     setup_df : :py:obj:`pandas.core.frame.DataFrame`, optional (default=None)
         Contains a single pseudo observation per setup calculated as variance weighted mean of all active
         (flag `keep_obs = True`) reduced observations of a setup and other information that is required for the
         subsequent parameter adjustment. If `None`, setup data ha not been determined yet. All Columns are listed in
@@ -275,16 +295,32 @@
         'tilty',  # [arcsec], optional
         'dhf_m',  # Distance between instrument top and physical reference point (float) [m]
         'dhb_m',  # Distance between instrument top and ground (float) [m]
         'keep_obs',  # Remove observation, if false (bool)
         'vg_mugalm',  # vertical gradient [µGal/m]
         'corr_tide_red_mugal',  # Alternative tidal correction [µGal], optional
         'duration_sec',  # Duration [sec]
+        'atm_pres_hpa',  # Measured atmospheric pressure [hPa]
+        'norm_atm_pres_hpa',  # Normal atmospheric pressure [hPa]
+        'corr_atm_pres_red_mugal',  # Normal atmospheric pressure correction [µGal]
     )
 
+    _OBS_DF_INIT_COL_IF_MISSING = {
+        'atm_pres_hpa': np.nan,
+        'norm_atm_pres_hpa': np.nan,
+        'corr_atm_pres_red_mugal': np.nan,
+    }
+
+    _SURVEY_ATTRIBUTES_INIT = {
+        'setup_atm_pres_correction_type': '',
+        'obs_atm_pres_correction_type': 'no_atm_pres_corr',
+        'red_atm_pres_correction_type': '',
+        'red_tide_correction_description': '',
+    }
+
     _SETUP_DF_COLUMNS = (
         'station_name',  # Name of station (str)
         'setup_id',  # Unique ID of setup (int)
         'g_mugal',  # Variance weighted mean of all active observations in setup [µGal] (float)
         'sd_g_mugal',  # Standard deviation of `g_mugal` (float) [µGal]
         'epoch_unix',  # Reference epoch of `g_mugal` (unix time [sec])
         'epoch_dt',  # Reference epoch of `g_mugal` (datetime obj)
@@ -309,21 +345,24 @@
                  gravimeter_serial_number='',
                  gravimeter_type='',
                  data_file_name='',
                  data_file_type='',
                  obs_df=None,
                  obs_tide_correction_type='',  # of "g_obs_mugal"
                  obs_reference_height_type='',  # of "g_obs_mugal"
+                 obs_atm_pres_correction_type='',  # of "g_obs_mugal"
                  red_tide_correction_type='',  # of "g_red_mugal"
                  red_reference_height_type='',  # of "g_red_mugal"
+                 red_atm_pres_correction_type = '',  # of "g_red_mugal"
                  red_tide_correction_description='',  # of "g_red_mugal"
                  red_tide_corr_timeseries_interpol_method='',  # of "g_red_mugal"
                  red_tide_corr_timeseries_creation_dt=None,  # of "g_red_mugal"
                  setup_tide_correction_type='',
                  setup_reference_height_type='',
+                 setup_atm_pres_correction_type='',
                  setup_calc_method='',
                  setup_sd_method='',
                  keep_survey=True,  # Flag
                  setup_df=None,
                  ref_delta_t_dt=None,  # Datetime object (UTC)
                  setup_obs_list_df=None  #
                  ):
@@ -456,25 +495,25 @@
                                      '({})'.format(', '.join(REFERENCE_HEIGHT_TYPE.keys())))
             else:
                 self.obs_reference_height_type = obs_reference_height_type  # None
         else:
             raise TypeError('"obs_reference_height_type" needs to be a string')
 
         # red_reference_height_type:
-        if isinstance(red_tide_correction_type, str):
+        if isinstance(red_reference_height_type, str):
             if red_reference_height_type:
                 if red_reference_height_type in REFERENCE_HEIGHT_TYPE.keys():
                     self.red_reference_height_type = red_reference_height_type
                 else:
                     raise ValueError('"red_reference_height_type" needs to be a key in REFERENCE_HEIGHT_TYPE '
                                      '({})'.format(', '.join(REFERENCE_HEIGHT_TYPE.keys())))
             else:
                 self.red_reference_height_type = red_reference_height_type  # None
         else:
-            raise TypeError('"red_tide_correction_type" needs to be a string')
+            raise TypeError('"red_reference_height_type" needs to be a string')
 
         # red_tide_correction_description
         if isinstance(red_tide_correction_description, str):
             self.red_tide_correction_description = red_tide_correction_description
         else:
             raise TypeError('"red_tide_correction_description" needs to be a string')
 
@@ -486,14 +525,40 @@
 
         # red_tide_corr_timeseries_creation_dt
         if red_tide_corr_timeseries_creation_dt is not None:
             if not isinstance(red_tide_corr_timeseries_creation_dt, dt.datetime):
                 raise TypeError('`red_tide_corr_timeseries_creation_dt` needs to be a datetime object.')
         self.red_tide_corr_timeseries_creation_dt = red_tide_corr_timeseries_creation_dt
 
+        # obs_atm_pres_correction_type
+        if isinstance(obs_atm_pres_correction_type, str):
+            if obs_atm_pres_correction_type:
+                if obs_atm_pres_correction_type in ATM_PRES_CORRECTION_TYPES.keys():
+                    self.obs_atm_pres_correction_type = obs_atm_pres_correction_type
+                else:
+                    raise ValueError('"obs_atm_pres_correction_type" needs to be a key in ATM_PRES_CORRECTION_TYPES '
+                                     '({})'.format(', '.join(ATM_PRES_CORRECTION_TYPES.keys())))
+            else:
+                self.obs_atm_pres_correction_type = obs_atm_pres_correction_type  # None
+        else:
+            raise TypeError('"obs_atm_pres_correction_type" needs to be a string')
+
+        # red_atm_pres_correction_type
+        if isinstance(red_atm_pres_correction_type, str):
+            if red_atm_pres_correction_type:
+                if red_atm_pres_correction_type in ATM_PRES_CORRECTION_TYPES.keys():
+                    self.red_atm_pres_correction_type = red_atm_pres_correction_type
+                else:
+                    raise ValueError('"red_atm_pres_correction_type" needs to be a key in ATM_PRES_CORRECTION_TYPES '
+                                     '({})'.format(', '.join(ATM_PRES_CORRECTION_TYPES.keys())))
+            else:
+                self.red_atm_pres_correction_type = red_atm_pres_correction_type  # None
+        else:
+            raise TypeError('"red_atm_pres_correction_type" needs to be a string')
+
         # setup_tide_correction_type:
         if isinstance(setup_tide_correction_type, str):
             if setup_tide_correction_type:
                 if setup_tide_correction_type in REFERENCE_HEIGHT_TYPE.keys():
                     self.setup_tide_correction_type = setup_tide_correction_type
                 else:
                     raise ValueError('"setup_tide_correction_type" needs to be a key in REFERENCE_HEIGHT_TYPE '
@@ -512,14 +577,27 @@
                     raise ValueError('"setup_reference_height_type" needs to be a key in REFERENCE_HEIGHT_TYPE '
                                      '({})'.format(', '.join(REFERENCE_HEIGHT_TYPE.keys())))
             else:
                 self.setup_reference_height_type = setup_reference_height_type  # ''
         else:
             raise TypeError('"setup_reference_height_type" needs to be a string')
 
+        # setup_atm_pres_correction_type:
+        if isinstance(setup_atm_pres_correction_type, str):
+            if setup_atm_pres_correction_type:
+                if setup_atm_pres_correction_type in ATM_PRES_CORRECTION_TYPES.keys():
+                    self.setup_atm_pres_correction_type = setup_atm_pres_correction_type
+                else:
+                    raise ValueError('"setup_atm_pres_correction_type" needs to be a key in ATM_PRES_CORRECTION_TYPES '
+                                     '({})'.format(', '.join(ATM_PRES_CORRECTION_TYPES.keys())))
+            else:
+                self.setup_atm_pres_correction_type = setup_atm_pres_correction_type  # ''
+        else:
+            raise TypeError('"setup_atm_pres_correction_type" needs to be a string')
+
         # setup_calc_method:
         if isinstance(setup_calc_method, str):
             if setup_calc_method:
                 if setup_calc_method in SETUP_CALC_METHODS.keys():
                     self.setup_calc_method = setup_calc_method
                 else:
                     raise ValueError('"setup_calc_method" needs to be a key in SETUP_CALC_METHODS '
@@ -673,16 +751,18 @@
                    gravimeter_type=DEFAULT_GRAVIMETER_TYPE_CG5_SURVEY,
                    gravimeter_serial_number=cg5_survey.survey_parameters.instrument_sn,
                    data_file_name=os.path.split(cg5_survey.obs_filename)[1],  # Filename only, without path
                    data_file_type='cg5_obs_file_txt',
                    obs_df=obs_df,
                    obs_tide_correction_type=obs_tide_correction_type,
                    obs_reference_height_type='sensor_height',
+                   obs_atm_pres_correction_type='no_atm_pres_corr',
                    red_tide_correction_type='',  # Not specified
                    red_reference_height_type='',  # Not specified
+                   red_atm_pres_correction_type='',  # Not specified
                    keep_survey=keep_survey,
                    )
 
     @classmethod
     def from_cg5_obs_file(cls, filename, keep_survey=True):
         """Constructor that generates and populates the survey object directly from a CG5 observation file.
 
@@ -831,32 +911,44 @@
                    gravimeter_type=gravimeter_type,
                    gravimeter_serial_number=gravimeter_serial_number,
                    data_file_name=os.path.split(filename)[1],  # Filename only, without path
                    data_file_type='bev_obs_file',
                    obs_df=obs_df,
                    obs_tide_correction_type=obs_tide_correction_type,
                    obs_reference_height_type='sensor_height',
+                   obs_atm_pres_correction_type='no_atm_pres_corr',
                    red_tide_correction_type='',  # Not specified
                    red_reference_height_type='',  # Not specified
+                   red_atm_pres_correction_type='',  # Not specified
                    keep_survey=keep_survey,
                    )
 
     @classmethod
     def _obs_df_drop_columns(cls, obs_df):
         """Drop all columns of obs_df that are not listed in cls._OBS_DF_COLUMNS"""
         columns_to_be_dropped = list(set(obs_df.columns) - set(cls._OBS_DF_COLUMNS))
         obs_df.drop(columns=columns_to_be_dropped, inplace=True)
         return obs_df
 
     @classmethod
     def _obs_df_add_columns(cls, obs_df):
-        """Add and initialize (as None) all columns that are listed in cls._OBS_DF_COLUMNS and not present in input
-        obs_df."""
+        """Add and initialize all columns that are listed in cls._OBS_DF_COLUMNS and not present in input obs_df.
+
+        Notes
+        -----
+        Columns are initialized with the value `None`, if they are not a key in `cls._OBS_DF_INIT_COL_IF_MISSING`.
+        Otherwise, they are initialized with the according value in `cls._OBS_DF_INIT_COL_IF_MISSING`. This provides
+        the option to initialize columns with specific values, other than `None`, if required.
+        """
         columns_to_be_initialized_as_none = list(set(cls._OBS_DF_COLUMNS) - set(obs_df.columns))
         obs_df[columns_to_be_initialized_as_none] = None
+        cols_with_init_value = list(
+            set(cls._OBS_DF_INIT_COL_IF_MISSING.keys()).intersection(set(columns_to_be_initialized_as_none)))
+        for cols_name in cols_with_init_value:
+            obs_df[cols_name] = cls._OBS_DF_INIT_COL_IF_MISSING[cols_name]
         return obs_df
 
     @classmethod
     def _obs_df_reorder_columns(cls, obs_df):
         """Change order of columns of obs_df to the order specified in cls._OBS_DF_COLUMNS.
 
         See: https://erikrood.com/Python_References/change_order_dataframe_columns_final.html
@@ -900,48 +992,92 @@
             Index of the observation within the observation dataframe (`obs_df`) that will be activated or deactivated.
         flag_activate : bool
             Specified whether the observation with the index `obs_idx` will be activated (`TRUE`) or deactivated
             (`False`).
         """
         self.obs_df.at[obs_idx, 'keep_obs'] = flag_activate
 
-    def is_valid_obs_df(self, verbose=False) -> bool:
-        """Check, whether the observations DataFrame (`obs_df`) is valid.
+    def check_obs_df(self, verbose=True) -> bool:
+        """Check, whether the observations DataFrame (`obs_df`) is valid and try to add missing columns.
 
         This method carried out the following checks:
 
         - Check the columns as specified in :py:obj:`.Survey._OBS_DF_COLUMNS`?
 
           - Does `obs_df` have all required columns?
 
+          - If columns defined in :py:obj:`.Survey._OBS_DF_INIT_COL_IF_MISSING` are missing, they are added with the
+            defined initial value.
+
         Parameters
         ----------
         verbose : bool, optional (default=False)
-            If True, messages are printed that indicate why `obs_df` is not valid in case.
+            If True, messages are printed in the command line interface.
 
         Returns
         -------
-        bool
+        is_valid : bool
             True, if `obs_df` is valid.
+        error_msg : str
+            Error Message. Empty if no errors occured.
         """
         is_valid = True
+        error_msg = ''
 
+        # Invalid columns?
         invalid_cols = list(set(self.obs_df.columns) - set(self._OBS_DF_COLUMNS))
         if len(invalid_cols) > 0:
             is_valid = False
+            error_msg = f'The following columns in the observation dataframe of survey "{self.name}" are not valid: {", ".join(invalid_cols)}. '
             if verbose:
-                print(f'The following columns are not valid: {", ".join(invalid_cols)}')
+                print(error_msg)
 
+        # Missing columns?
         invalid_cols = list(set(self._OBS_DF_COLUMNS) - set(self.obs_df.columns))
         if len(invalid_cols) > 0:
-            is_valid = False
-            if verbose:
-                print(f'The following columns are missing: {", ".join(invalid_cols)}')
+            # Add columns with the default values, if defined in _OBS_DF_INIT_COL_IF_MISSING:
+            for invalid_col in invalid_cols:
+                if invalid_col in self._OBS_DF_INIT_COL_IF_MISSING:
+                    self.obs_df[invalid_col] = self._OBS_DF_INIT_COL_IF_MISSING[invalid_col]
+                    if verbose:
+                        print(f'Added column "{invalid_col}" with default value "'
+                              f'{self._OBS_DF_INIT_COL_IF_MISSING[invalid_col]}" in observation dataframe of survey "'
+                              f'{self.name}".')
+            # Check again:
+            self.obs_df = self._obs_df_reorder_columns(self.obs_df)
+            invalid_cols = list(set(self._OBS_DF_COLUMNS) - set(self.obs_df.columns))
+            if len(invalid_cols) > 0:
+                is_valid = False
+                error_msg_tmp = (f'The following columns in the observation dataframe of survey "'
+                                 f'{self.name}" are missing: {", ".join(invalid_cols)}. ')
+                error_msg = error_msg + error_msg_tmp
+                if verbose:
+                    print(error_msg_tmp)
 
-        return is_valid
+        return is_valid, error_msg
+
+    def init_missing_attributes(self, verbose=True) -> bool:
+        """Initialize attributes defined in `_SURVEY_ATTRIBUTES_INIT`, if they are missing the current Survey instance.
+
+        Notes
+        -----
+        This method is useful to establish downward compatibility between the current GravTools version and campaign
+        data (pkl files) created/saved with previous version.
+
+        Parameters
+        ----------
+        verbose : bool, optional (default=False)
+            If True, messages are printed in the command line interface.
+        """
+        attributes = dir(self)
+        for attribute, init_value in self._SURVEY_ATTRIBUTES_INIT.items():
+            if attribute not in attributes:
+                setattr(self, attribute, init_value)
+                if verbose:
+                    print(f'Added attribute "{attribute}" (init. value: "{init_value}") to Survey object of survey "{self.name}".')
 
     def obs_df_drop_redundant_columns(self):
         """Drop all columns of obs_df that are not listed in self._OBS_DF_COLUMNS"""
         columns_to_be_dropped = list(set(self.obs_df.columns) - set(self._OBS_DF_COLUMNS))
         self.obs_df.drop(columns=columns_to_be_dropped, inplace=True)
 
     @classmethod
@@ -1026,20 +1162,24 @@
                                         how='left', suffixes=('_x', ''))
 
         # Populate all missing VGs with the default value:
         self.obs_df.loc[self.obs_df['vg_mugalm'].isna(), 'vg_mugalm'] = VG_DEFAULT
 
         # Drop columns that are not required and check for validity:
         self.obs_df_drop_redundant_columns()
-        if not self.is_valid_obs_df():
-            raise AssertionError('The DataFrame "obs_df" is not valid.')
+        self.obs_df = self._obs_df_reorder_columns(self.obs_df)
+        valid_flag, error_msg = self.check_obs_df(verbose=True)
+        if not valid_flag:
+            raise RuntimeError(error_msg)
 
     def reduce_observations(self,
                             target_ref_height: str = None,
                             target_tide_corr: str = None,
+                            target_atm_pres_corr: str = None,
+                            atm_pres_admittance: float = ATM_PRES_CORRECTION_ADMITTANCE_DEFAULT,
                             tide_corr_timeseries_interpol_method = '',
                             correction_time_series=None,
                             verbose: bool = False,
                             ) -> [bool, str]:
         """Reduce the observed gravity values by applying the selected corrections.
 
         The following corrections can be applied:
@@ -1062,14 +1202,21 @@
         target_ref_height : string, specifying the target reference height type (default = `None`).
             The target reference height type has to be listed in :py:obj:`gravtools.settings.REFERENCE_HEIGHT_TYPE`.
             Default is `None` indicating that the reference heights of the input data are not changed.
         target_tide_corr : str, specifying the tidal correction type to be applied (default = `None`).
             The target tidal correction type specifies what kind of tidal correction will be applied. Valid types have
             to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`. Default is `None` indicating that the
             tidal corrections are not considered here (tidal corrections are inherited from input data).
+        target_atm_pres_corr : str, optional (default = `None`)
+            Specifying the atmospheric press ure correction type to be applied to all surveys. Valid types to be listed
+            in :py:obj:`gravtools.settings.ATM_PRES_CORRECTION_TYPES`. Default is `None` indicating that the respective
+            corrections of the input data are not changed.
+        atm_pres_admittance : float, optional (default = `settings.ATM_PRES_CORRECTION_ADMITTANCE_DEFAULT`)
+            Admittance factor for the determination of pressure corrections based on the difference between measured and
+            normal air pressure. The default value is taken from `settings.ATM_PRES_CORRECTION_ADMITTANCE_DEFAULT`.
         tide_corr_timeseries_interpol_method : str, optional (default='')
             Interpolation method used to calculate tidal corrections from time series data. If tidal corrections are
             obtained from other sources or models, this attribute is irrelevant and has to be empty!
         correction_time_series : `CorrectionTimeSeries` object, optional (default=None)
             Correction time series object that contains time series of tidal corrections for stations in surveys. This
             argument is required, if tidal corrections should be derived from time series data, i.e. if
             `self.target_tide_corr = from_time_series`.
@@ -1079,15 +1226,15 @@
         # Init.:
         tide_corr_timeseries_interpol_method_out = ''
 
         # Create a copy auf obs_df in order prevent problems with manipulation assigned py reference variables:
         obs_df = self.obs_df.copy(deep=True)
 
         # Initialize pandas series for reduced data by copying the observation data as loaded from the input file:
-        g_red_mugal = obs_df['g_obs_mugal']
+        g_red_mugal = obs_df['g_obs_mugal'].copy(deep=True)
         sd_g_red_mugal = obs_df['sd_g_obs_mugal']
 
         # Check whether field for reduced data are initialized correctly:
         flag_all_field_are_nan = all([obs_df['g_red_mugal'].isna().all(),
                                       obs_df['sd_g_red_mugal'].isna().all(),
                                       obs_df['corr_tide_red_mugal'].isna().all()
                                       ])
@@ -1195,25 +1342,25 @@
                         g_red_mugal = g_red_mugal - (obs_df['dhf_m'] + dst_m) * \
                                       obs_df['vg_mugalm']
                         # sd_g_red_mugal = sd_g_red_mugal  # Keep SD
                 if verbose:
                     print('...done!')
 
         # 2.) Check tidal corrections:
-        # Check if the target tidal correction type is valid:
-        if target_tide_corr not in TIDE_CORRECTION_TYPES:
-            error_msg = f'"{target_tide_corr}" is unknown ab invalid!'
-            raise RuntimeError(f'Survey "{self.name}":' + error_msg)
-        tide_correction_description = TIDE_CORRECTION_TYPES[target_tide_corr]
-        if verbose:
-            print(f'Tidal corrections "{target_tide_corr}" ({tide_correction_description}):')
         if target_tide_corr is None:  # Do nothing
             if verbose:
-                print(f' - Tidal corrections are not changed!')
+                print(f'Tidal corrections are not changed!')
         else:
+            # Check if the target tidal correction type is valid:
+            if target_tide_corr not in TIDE_CORRECTION_TYPES:
+                error_msg = f'"{target_tide_corr}" is invalid!'
+                raise RuntimeError(f'Survey "{self.name}":' + error_msg)
+            tide_correction_description = TIDE_CORRECTION_TYPES[target_tide_corr]
+            if verbose:
+                print(f'Tidal corrections "{target_tide_corr}" ({tide_correction_description}):')
             # Check if reduction is necessary and/or possible:
             # - If time series data is used, corrections have to be calculated anyway, because the time series
             #   may have changed since their last determination!
             if (self.obs_tide_correction_type == target_tide_corr) & (target_tide_corr != 'from_time_series'):
                 if verbose:
                     print(f' - Observations are already reduced by: {target_tide_corr}')
                 corr_tide_red_mugal = obs_df['corr_tide_mugal']
@@ -1269,22 +1416,78 @@
                         tide_corr_timeseries_interpol_method_out = tide_corr_timeseries_interpol_method
                 else:
                     raise RuntimeError(f'Tidal corrections of observation data ("{self.obs_tide_correction_type}") not '
                                        f'supported!')
                 if verbose:
                     print('...done!')
 
-            # Apply changes, if no exceptions were raised:
-            self.red_tide_correction_type = target_tide_corr
-            self.red_reference_height_type = target_ref_height
-            self.red_tide_correction_description = tide_correction_description
-            self.red_tide_corr_timeseries_interpol_method = tide_corr_timeseries_interpol_method_out
-            self.obs_df['g_red_mugal'] = g_red_mugal
-            self.obs_df['sd_g_red_mugal'] = sd_g_red_mugal
+        # 3.) Check atmospheric pressure corrections:
+        if target_atm_pres_corr is None:  # Do nothing
+            if verbose:
+                print(f'Atmospheric pressure corrections are not changed!')
+        else:
+            # Check if the target correction type is valid:
+            if target_atm_pres_corr not in ATM_PRES_CORRECTION_TYPES:
+                error_msg = f'"{target_atm_pres_corr}" is invalid!'
+                raise RuntimeError(f'Survey "{self.name}":' + error_msg)
+            if verbose:
+                print(f'Atmospheric pressure corrections "{target_atm_pres_corr}" ({ATM_PRES_CORRECTION_TYPES[target_atm_pres_corr]}):')
+
+            # Check, if an admittance factor is available:
+            if atm_pres_admittance is None:
+                error_msg = (f'The admittance factor for the determination of atmospheric pressure corrections is not'
+                             f'available (is None).')
+                raise RuntimeError(f'Survey "{self.name}":' + error_msg)
+
+            if self.obs_atm_pres_correction_type == 'no_atm_pres_corr':
+                if target_atm_pres_corr == 'no_atm_pres_corr':
+                    corr_atm_pres_red_mugal = None
+                    norm_atm_pres_hpa = None
+                if target_atm_pres_corr == 'iso_2533_1975':
+                    height_m = obs_df['alt_m']
+                    atm_pres_hpa = obs_df['atm_pres_hpa']
+                    corr_atm_pres_red_mugal, norm_atm_pres_hpa = atmosphere_correction.pressure_correction_iso_pandas_series(height_m,
+                                                                                                                             atm_pres_hpa,
+                                                                                                                             admittance=atm_pres_admittance)
+                    # Apply non-NaN values only:
+                    tmp_filter = ~corr_atm_pres_red_mugal.isna()
+                    g_red_mugal.loc[tmp_filter] = g_red_mugal.loc[tmp_filter] - corr_atm_pres_red_mugal.loc[tmp_filter]  # TODO: sign correct?
+                    if verbose:
+                        num_with_p_corr = len(tmp_filter.loc[tmp_filter])
+                        number_of_obs = len(tmp_filter)
+                        if num_with_p_corr != number_of_obs:
+                            print(f'WARNING: Pressure corrections are available for {num_with_p_corr} of {number_of_obs} observations in survey {self.name} only, probably due to missing pressure observations.')
+
+            # This case should not be possible wit the current instruments since they are not capable to calculate
+            # atmospheric corrections and provide them along with the observation data in the input files!
+            # elif self.obs_atm_pres_correction_type == 'iso_2533_1975':
+            #     # Undo the corrections...
+            #     if target_atm_pres_corr == 'no_atm_pres_corr':
+            #         corr_atm_pres_red_mugal = 0
+
+            else:
+                raise RuntimeError(f'Atmosphere pressure corrections of observation data '
+                                   f'("{self.obs_atm_pres_correction_type}") not supported!')
+
+            if verbose:
+                print('...done!')
+
+        # 4.) Apply changes, if no exceptions were raised:
+        self.red_tide_correction_type = target_tide_corr
+        self.red_reference_height_type = target_ref_height
+        self.red_atm_pres_correction_type = target_atm_pres_corr
+        self.red_tide_correction_description = tide_correction_description
+        self.red_tide_corr_timeseries_interpol_method = tide_corr_timeseries_interpol_method_out
+        self.obs_df['g_red_mugal'] = g_red_mugal
+        self.obs_df['sd_g_red_mugal'] = sd_g_red_mugal
+        if target_tide_corr is not None:
             self.obs_df['corr_tide_red_mugal'] = corr_tide_red_mugal
+        if target_atm_pres_corr is not None:
+            self.obs_df['corr_atm_pres_red_mugal'] = corr_atm_pres_red_mugal
+            self.obs_df['norm_atm_pres_hpa'] = norm_atm_pres_hpa
 
     def get_tidal_corrections_from_timeseries(self, correction_time_series, interpolation_method : str) -> np.ndarray  :
         """Derives tidal corrections for observations from time series data.
 
         Notes
         -----
         The derived corrections have to be ADDED to the observations in order to reduce tidal effects!
@@ -1550,14 +1753,15 @@
                 print('Nothing to delete. Setup data is empty.')
         else:
             if verbose:
                 print('Setup data deleted.')
             self.setup_df = None
             self.setup_reference_height_type = ''
             self.setup_tide_correction_type = ''
+            self.setup_atm_pres_correction_type = '',
             self.setup_calc_method = ''
             self.setup_obs_list_df = None
 
     def calculate_setup_data(self, obs_type='reduced',
                              ref_delta_t_campaign_dt=None,
                              active_obs_only_for_ref_epoch=True,
                              method='variance_weighted_mean',
@@ -1746,17 +1950,19 @@
                 sd_setup_mugal_list = [np.nan] * len(g_mugal_list)
                 number_obs_list = [1] * len(g_mugal_list)
                 dhf_sensor_m_list = active_obs_df['dhf_m'] + GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m[self.gravimeter_type]
 
             if obs_type == 'observed':
                 self.setup_tide_correction_type = self.obs_tide_correction_type
                 self.setup_reference_height_type = self.obs_reference_height_type
+                self.setup_atm_pres_correction_type = self.obs_atm_pres_correction_type
             elif obs_type == 'reduced':
                 self.setup_tide_correction_type = self.red_tide_correction_type
                 self.setup_reference_height_type = self.red_reference_height_type
+                self.setup_atm_pres_correction_type = self.red_atm_pres_correction_type
             self.setup_calc_method = method
             self.setup_sd_method = method_sd
             self.create_setup_obs_list()
 
             if method_sd == 'sd_default_per_setup':
                 if verbose:
                     print(f'Use a default SD of {default_sd_mugal} µGal for all setup observations.')
@@ -1839,15 +2045,15 @@
         if self.obs_df is not None:
             return self.obs_df['obs_epoch'].max().strftime('%H:%M:%S')
         else:
             return ''
 
     @property
     def duration_hhmmss_str(self):
-        """Returns the timespan (Timedalta) between first and last observation in the survey in hh:mm:ss format."""
+        """Returns the timespan (Timedelta) between first and last observation in the survey in hh:mm:ss format."""
         if self.obs_df is not None:
             duration = self.obs_df['obs_epoch'].max() - self.obs_df['obs_epoch'].min()
             if duration.days == 0:
                 return format_seconds_to_hhmmss(duration.seconds)
             else:
                 return f'{duration.days}d ' + format_seconds_to_hhmmss(duration.seconds)
         else:
@@ -1871,10 +2077,8 @@
 
     @property
     def observed_stations_str(self):
         """Returns a string with a list of all stations observed in this survey."""
         if self.obs_df is not None:
             return f', '.join(self.observed_stations)
         else:
-            return None
-
-
+            return None
```

### Comparing `grav-toolbox-0.2.2/gravtools/models/vg_lsm.py` & `grav-toolbox-0.2.3/gravtools/models/vg_lsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,21 +288,30 @@
             tmp_str += f'Degree of drift polynomial: {drift_pol_degree}\n'
             tmp_str += f'Degree of VG polynomial: {vg_polynomial_degree}\n'
             tmp_str += f'VG polynomial height offset [m]: {vg_polynomial_ref_height_offset_m:4.3f}\n'
             tmp_str += f'A priori std. deviation of unit weight [µGal]: {sig0_mugal}\n'
             tmp_str += f'Confidence level Chi-test: {confidence_level_chi_test:4.2f}\n'
             tmp_str += f'Confidence level Tau-test: {confidence_level_tau_test:4.2f}\n'
             tmp_str += f'\n'
-            tmp_str += f'---- Set up and populate matrices ----\n'
+            tmp_str += f'---- Survey infos ----\n'
+            tmp_str += self.survey_info_string
+            tmp_str += f'\n'
+            tmp_str += f'\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # Initialize matrices:
+        if verbose or self.write_log:
+            tmp_str = f'---- Set up and populate matrices ----\n'
+            if verbose:
+                print(tmp_str)
+            if self.write_log:
+                self.log_str += tmp_str
         # => Initialize complete matrices first and then populate them. This is most efficient!
         # - Observation model:
         mat_A = np.zeros([number_of_observations, number_of_parameters])  # Design matrix
         mat_L = np.zeros((number_of_observations, 1))  # Observations
         mat_sig_ll = np.zeros(number_of_observations)  # Variances of obs.
 
         # Populate matrices:
@@ -379,15 +388,15 @@
         # Set up all required matrices:
         mat_sig_ll = np.diag(mat_sig_ll)
         mat_Qll = mat_sig_ll / (sig0_mugal ** 2)
         mat_P = np.linalg.inv(mat_Qll)
 
         if verbose or self.write_log:
             tmp_str = f'\n'
-            tmp_str += f'---- Solve equation system: Results and statistics ----\n'
+            tmp_str += f'---- Results and statistics ----\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # Solve equation system:
         mat_N = mat_A.T @ mat_P @ mat_A  # Normal equation matrix
```

### Comparing `grav-toolbox-0.2.2/gravtools/scripts/__init__.py` & `grav-toolbox-0.2.3/gravtools/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/scripts/create_correction_time_seriens_from_tsf.py` & `grav-toolbox-0.2.3/gravtools/scripts/create_correction_time_seriens_from_tsf.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/scripts/load_tfs_file.py` & `grav-toolbox-0.2.3/gravtools/scripts/load_tfs_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/scripts/run_gui.py` & `grav-toolbox-0.2.3/gravtools/scripts/run_gui.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/settings.py` & `grav-toolbox-0.2.3/gravtools/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,22 @@
     'cg5_longman1959': 'Instrument-implemented tidal correction of the Scintrex CG-5',
     'longman1959': 'Tidal corrections by the model of Longman (1959)',
     'no_tide_corr': 'No tide correction applied',
     'from_time_series': 'Interpolated from correction time series',
     'unknown': 'Unknown whether a tide correction was applied',
 }
 
+ATM_PRES_CORRECTION_TYPES = {
+    'no_atm_pres_corr': 'No atmospheric pressure correction applied',
+    'iso_2533_1975': 'Atmopheric pressure correction using ISO 2533:1975 normal air pressure',
+}
+
+# Default admittance factor for the calculation of atmospheric pressure correction using the ISO 2533:1975 normal air pressure
+ATM_PRES_CORRECTION_ADMITTANCE_DEFAULT = 0.3
+
 # Conversion factors of different units of gravity to µGal:
 # - Keys: Units as used e.g. in TSF files by Tsoft
 # - Values: Multiplicative conversion factors to µGal
 UNIT_CONVERSION_TO_MUGAL = {
     'nm/s^2': 1e-1  # 1 nm/s^2 * 0.1 = 1 µGal
 }
```

### Comparing `grav-toolbox-0.2.2/gravtools/tides/__init__.py` & `grav-toolbox-0.2.3/gravtools/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/tides/correction_time_series.py` & `grav-toolbox-0.2.3/gravtools/tides/correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/tides/longman1959.py` & `grav-toolbox-0.2.3/gravtools/tides/longman1959.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,28 +85,30 @@
 def calculate_julian_century(dates: Union[np.ndarray, pd.DatetimeIndex]):
     """
     Calculate the decimal Julian century and floating point hour, as referenced from
     1899, December 31 at 12:00:00
     This function accepts either a numpy ndarray or pandas DatetimeIndex as input,
     and returns a 2-tuple of the corresponding Julian century decimals and floating
     point hours.
+
     Parameters
     ----------
     dates : Union[np.ndarray, pd.DatetimeIndex]
         1-dimensional array of DateTime objects to convert into
         century/hours arrays
+
     Notes
     -----
-    All DateTimes should be supplied as UTC values, using a timezone-naive DateTime object
+    All DateTimes should be supplied as UTC values, using a timezone-naive DateTime object.
     This can be accomplished either by using datetime.utcnow(), or by constructing datetime
     objects where the times are specified as UTC values
     Reference Date: 1899 December 31 12:00:00
-    Reference ordinal: 693961.5 (MATLAB Serial date from January 0, 0000)
-        Delta 366 days
+    Reference ordinal: 693961.5 (MATLAB Serial date from January 0, 0000) Delta 366 days
     Reference ordinal: 694327.5 (Python ordinal from January 1, 0001)
+
     Returns
     -------
     2-tuple of:
         T : np.ndarray
             Number of Julian centuries (36525 days) from GMT Noon on
             December 31, 1899
         t0 : np.ndarray
@@ -128,24 +130,26 @@
     """
     Find the total gravity correction due to the Sun/Moon for the given
     latitude, longitude, altitude, and time - supplied as numpy 1-d arrays.
     Corrections are calculated for each corresponding set of data in the
     supplied arrays, all arrays must be of the same shape (length and dimension)
     This function returns the Lunar, Solar, and Total gravity corrections as
     a 3-tuple of numpy 1-d arrays.
+
     Parameters
     ----------
     lat : np.ndarray
         1-dimensional array of float values denoting latitudes
     lon : np.ndarray
         1-dimensional array of float values denoting longitudes
     alt : np.ndarray
         1-dimensional array of float values denoting altitude in meters
     time : np.ndarray
         1-dimensional array of DateTime objects denoting the time series
+
     Returns
     -------
     3-Tuple
         gMoon (gm): Vertical component of tidal acceleration due to the moon
         gSun (gs): Vertical component of tidal acceleration due to the sun
         gTotal (g0): Total vertical component of tidal acceleration (moon + sun)
     """
@@ -288,14 +292,15 @@
 
 def solve_point_corr(lat: float, lon: float, alt: float, t0=datetime.utcnow(), n=3600, increment='S'):
     """
     Utility function to generate a tide correction DataFrame for a static lat/lon/alt given start time t0,
     an increment, and count (n) of datapoints to generate.
     Default parameters are supplied that will generate a correction series with one second increment over a one hour
     period, with start time being the time of execution.
+
     Parameters
     ----------
     lat : float
         Latitude in decimal degrees
     lon : float
         Longitude in decimal degrees
     alt : float
@@ -303,21 +308,23 @@
     t0 : DateTime
         Starting date/time
     n : int
         Number of data points to generate
     increment : String
         Increment between data points, uses Pandas offset aliases:
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Timedelta.html#pandas.Timedelta
+
         Common options:
-            H : Hourly Frequency
-            T, min : Minutely frequency
-            S : Secondly frequency
-            L, ms : millisecond frequency
-            U, us : microsecond frequency
-            N : nanosecond frequency
+            * H : Hourly Frequency
+            * T, min : Minutely frequency
+            * S : Secondly frequency
+            * L, ms : millisecond frequency
+            * U, us : microsecond frequency
+            * N : nanosecond frequency
+
     Returns
     -------
     df : pd.DataFrame
         DataFrame (index=DateTime, lat, lon, alt, gm, gs, g0) shape: (n, 4)
         Pandas DataFrame indexed by DateTime containing the latitude, longitude, altitude, lunar, solar,
         and total corrections.
     Notes
```

### Comparing `grav-toolbox-0.2.2/gravtools/tides/tide_data.py` & `grav-toolbox-0.2.3/gravtools/tides/tide_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/gravtools/tides/tide_data_tfs.py` & `grav-toolbox-0.2.3/gravtools/tides/tide_data_tfs.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.2/setup.cfg` & `grav-toolbox-0.2.3/setup.cfg`

 * *Files identical despite different names*

