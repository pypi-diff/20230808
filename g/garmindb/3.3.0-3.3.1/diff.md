# Comparing `tmp/garmindb-3.3.0.tar.gz` & `tmp/garmindb-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garmindb-3.3.0.tar", last modified: Sat Feb 25 12:59:40 2023, max compression
+gzip compressed data, was "garmindb-3.3.1.tar", last modified: Tue Aug  8 11:08:53 2023, max compression
```

## Comparing `garmindb-3.3.0.tar` & `garmindb-3.3.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.603058 garmindb-3.3.0/
--rw-r--r--   0 tgoetz     (501) staff       (20)    18092 2020-02-08 21:26:46.000000 garmindb-3.3.0/LICENSE
--rw-r--r--   0 tgoetz     (501) staff       (20)       74 2021-12-02 23:58:59.000000 garmindb-3.3.0/MANIFEST.in
--rw-r--r--   0 tgoetz     (501) staff       (20)     7143 2023-02-25 12:59:40.602745 garmindb-3.3.0/PKG-INFO
--rw-r--r--   0 tgoetz     (501) staff       (20)     6614 2022-07-24 19:28:30.000000 garmindb-3.3.0/README.md
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.583967 garmindb-3.3.0/garmindb/
--rw-r--r--   0 tgoetz     (501) staff       (20)     1148 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/GarminConnectConfig.json.example
--rw-r--r--   0 tgoetz     (501) staff       (20)     1645 2022-07-24 19:28:30.000000 garmindb-3.3.0/garmindb/__init__.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      935 2021-12-02 23:58:59.000000 garmindb-3.3.0/garmindb/activities_fit_data.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    20102 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/activity_fit_file_processor.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2277 2021-12-02 23:58:59.000000 garmindb-3.3.0/garmindb/activity_fit_plugin_base.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)    12925 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/analyze.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     6224 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/checkup.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1889 2022-02-13 19:52:28.000000 garmindb-3.3.0/garmindb/config.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    10667 2022-02-13 19:52:28.000000 garmindb-3.3.0/garmindb/config_manager.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     2607 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/copy.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)    17683 2022-10-21 12:31:56.000000 garmindb-3.3.0/garmindb/download.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2480 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/export_activities.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2270 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/fit_data.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    12456 2022-07-24 19:28:30.000000 garmindb-3.3.0/garmindb/fit_file_processor.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.587506 garmindb-3.3.0/garmindb/fitbitdb/
--rw-r--r--   0 tgoetz     (501) staff       (20)      306 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/fitbitdb/__init__.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     3681 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/fitbitdb/analyze.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     7409 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/fitbitdb/fitbit_db.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     3479 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/fitbitdb/import_csv.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     4850 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/garmin_connect_config_manager.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    13883 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/garmin_connect_enums.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)    17610 2021-12-02 23:58:59.000000 garmindb-3.3.0/garmindb/garmin_json_data.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     7395 2021-12-02 23:58:59.000000 garmindb-3.3.0/garmindb/garmin_tcx_data.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.590455 garmindb-3.3.0/garmindb/garmindb/
--rw-r--r--   0 tgoetz     (501) staff       (20)      771 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/garmindb/__init__.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    22829 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/garmindb/activities_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    20819 2023-02-20 02:49:53.000000 garmindb-3.3.0/garmindb/garmindb/garmin_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     3877 2022-02-03 23:57:21.000000 garmindb-3.3.0/garmindb/garmindb/garmin_summary_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    11754 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/garmindb/monitoring_db.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)    10117 2022-02-03 23:57:21.000000 garmindb-3.3.0/garmindb/graphs.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)    17358 2022-10-21 12:31:56.000000 garmindb-3.3.0/garmindb/import_monitoring.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     3373 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/maps.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     5791 2022-10-21 12:31:56.000000 garmindb-3.3.0/garmindb/monitoring_fit_file_processor.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      735 2021-12-02 23:58:59.000000 garmindb-3.3.0/garmindb/monitoring_fit_plugin_base.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.592642 garmindb-3.3.0/garmindb/mshealthdb/
--rw-r--r--   0 tgoetz     (501) staff       (20)      343 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/mshealthdb/__init__.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     4005 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/mshealthdb/analyze.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     6079 2022-03-04 21:30:39.000000 garmindb-3.3.0/garmindb/mshealthdb/import_csv.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     8821 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/mshealthdb/mshealth_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      544 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/open_with_basecamp.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      546 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/open_with_google_earth.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      808 2021-12-02 23:58:59.000000 garmindb-3.3.0/garmindb/plugin_base.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1135 2021-12-02 23:58:59.000000 garmindb-3.3.0/garmindb/plugin_manager.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1960 2022-07-24 19:28:30.000000 garmindb-3.3.0/garmindb/sleep_fit_file_processor.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      640 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/statistics.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.594144 garmindb-3.3.0/garmindb/summarydb/
--rw-r--r--   0 tgoetz     (501) staff       (20)      294 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/summarydb/__init__.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     9702 2021-12-23 14:56:41.000000 garmindb-3.3.0/garmindb/summarydb/summary_base.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2303 2021-12-23 14:56:41.000000 garmindb-3.3.0/garmindb/summarydb/summary_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     4868 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/tcx.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      707 2021-06-27 22:56:11.000000 garmindb-3.3.0/garmindb/version.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      369 2023-02-25 12:48:56.000000 garmindb-3.3.0/garmindb/version_info.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.585568 garmindb-3.3.0/garmindb.egg-info/
--rw-r--r--   0 tgoetz     (501) staff       (20)     7143 2023-02-25 12:59:40.000000 garmindb-3.3.0/garmindb.egg-info/PKG-INFO
--rw-r--r--   0 tgoetz     (501) staff       (20)     2118 2023-02-25 12:59:40.000000 garmindb-3.3.0/garmindb.egg-info/SOURCES.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)        1 2023-02-25 12:59:40.000000 garmindb-3.3.0/garmindb.egg-info/dependency_links.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)      216 2023-02-25 12:59:40.000000 garmindb-3.3.0/garmindb.egg-info/requires.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)        9 2023-02-25 12:59:40.000000 garmindb-3.3.0/garmindb.egg-info/top_level.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)      104 2021-06-27 22:56:11.000000 garmindb-3.3.0/pyproject.toml
--rw-r--r--   0 tgoetz     (501) staff       (20)      216 2023-02-25 12:48:38.000000 garmindb-3.3.0/requirements.txt
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.597498 garmindb-3.3.0/scripts/
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     2222 2021-12-23 14:56:41.000000 garmindb-3.3.0/scripts/fitbit.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     1483 2022-01-31 22:32:22.000000 garmindb-3.3.0/scripts/garmindb_bug_report.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1699 2021-12-02 23:58:59.000000 garmindb-3.3.0/scripts/garmindb_checkup.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)    17404 2022-07-24 19:28:30.000000 garmindb-3.3.0/scripts/garmindb_cli.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     3316 2021-06-27 22:56:11.000000 garmindb-3.3.0/scripts/garmindb_graphs.py
--rwxr-xr-x   0 tgoetz     (501) staff       (20)     2300 2021-12-23 14:56:41.000000 garmindb-3.3.0/scripts/mshealth.py
--rw-r--r--   0 tgoetz     (501) staff       (20)       38 2023-02-25 12:59:40.603143 garmindb-3.3.0/setup.cfg
--rw-r--r--   0 tgoetz     (501) staff       (20)     2352 2022-01-31 22:32:22.000000 garmindb-3.3.0/setup.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:59:40.602356 garmindb-3.3.0/test/
--rw-r--r--   0 tgoetz     (501) staff       (20)     7013 2021-06-27 22:56:11.000000 garmindb-3.3.0/test/test_activities_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1718 2021-06-27 22:56:11.000000 garmindb-3.3.0/test/test_copy.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2060 2022-03-04 21:30:39.000000 garmindb-3.3.0/test/test_db_base.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    12870 2022-07-24 19:28:30.000000 garmindb-3.3.0/test/test_fit_file.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     5197 2022-07-24 19:28:30.000000 garmindb-3.3.0/test/test_garmin_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     5091 2021-06-27 22:56:11.000000 garmindb-3.3.0/test/test_garmin_db_objects.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      994 2022-03-04 21:30:39.000000 garmindb-3.3.0/test/test_garmin_summary_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     5300 2021-06-27 22:56:11.000000 garmindb-3.3.0/test/test_monitoring_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1237 2021-06-27 22:56:11.000000 garmindb-3.3.0/test/test_profile_file.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      921 2022-03-04 21:30:39.000000 garmindb-3.3.0/test/test_summary_db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1887 2019-12-10 12:19:48.000000 garmindb-3.3.0/test/test_summary_db_base.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1641 2021-06-27 22:56:11.000000 garmindb-3.3.0/test/test_tcx_file.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2424 2021-06-27 22:56:11.000000 garmindb-3.3.0/test/test_tcx_loop.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:53.012440 garmindb-3.3.1/
+-rw-r--r--   0 tgoetz     (501) staff       (20)    18092 2020-02-08 21:26:46.000000 garmindb-3.3.1/LICENSE
+-rw-r--r--   0 tgoetz     (501) staff       (20)       74 2021-12-02 23:58:59.000000 garmindb-3.3.1/MANIFEST.in
+-rw-r--r--   0 tgoetz     (501) staff       (20)     7143 2023-08-08 11:08:53.012112 garmindb-3.3.1/PKG-INFO
+-rw-r--r--   0 tgoetz     (501) staff       (20)     6614 2022-07-24 19:28:30.000000 garmindb-3.3.1/README.md
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:52.993677 garmindb-3.3.1/garmindb/
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1148 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/GarminConnectConfig.json.example
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1645 2022-07-24 19:28:30.000000 garmindb-3.3.1/garmindb/__init__.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      935 2021-12-02 23:58:59.000000 garmindb-3.3.1/garmindb/activities_fit_data.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    20102 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/activity_fit_file_processor.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2277 2021-12-02 23:58:59.000000 garmindb-3.3.1/garmindb/activity_fit_plugin_base.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)    12925 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/analyze.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     6224 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/checkup.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1889 2022-02-13 19:52:28.000000 garmindb-3.3.1/garmindb/config.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    10671 2023-08-08 10:54:01.000000 garmindb-3.3.1/garmindb/config_manager.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     2607 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/copy.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)    18277 2023-08-08 10:54:01.000000 garmindb-3.3.1/garmindb/download.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2480 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/export_activities.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2270 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/fit_data.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    12314 2023-08-08 10:54:01.000000 garmindb-3.3.1/garmindb/fit_file_processor.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:52.996488 garmindb-3.3.1/garmindb/fitbitdb/
+-rw-r--r--   0 tgoetz     (501) staff       (20)      306 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/fitbitdb/__init__.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     3681 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/fitbitdb/analyze.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     7409 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/fitbitdb/fitbit_db.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     3479 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/fitbitdb/import_csv.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     4850 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/garmin_connect_config_manager.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    13881 2023-08-08 10:54:01.000000 garmindb-3.3.1/garmindb/garmin_connect_enums.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)    17648 2023-08-08 10:54:01.000000 garmindb-3.3.1/garmindb/garmin_json_data.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     7395 2021-12-02 23:58:59.000000 garmindb-3.3.1/garmindb/garmin_tcx_data.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:52.999119 garmindb-3.3.1/garmindb/garmindb/
+-rw-r--r--   0 tgoetz     (501) staff       (20)      771 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/garmindb/__init__.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    22829 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/garmindb/activities_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    20819 2023-02-20 02:49:53.000000 garmindb-3.3.1/garmindb/garmindb/garmin_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     3877 2022-02-03 23:57:21.000000 garmindb-3.3.1/garmindb/garmindb/garmin_summary_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    11754 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/garmindb/monitoring_db.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)    10117 2022-02-03 23:57:21.000000 garmindb-3.3.1/garmindb/graphs.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)    17358 2022-10-21 12:31:56.000000 garmindb-3.3.1/garmindb/import_monitoring.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     3373 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/maps.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     5791 2022-10-21 12:31:56.000000 garmindb-3.3.1/garmindb/monitoring_fit_file_processor.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      735 2021-12-02 23:58:59.000000 garmindb-3.3.1/garmindb/monitoring_fit_plugin_base.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:53.000981 garmindb-3.3.1/garmindb/mshealthdb/
+-rw-r--r--   0 tgoetz     (501) staff       (20)      343 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/mshealthdb/__init__.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     4005 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/mshealthdb/analyze.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     6079 2022-03-04 21:30:39.000000 garmindb-3.3.1/garmindb/mshealthdb/import_csv.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     8821 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/mshealthdb/mshealth_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      544 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/open_with_basecamp.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      546 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/open_with_google_earth.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      808 2021-12-02 23:58:59.000000 garmindb-3.3.1/garmindb/plugin_base.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1135 2021-12-02 23:58:59.000000 garmindb-3.3.1/garmindb/plugin_manager.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1960 2022-07-24 19:28:30.000000 garmindb-3.3.1/garmindb/sleep_fit_file_processor.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      640 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/statistics.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:53.002451 garmindb-3.3.1/garmindb/summarydb/
+-rw-r--r--   0 tgoetz     (501) staff       (20)      294 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/summarydb/__init__.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     9702 2021-12-23 14:56:41.000000 garmindb-3.3.1/garmindb/summarydb/summary_base.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2303 2021-12-23 14:56:41.000000 garmindb-3.3.1/garmindb/summarydb/summary_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     4868 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/tcx.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      707 2021-06-27 22:56:11.000000 garmindb-3.3.1/garmindb/version.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      369 2023-08-08 10:56:07.000000 garmindb-3.3.1/garmindb/version_info.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:52.995173 garmindb-3.3.1/garmindb.egg-info/
+-rw-r--r--   0 tgoetz     (501) staff       (20)     7143 2023-08-08 11:08:52.000000 garmindb-3.3.1/garmindb.egg-info/PKG-INFO
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2118 2023-08-08 11:08:52.000000 garmindb-3.3.1/garmindb.egg-info/SOURCES.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)        1 2023-08-08 11:08:52.000000 garmindb-3.3.1/garmindb.egg-info/dependency_links.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)      216 2023-08-08 11:08:52.000000 garmindb-3.3.1/garmindb.egg-info/requires.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)        9 2023-08-08 11:08:52.000000 garmindb-3.3.1/garmindb.egg-info/top_level.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)      104 2021-06-27 22:56:11.000000 garmindb-3.3.1/pyproject.toml
+-rw-r--r--   0 tgoetz     (501) staff       (20)      216 2023-08-08 10:54:01.000000 garmindb-3.3.1/requirements.txt
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:53.006242 garmindb-3.3.1/scripts/
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     2222 2021-12-23 14:56:41.000000 garmindb-3.3.1/scripts/fitbit.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     1483 2022-01-31 22:32:22.000000 garmindb-3.3.1/scripts/garmindb_bug_report.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1699 2021-12-02 23:58:59.000000 garmindb-3.3.1/scripts/garmindb_checkup.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)    17404 2022-07-24 19:28:30.000000 garmindb-3.3.1/scripts/garmindb_cli.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     3316 2021-06-27 22:56:11.000000 garmindb-3.3.1/scripts/garmindb_graphs.py
+-rwxr-xr-x   0 tgoetz     (501) staff       (20)     2300 2021-12-23 14:56:41.000000 garmindb-3.3.1/scripts/mshealth.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)       38 2023-08-08 11:08:53.012530 garmindb-3.3.1/setup.cfg
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2352 2022-01-31 22:32:22.000000 garmindb-3.3.1/setup.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 11:08:53.011670 garmindb-3.3.1/test/
+-rw-r--r--   0 tgoetz     (501) staff       (20)     7013 2021-06-27 22:56:11.000000 garmindb-3.3.1/test/test_activities_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1718 2021-06-27 22:56:11.000000 garmindb-3.3.1/test/test_copy.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2060 2022-03-04 21:30:39.000000 garmindb-3.3.1/test/test_db_base.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    12870 2022-07-24 19:28:30.000000 garmindb-3.3.1/test/test_fit_file.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     5197 2022-07-24 19:28:30.000000 garmindb-3.3.1/test/test_garmin_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     5091 2021-06-27 22:56:11.000000 garmindb-3.3.1/test/test_garmin_db_objects.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      994 2022-03-04 21:30:39.000000 garmindb-3.3.1/test/test_garmin_summary_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     5300 2021-06-27 22:56:11.000000 garmindb-3.3.1/test/test_monitoring_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1237 2021-06-27 22:56:11.000000 garmindb-3.3.1/test/test_profile_file.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      921 2022-03-04 21:30:39.000000 garmindb-3.3.1/test/test_summary_db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1887 2019-12-10 12:19:48.000000 garmindb-3.3.1/test/test_summary_db_base.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1641 2021-06-27 22:56:11.000000 garmindb-3.3.1/test/test_tcx_file.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2424 2021-06-27 22:56:11.000000 garmindb-3.3.1/test/test_tcx_loop.py
```

### Comparing `garmindb-3.3.0/LICENSE` & `garmindb-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/PKG-INFO` & `garmindb-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmindb
-Version: 3.3.0
+Version: 3.3.1
 Summary: Download data from Garmin Connect and store it in a SQLite db for analysis.
 Home-page: https://github.com/tcgoetz/GarminDB
 Author: Tom Goetz
 Project-URL: Bug Tracker, https://github.com/tcgoetz/GarminDB/issues
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `garmindb-3.3.0/README.md` & `garmindb-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/GarminConnectConfig.json.example` & `garmindb-3.3.1/garmindb/GarminConnectConfig.json.example`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/__init__.py` & `garmindb-3.3.1/garmindb/__init__.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/activities_fit_data.py` & `garmindb-3.3.1/garmindb/activities_fit_data.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/activity_fit_file_processor.py` & `garmindb-3.3.1/garmindb/activity_fit_file_processor.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/activity_fit_plugin_base.py` & `garmindb-3.3.1/garmindb/activity_fit_plugin_base.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/analyze.py` & `garmindb-3.3.1/garmindb/analyze.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/checkup.py` & `garmindb-3.3.1/garmindb/checkup.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/config.py` & `garmindb-3.3.1/garmindb/config.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/config_manager.py` & `garmindb-3.3.1/garmindb/config_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,8 +261,8 @@
         activity = cls.graphs.get(activity)
         if activity is not None:
             return activity.get(key)
 
     @classmethod
     def default_display_activities(cls):
         """Return a list of the default activities to display."""
-        return [Sport.strict_from_string(activity) for activity in cls.default_display_activities]
+        return [Sport.strict_from_string(activity) for activity in super().default_display_activities]
```

### Comparing `garmindb-3.3.0/garmindb/copy.py` & `garmindb-3.3.1/garmindb/copy.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/download.py` & `garmindb-3.3.1/garmindb/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class Download():
     """Class for downloading health data from Garmin Connect."""
 
     garmin_connect_base_url = "https://connect.garmin.com"
     garmin_connect_enus_url = garmin_connect_base_url + "/en-US"
 
     garmin_connect_sso_login = 'signin'
+    garmin_connect_mfa_login = 'verifyMFA/loginEnterMfaCode'
 
     garmin_connect_login_url = garmin_connect_enus_url + "/signin"
 
     garmin_connect_css_url = 'https://static.garmincdn.com/com.garmin.connect/ui/css/gauth-custom-v1.2-min.css'
 
     garmin_connect_privacy_url = "//connect.garmin.com/en-U/privacy"
 
@@ -142,14 +143,25 @@
             'Content-Type'  : 'application/x-www-form-urlencoded'
         }
         try:
             response = self.sso_rest_client.post(self.garmin_connect_sso_login, post_headers, params, data)
         except RestException as e:
             root_logger.error("Exception during login post: %s", e)
             return False
+        mfa = re.search(r'performMFACheck\s*="(.*)"', response.text, re.M)
+        if mfa and mfa.group(1) == 'true':
+            logger.debug("MFA request found in (%s).", response.text)
+            data = {
+                'mfa-code' : input("Enter MFA code: "),
+                'embed'    : 'false',
+                '_csrf'    : found.group(1)
+            }
+            response = self.sso_rest_client.post(self.garmin_connect_mfa_login, post_headers, params, data)
+        else:
+            logger.debug("no MFA request found.")
         found = re.search(r"\?ticket=([\w-]*)", response.text, re.M)
         if not found:
             logger.error("Login ticket not found (%d).", response.status_code)
             RestClient.save_binary_file('login_post.html', response)
             return False
         params = {
             'ticket' : found.group(1)
```

### Comparing `garmindb-3.3.0/garmindb/export_activities.py` & `garmindb-3.3.1/garmindb/export_activities.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/fit_data.py` & `garmindb-3.3.1/garmindb/fit_data.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/fit_file_processor.py` & `garmindb-3.3.1/garmindb/fit_file_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,32 +122,27 @@
         }
         File.s_insert_or_update(self.garmin_db_session, file)
 
     def _write_device_info_entry(self, fit_file, message_fields):
         timestamp = fit_file.utc_datetime_to_local(message_fields.timestamp)
         device_type = message_fields.get('device_type', fitfile.MainDeviceType.fitness_tracker)
         serial_number = message_fields.serial_number
-        manufacturer = Device.Manufacturer.convert(message_fields.manufacturer)
-        product = message_fields.product
         source_type = message_fields.source_type
         # local devices are part of the main device. Base missing fields off of the main device.
         if source_type is fitfile.field_enums.SourceType.local:
             if serial_number is None and self.serial_number is not None and device_type is not None:
                 serial_number = Device.local_device_serial_number(self.serial_number, device_type)
-            if manufacturer is None:
-                manufacturer = self.manufacturer
-            if product is None:
-                product = self.product
         if serial_number is not None:
+            manufacturer = Device.Manufacturer.convert(message_fields.manufacturer)
             device = {
                 'serial_number'     : serial_number,
                 'timestamp'         : timestamp,
                 'device_type'       : fitfile.field_enums.name_for_enum(device_type),
-                'manufacturer'      : manufacturer,
-                'product'           : fitfile.field_enums.name_for_enum(product),
+                'manufacturer'      : manufacturer or self.manufacturer,
+                'product'           : fitfile.field_enums.name_for_enum(message_fields.product or self.product),
                 'hardware_version'  : message_fields.hardware_version
             }
             Device.s_insert_or_update(self.garmin_db_session, device, ignore_none=True)
             device_info = {
                 'file_id'               : File.s_get_id(self.garmin_db_session, fit_file.filename),
                 'serial_number'         : serial_number,
                 'timestamp'             : timestamp,
```

### Comparing `garmindb-3.3.0/garmindb/fitbitdb/analyze.py` & `garmindb-3.3.1/garmindb/fitbitdb/analyze.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/fitbitdb/fitbit_db.py` & `garmindb-3.3.1/garmindb/fitbitdb/fitbit_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/fitbitdb/import_csv.py` & `garmindb-3.3.1/garmindb/fitbitdb/import_csv.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/garmin_connect_config_manager.py` & `garmindb-3.3.1/garmindb/garmin_connect_config_manager.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/garmin_connect_enums.py` & `garmindb-3.3.1/garmindb/garmin_connect_enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,20 +245,20 @@
         Sport.virtual_run                             : Sport.virtual_run,
         Sport.safety                                  : Sport.safety,
         Sport.assistance                              : Sport.assistance,
         Sport.incident_detected                       : Sport.incident_detected,
         Sport.ccr_diving                              : Sport.ccr_diving,
         Sport.auto_racing                             : Sport.auto_racing,
         Sport.breathwork                              : Sport.breathwork,
-        Sport.other                                   : Sport.other,
+        Sport.other                                   : Sport.other
     }
     special_remaps = {
         Sport.other                                   : remap_gc_sport_to_fit.get(gc_sub_sport),
         Sport.top_level                               : remap_gc_sport_to_fit.get(gc_sub_sport),
-        Sport.winter_sports                           : remap_winter_sports.get(gc_sub_sport),
+        Sport.winter_sports                           : remap_winter_sports.get(gc_sub_sport)
     }
     if gc_sport in special_remaps.keys():
         return (special_remaps[gc_sport], fitfile.Sport.generic)
     return (remap_gc_sport_to_fit.get(gc_sport), remap_gc_sub_sport_to_fit.get(gc_sub_sport))
 
 
 def get_details_sport(json_data):
```

### Comparing `garmindb-3.3.0/garmindb/garmin_json_data.py` & `garmindb-3.3.1/garmindb/garmin_json_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         max_temperature = self._get_field_obj(json_data, 'maxTemperature', fitfile.Temperature.from_celsius)
         min_temperature = self._get_field_obj(json_data, 'minTemperature', fitfile.Temperature.from_celsius)
         avg_temperature = self._get_field_obj(json_data, 'averageTemperature', fitfile.Temperature.from_celsius)
         start_time = dateutil.parser.parse(self._get_field(json_data, 'startTimeLocal'), ignoretz=True)
         elapsed_time = fitfile.conversions.secs_to_dt_time(self._get_field(json_data, 'elapsedDuration', int))
         return {
             'start_time'                : start_time,
-            'stop_time'                 : start_time + fitfile.conversions.time_to_timedelta(elapsed_time),
+            'stop_time'                 : start_time + fitfile.conversions.time_to_timedelta(elapsed_time) if elapsed_time is not None else None,
             'elapsed_time'              : elapsed_time,
             'moving_time'               : fitfile.conversions.secs_to_dt_time(self._get_field(json_data, 'movingDuration', int)),
             'start_lat'                 : self._get_field(json_data, 'startLatitude', float),
             'start_long'                : self._get_field(json_data, 'startLongitude', float),
             'stop_lat'                  : self._get_field(json_data, 'endLatitude', float),
             'stop_long'                 : self._get_field(json_data, 'endLongitude', float),
             'distance'                  : distance.kms_or_miles(self.measurement_system),
```

### Comparing `garmindb-3.3.0/garmindb/garmin_tcx_data.py` & `garmindb-3.3.1/garmindb/garmin_tcx_data.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/garmindb/__init__.py` & `garmindb-3.3.1/garmindb/garmindb/__init__.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/garmindb/activities_db.py` & `garmindb-3.3.1/garmindb/garmindb/activities_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/garmindb/garmin_db.py` & `garmindb-3.3.1/garmindb/garmindb/garmin_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/garmindb/garmin_summary_db.py` & `garmindb-3.3.1/garmindb/garmindb/garmin_summary_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/garmindb/monitoring_db.py` & `garmindb-3.3.1/garmindb/garmindb/monitoring_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/graphs.py` & `garmindb-3.3.1/garmindb/graphs.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/import_monitoring.py` & `garmindb-3.3.1/garmindb/import_monitoring.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/maps.py` & `garmindb-3.3.1/garmindb/maps.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/monitoring_fit_file_processor.py` & `garmindb-3.3.1/garmindb/monitoring_fit_file_processor.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/monitoring_fit_plugin_base.py` & `garmindb-3.3.1/garmindb/monitoring_fit_plugin_base.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/mshealthdb/analyze.py` & `garmindb-3.3.1/garmindb/mshealthdb/analyze.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/mshealthdb/import_csv.py` & `garmindb-3.3.1/garmindb/mshealthdb/import_csv.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/mshealthdb/mshealth_db.py` & `garmindb-3.3.1/garmindb/mshealthdb/mshealth_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/open_with_basecamp.py` & `garmindb-3.3.1/garmindb/open_with_basecamp.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/open_with_google_earth.py` & `garmindb-3.3.1/garmindb/open_with_google_earth.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/plugin_base.py` & `garmindb-3.3.1/garmindb/plugin_base.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/plugin_manager.py` & `garmindb-3.3.1/garmindb/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/sleep_fit_file_processor.py` & `garmindb-3.3.1/garmindb/sleep_fit_file_processor.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/statistics.py` & `garmindb-3.3.1/garmindb/statistics.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/summarydb/summary_base.py` & `garmindb-3.3.1/garmindb/summarydb/summary_base.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/summarydb/summary_db.py` & `garmindb-3.3.1/garmindb/summarydb/summary_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/tcx.py` & `garmindb-3.3.1/garmindb/tcx.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb/version.py` & `garmindb-3.3.1/garmindb/version.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/garmindb.egg-info/PKG-INFO` & `garmindb-3.3.1/garmindb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmindb
-Version: 3.3.0
+Version: 3.3.1
 Summary: Download data from Garmin Connect and store it in a SQLite db for analysis.
 Home-page: https://github.com/tcgoetz/GarminDB
 Author: Tom Goetz
 Project-URL: Bug Tracker, https://github.com/tcgoetz/GarminDB/issues
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `garmindb-3.3.0/garmindb.egg-info/SOURCES.txt` & `garmindb-3.3.1/garmindb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/scripts/fitbit.py` & `garmindb-3.3.1/scripts/fitbit.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/scripts/garmindb_bug_report.py` & `garmindb-3.3.1/scripts/garmindb_bug_report.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/scripts/garmindb_checkup.py` & `garmindb-3.3.1/scripts/garmindb_checkup.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/scripts/garmindb_cli.py` & `garmindb-3.3.1/scripts/garmindb_cli.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/scripts/garmindb_graphs.py` & `garmindb-3.3.1/scripts/garmindb_graphs.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/scripts/mshealth.py` & `garmindb-3.3.1/scripts/mshealth.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/setup.py` & `garmindb-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_activities_db.py` & `garmindb-3.3.1/test/test_activities_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_copy.py` & `garmindb-3.3.1/test/test_copy.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_db_base.py` & `garmindb-3.3.1/test/test_db_base.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_fit_file.py` & `garmindb-3.3.1/test/test_fit_file.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_garmin_db.py` & `garmindb-3.3.1/test/test_garmin_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_garmin_db_objects.py` & `garmindb-3.3.1/test/test_garmin_db_objects.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_garmin_summary_db.py` & `garmindb-3.3.1/test/test_garmin_summary_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_monitoring_db.py` & `garmindb-3.3.1/test/test_monitoring_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_profile_file.py` & `garmindb-3.3.1/test/test_profile_file.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_summary_db.py` & `garmindb-3.3.1/test/test_summary_db.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_summary_db_base.py` & `garmindb-3.3.1/test/test_summary_db_base.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_tcx_file.py` & `garmindb-3.3.1/test/test_tcx_file.py`

 * *Files identical despite different names*

### Comparing `garmindb-3.3.0/test/test_tcx_loop.py` & `garmindb-3.3.1/test/test_tcx_loop.py`

 * *Files identical despite different names*

