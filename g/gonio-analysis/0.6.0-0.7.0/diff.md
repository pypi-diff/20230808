# Comparing `tmp/gonio-analysis-0.6.0.tar.gz` & `tmp/gonio-analysis-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gonio-analysis-0.6.0.tar", last modified: Sat Jan  8 22:18:19 2022, max compression
+gzip compressed data, was "gonio-analysis-0.7.0.tar", last modified: Tue Aug  8 15:49:39 2023, max compression
```

## Comparing `gonio-analysis-0.6.0.tar` & `gonio-analysis-0.7.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.772480 gonio-analysis-0.6.0/
--rw-r--r--   0 joni      (1000) joni      (1000)     1799 2020-11-08 23:19:51.000000 gonio-analysis-0.6.0/.gitignore
--rw-r--r--   0 joni      (1000) joni      (1000)    35150 2020-11-08 23:19:51.000000 gonio-analysis-0.6.0/LICENSE
--rw-r--r--   0 joni      (1000) joni      (1000)     2834 2022-01-08 22:18:19.772480 gonio-analysis-0.6.0/PKG-INFO
--rw-r--r--   0 joni      (1000) joni      (1000)     2313 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/README.md
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.760480 gonio-analysis-0.6.0/bin/
--rwxr-xr-x   0 joni      (1000) joni      (1000)       81 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/bin/pupilanalysis
--rwxr-xr-x   0 joni      (1000) joni      (1000)       67 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/bin/pupilanalysis-tkgui
--rw-r--r--   0 joni      (1000) joni      (1000)      162 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/bin/pupilanalysis-tkgui.cmd
--rw-r--r--   0 joni      (1000) joni      (1000)      164 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/bin/pupilanalysis.cmd
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.760480 gonio-analysis-0.6.0/gonio_analysis.egg-info/
--rw-r--r--   0 joni      (1000) joni      (1000)     2834 2022-01-08 22:18:19.000000 gonio-analysis-0.6.0/gonio_analysis.egg-info/PKG-INFO
--rw-r--r--   0 joni      (1000) joni      (1000)     2931 2022-01-08 22:18:19.000000 gonio-analysis-0.6.0/gonio_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 joni      (1000) joni      (1000)        1 2022-01-08 22:18:19.000000 gonio-analysis-0.6.0/gonio_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 joni      (1000) joni      (1000)      105 2022-01-08 22:18:19.000000 gonio-analysis-0.6.0/gonio_analysis.egg-info/requires.txt
--rw-r--r--   0 joni      (1000) joni      (1000)       14 2022-01-08 22:18:19.000000 gonio-analysis-0.6.0/gonio_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.762480 gonio-analysis-0.6.0/gonioanalysis/
--rw-r--r--   0 joni      (1000) joni      (1000)     4481 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/__init__.py
--rw-r--r--   0 joni      (1000) joni      (1000)     7421 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/antenna_level.py
--rw-r--r--   0 joni      (1000) joni      (1000)     5703 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/binary_search.py
--rw-r--r--   0 joni      (1000) joni      (1000)    16044 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/coordinates.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2649 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/directories.py
--rw-r--r--   0 joni      (1000) joni      (1000)     6510 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/droso.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.763481 gonio-analysis-0.6.0/gonioanalysis/drosom/
--rw-r--r--   0 joni      (1000) joni      (1000)      787 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/README.txt
--rw-r--r--   0 joni      (1000) joni      (1000)        0 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/__init__.py
--rw-r--r--   0 joni      (1000) joni      (1000)     4082 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/analyser_commands.py
--rw-r--r--   0 joni      (1000) joni      (1000)    56518 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/analysing.py
--rw-r--r--   0 joni      (1000) joni      (1000)      827 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/fitting.py
--rw-r--r--   0 joni      (1000) joni      (1000)    10319 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/kinematics.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.763481 gonio-analysis-0.6.0/gonioanalysis/drosom/linked_data/
--rw-r--r--   0 joni      (1000) joni      (1000)       48 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/linked_data/__init__.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2318 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/linked_data/electrophysiology.py
--rw-r--r--   0 joni      (1000) joni      (1000)     5398 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/loading.py
--rw-r--r--   0 joni      (1000) joni      (1000)     7742 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/optic_flow.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2776 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/orientation_analysis.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.764480 gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/
--rw-r--r--   0 joni      (1000) joni      (1000)      155 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/__init__.py
--rw-r--r--   0 joni      (1000) joni      (1000)    45976 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/basics.py
--rw-r--r--   0 joni      (1000) joni      (1000)    23535 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/common.py
--rw-r--r--   0 joni      (1000) joni      (1000)    17357 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/compare_opticflow.py
--rw-r--r--   0 joni      (1000) joni      (1000)    18139 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/illustrate_experiments.py
--rw-r--r--   0 joni      (1000) joni      (1000)    12345 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/plotter.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.764480 gonio-analysis-0.6.0/gonioanalysis/drosom/reports/
--rw-r--r--   0 joni      (1000) joni      (1000)      109 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/reports/__init__.py
--rw-r--r--   0 joni      (1000) joni      (1000)    17752 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/reports/left_right.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2955 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/reports/pdf_summary.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2581 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/reports/repeats.py
--rw-r--r--   0 joni      (1000) joni      (1000)     1720 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/reports/stats.py
--rw-r--r--   0 joni      (1000) joni      (1000)    12181 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/sinesweep.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.765480 gonio-analysis-0.6.0/gonioanalysis/drosom/special/
--rw-r--r--   0 joni      (1000) joni      (1000)        0 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/special/__init__.py
--rw-r--r--   0 joni      (1000) joni      (1000)    26981 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/special/norpa_rescues.py
--rw-r--r--   0 joni      (1000) joni      (1000)     1812 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/special/paired.py
--rw-r--r--   0 joni      (1000) joni      (1000)    10546 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/terminal.py
--rw-r--r--   0 joni      (1000) joni      (1000)     3411 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosom/transmittance_analysis.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.765480 gonio-analysis-0.6.0/gonioanalysis/drosox/
--rw-r--r--   0 joni      (1000) joni      (1000)     5602 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosox/analysing.py
--rw-r--r--   0 joni      (1000) joni      (1000)     8565 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/drosox/loading.py
--rw-r--r--   0 joni      (1000) joni      (1000)    12145 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosox/plotting.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2519 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/drosox/terminal.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2918 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/image_tools.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.769480 gonio-analysis-0.6.0/gonioanalysis/images/
--rw-r--r--   0 joni      (1000) joni      (1000)    55229 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/dpp.tif
--rw-r--r--   0 joni      (1000) joni      (1000)   197818 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/droso_roll.png
--rw-r--r--   0 joni      (1000) joni      (1000)   215972 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/from_mikko.png
--rw-r--r--   0 joni      (1000) joni      (1000)   227021 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/from_mikko_annotated.png
--rw-r--r--   0 joni      (1000) joni      (1000)   309895 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/mikkos_alternative_fly.png
--rw-r--r--   0 joni      (1000) joni      (1000)  2456870 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/rotation_roll.png
--rw-r--r--   0 joni      (1000) joni      (1000)  2393579 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/rotation_yaw.png
--rw-r--r--   0 joni      (1000) joni      (1000)   199370 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/images/side_aligning_pupil_antenna_whiteBG.jpg
--rw-r--r--   0 joni      (1000) joni      (1000)      938 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/rotary_encoders.py
--rw-r--r--   0 joni      (1000) joni      (1000)      888 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/settings.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.770480 gonio-analysis-0.6.0/gonioanalysis/tkgui/
--rw-r--r--   0 joni      (1000) joni      (1000)       34 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/__init__.py
--rw-r--r--   0 joni      (1000) joni      (1000)       65 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/__main__.py
--rw-r--r--   0 joni      (1000) joni      (1000)     9034 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/core.py
--rw-r--r--   0 joni      (1000) joni      (1000)    23330 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/examine.py
--rw-r--r--   0 joni      (1000) joni      (1000)    21647 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/menu_commands.py
--rw-r--r--   0 joni      (1000) joni      (1000)     6116 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/plotting.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2917 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/run_measurement.py
--rw-r--r--   0 joni      (1000) joni      (1000)     1216 2021-11-23 08:58:40.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/settings.py
--rw-r--r--   0 joni      (1000) joni      (1000)    23827 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/tkgui/widgets.py
--rw-r--r--   0 joni      (1000) joni      (1000)       22 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/gonioanalysis/version.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.771480 gonio-analysis-0.6.0/scripts/
--rw-r--r--   0 joni      (1000) joni      (1000)     1609 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/scripts/add_gridlines.py
--rw-r--r--   0 joni      (1000) joni      (1000)     1401 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/scripts/compress_datadir.py
--rw-r--r--   0 joni      (1000) joni      (1000)     4502 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/scripts/create_alr_data.py
--rw-r--r--   0 joni      (1000) joni      (1000)     3284 2021-04-27 09:49:44.000000 gonio-analysis-0.6.0/scripts/drosox_spin.py
--rw-r--r--   0 joni      (1000) joni      (1000)     1382 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/scripts/framepuller.py
--rw-r--r--   0 joni      (1000) joni      (1000)      443 2020-11-08 23:19:52.000000 gonio-analysis-0.6.0/scripts/make_cmds.py
--rw-r--r--   0 joni      (1000) joni      (1000)     1355 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/scripts/optimal_sampling.py
--rw-r--r--   0 joni      (1000) joni      (1000)     1200 2020-11-08 23:19:52.000000 gonio-analysis-0.6.0/scripts/plot_spatial_calibration.py
--rw-r--r--   0 joni      (1000) joni      (1000)     2939 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/scripts/videowrapper.py
--rw-r--r--   0 joni      (1000) joni      (1000)       38 2022-01-08 22:18:19.772480 gonio-analysis-0.6.0/setup.cfg
--rw-r--r--   0 joni      (1000) joni      (1000)     1058 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/setup.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.771480 gonio-analysis-0.6.0/tests/
--rw-r--r--   0 joni      (1000) joni      (1000)      871 2021-05-02 22:53:52.000000 gonio-analysis-0.6.0/tests/test_terminal.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2022-01-08 22:18:19.772480 gonio-analysis-0.6.0/windows_installer/
--rw-r--r--   0 joni      (1000) joni      (1000)      595 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/windows_installer/get_tkdeps.py
--rw-r--r--   0 joni      (1000) joni      (1000)    26886 2020-11-20 00:35:27.000000 gonio-analysis-0.6.0/windows_installer/logo_colored.ico
--rw-r--r--   0 joni      (1000) joni      (1000)     2288 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/windows_installer/make_installer.py
--rw-r--r--   0 joni      (1000) joni      (1000)     5078 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/windows_installer/movemeter_logo.ico
--rw-r--r--   0 joni      (1000) joni      (1000)      609 2022-01-08 22:07:18.000000 gonio-analysis-0.6.0/windows_installer/pynsist_template.cfg
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.556613 gonio-analysis-0.7.0/
+-rw-r--r--   0 joni      (1000) joni      (1000)     1799 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/.gitignore
+-rw-r--r--   0 joni      (1000) joni      (1000)    35150 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/LICENSE
+-rw-r--r--   0 joni      (1000) joni      (1000)     4037 2023-08-08 15:49:39.556613 gonio-analysis-0.7.0/PKG-INFO
+-rw-r--r--   0 joni      (1000) joni      (1000)     3552 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/README.md
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.458613 gonio-analysis-0.7.0/bin/
+-rwxr-xr-x   0 joni      (1000) joni      (1000)       81 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/bin/pupilanalysis
+-rwxr-xr-x   0 joni      (1000) joni      (1000)       67 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/bin/pupilanalysis-tkgui
+-rw-r--r--   0 joni      (1000) joni      (1000)      162 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/bin/pupilanalysis-tkgui.cmd
+-rw-r--r--   0 joni      (1000) joni      (1000)      164 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/bin/pupilanalysis.cmd
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.459613 gonio-analysis-0.7.0/gonio_analysis.egg-info/
+-rw-r--r--   0 joni      (1000) joni      (1000)     4037 2023-08-08 15:49:39.000000 gonio-analysis-0.7.0/gonio_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 joni      (1000) joni      (1000)     2921 2023-08-08 15:49:39.000000 gonio-analysis-0.7.0/gonio_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 joni      (1000) joni      (1000)        1 2023-08-08 15:49:39.000000 gonio-analysis-0.7.0/gonio_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 joni      (1000) joni      (1000)      105 2023-08-08 15:49:39.000000 gonio-analysis-0.7.0/gonio_analysis.egg-info/requires.txt
+-rw-r--r--   0 joni      (1000) joni      (1000)       14 2023-08-08 15:49:39.000000 gonio-analysis-0.7.0/gonio_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.463613 gonio-analysis-0.7.0/gonioanalysis/
+-rw-r--r--   0 joni      (1000) joni      (1000)     4481 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/__init__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     7421 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/antenna_level.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     5703 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/binary_search.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    17456 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/coordinates.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2734 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/directories.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     6510 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/droso.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.467613 gonio-analysis-0.7.0/gonioanalysis/drosom/
+-rw-r--r--   0 joni      (1000) joni      (1000)      787 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/README.txt
+-rw-r--r--   0 joni      (1000) joni      (1000)        0 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/__init__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     3792 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/analyser_commands.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    54373 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/analysing.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     4190 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/export.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      827 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/fitting.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    10319 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/kinematics.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.468613 gonio-analysis-0.7.0/gonioanalysis/drosom/linked_data/
+-rw-r--r--   0 joni      (1000) joni      (1000)       48 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/linked_data/__init__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2318 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/linked_data/electrophysiology.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     6356 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/loading.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     8354 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/optic_flow.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2780 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/orientation_analysis.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.470613 gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/
+-rw-r--r--   0 joni      (1000) joni      (1000)      155 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/__init__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    46053 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/basics.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    24093 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/common.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    17357 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/compare_opticflow.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    18334 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/illustrate_experiments.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.472613 gonio-analysis-0.7.0/gonioanalysis/drosom/reports/
+-rw-r--r--   0 joni      (1000) joni      (1000)      109 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/reports/__init__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    17752 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/reports/left_right.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2955 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/reports/pdf_summary.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2581 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/reports/repeats.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     1720 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/reports/stats.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    12181 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/sinesweep.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.473613 gonio-analysis-0.7.0/gonioanalysis/drosom/special/
+-rw-r--r--   0 joni      (1000) joni      (1000)        0 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/special/__init__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    26981 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/special/norpa_rescues.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     1812 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/special/paired.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    10336 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/terminal.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     3411 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosom/transmittance_analysis.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.475613 gonio-analysis-0.7.0/gonioanalysis/drosox/
+-rw-r--r--   0 joni      (1000) joni      (1000)     5602 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosox/analysing.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     8565 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosox/loading.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    12145 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosox/plotting.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2519 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/drosox/terminal.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2918 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/image_tools.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.542613 gonio-analysis-0.7.0/gonioanalysis/images/
+-rw-r--r--   0 joni      (1000) joni      (1000)    55229 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/dpp.tif
+-rw-r--r--   0 joni      (1000) joni      (1000)   197818 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/droso_roll.png
+-rw-r--r--   0 joni      (1000) joni      (1000)   215972 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/from_mikko.png
+-rw-r--r--   0 joni      (1000) joni      (1000)   227021 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/from_mikko_annotated.png
+-rw-r--r--   0 joni      (1000) joni      (1000)   309895 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/mikkos_alternative_fly.png
+-rw-r--r--   0 joni      (1000) joni      (1000)  2456870 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/rotation_roll.png
+-rw-r--r--   0 joni      (1000) joni      (1000)  2393579 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/rotation_yaw.png
+-rw-r--r--   0 joni      (1000) joni      (1000)   199370 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/images/side_aligning_pupil_antenna_whiteBG.jpg
+-rw-r--r--   0 joni      (1000) joni      (1000)      938 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/rotary_encoders.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      888 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/settings.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.549613 gonio-analysis-0.7.0/gonioanalysis/tkgui/
+-rw-r--r--   0 joni      (1000) joni      (1000)       34 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/__init__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)       65 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/__main__.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     9034 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/core.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    23330 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/examine.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    21990 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/menu_commands.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     6043 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/plotting.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2917 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/run_measurement.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      285 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/settings.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    23827 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/gonioanalysis/tkgui/widgets.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      287 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/gonioanalysis/version.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.552613 gonio-analysis-0.7.0/scripts/
+-rw-r--r--   0 joni      (1000) joni      (1000)     1609 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/add_gridlines.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2304 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/scripts/compress_datadir.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     4502 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/create_alr_data.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     3284 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/drosox_spin.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     1382 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/framepuller.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      443 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/make_cmds.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     1355 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/optimal_sampling.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     1200 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/plot_spatial_calibration.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     2939 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/scripts/videowrapper.py
+-rw-r--r--   0 joni      (1000) joni      (1000)       38 2023-08-08 15:49:39.556613 gonio-analysis-0.7.0/setup.cfg
+-rw-r--r--   0 joni      (1000) joni      (1000)     1257 2023-08-08 15:44:45.000000 gonio-analysis-0.7.0/setup.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.553613 gonio-analysis-0.7.0/tests/
+-rw-r--r--   0 joni      (1000) joni      (1000)      871 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/tests/test_terminal.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-08 15:49:39.555613 gonio-analysis-0.7.0/windows_installer/
+-rw-r--r--   0 joni      (1000) joni      (1000)      595 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/windows_installer/get_tkdeps.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    26886 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/windows_installer/logo_colored.ico
+-rw-r--r--   0 joni      (1000) joni      (1000)     2288 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/windows_installer/make_installer.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     5078 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/windows_installer/movemeter_logo.ico
+-rw-r--r--   0 joni      (1000) joni      (1000)      609 2022-02-19 20:01:42.000000 gonio-analysis-0.7.0/windows_installer/pynsist_template.cfg
```

### Comparing `gonio-analysis-0.6.0/.gitignore` & `gonio-analysis-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/LICENSE` & `gonio-analysis-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/PKG-INFO` & `gonio-analysis-0.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,120 @@
-Metadata-Version: 2.1
-Name: gonio-analysis
-Version: 0.6.0
-Summary: Spatial motion analysis program
-Home-page: https://github.com/jkemppainen/gonio-analysis
-Author: Joni Kemppainen
-Author-email: jjtkemppainen1@sheffield.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<h1>GonioAnalysis - A goniometric analysis program</h1>
+Gonio Analysis is a specialised spatial motion analysis software,
+mainly for GonioImsoft's data.
 
-<h1>Goniometric Analysis suite</h1>
-Specialised spatial motion analysis software for Gonio Imsoft data.
-
-In general, can be used for data that follows hierarchy
+In general, GonioAnalysis can be used for data following the hierarchy
 ```
 data_directory
 ├── specimen_01
 │   ├── experiment_01
 │   │   ├── image_001.tif
 │   │   └── image_002.tif
 │   └── ...
 └── ...
 ```
 
+but special (GonioImsoft) naming scheme is needed for some functionality.
+Tiff files or stacks are the preferred image format.
+
+*WARNING!* GonioAnalysis is still in early development!
+
 
 <h2>Installing</h2>
 
-There are two supported installation ways at the moment.
-On Windows, the stand-alone installer is possibly the best option unless you feel familiar with Python.
-On other platforms, use pip.
+Two installation methods are supported:
+
+- The stand-alone installer (Windows only)
+- Python packaging (all platforms)
+
 
 <h3>Installer on Windows (easiest)</h3>
 
-A Windows installer that bundles together the Gonio Analysis suite and all its depencies,
-including a complete Python runtime, is provided at
+A Windows installer bundles together the Gonio Analysis suite and all its depencies,
+including a complete Python runtime. It is ideal for users not having Python installed before.
+
+The installer can be found at
 [Releases](https://github.com/jkemppainen/gonio-analysis/releases).
 
 The installer creates a start menu shorcut called <em>Gonio Analysis</em>,
 which can be used to launch the program.
 
-To uninstall, use <em>Add or Remove programs</em> feature in Windows.
+To uninstall the program, use the Windows <em>Add or Remove programs</em>.
 
 
 <h3>Using pip (the python standard way)</h3>
 
 The latest version from [PyPi](https://pypi.org/) can be installed with the command
 
 ```
 pip install gonio-analysis
 ```
 
-This should install all the required dependencies, except when on Windows, OpenCV may require
+This should install all the required dependencies. On Windows, OpenCV may require
 [Visual C++ Runtime 2015](https://www.microsoft.com/download/details.aspx?id=48145) to be installed.
 
 
-Afterwards, to upgrade an existing installation to the latest version
-
+Launch the program by
 ```
-pip install --upgrade gonio-analysis
+python -m gonioanalysis.tkgui
 ```
 
-In case of regressions, a specific version of the suite (for example 0.1.2) can be installed
+
+<h4>Managing versions using pip</h4>
+
+Upgrade to the latest version
 
 ```
-pip install gonio-analysis==0.1.2
+pip install --upgrade gonio-analysis
 ```
 
-Finally, to open the program
+Downgrade to a selected version
 
 ```
-python -m gonioanalysis.tkgui
+pip install gonio-analysis==0.1.2
 ```
 
-<h2>How to use</h2>
 
-First, open a data directory (containing the folders containing the images).
-Next, select the regions of interest (ROIs) and then run the motion analysis.
-The ROIs and movements are saved on disk (<em>C:\Users\USER\GonioAnalysis</em> or <em>/home/USER/.gonioanalysis</em>), so these steps are needed only once per specimen.
+<h2>Usage instructions</h2>
+
+Start by opening your data directory (this should contain the folders containing the images).
+Next, select the regions of interest (ROIs), and then, run the motion analysis.
+This may take a while.
+The ROIs and movements are saved on disk (<em>C:\Users\USER\GonioAnalysis</em> or <em>/home/USER/.gonioanalysis</em>),
+meaning that this part of the analysis (ROIs and movement analysis) has to be performed
+only once per specimen (unless you want to re-analyse).
 
 After the initial steps you, can perform further analyses in the program or
 export the data by
-1) copy-pasting to your favourite spread sheet or plotting program
+1) copy-pasting the results to an external program
 or 2) exporting CSV files.
 
-<h3>Notes</h3>
-This is still an early development version (expect rough edges).
+Many other features are present but yet undocumented.
+
+
+<h2>Contributing</h2>
+
+- Any problems or missing features,
+[Issues](https://github.com/jkemppainen/gonio-analysis/issues).
+
+- For general chatting,
+[Discussions](https://github.com/jkemppainen/gonio-analysis/discussions)
+
+See also below for the project's future plans.
+
 
+<h2>About the project</h2>
 
+This program was created in the University of Sheffield
+to analyse the photomechanical
+photoreceptor microsaccades that occur in the insect compound eyes.
+For more information, please see
+our [GHS-DPP methods @ Communications Biology](https://www.nature.com/articles/s42003-022-03142-0),
+or visit
+[the lab's website](https://cognition.group.shef.ac.uk/).
 
+Currently, it is maintained
+the original developer [jkemppainen](https://github.com/jkemppainen).
+Future efforts are mainly targeted towards ease-of-use
+(UI redesign/cleaning, exposing settings, documentation),
+bug-clearing (especially with non-GonioImsoft data)
+and performance (cross-correlation analysis).
```

### Comparing `gonio-analysis-0.6.0/gonio_analysis.egg-info/PKG-INFO` & `gonio-analysis-0.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,134 @@
 Metadata-Version: 2.1
 Name: gonio-analysis
-Version: 0.6.0
+Version: 0.7.0
 Summary: Spatial motion analysis program
 Home-page: https://github.com/jkemppainen/gonio-analysis
 Author: Joni Kemppainen
-Author-email: jjtkemppainen1@sheffield.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: joni.kemppainen@windowslive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1>Goniometric Analysis suite</h1>
-Specialised spatial motion analysis software for Gonio Imsoft data.
+<h1>GonioAnalysis - A goniometric analysis program</h1>
+Gonio Analysis is a specialised spatial motion analysis software,
+mainly for GonioImsoft's data.
 
-In general, can be used for data that follows hierarchy
+In general, GonioAnalysis can be used for data following the hierarchy
 ```
 data_directory
 ├── specimen_01
 │   ├── experiment_01
 │   │   ├── image_001.tif
 │   │   └── image_002.tif
 │   └── ...
 └── ...
 ```
 
+but special (GonioImsoft) naming scheme is needed for some functionality.
+Tiff files or stacks are the preferred image format.
+
+*WARNING!* GonioAnalysis is still in early development!
+
 
 <h2>Installing</h2>
 
-There are two supported installation ways at the moment.
-On Windows, the stand-alone installer is possibly the best option unless you feel familiar with Python.
-On other platforms, use pip.
+Two installation methods are supported:
+
+- The stand-alone installer (Windows only)
+- Python packaging (all platforms)
+
 
 <h3>Installer on Windows (easiest)</h3>
 
-A Windows installer that bundles together the Gonio Analysis suite and all its depencies,
-including a complete Python runtime, is provided at
+A Windows installer bundles together the Gonio Analysis suite and all its depencies,
+including a complete Python runtime. It is ideal for users not having Python installed before.
+
+The installer can be found at
 [Releases](https://github.com/jkemppainen/gonio-analysis/releases).
 
 The installer creates a start menu shorcut called <em>Gonio Analysis</em>,
 which can be used to launch the program.
 
-To uninstall, use <em>Add or Remove programs</em> feature in Windows.
+To uninstall the program, use the Windows <em>Add or Remove programs</em>.
 
 
 <h3>Using pip (the python standard way)</h3>
 
 The latest version from [PyPi](https://pypi.org/) can be installed with the command
 
 ```
 pip install gonio-analysis
 ```
 
-This should install all the required dependencies, except when on Windows, OpenCV may require
+This should install all the required dependencies. On Windows, OpenCV may require
 [Visual C++ Runtime 2015](https://www.microsoft.com/download/details.aspx?id=48145) to be installed.
 
 
-Afterwards, to upgrade an existing installation to the latest version
-
+Launch the program by
 ```
-pip install --upgrade gonio-analysis
+python -m gonioanalysis.tkgui
 ```
 
-In case of regressions, a specific version of the suite (for example 0.1.2) can be installed
+
+<h4>Managing versions using pip</h4>
+
+Upgrade to the latest version
 
 ```
-pip install gonio-analysis==0.1.2
+pip install --upgrade gonio-analysis
 ```
 
-Finally, to open the program
+Downgrade to a selected version
 
 ```
-python -m gonioanalysis.tkgui
+pip install gonio-analysis==0.1.2
 ```
 
-<h2>How to use</h2>
 
-First, open a data directory (containing the folders containing the images).
-Next, select the regions of interest (ROIs) and then run the motion analysis.
-The ROIs and movements are saved on disk (<em>C:\Users\USER\GonioAnalysis</em> or <em>/home/USER/.gonioanalysis</em>), so these steps are needed only once per specimen.
+<h2>Usage instructions</h2>
+
+Start by opening your data directory (this should contain the folders containing the images).
+Next, select the regions of interest (ROIs), and then, run the motion analysis.
+This may take a while.
+The ROIs and movements are saved on disk (<em>C:\Users\USER\GonioAnalysis</em> or <em>/home/USER/.gonioanalysis</em>),
+meaning that this part of the analysis (ROIs and movement analysis) has to be performed
+only once per specimen (unless you want to re-analyse).
 
 After the initial steps you, can perform further analyses in the program or
 export the data by
-1) copy-pasting to your favourite spread sheet or plotting program
+1) copy-pasting the results to an external program
 or 2) exporting CSV files.
 
-<h3>Notes</h3>
-This is still an early development version (expect rough edges).
+Many other features are present but yet undocumented.
+
+
+<h2>Contributing</h2>
+
+- Any problems or missing features,
+[Issues](https://github.com/jkemppainen/gonio-analysis/issues).
+
+- For general chatting,
+[Discussions](https://github.com/jkemppainen/gonio-analysis/discussions)
+
+See also below for the project's future plans.
+
 
+<h2>About the project</h2>
 
+This program was created in the University of Sheffield
+to analyse the photomechanical
+photoreceptor microsaccades that occur in the insect compound eyes.
+For more information, please see
+our [GHS-DPP methods @ Communications Biology](https://www.nature.com/articles/s42003-022-03142-0),
+or visit
+[the lab's website](https://cognition.group.shef.ac.uk/).
 
+Currently, it is maintained
+the original developer [jkemppainen](https://github.com/jkemppainen).
+Future efforts are mainly targeted towards ease-of-use
+(UI redesign/cleaning, exposing settings, documentation),
+bug-clearing (especially with non-GonioImsoft data)
+and performance (cross-correlation analysis).
```

### Comparing `gonio-analysis-0.6.0/gonio_analysis.egg-info/SOURCES.txt` & `gonio-analysis-0.7.0/gonio_analysis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 gonioanalysis/rotary_encoders.py
 gonioanalysis/settings.py
 gonioanalysis/version.py
 gonioanalysis/drosom/README.txt
 gonioanalysis/drosom/__init__.py
 gonioanalysis/drosom/analyser_commands.py
 gonioanalysis/drosom/analysing.py
+gonioanalysis/drosom/export.py
 gonioanalysis/drosom/fitting.py
 gonioanalysis/drosom/kinematics.py
 gonioanalysis/drosom/loading.py
 gonioanalysis/drosom/optic_flow.py
 gonioanalysis/drosom/orientation_analysis.py
 gonioanalysis/drosom/sinesweep.py
 gonioanalysis/drosom/terminal.py
@@ -36,15 +37,14 @@
 gonioanalysis/drosom/linked_data/__init__.py
 gonioanalysis/drosom/linked_data/electrophysiology.py
 gonioanalysis/drosom/plotting/__init__.py
 gonioanalysis/drosom/plotting/basics.py
 gonioanalysis/drosom/plotting/common.py
 gonioanalysis/drosom/plotting/compare_opticflow.py
 gonioanalysis/drosom/plotting/illustrate_experiments.py
-gonioanalysis/drosom/plotting/plotter.py
 gonioanalysis/drosom/reports/__init__.py
 gonioanalysis/drosom/reports/left_right.py
 gonioanalysis/drosom/reports/pdf_summary.py
 gonioanalysis/drosom/reports/repeats.py
 gonioanalysis/drosom/reports/stats.py
 gonioanalysis/drosom/special/__init__.py
 gonioanalysis/drosom/special/norpa_rescues.py
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/__init__.py` & `gonio-analysis-0.7.0/gonioanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/antenna_level.py` & `gonio-analysis-0.7.0/gonioanalysis/antenna_level.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/binary_search.py` & `gonio-analysis-0.7.0/gonioanalysis/binary_search.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/coordinates.py` & `gonio-analysis-0.7.0/gonioanalysis/coordinates.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,64 @@
 Working in 3D space
 '''
 import math
 from math import sin, cos, tan, radians, pi, acos, atan, sqrt, degrees, atan2
 
 import numpy as np
 
+
+def where_vertical_between(points_3d, lower=None, upper=None, reverse=False):
+    ''''Returns a boolean array based on points' vertical angle.
+
+    Takes in 3D points and returns an 1D True/False array of length points_3d
+    
+    Arguments
+    ---------
+    points_3d : sequence
+        A sequence of (x,y,z) points
+    lower : float
+        Lower vertical angle degree in degrees
+    upper : float
+    reverse : bool
+        If True, inverses the returned array (True -> False and vice versa).
+
+    Returns
+    -------
+    booleans : ndarray
+        1D True/False array
+    '''
+    
+    # Calculate each point's vertical angle in degrees
+    verticals = np.degrees(np.arcsin(points_3d[:,2]/ np.cos(points_3d[:,0]) ))
+
+    # Check each point's y coordinate; If it is negative, we
+    # have to fix its angle
+    # FIXME: Do this in numpy for better performance
+    for i_point in range(len(points_3d)):
+        if points_3d[i_point][1] < 0:
+            if verticals[i_point] > 0:
+                verticals[i_point] = 180-verticals[i_point]
+            else:
+                verticals[i_point] = -180-verticals[i_point]
+
+    booleans = np.ones(len(points_3d), dtype=bool)
+    if lower is not None:
+        booleans = booleans * (verticals > lower)
+    if upper is not None:
+        booleans = booleans * (verticals < upper)
+    
+    if reverse:
+        booleans = np.invert(booleans)
+
+    return booleans
+ 
+
+
+
+
 def to_spherical(x,y,z, return_degrees=False):
     '''
     Transform to spherical coordinates (ISO)
     
     return_degrees     If true, return angles in degrees instead of radians
 
     Returns: r, phi, theta
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/directories.py` & `gonio-analysis-0.7.0/gonioanalysis/directories.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 
 CODE_ROOTDIR = os.path.dirname(os.path.realpath(__file__))
 USER_HOMEDIR = os.path.expanduser('~')
 
 if platform.system() == "Windows":
     GONIODIR = os.path.join(USER_HOMEDIR, 'GonioAnalysis')
 else:
-    GONIODIR = os.path.join(USER_HOMEDIR, '.Gonioanalysis')
+    GONIODIR = os.path.join(USER_HOMEDIR, '.gonioanalysis')
 
 
 ANALYSES_SAVEDIR = os.path.join(GONIODIR, 'final_results')
 PROCESSING_TEMPDIR = os.path.join(GONIODIR, 'intermediate_data')
 PROCESSING_TEMPDIR_BIGFILES = os.path.join(GONIODIR, 'intermediate_bigfiles')
 
 
 # DIRECTORIES THAT HAVE TO BE CREATED
-ALLDIRS= {'ANALYSES_SAVEDIR': ANALYSES_SAVEDIR,
+ALLDIRS= {
+        'GONIODIR': GONIODIR,
+        'ANALYSES_SAVEDIR': ANALYSES_SAVEDIR,
         'PROCESSING_TEMPDIR': PROCESSING_TEMPDIR,
-        'PROCESSING_TEMPDIR_BIGFILES': PROCESSING_TEMPDIR_BIGFILES}
+        'PROCESSING_TEMPDIR_BIGFILES': PROCESSING_TEMPDIR_BIGFILES
+        }
 
 
 def print_directories():
 
     print('These are the directories')
     
     for key, item in ALLDIRS.items():
@@ -59,27 +62,27 @@
             return False
         else:
             print("Choice not understood, please type yes or no")
 
 
 
 def directories_check(ui=cli_ask_creation):
-    '''
-    Perform a check that the saving directories exist.
+    '''Checks if the save directories exists, and creates if not.
     
-    ui      Callable that returns True if user wants to create
-                the directories or False if not.
-                As the first argument it gets the list of to be created directories
-
-                If ui is not callable, raise an error.
+    ARGUMENTS
+    ---------
+    ui : None or callable
+        A callable that returns True if selects yes (wants to create the
+        directories or False if not. The callable receives a list as its
+        first (and only) argument that contains the to-be-created
+        directories.
     '''
     non_existant = []
     
     for key, item in ALLDIRS.items():
-
         if not os.path.exists(item):
             non_existant.append(item)
 
     # If some directories are not created, launch an input requiring
     # user interaction.
     if non_existant:
         if callable(ui):
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/droso.py` & `gonio-analysis-0.7.0/gonioanalysis/droso.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/README.txt` & `gonio-analysis-0.7.0/gonioanalysis/drosom/README.txt`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/analyser_commands.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/analyser_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,42 +4,35 @@
 '''
 
 import numpy as np
 
 from gonioanalysis.drosom import plotting
 from gonioanalysis.drosom.plotting.common import save_3d_animation
 from gonioanalysis.drosom.plotting import basics, illustrate_experiments
-from gonioanalysis.drosom.plotting.plotter import MPlotter
 from gonioanalysis.drosom.plotting import complete_flow_analysis, error_at_flight
 from gonioanalysis.drosom.special.norpa_rescues import norpa_rescue_manyrepeats
 from gonioanalysis.drosom.special.paired import cli_group_and_compare
 import gonioanalysis.drosom.reports as reports
+import gonioanalysis.drosom.export as export
 
 I_WORKER = None
 N_WORKERS = None
 
-plotter = MPlotter()
-
 
 # Functions that take only one input argument that is the MAnalyser
 ANALYSER_CMDS = {}
 ANALYSER_CMDS['pass'] = print
 ANALYSER_CMDS['vectormap'] = basics.plot_3d_vectormap
-ANALYSER_CMDS['vectormap_mayavi'] = plotter.plot_3d_vectormap_mayavi
 ANALYSER_CMDS['vectormap_video'] = lambda analyser: save_3d_animation(analyser, plot_function=basics.plot_3d_vectormap, guidance=True, i_worker=I_WORKER, N_workers=N_WORKERS) 
-ANALYSER_CMDS['vectormap_oldvideo'] = lambda analyser: plotter.plot_3d_vectormap(analyser, animation=True)
+ANALYSER_CMDS['export_vectormap'] = export.export_vectormap
 ANALYSER_CMDS['magtrace'] = basics.plot_1d_magnitude
 ANALYSER_CMDS['2d_vectormap'] =  basics.plot_2d_vectormap
-ANALYSER_CMDS['trajectories'] = plotter.plot_2d_trajectories
-ANALYSER_CMDS['2dmagnitude'] = plotter.plotMagnitude2D
-
+ANALYSER_CMDS['trajectories'] = basics.plot_xy_trajectory
 
 # Analyser + image_folder
-#ANALYSER_CMDS['1dmagnitude'] = plotter.plot_1d_magnitude_from_folder
-
 ANALYSER_CMDS['moving_rois_video'] = illustrate_experiments.moving_rois
 ANALYSER_CMDS['illustrate_experiments_video'] = illustrate_experiments.illustrate_experiments
 ANALYSER_CMDS['rotation_mosaic'] = illustrate_experiments.rotation_mosaic
 ANALYSER_CMDS['norpa_rescue_manyrepeats'] = norpa_rescue_manyrepeats
 ANALYSER_CMDS['compare_paired'] = cli_group_and_compare
 ANALYSER_CMDS['lr_displacements'] = lambda analyser: reports.left_right_displacements(analyser, 'test')
 ANALYSER_CMDS['left_right_summary'] = reports.left_right_summary
@@ -48,16 +41,14 @@
 rotations = np.linspace(-180,180, 360)
 ANALYSER_CMDS['flow_analysis_yaw'] = lambda analyser: complete_flow_analysis(analyser, rotations, 'yaw')
 ANALYSER_CMDS['flow_analysis_roll'] = lambda analyser: complete_flow_analysis(analyser, rotations, 'roll')
 ANALYSER_CMDS['flow_analysis_pitch'] = lambda analyser: complete_flow_analysis(analyser, rotations, 'pitch')
 
 ANALYSER_CMDS['error_at_flight'] = error_at_flight
 
-ANALYSER_CMDS['export_vectormap'] = lambda analyser: analyser.export_3d_vectors()
-
 
 # Functions that take two input arguments;
 # MAanalyser object and the name of the imagefolder, in this order
 IMAGEFOLDER_CMDS = {}
 IMAGEFOLDER_CMDS['magtrace'] = basics.plot_1d_magnitude
 
 
@@ -67,18 +58,22 @@
 DUALANALYSER_CMDS['compare'] = basics.compare_3d_vectormaps
 DUALANALYSER_CMDS['compare_compact'] = basics.compare_3d_vectormaps_compact
 DUALANALYSER_CMDS['compare_manyviews'] = basics.compare_3d_vectormaps_manyviews
 
 DUALANALYSER_CMDS['difference_video'] = lambda analyser1, analyser2: save_3d_animation([analyser1, analyser2],
         plot_function=basics.plot_3d_differencemap, guidance=False, hide_axes=True, colorbar=False, hide_text=True,
         i_worker=I_WORKER, N_workers=N_WORKERS) 
+DUALANALYSER_CMDS['export_differencemap'] = export.export_differencemap
+
 
 # Manyviews videos
 for animation_type in ['rotate_plot', 'rotate_arrows', 'pitch_rot', 'yaw_rot', 'roll_rot']:
     DUALANALYSER_CMDS['compare_manyviews_{}_video'.format(animation_type.replace('_',''))] = lambda an1, an2, at=animation_type: save_3d_animation([an1, an2], plot_function=basics.compare_3d_vectormaps_manyviews, animation_type=at)
 
 
 # Functions that take in a list of manalysers (first positional argument)
 MULTIANALYSER_CMDS = {}
 MULTIANALYSER_CMDS['magnitude_probability'] = basics.plot_magnitude_probability
 MULTIANALYSER_CMDS['moving_rois_mosaic'] = illustrate_experiments.moving_rois_mosaic
 
+
+
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/analysing.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/analysing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,329 +1,196 @@
-'''
-Analysing motion from goniometrically measured image series.
-
--------
-Classes
--------
-  MAnalyser
-    Main programmatic interfacce to process and interact with imaging data
-    produced by gonio-imsoft        
-
-  MAverager         
-    Takes in many MAnalysers to generate a mean specimen.
-    Only implements some of MAnalyser methods 
-
-  VectorGettable
-    Internal, caches results for better performance
-
-
+'''Main MAnalyser classes for goniometric motion analysis.
 '''
 
 import os
 import json
 import ast
 import math
 import datetime
 
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.spatial import cKDTree as KDTree
 
 from gonioanalysis.drosom.loading import load_data, angles_from_fn, arange_fns
-from gonioanalysis.coordinates import camera2Fly, camvec2Fly, rotate_about_x, nearest_neighbour, mean_vector, optimal_sampling
+from gonioanalysis.coordinates import (
+        camera2Fly,
+        camvec2Fly,
+        rotate_about_x,
+        nearest_neighbour,
+        mean_vector,
+        optimal_sampling,
+        where_vertical_between,
+        )
 from gonioanalysis.directories import ANALYSES_SAVEDIR, PROCESSING_TEMPDIR
 from gonioanalysis.rotary_encoders import to_degrees, step2degree, DEFAULT_STEPS_PER_REVOLUTION
 
 from roimarker import Marker
 from movemeter import Movemeter
 
 
 
-def vertical_filter_points(points_3d, vertical_lower=None, vertical_upper=None, reverse=False):
-    ''''
-    Takes in 3D points and returns an 1D True/False array of length points_3d
-    '''
+class AnalyserBase:
+    '''Common base class for all analysers.
     
-    verticals = np.degrees(np.arcsin(points_3d[:,2]/ np.cos(points_3d[:,0]) ))
-
-    for i_point in range(len(points_3d)):
-        if points_3d[i_point][1] < 0:
-            if verticals[i_point] > 0:
-                verticals[i_point] = 180-verticals[i_point]
-            else:
-                verticals[i_point] = -180-verticals[i_point]
-
-    
-    booleans = np.ones(len(points_3d), dtype=np.bool)
-    if vertical_lower is not None:
-        booleans = booleans * (verticals > vertical_lower)
-    if vertical_upper is not None:
-        booleans = booleans * (verticals < vertical_upper)
-    
-    if reverse:
-        booleans = np.invert(booleans)
-
-    return booleans
- 
+    Features
+    --------
+    - setting vertical and horizontal ange limits
+    - exposing selected attributes as UI options
 
-
-class ShortNameable:
-    '''
-    Inheriting this class adds getting and setting
-    short_name attribute, and style for matplotlib text.
+    Attributes
+    ----------
+    ui_options : dict
+        Info about attributes should be exposed in a user interface. Each item
+        is another dictionary with keys "help" (help string) and "type" (type
+        conversion function such as int).
+    va_limits, ha_limits : list
+        Vertical angle and horizontal angle limits for get_3d_vectors.
     '''
 
-    def get_short_name(self):
-        '''
-        Returns the short_name of object or an emptry string if the short_name
-        has not been set.
-        '''
-        try:
-            return self.short_name
-        except AttributeError:
-            return ''
-
-    def set_short_name(self, short_name):
-        self.short_name = short_name
-
-
-    
-class SettingAngleLimits:
-    
     def __init__(self):
+        self.ui_options = {}
+        
         self.va_limits = [None, None]
         self.ha_limits = [None, None]
         self.alimits_reverse = False
 
-    def set_angle_limits(self, va_limits=(None, None), reverse=False):
-        '''
-        Limit get_3d_vectors
-
-        All units in degrees.
-        '''
-        self.va_limits = va_limits
-        self.alimits_reverse = reverse
-
-
-
-class VectorGettable:
-    '''
-    Inheriting this class grants abilities to get vectors and caches results
-    for future use, minimizing computational time penalty when called many times.
-    '''
 
-    def __init__(self):
-        self.cached = {}
-
-        # Define class methods dynamically
-        #for key in self.cached:
-        #    exec('self.get_{} = ')
-
-
-    def _get(self, key, *args, **kwargs):
+    def get_ui_options(self):
+        '''Lists UI options for the analyser: Their values, help and convert.
         '''
-
-        '''
-        dkey = ''
-        for arg in args:
-            dkey += arg
-        for key, val in kwargs.items():
-            dkey += '{}{}'.format(key, val)
-        
-        try:
-            self.cached[dkey]
-        except KeyError:
-            self.cached[dkey] = self._get_3d_vectors(*args, **kwargs)
-        return self.cached[dkey]
-
-
-    def get_3d_vectors(self, *args, **kwargs):
-        '''
-        Returns the sampled points and cartesian 3D-vectors at these points.
-        '''
-        #return self._get('3d_vectors', *args, **kwargs)
-        return self._get_3d_vectors(*args, **kwargs)
-
-
-
-class Discardeable():
-    '''
-    Inheriting this class and initializing it grants 
-    '''
-    def __init__(self):
-        self.discard_savefn = os.path.join(PROCESSING_TEMPDIR, 'Manalyser', 'discarded_recordings',
-                'discarded_{}.json'.format(self.folder))
+        dictionary = []
+        for key in self.ui_options:
+            dictionary[key] = {}
+            dictionary[key]['value'] = getattr(self, key, None)
+            dictionary[key]['help'] = self.ui_options[key]['help']
+            dictionary[key]['type'] = self.ui_options[key]['type']
         
-        os.makedirs(os.path.dirname(self.self.discard_savefn), exist_ok=True)
-
-        self.load_discarded()
-
-
-    def discard_recording(self, image_folder, i_repeat):
-        '''
-        Discard a recording
-
-        image_folder    Is pos-folder
-        i_repeat        From 0 to n, or 'all' to discard all repeats
-        '''
-        if image_folder not in self.discarded_recordings.keys():
-            self.discarded_recordings[image_folder] = []
-
-        self_discarded_recordings[image_folder].append(i_repeat)
-
+        return dictionary
 
-    def is_discarded(self, image_folder, i_repeat):
+    def set_ui_options(self, dictionary):
         '''
-        Checks if image_folder and i_repeats is discarded.
         '''
-        if image_folder in self.discarded_recordings.keys():
-            if i_repeat in self.discarded_recordings[image_folder] or 'all' in self.discarded_recordings[image_folder]:
-                return True
-        return False
-
-
-    def save_discarder(self):
-        '''
-        Save discarded recordings.
+        for key, item in dictionary.items():
+            if key in self.ui_options:
+                convert = self.ui_options[key].get('type', str)
+                setattr(self, key, convert(item))
+            else:
+                valid_keys = list(self.ui_options.keys())
+                raise KeyError(f'Key "{key}" not valid. Valid keys are {valid_keys}')
+            
 
-        This has to be called manually ( not called at self.discard_recording() )
+    def set_angle_limits(self, va_limits=(None, None), reverse=False):
         '''
-        with open(self.discard_savefn, 'w') as fp:
-            json.dump(self.discarded_recordings, fp)
-
+        Limit get_3d_vectors
 
-    def load_discarded(self):
-        '''
-        Load discard data from disk or if does not exists, initialize
-        self.discarded_recordings
-        
-        Is called at __init__
+        All units in degrees.
         '''
-        if os.path.exists(self.discard_savefn):
-            with open(self.discard_savefn, 'r') as fp:
-                self.discarded_recordings = json.load(fp)
-        else:
-            self.discarded_recordings = {}
+        self.va_limits = va_limits
+        self.alimits_reverse = reverse
 
 
 
-class MAnalyser(VectorGettable, SettingAngleLimits, ShortNameable):
-    '''
-    Cross-correlation analysis of DrosoM data, saving and loading, and getting
-    the analysed data out.
+class MAnalyser(AnalyserBase):
+    '''Motion analysis for GonioImsoft data.
 
-    ------------------
-    Input argument naming convetions
-    ------------------
-    - specimen_name
-    - recording_name
-
-    -----------
     Attributes
-    -----------
-    - self.movements      self.movements[eye][angle][i_repeat][x/y/time]
-                    where eye = "left" or "right"
-                    angle = recording_name.lstrip('pos'), so for example angle="(0, 0)_uv"
-        
-    
-    eyes : tuple of strings
-        By default, ("left", "right")
-    
+    ----------
+    data_path : string
+        A full file path to the specimen folder's location.
+    folder : string
+        The name of the specimen folder.
     active_analysis : string
-        Name of the active analysis. Sets MOVEMENTS_SAVEFN
-    
+        Name of the active analysis
+    ROIs
+    movements : dict
+        Nested dictionary of the measured 2D movements from Movemeter.
+        
+        Nested structure
+        -----------------
+        self.movements[eye][angle][i_repeat][x/y/time]
+            eye = "left" or "right"
+            angle = recording_name.lstrip('pos') // for example angle="(0, 0)_uv"
+    eyes : tuple of strings
+        Default ("left", "right").
     vector_rotation : float or None
         Rotation of 2D vectors (affects 3D)
-
+    imagefolder_skiplist : dict
     '''
 
-    def __init__(self, data_path, folder, clean_tmp=False, no_data_load=False):
-        '''
-        INPUT ARGUMENTS     DESCRIPTION 
-        data_path           directory where DrosoM folder lies
-        folder              Name of the DrosoM folder, for example "DrosoM1"
-        no_data_load        Skip loading data in the constructor
+    def __init__(self, data_path, folder, clean_tmp=False, no_data_load=False,
+                 active_analysis=''):
+        '''Initialize the MAnalyser object.
+
+        Arguments
+        ---------
+        no_data_load : bool
+            If True, skips loading data at constructing the object (use if
+            needing many short lived objects.
+        active_analysis : string
+            Name of the activated analysis
         '''
         super().__init__()
-        #Discardeable().__init__()
+        self._no_data_load = no_data_load
         
         self.ROIs = None 
-        
-        
         self.data_path = data_path
         self.folder = folder
 
         
         # Skip image_folders. i_repeat
         self.imagefolder_skiplist = {}
-        
 
+        # Python dictionary for linked data
+        self.linked_data = {}
+        
         self.manalysers = [self]
         self.eyes = ("left", "right")
         self.vector_rotation = None
         
+        # Different file or folder paths
         self._rois_skelefn = 'rois_{}{}.json' # specimen_name active_analysis
         self._movements_skelefn = 'movements_{}_{}{}.json' # specimen_name, eye, active_analysis
+        self._skiplist_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, 'imagefolder_skiplist.json')
+        self._crops_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, self._rois_skelefn.format(folder, ''))
+        self._movements_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, self._movements_skelefn.format(folder, '{}', ''))
+        self._link_savedir= os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, 'linked_data')
         
-        self.skiplist_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, 'imagefolder_skiplist.json')
-        self.CROPS_SAVEFN = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, self._rois_skelefn.format(folder, ''))
-        self.MOVEMENTS_SAVEFN = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, self._movements_skelefn.format(folder, '{}', ''))
-
-        self.LINK_SAVEDIR = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', folder, 'linked_data')
         
-
-        self.active_analysis = ''
-
-
-
-        if no_data_load:
-            # no_data_load was speciefied, skip all data loading
-            pass
-
-            # Python dictionary for linked data
-            self.linked_data = {}
-
-
-        else:
+        # Load some things
+        if no_data_load == False:
             self.stacks = load_data(os.path.join(self.data_path, self.folder))
 
-            if os.path.isfile(self.skiplist_savefn):
-                with open(self.skiplist_savefn, 'r') as fp:
+            if os.path.isfile(self._skiplist_savefn):
+                with open(self._skiplist_savefn, 'r') as fp:
                     self.imagefolder_skiplist = json.load(fp)
             
-
-            # Load movements and ROIs if they exists
-            if self.are_rois_selected():
-                self.load_ROIs()
-            
-            if self.is_measured():
-                self.load_analysed_movements()
-
             self.antenna_level_correction = self._getAntennaLevelCorrection(folder)
 
             self.load_linked_data()
-            
-            # Ensure the directories where the crops and movements are saved exist
-            os.makedirs(os.path.dirname(self.CROPS_SAVEFN), exist_ok=True)
-            os.makedirs(os.path.dirname(self.MOVEMENTS_SAVEFN), exist_ok=True)
 
+            # Ensure the directories where the crops and movements are saved exist
+            os.makedirs(os.path.dirname(self._crops_savefn), exist_ok=True)
+            os.makedirs(os.path.dirname(self._movements_savefn), exist_ok=True)
 
-        # For cahcing frequently used data
-        self.cahced = {'3d_vectors': None}
-    
-        self.stop_now = False
-        self.va_limits = [None, None]
-        self.ha_limits = [None, None]
-        self.alimits_reverse = False
 
-        # If receptive fields == True then give out receptive field
-        # movement directions instead of DPP movement directions
-        self.receptive_fields = False
+        # Set the active analysis, and loads ROIs and movements if available
+        self.active_analysis = active_analysis
 
+        self.stop_now = False
+    
+        # No data load to affect only this constructor
+        self._no_data_load = False
+        
+        # Info data about available UI options
+        self.ui_options = {
+                'vector_rotation': {'help': 'Vector rotation in the 2D imaging plane', 'type': float}
+                }
     
+
     @property
     def name(self):
         return self.folder
     
     @name.setter
     def name(self, name):
         self.folder=name
@@ -335,77 +202,78 @@
             return 'default'
         else:
             return self.__active_analysis
 
 
     @active_analysis.setter
     def active_analysis(self, name):
-        '''
-        Setting active analysis sets self.MOVEMENTS_SAVEFN.
-        
+        '''Sets the active analysis and loads ROIs an movements.
+
+        Arguments
+        ---------
         name : string
-            The default is "default"
+            The analysis default is "default" or "" (empty string).
         '''
         
         if name == 'default':
             name = ''
 
+        self.__active_analysis = name
+        
         if name == '':
-            self.CROPS_SAVEFN = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._rois_skelefn.format(self.folder, ''))
-            self.MOVEMENTS_SAVEFN = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._movements_skelefn.format(self.folder, '{}', ''))
+            self._crops_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._rois_skelefn.format(self.folder, ''))
+            self._movements_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._movements_skelefn.format(self.folder, '{}', ''))
         else:
-            self.CROPS_SAVEFN = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._rois_skelefn.format(self.folder, '_'+name))
-            self.MOVEMENTS_SAVEFN = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._movements_skelefn.format(self.folder, '{}', '_'+name))
+            self._crops_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._rois_skelefn.format(self.folder, '_'+name))
+            self._movements_savefn = os.path.join(PROCESSING_TEMPDIR, 'MAnalyser_data', self.folder, self._movements_skelefn.format(self.folder, '{}', '_'+name))
     
-        if self.are_rois_selected():
-            self.load_ROIs()
-        else:
-            try:
-                del self.ROIs
-            except AttributeError:
-                pass
-        if self.is_measured():
-            self.load_analysed_movements()
-        else:
-            try:
-                del self.movements
-            except AttributeError:
-                pass
+        if self._no_data_load == False:
 
-        self.__active_analysis = name
-        
+            if self.are_rois_selected():
+                self.load_ROIs()
+            else:
+                try:
+                    del self.ROIs
+                except AttributeError:
+                    pass
+            if self.is_measured():
+                self.load_analysed_movements()
+            else:
+                try:
+                    del self.movements
+                except AttributeError:
+                    pass
+            
 
 
 
     def list_analyses(self):
-        '''
-        Returns a list of analysis names that exist.
+        '''Returns a list of existing analysis names.
         '''
         
-        manalyser_dir = os.path.dirname(self.MOVEMENTS_SAVEFN)
+        manalyser_dir = os.path.dirname(self._movements_savefn)
 
         if os.path.isdir(manalyser_dir):
             fns = [fn for fn in os.listdir(manalyser_dir) if
                     self._movements_skelefn.split('{')[0] in fn and
-                    self.eyes[0] in ''.join(fn.split('_')[-2:])]
+                    self.eyes[0] in fn]
         else:
             fns = []
 
 
         names = []
 
         for fn in fns:
             secondlast, last = fn.split('.')[0].split('_')[-2:]
             
-            if secondlast in self.eyes and last not in self.eyes:
-                names.append(last)
-            elif secondlast not in self.eyes and last in self.eyes:
+            if fn.split('.')[0].split('_')[-1] in self.eyes:
                 names.append('default')
             else:
-                RuntimeWarning('Fixme list_analyses in MAnalyser')
+                analysis = fn.split(self.eyes[0])[1].split('.')[0].removeprefix('_')
+                names.append(analysis)
 
         return names
 
 
     def __fileOpen(self, fn):
         with open(fn, 'r') as fp:
             data = json.load(fp)
@@ -426,15 +294,15 @@
         '''
         
         if self.imagefolder_skiplist.get(image_folder, None) is None:
             self.imagefolder_skiplist[image_folder] = []
 
         self.imagefolder_skiplist[image_folder].append(i_repeat)
         
-        with open(self.skiplist_savefn, 'w') as fp:
+        with open(self._skiplist_savefn, 'w') as fp:
             json.dump(self.imagefolder_skiplist, fp)
 
 
 
     def list_rotations(self, list_special=True, special_separated=False,
             horizontal_condition=None, vertical_condition=None,
             _return_imagefolders=False):
@@ -573,38 +441,44 @@
         FIXME: Alphabetical order not right because no zero padding
         
         image_folder        Name of the image folder
         absolute_path       If true, return filenames with absolute path instead of relative
 
         '''
 
-        fns = [fn for fn in os.listdir(os.path.join(self.data_path, self.folder, image_folder)) if fn.endswith('.tiff') or fn.endswith('.tif')]
-        
-        fns = arange_fns(fns)
+        #fns = [fn for fn in os.listdir(os.path.join(self.data_path, self.folder, image_folder)) if fn.endswith('.tiff') or fn.endswith('.tif')]
+        #fns = arange_fns(fns)
+        #if absolute_path:
+        #    fns = [os.path.join(self.data_path, self.folder, image_folder, fn) for fn in fns]
+        
+        fns = []
+        # Flatten out the i_repeat structure
+        for repetitions_images in self.stacks[image_folder.removeprefix('pos')]:
+            fns.extend(repetitions_images)
 
-        if absolute_path:
-            fns = [os.path.join(self.data_path, self.folder, image_folder, fn) for fn in fns]
+        if not absolute_path:
+            fns = [os.path.basename(fn) for fn in fns]
 
         return fns
 
    
     def get_specimen_name(self):
         '''
         Return the name of the data (droso) folder, such as DrosoM42
         '''              
         return self.folder
   
 
-    @staticmethod
-    def get_imagefolder(image_fn):
-        '''
-        Gets the name of the folder where an image lies, for example
-        /a/b/c/image -> c
+    def get_imagefolder(self, image_fn):
+        '''Gets the image containing folder (for example, /a/b/c/image -> c).
 
-        based on the image filename.
+        Arguments
+        ---------
+        image_fn : string
+            Full path to the image.
         '''
         return os.path.split(os.path.dirname(image_fn))[1]
     
     
     @staticmethod
     def _getAntennaLevelCorrection(fly_name): 
         fn = os.path.join(ANALYSES_SAVEDIR, 'antenna_levels', fly_name+'.txt')
@@ -777,15 +651,15 @@
         
         Notice that this means that when the horizontal angle is zero (fly is facing towards the camera),
         image rotation has to be so that the eyes are on image's left and right halves.
         '''
 
         self.ROIs = {'left': {}, 'right': {}}
 
-        with open(self.CROPS_SAVEFN, 'r') as fp:
+        with open(self._crops_savefn, 'r') as fp:
             marker_markings = json.load(fp)
 
         for image_fn, ROIs in marker_markings.items():
             
             # Since use to relative filenames in the ROIs savefile
             image_fn = os.path.join(self.data_path, self.folder, image_fn)
 
@@ -799,14 +673,18 @@
             pos = self.get_imagefolder(image_fn)
             try:
                 horizontal, pitch = angles_from_fn(pos)
             except:
                 horizontal, pitch = (0, 0)
             pos = pos[3:]
 
+            if '_cam' in image_fn:
+                i_camera = int(image_fn[image_fn.index('_cam') + 4])
+                pos += f'_cam{i_camera}'
+
             # ROI belonging to the eft/right eye is determined solely by
             # the horizontal angle when only 1 ROI exists for the position
             if len(ROIs) == 1:
                 
                 if horizontal > 0:
                     self.ROIs['left'][pos] = ROIs[0]
                 else:
@@ -819,14 +697,20 @@
                     self.ROIs['left'][pos] = ROIs[0]
                     self.ROIs['right'][pos] = ROIs[1]
                 else:
                     self.ROIs['left'][pos]= ROIs[1]
                     self.ROIs['right'][pos] = ROIs[0]
             
             elif len(ROIs) > 2:
+
+                # With drift_correction, many ROIs are possible
+                #if self.active_analysis == 'drift_correction':
+                #    for i_roi, roi in enumerate(ROIs):
+                #        self.ROIs[f'roi{i_roi}'] = roi
+
                 print('Warning. len(ROIs) == {} for {}'.format(len(ROIs), image_fn))
 
         self.N_folders_having_rois = len(marker_markings)
         
         
 
     def select_ROIs(self, **kwargs):
@@ -836,24 +720,24 @@
 
         kwargs      Passed to the marker constructor
         '''
         
         to_cropping = [stacks[0][0] for str_angles, stacks in self.stacks.items()]
 
         fig, ax = plt.subplots()
-        marker = Marker(fig, ax, to_cropping, self.CROPS_SAVEFN,
+        marker = Marker(fig, ax, to_cropping, self._crops_savefn,
                 relative_fns_from=os.path.join(self.data_path, self.folder), **kwargs)
         marker.run()
 
 
     def are_rois_selected(self):
         '''
         Returns True if a file for crops/ROIs is found.
         '''
-        return os.path.exists(self.CROPS_SAVEFN)
+        return os.path.exists(self._crops_savefn)
 
 
     def count_roi_selected_folders(self):
         '''
         Returns the number of imagefolders that have ROIs selected
         '''
         if self.are_rois_selected():
@@ -889,15 +773,15 @@
         return rois
 
 
     def is_measured(self):
         '''
         Returns (True, True) if analyseMovement results can be found for the fly and bot eyes.
         '''
-        return all((os.path.exists(self.MOVEMENTS_SAVEFN.format('left')), os.path.exists(self.MOVEMENTS_SAVEFN.format('right'))))
+        return all((os.path.exists(self._movements_savefn.format('left')), os.path.exists(self._movements_savefn.format('right'))))
 
 
 
     def folder_has_movements(self, image_folder):
         '''
         Returns True if for specified image_folder has movements
         measured. Otherwise False.
@@ -911,19 +795,45 @@
             if len(self.get_displacements_from_folder(image_folder)) > 0:
                 return True
         return False
 
 
     def load_analysed_movements(self):
         self.movements = {}
-        with open(self.MOVEMENTS_SAVEFN.format('right'), 'r') as fp:
+        with open(self._movements_savefn.format('right'), 'r') as fp:
             self.movements['right'] = json.load(fp)
-        with open(self.MOVEMENTS_SAVEFN.format('left'), 'r') as fp:
+        with open(self._movements_savefn.format('left'), 'r') as fp:
             self.movements['left'] = json.load(fp)
         
+        if self.__active_analysis == 'drift_correction':
+            for key in self.movements['right']:
+                if key not in self.movements['left']:
+                    self.movements['left'] = self.movements['right']
+
+        # Special analysis name: "drift_correction". If present, subtracted
+        # from all the active analysis
+        if 'drift_correction' in self.list_analyses() and self.__active_analysis != 'drift_correction':
+            dc_analyser = MAnalyser(
+                    self.data_path, self.folder, active_analysis='drift_correction')
+            
+            for eye in ['left', 'right']:
+                for image_folder, data in dc_analyser.movements[eye].items():
+                    if image_folder not in self.movements[eye]:
+                        continue
+                    for i_repeat in range(len(data)):
+                        A = self.movements[eye][image_folder][i_repeat]
+                        B = data[i_repeat]
+                        for key in ['x', 'y']:
+                            dcx = np.array(list(range(len(B[key]))))
+                            fit = np.polynomial.polynomial.Polynomial.fit(dcx, B[key],1)
+                            corrected = (np.array(A[key]) - fit(dcx) ).tolist()
+                            #corrected = [a-b for a, b in zip(A[key], B[key])]
+                            self.movements[eye][image_folder][i_repeat][key] = corrected
+
+
         if self.imagefolder_skiplist:
             
             for image_folder, skip_repeats in self.imagefolder_skiplist.items():
                 for eye in self.eyes:
 
                     if self.movements[eye].get(image_folder[3:], None) is None:
                         continue
@@ -935,15 +845,15 @@
                     
 
 
     def measure_both_eyes(self, **kwargs):
         '''
         Wrapper to self.measure_movement() for both left and right eyes.
         '''
-        for eye in ['left', 'right']:
+        for eye in self.ROIs:
             self.measure_movement(eye, **kwargs)
 
 
     def measure_movement(self, eye, only_folders=None,
             max_movement=30, absolute_coordinates=False, join_repeats=False,
             stop_event=None):
         '''
@@ -963,15 +873,15 @@
             
 
         Cross-correlation analysis is the slowest part of the DrosoM pipeline.
         '''
         
         self.movements = {}
         
-        if not os.path.exists(self.CROPS_SAVEFN):
+        if not os.path.exists(self._crops_savefn):
             self.selectROIs() 
         self.load_ROIs()
         
 
         angles = []
         stacks = []
         ROIs = []
@@ -1049,25 +959,25 @@
 
         else:
             self.movements = {}
             
         # If only_folders set ie. only some angles were (re)measured,
         # load previous movements also for saving
         if only_folders:
-            with open(self.MOVEMENTS_SAVEFN.format(eye), 'r') as fp:
+            with open(self._movements_savefn.format(eye), 'r') as fp:
                  previous_movements = json.load(fp)
             
             # Update previous movements with the new movements and set
             # the updated previous movements to be the current movements
             previous_movements.update(self.movements)
             self.movements = previous_movements
 
 
         # Save movements
-        with open(self.MOVEMENTS_SAVEFN.format(eye), 'w') as fp:
+        with open(self._movements_savefn.format(eye), 'w') as fp:
             json.dump(self.movements, fp)
         
         
         #for key, data in self.movements.items():
         #    plt.plot(data['x'])
         #    plt.plot(data['y'])
         #    plt.show()
@@ -1175,35 +1085,34 @@
         '''
         angles = [list(ast.literal_eval(angle)) for angle in self.movements[eye]]
         movement_dict = [self.movements[eye][str(angle)] for angle in angles]
         
         return angles, movement_dict
     
 
-    def get_2d_vectors(self, eye, mirror_horizontal=True, mirror_pitch=True, correct_level=True, repeats_separately=False):
+    def get_2d_vectors(self, eye, mirror_horizontal=True, mirror_pitch=True,
+                       correct_level=True, repeats_separately=False,
+                       mirror_movements=False):
         '''
         Creates 2D vectors from the movements analysis data.
             Vector start point: ROI's position at the first frame
             Vector end point: ROI's position at the last frame
 
         mirror_pitch    Should make so that the negative values are towards dorsal and positive towards frontal
                             (this is how things on DrosoX were)
+        mirror_movements : bool
+            If True, mirrors the movement directions (X=-X and Y=-Y)
         '''
 
         # Make the order of angles deterministic
         sorted_angle_keys = sorted(self.movements[eye])
 
         angles = [list(ast.literal_eval(angle.split(')')[0]+')' )) for angle in sorted_angle_keys]
-        
-           
         values = [self.movements[eye][angle] for angle in sorted_angle_keys]
-        #suffix = sorted_angle_keys[0].split(')')[1]
-        #values = [self.movements[eye][angle] for angle in [str(tuple(a))+suffix for a in angles]]
 
-     
         to_degrees(angles)
         
         if correct_level:
             angles = self._correctAntennaLevel(angles)
 
         
         if mirror_horizontal:
@@ -1213,16 +1122,14 @@
         else:
             xdirchange = 1
         
         if mirror_pitch:
             for i in range(len(angles)):
                 angles[i][1] *= -1
 
-        
-
         # Vector X and Y components
         # Fix here if repetitions are needed to be averaged
         # (don't take only x[0] but average)
         if repeats_separately:
             tmp_angles = []            
             X = []
             Y = []
@@ -1236,27 +1143,18 @@
             angles = tmp_angles
 
         else:
 
             X = [xdirchange*(x[0]['x'][-1]-x[0]['x'][0]) for x in values]
             Y = [x[0]['y'][-1]-x[0]['y'][0] for x in values]
         
-
-
-        #i_frame = int(len(values[0][0]['x'])/3)
-        #X = [xdirchange*(x[0]['x'][i_frame]-x[0]['x'][0]) for x in values]
-        #Y = [x[0]['y'][i_frame]-x[0]['y'][0] for x in values]
-        
-        if self.receptive_fields:
+        if mirror_movements:
             X = [-x for x in X]
             Y = [-y for y in Y]
 
-        #X = [0.1 for x in values]
-        #Y = [0. for x in values]
-
         if self.vector_rotation:
             r = math.radians(self.vector_rotation)
             for i in range(len(X)):
                 x = X[i]
                 y = Y[i]
                 
                 if angles[i][1] > 0:
@@ -1268,15 +1166,14 @@
                     sr = sr
                 elif eye == 'right':
                     sr = -sr
 
                 X[i] = x * math.cos(sr) - y * math.sin(sr)
                 Y[i] = x * math.sin(sr) + y * math.cos(sr)
 
-
         return angles, X, Y
 
 
             
     def get_magnitude_traces(self, eye, image_folder=None,
             mean_repeats=False, mean_imagefolders=False,
             microns=False, _phase=False, _derivative=False):
@@ -1410,15 +1307,15 @@
             x = -movements['x'][i]
             y = -movements['y'][i]
             
             moving_ROI.append([rx+x,ry+y,rw,rh])
         return moving_ROI
         
     
-    def _get_3d_vectors(self, eye, return_angles=False, correct_level=True, repeats_separately=False, normalize_length=0.1, strict=None, vertical_hardborder=None):
+    def get_3d_vectors(self, eye, return_angles=False, correct_level=True, repeats_separately=False, normalize_length=0.1, strict=None, vertical_hardborder=None):
         '''
         Returns 3D vectors and their starting points.
     
         correct_level           Use estimated antenna levels
 
         va_limits       Vertical angle limits in degrees, (None, None) for no limits
         '''
@@ -1447,16 +1344,16 @@
             x1,y1,z1 = point1
 
             #vectors.append( (tuple(angle), (x0,x1), (y0,y1), (z0, z1)) )
             points[i] = np.array(point0)            
             vectors[i] = np.array(point1) - points[i] 
 
         # Vertical/horizontal angle limiting
-        booleans = vertical_filter_points(points, vertical_lower=self.va_limits[0],
-                vertical_upper=self.va_limits[1], reverse=self.alimits_reverse)
+        booleans = where_vertical_between(points, lower=self.va_limits[0],
+                upper=self.va_limits[1], reverse=self.alimits_reverse)
         points = points[booleans]
         vectors = vectors[booleans]
 
         if return_angles:
             return points, vectors, angles
         else:
             return points, vectors
@@ -1509,70 +1406,77 @@
         self.linked_data[key] = data
 
 
     def save_linked_data(self):
         '''
         Attempt saving the linked data on disk in JSON format.
         '''
-        os.makedirs(self.LINK_SAVEDIR, exist_ok=True)
+        os.makedirs(self._link_savedir, exist_ok=True)
         
         for key, data in self.linked_data.items():
-            with open(os.path.join(self.LINK_SAVEDIR, "{}.json".format(key)), 'w') as fp:
+            with open(os.path.join(self._link_savedir, "{}.json".format(key)), 'w') as fp:
                 json.dump(data, fp)
 
     
     def load_linked_data(self):
         '''
         Load linked data from specimen datadir.
         '''
         # Initialize linked data to an empty dict
         self.linked_data = {}
 
         # Check if linked data directory exsists, if not, the no linked data for this specimen
-        if os.path.exists(self.LINK_SAVEDIR):
+        if os.path.exists(self._link_savedir):
 
-            dfiles = [fn for fn in os.listdir(self.LINK_SAVEDIR) if fn.endswith('.json')]
+            dfiles = [fn for fn in os.listdir(self._link_savedir) if fn.endswith('.json')]
             
             for dfile in dfiles:
-                with open(os.path.join(self.LINK_SAVEDIR, dfile), 'r') as fp:
+                with open(os.path.join(self._link_savedir, dfile), 'r') as fp:
                     data = json.load(fp)
                     self.linked_data[dfile.replace('.json', '')] = data
         
 
-
-class MAverager(VectorGettable, ShortNameable, SettingAngleLimits):
+class MAverager(AnalyserBase):
     '''
     Combining and averaging results from many MAnalyser objects.
     
     MAverager acts like MAnalyser object for getting data (like get_2d_vectors)
     but lacks the movement analysis (cross-correlation) related parts.
     '''
-    def __init__(self, manalysers, short_name=''):
-        
+    def __init__(self, manalysers):
+        super().__init__()
+
         self.manalysers = manalysers
 
         self.interpolation = {}
-        self.va_limits = [None, None]
-        self.ha_limits = [None, None]
-        self.alimits_reverse = False
 
         self.intp_step = (5, 5)
         
         self.eyes = manalysers[0].eyes
-        self.vector_rotation = None
+        self.vector_rotation = manalysers[0].vector_rotation
 
         self.interpolated_raw= {}
-
+        
+        # Info data about available UI options
+        self.ui_options = manalysers[0].ui_options.copy() 
 
     def get_N_specimens(self):
         return len(self.manalysers)
 
 
     def get_specimen_name(self):
         return 'averaged_'+'_'.join([manalyser.folder for manalyser in self.manalysers])
+    
+    @property
+    def name(self):
+        return self.get_specimen_name()
+    
+    @name.setter
+    def name(self, name):
+        return
 
 
     def setInterpolationSteps(self, horizontal_step, vertical_step):
         '''
         Set the resolution of the N-nearest neighbour interpolation in Maverager.get_2d_vectors.
 
         INPUT ARGUMENTS
@@ -1716,39 +1620,15 @@
                     newpoints.append(point)
                     newvecs.append(vec)
             points = np.array(newpoints)
             vectors = np.array(newvecs)
 
         
         # Vertical/horizontal angle limiting
-        booleans = vertical_filter_points(points, vertical_lower=self.va_limits[0],
-                vertical_upper=self.va_limits[1], reverse=self.alimits_reverse)
+        booleans = where_vertical_between(points, lower=self.va_limits[0],
+                upper=self.va_limits[1], reverse=self.alimits_reverse)
         points = points[booleans]
         vectors = vectors[booleans]
         
 
         return points, vectors
 
-
-    def export_3d_vectors(self, *args, **kwargs):
-        '''
-        Exports the 3D vectors in json format.
-
-        optic_flow          If true, export optic flow instead of the fly vectors
-        '''
-        
-        folder = os.path.join(ANALYSES_SAVEDIR, 'exported_3d_vectors')
-        os.makedirs(folder, exist_ok=True)
-        
-        if optic_flow:
-            fn = '3d_optic_flow_vectors_{}_{}.json'.format(self.get_specimen_name(), datetime.datetime.now())
-        else:
-            fn = '3d_vectors_{}_{}.json'.format(self.get_specimen_name(), datetime.datetime.now())
-        
-        data = {}
-        for eye in ['left', 'right']:
-            points, vectors = self.get_3d_vectors(eye, *args, *kwargs)
-            
-            data[eye] = {'points': points.tolist(), 'vectors': vectors.tolist()}
-        
-        with open(os.path.join(folder, fn), 'w') as fp:
-            json.dump(data, fp)
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/fitting.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/fitting.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/kinematics.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/kinematics.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/linked_data/electrophysiology.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/linked_data/electrophysiology.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/loading.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/loading.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import ast
 
 from gonioanalysis.rotary_encoders import to_degrees
 
 
 REPETITION_INDICATOR  = 'rep'
 POSITION_INDICATOR = 'pos'
+CAMERA_INDICATOR = '_cam{}'
 
 IMAGE_NAME_EXTENSIONS = ('.tiff', '.tif')
 
 
 def arange_fns(fns):
     '''
     Arange filenames based on REPETITION_INDICATOR and POSITION_INDICATOR
@@ -120,34 +121,39 @@
         #raise ValueError("Cannot find ')' after 'pos' in filename {}".format(fn))
         return (0,0)
     return ast.literal_eval(fn[i_start:i_end])
 
 
 
 def load_data(drosom_folder):
-    '''
-    Loads DrosoM imaging data from the following save structure
+    '''Loads GonioImsoft imaging data filenames into a dictionary.
 
-    DrosoM2
-        pos(0, 0)
-            .tif files
-        pos(20, 20)
-            .tif files
-        pos(0, 10)
-            .tif files
-        ...
+    The data has to be saved according to the folder hierarchy:
 
-    in a dictionary where the keys are str((horizontal, pitch)) and the items are
-    a list of image stacks:
-        
-        stacks_dictionary = {"(hor1, pitch1): [[stack_rep1], [stack_rep2], ...]"},
+        LEVEL   Content             Examples
+        1       specimen_folder     "DrosoM2"
+        2       image_folder        "pos(0, 0)" "pos(20, 20)") "pos(0, 10)_somesuffixhere"
+        3       image files         "im_pos(0, 0)_rep0_stack.tiff", "im_pos(0, 0)_rep0_cam2_stack.tiff"
+
+    Arguments
+    ---------
+    drosom_folder : string
+        Path to the specimen folder that contains the image folders.
+    
+    Returns
+    -------
+    stacks_dictionary : dict
+        Contains the str((horizontal, pitch)) as keys and a list of image stacks
+        as values.
         
-        where stack_rep1 = [image1_fn, image2_fn, ...].
+            stacks_dictionary = {"(hor1, pitch1): [[stack_rep1], [stack_rep2], ...]"},
+            where stack_rep1 = [image1_fn, image2_fn, ...].
     
-    Horizontal and pitch are given in rotatry encoder steps, not degrees.
+        Notice 1: The horizontal and pitch angles in the keys are in
+        rotary encoder steps (not degrees).
     
     '''
     
     stacks_dictionary = {}
 
     pos_folders = [fn for fn in os.listdir(drosom_folder) if os.path.isdir(os.path.join(drosom_folder, fn))]
 
@@ -162,31 +168,43 @@
         files = os.listdir(os.path.join(drosom_folder, folder))
         tiff_files = [f for f in files if f.endswith(IMAGE_NAME_EXTENSIONS)]
         
         if len(tiff_files) == 0:
             # Skip if no images in the folder
             continue
 
-        tiff_files = arange_fns(tiff_files)
-
-        stacks_dictionary[str_angles] = []
-
-        # Subdivide into repetitions
-        for tiff in tiff_files:
-            try:
-                i_repetition = int(tiff[tiff.index(REPETITION_INDICATOR)+len(REPETITION_INDICATOR):].split('_')[0])
-            except ValueError:
-                print('Warning: Cannot determine i_repetition for {}'.format(tiff))
-                i_repetition = 0
-
-            while i_repetition >= len(stacks_dictionary[str_angles]):
-                stacks_dictionary[str_angles].append([])
+        # Detect if many cameras have been used ("_cam{i}_" in any image filenames)      
+        cameras = {}
+        for i_camera in range(10):
+            indicator = CAMERA_INDICATOR.format(i_camera)
+            matching = [fn for fn in tiff_files if indicator in fn]
+            if matching:
+                cameras[f'_cam{i_camera}'] = matching
+
+        if not cameras:
+            cameras = {'': tiff_files}
+
+        
+        for camera, images in cameras.items():
+
+            cameras_images = arange_fns(images)
+            key = str_angles + camera
+            stacks_dictionary[key] = []
+
+            # Subdivide into repetitions
+            for tiff in cameras_images:
+                try:
+                    i_repetition = int(tiff[tiff.index(REPETITION_INDICATOR)+len(REPETITION_INDICATOR):].split('_')[0])
+                except ValueError:
+                    print('Warning: Cannot determine i_repetition for {}'.format(tiff))
+                    i_repetition = 0
+
+                while i_repetition >= len(stacks_dictionary[str_angles+camera]):
+                    stacks_dictionary[key].append([])
+                
+                stacks_dictionary[key][i_repetition].append(os.path.join(drosom_folder, folder, tiff))
             
-
-                        
-            stacks_dictionary[str_angles][i_repetition].append(os.path.join(drosom_folder, folder, tiff))
-        
-        # Remove empty lists, if one repetition index or more is missing from the data
-        stacks_dictionary[str_angles] = [alist for alist in stacks_dictionary[str_angles] if not alist == []]
+            # Remove empty lists, if one repetition index or more is missing from the data
+            stacks_dictionary[key] = [alist for alist in stacks_dictionary[key] if not alist == []]
 
     return stacks_dictionary
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/optic_flow.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/optic_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 '''
 Estimating optic flow field
 '''
 
 from math import cos, sin, radians
 
 import numpy as np
+import scipy
 from scipy.spatial import cKDTree as KDTree
 from scipy.stats import mannwhitneyu
 
 import gonioanalysis.coordinates as coordinates
 from gonioanalysis.drosom.analysing import MAnalyser
+from gonioanalysis.version import used_scipy_version
 
 
 def flow_direction(point, xrot=0):
     '''
     Estimates optic flow at the given point by placing the optic flow vector to
     the point, and forcing it to the tangent plane of the sphere.
 
@@ -65,16 +67,18 @@
     
     N_vectors = len(vectors_A)
 
     errors = np.empty(N_vectors)
 
     kdtree = KDTree(points_B)
     
-
-    distances, indices = kdtree.query(points_A, k=10, n_jobs=-1)
+    if used_scipy_version < (1,6,0):
+        distances, indices = kdtree.query(points_A, k=10, n_jobs=-1)
+    else:
+        distances, indices = kdtree.query(points_A, k=10, workers=-1)
     weights = 1/(np.array(distances)**2)
     
     # Check for any inf
     for i_weights in range(weights.shape[0]):
         if any(np.isinf(weights[i_weights])):
             weights[i_weights] = np.isinf(weights[i_weights]).astype('int')
 
@@ -150,15 +154,18 @@
     un_points_A, un_indices_A = _find_unique_points(points_A)
     un_points_B, un_indices_B = _find_unique_points(points_B)
 
     kdtree = KDTree(points_B)
     
     for point, indices_A in zip(un_points_A, un_indices_A):
         # Closest point
-        distance_B, index_B = kdtree.query(point, k=1, n_jobs=-1)
+        if used_scipy_version < (1,6,0):
+            distance_B, index_B = kdtree.query(point, k=1, n_jobs=-1)
+        else:
+            distance_B, index_B = kdtree.query(point, k=1, workers=-1)
         
         Avecs = [vectors_A[i] for i in indices_A]
         Bvecs = [vectors_B[i] for i in un_indices_B[index_B]]
         
         # Mean of Avecs
         mean_Avec = np.mean(Avecs, axis=0)
         
@@ -184,24 +191,32 @@
             
         print('inited')
         
         self.manalysers = [self]
         self.folder = 'optic_flow'
         self.eyes = ['left', 'right']
         self.vector_rotation = 0
-
+        
 
         # FAnalyser specific
         self.pitch_rot = 0
         self.roll_rot = 0
         self.yaw_rot = 0
         self.points = {'right': coordinates.optimal_sampling(np.arange(0, 60, 5), np.arange(-100, 100, 5)),
                 'left': coordinates.optimal_sampling(np.arange(-60, 0, 5), np.arange(-100, 100, 5))}
         
         self.constant_points = False
+        
+
+        self.ui_options = {
+                'pitch_rot': {'help': 'Pitch rotation', 'type': float},
+                'roll_rot': {'help': 'Roll rotation', 'type': float},
+                'yaw_rot': {'help': 'Yaw rotation', 'type': float},
+                }
+
 
     def get_3d_vectors(self, eye, constant_points=None, *args, **kwargs):
         '''
         
         constant_points : bool
             If true, points stay the same and only vectors get rotated.
             If false, smooth rotation of the whole optic flow sphere.
@@ -233,19 +248,20 @@
                 indices = [i for i, point in enumerate(points) if point[0] <= 0]
             elif eye == 'right':
                 indices = [i for i, point in enumerate(points) if point[0] >= 0]
 
             points = [points[i] for i in indices]
             vectors = [vectors[i] for i in indices]
         
-        return points, vectors
+        return np.array(points), np.array(vectors)
 
     
     def is_measured(self, *args, **kwargs):
         return True
 
     def are_rois_selected(self, *args, **kwargs):
         return True
 
     def load_analysed_movements(self, *args, **kwargs):
         return None
 
+
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/orientation_analysis.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/orientation_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 
 
                 extended_roi = [roi[0]-roi[2]/2, roi[1]-roi[3]/2, 2*roi[2], 2*roi[3]]
 
                 rois.append(extended_roi)
 
         fig, ax = plt.subplots(num='Draw arrows for the {} eye'.format(eye))
-        marker = Marker(fig, ax, images, self.MOVEMENTS_SAVEFN.format(eye),
+        marker = Marker(fig, ax, images, self._movements_savefn.format(eye),
                 relative_fns_from=os.path.join(self.data_path, self.folder),
                 drop_imagefn=True,
                 selection_type='arrow',
                 crops=rois,
                 callback_on_exit=lambda eye=eye: self._hotedit_marker_output(eye))
 
         marker.run()
@@ -72,15 +72,15 @@
 
 
     def _hotedit_marker_output(self, eye):
         '''
         Edits Marker output to be Movemeter like output.
         '''
 
-        with open(self.MOVEMENTS_SAVEFN.format(eye), 'r') as fp:
+        with open(self._movements_savefn.format(eye), 'r') as fp:
             marker_data = json.load(fp)
 
         edited_data = {}
 
         for image_folder, arrows in marker_data.items():
             
             repeats = []
@@ -91,17 +91,17 @@
                 repeats.append( {'x': [0, x1-x2], 'y': [0, y1-y2]} )
 
             # drop pos prefix [3:]
             if repeats != []:
                 edited_data[image_folder[3:]] = repeats
        
 
-        with open(self.MOVEMENTS_SAVEFN.format(eye), 'w') as fp:
+        with open(self._movements_savefn.format(eye), 'w') as fp:
             json.dump(edited_data, fp)
 
    
     
     def is_measured(self):
-        fns = [self.MOVEMENTS_SAVEFN.format(eye) for eye in self.eyes]
+        fns = [self._movements_savefn.format(eye) for eye in self.eyes]
         return all([os.path.exists(fn) for fn in fns])
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/basics.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 EYE_COLORS = {'right': 'blue', 'left': 'red'}
 REPEAT_COLORS = ['green', 'orange', 'pink']
 
 
 DEFAULT_ELEV = 10
 DEFAULT_AZIM = 70
 DEFAULT_FIGSIZE = (16,9)
+DEFAULT_DPI = 100
 
 def plot_1d_magnitude(manalyser, image_folder=None, i_repeat=None,
         mean_repeats=False, mean_imagefolders=False, mean_eyes=False,
         color_eyes=False, gray_repeats=False, progressive_colors=False,
         show_mean=False, show_std=False,
         show_label=True, milliseconds=False, microns=False,
         phase=False, derivative=False,
@@ -519,15 +520,15 @@
         
         # OAnalyser specific for Drosophila; Assuming that R3-R6 line is
         # analysed, let's also draw the line from R3 to R1.
         if arrow_rotations[0] == 0 and len(arrow_rotations) == 1:
             arrow_rotations.append(29)
 
     if ax is None:
-        fig = plt.figure(figsize=DEFAULT_FIGSIZE)
+        fig = plt.figure(figsize=kwargs.pop('figsize', DEFAULT_FIGSIZE), dpi=kwargs.pop('dpi', DEFAULT_DPI))
         ax = fig.add_subplot(111, projection='3d')
     
     vectors = {}
 
     original_rotation = manalyser.vector_rotation
 
     if animation_type == 'rotate_plot':
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/common.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
  
 from gonioanalysis.coordinates import (
         nearest_neighbour,
         get_rotation_matrix,
         rotate_points
         )
 from gonioanalysis.directories import ANALYSES_SAVEDIR
+from gonioanalysis.version import used_scipy_version
+
 
 CURRENT_ARROW_LENGTH = 1
 
 VECTORMAP_PULSATION_PARAMETERS = {'step_size': 0.02, 'low_val': 0.33, 'high_val': 1}
 
 
 
@@ -42,18 +44,28 @@
 class Arrow3D(FancyArrowPatch):
     def __init__(self, x0, y0, z0, x1, y1, z1, *args, **kwargs):
         FancyArrowPatch.__init__(self, (0,0), (0,0), *args, **kwargs)
         self._verts3d = (x0, x1), (y0, y1), (z0, z1)
 
     def draw(self, renderer):
         xs3d, ys3d, zs3d = self._verts3d
-        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, renderer.M)
+        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, self.axes.M)
         self.set_positions((xs[0],ys[0]),(xs[1],ys[1]))
         FancyArrowPatch.draw(self, renderer)
 
+    def do_3d_projection(self, renderer=None):
+        '''Fix for newer matplotlib versions.
+        See https://github.com/matplotlib/matplotlib/issues/21688
+        '''
+        xs3d, ys3d, zs3d = self._verts3d
+        xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, self.axes.M)
+        self.set_positions((xs[0],ys[0]),(xs[1],ys[1]))
+
+        return np.min(zs)
+
 
 def add_line(ax, x0, y0, z0, x1, y1, z1, camerapos=None, **kwargs):
     '''
     Add a centered 3D line plot
     '''
     if camerapos and is_behind_sphere(*camerapos, (x0,y0,z0)):
         return None
@@ -409,16 +421,16 @@
     else:
         ax.set_xlabel('x')
         ax.set_ylabel('y')
         ax.set_zlabel('z')
 
 
 
-    if not camerapos:
-        camerapos = (ax.elev, ax.azim)
+    #if not camerapos:
+    #    camerapos = (ax.elev, ax.azim)
  
     if guidance:
         plot_guidance(ax, camerapos=camerapos, hide_text=hide_text)
 
     if draw_sphere:
         N = 75
         phi, theta = np.meshgrid(np.linspace(0, 2*np.pi, N), np.linspace(0, np.pi, N))
@@ -543,17 +555,20 @@
 
         x = (np.sin(theta) * np.cos(phi))
         y = (np.sin(theta) * np.sin(phi))
         z = np.cos(theta)
         
         errs = np.empty_like(x)
         positions = [[x.flat[i], y.flat[i], z.flat[i]] for i in range(x.size)]
-
-        distances, i_points = kdtree.query( positions, n_jobs=-1 )
         
+        if used_scipy_version < (1,6,0):
+            distances, i_points = kdtree.query( positions, n_jobs=-1 )
+        else:
+            distances, i_points = kdtree.query( positions, workers=-1 )
+
         for i in range(errs.size):
             if distances[i] < intp_dist:
                 errs.flat[i] = values[i_points[i]]
             else:
                 errs.flat[i] = 0
         return errs
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/compare_opticflow.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/compare_opticflow.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/plotting/illustrate_experiments.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/plotting/illustrate_experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from scipy.spatial import cKDTree as KDTree
 import cv2
 
 from gonioanalysis.directories import ANALYSES_SAVEDIR
 import gonioanalysis.coordinates as coordinates
 from gonioanalysis.drosom.plotting.common import vector_plot
 from gonioanalysis.drosom.loading import angles_from_fn
-
+from gonioanalysis.version import used_scipy_version
 
 def _load_image(fn, roi, e):
 
     image = tifffile.imread(fn)
     
     x,y,w,h = [int(round(z)) for z in roi]
     
@@ -515,15 +515,18 @@
 
     intp_v = np.arange(vmin, vmax, vstep)[::-1]
     intp_h = np.arange(hmin, hmax, hstep)
 
     for i_v, vrot in enumerate(intp_v):
         for i_h, hrot in enumerate(intp_h):
             
-            distance, i_point = kdtree.query( (hrot, vrot), n_jobs=-1)
+            if used_scipy_version < (1,6,0):
+                distance, i_point = kdtree.query( (hrot, vrot), n_jobs=-1)
+            else:
+                distance, i_point = kdtree.query( (hrot, vrot), workers=-1)
             
             if distance > math.sqrt((hstep/1.5)**2 + (vstep/1.5)**2):
                 continue
 
             plot_data.append((i_v, i_h, i_point))
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/reports/left_right.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/reports/left_right.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/reports/pdf_summary.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/reports/pdf_summary.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/reports/repeats.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/reports/repeats.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/reports/stats.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/reports/stats.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/sinesweep.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/sinesweep.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/special/norpa_rescues.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/special/norpa_rescues.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/special/paired.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/special/paired.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/terminal.py` & `gonio-analysis-0.7.0/gonioanalysis/tkgui/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,318 +1,254 @@
-#!/usr/bin/env python3
-'''
-Analyse Gonio Imsoft data and output the results.
-'''
-import sys
-import os
-import datetime
-import argparse
 
-import numpy as np
-import matplotlib.pyplot as plt
+import os
+import subprocess
+import sys
+import platform
 
-from gonioanalysis.drosom import analyser_commands
-from gonioanalysis.drosom.analyser_commands import (
-        ANALYSER_CMDS,
-        DUALANALYSER_CMDS,
-        MULTIANALYSER_CMDS,
-        )
-from gonioanalysis.directories import ANALYSES_SAVEDIR, PROCESSING_TEMPDIR_BIGFILES
-from gonioanalysis.droso import DrosoSelect
-from gonioanalysis.antenna_level import AntennaLevelFinder
-from gonioanalysis.drosom.analysing import MAnalyser, MAverager
+from gonioanalysis.droso import SpecimenGroups
+from gonioanalysis.directories import CODE_ROOTDIR
+from gonioanalysis.drosom.analysing import MAnalyser
 from gonioanalysis.drosom.orientation_analysis import OAnalyser
-from gonioanalysis.drosom.optic_flow import FAnalyser
 from gonioanalysis.drosom.transmittance_analysis import TAnalyser
-from gonioanalysis.drosom import plotting
-from gonioanalysis.drosom.plotting.plotter import MPlotter
-from gonioanalysis.drosom.plotting import complete_flow_analysis, error_at_flight
-from gonioanalysis.drosom.special.norpa_rescues import norpa_rescue_manyrepeats
-from gonioanalysis.drosom.special.paired import cli_group_and_compare
-import gonioanalysis.drosom.reports as reports
+from gonioanalysis.directories import ANALYSES_SAVEDIR
 
 
-if '--tk_waiting_window' in sys.argv:
-    from gonioanalysis.tkgui.widgets import WaitingWindow
+class Core:
+    '''
+    Tkinter independent functions, reusable for other GUI implementations.
+    
+    Attributes
+    ----------
+    data_directory : list of strings
+        Current data directories
+    current_specimen : string
+        Name of the current specimen
+    analyser : object
+        MAnalyser (or OAnalsyer) object of the current specimen
+    selected_recording : string
+        Selected recording name (image_folder)
+    analyser_class : class
+        Class of the new analysers to create (MAnalyser or OAnalyser)
+    analyser_classes: list of classes
+        List of available analyser classes for reference
+    active_analysis : string or None
+        Name of the active analysis
+    '''
 
+    def __init__(self):
+        
+        self.data_directory = []
+        self.current_specimen = None
+        self.analyser = None
+        self.selected_recording = None
+        
+        self.analyser_class = MAnalyser
+        self.analyser_classes = [MAnalyser, OAnalyser, TAnalyser]
+        
+        self.active_analysis = None
 
+        self._folders = {}
 
-Analysers = {'orientation': OAnalyser, 'motion': MAnalyser, 'flow': FAnalyser,
-        'transmittance': TAnalyser}
+        self.groups = SpecimenGroups()
 
-analyses = {**ANALYSER_CMDS, **DUALANALYSER_CMDS, **MULTIANALYSER_CMDS}
 
+    def set_data_directory(self, data_directory):
+        '''
+        Update Core's knowledge about the currently selected data_directory.
 
-def roimovement_video(analyser):
-    '''
-    Create a video where the imaging data is played and the analysed ROI is moved on the
-    image, tracking the moving feature.
+        Arguments
+        ---------
+        data_directory : list of strings
+            List of paths to the data
+        '''
+        self.data_directory = data_directory
+        
+        self._folders = {}
+        for data_directory in self.data_directory:
+            self._folders[data_directory] = os.listdir(data_directory)
 
-    Good for confirming visually that the movment analysis works.
-    '''
 
-    print(analyser.getFolderName())
-    images, ROIs, angles = analyser.get_time_ordered()
-    
-    workdir = os.path.join(PROCESSING_TEMPDIR_BIGFILES, 'movie_{}'.format(str(datetime.datetime.now())))
-    os.makedirs(workdir, exist_ok=True)
+    def set_current_specimen(self, specimen_name):
+        '''
+        Update Core's knowledge about the currently selected specimen.
+        '''
+        self.current_specimen = specimen_name
+        self.analyser = self.get_manalyser(specimen_name)
 
-    newnames = [os.path.join(workdir, '{:>0}.jpg'.format(i)) for i in range(len(images))]
     
-
-    adj = ROIAdjuster()
-    newnames = adj.writeAdjusted(images, ROIs, newnames, extend_factor=3, binning=1)
+    def set_selected_recording(self, selected_recording):
+        self.selected_recording = selected_recording
     
-    enc = Encoder()
-    fps = 25
-    enc.encode(newnames, os.path.join(ANALYSES_SAVEDIR, 'movies','{}_{}fps.mp4'.format(analyser.getFolderName(), fps)), fps)
- 
-    for image in newnames:
-        os.remove(image)
-    try:
-        os.rmdir(workdir)
-    except OSError:
-        print("Temporal directory {} left behind because it's not empty".format(workdir))
-       
 
-   
-def export_optic_flow():
-    '''
-    Exports the optic flow vectors.
-    '''
-    import json
-    from gonioanalysis.coordinates import optimal_sampling
-    from gonioanalysis.drosom.optic_flow import flow_vectors
-    points = optimal_sampling(np.arange(-90, 90, 5), np.arange(-180, 180, 5))
-    vectors = flow_vectors(points)
-    
-    with open('optic_flow_vectors.json', 'w') as fp:
-        json.dump({'points': np.array(points).tolist(), 'vectors': np.array(vectors).tolist()}, fp)
-            
+    def set_analyser_class(self, class_name):
+        index = [i for i, ac in enumerate(self.analyser_classes) if ac.__name__ == class_name]
+        self.analyser_class = self.analyser_classes[index[0]]
+        
+        if self.data_directory:
+            self.update_gui(changed_specimens=True)
 
 
-         
-def main(custom_args=None):
-    
-    if custom_args is None:
-        custom_args = sys.argv[1:]
-    
-    parser = argparse.ArgumentParser(description=__doc__)
-    
-    
-    # DATA ARGUMENTS
-    parser.add_argument('-D', '--data_directory', nargs='+',
-            help='Data directory')
-
-    parser.add_argument('-S', '--specimens', nargs='+',
-            help=('Comma separeted list of specimen names.'
-                ' Separate groups by space when averaging is on.'
-                ' If needed, wanted image folders can be specified with semicolons'
-                ' for example, specimen1;imf1;imf2:specimen2;imf1'
-                ' (does not work with groups). If image folders contain commas, use'
-                ' semicolons, use colons (:) to separate specimens'))
-    
+    def list_specimens(self, with_rois=None, with_movements=None, with_correction=None):
+        '''
+        List specimens in the data directory. May contain bad folders also (no check for contents)
 
-    # Analyser settings
-    parser.add_argument('-a', '--average', action='store_true',
-            help='Average and interpolate the results over the specimens')
-    
-    parser.add_argument('--short-name', nargs=1,
-            help='Short name to set if --average is set')
+        With the following keyword arguments one select only the specimens fulfilling the conditions
+        by setting the keyword argument either to True (has to fulfill condition), False (negative)
+        or to None (the condition is not considered)
 
-    parser.add_argument('-t', '--type', nargs='+',
-            help='Analyser type, either "motion" or "orientation". Space separate gor groups')
-    
-    parser.add_argument('-r', '--reselect-rois', action='store_true',
-            help='Reselect ROIs')
- 
-    parser.add_argument('-R', '--recalculate-movements', action='store_true',
-            help='Recalculate with Movemeter')
-
-    parser.add_argument('--reverse-directions', action='store_true',
-            help='Reverse movement directions')
-
-    parser.add_argument('--active-analysis', nargs='?', default='',
-            help='Name of the analysis')
-
-    # Other settings
-    parser.add_argument('--tk_waiting_window', action='store_true',
-            help='(internal) Launches a tkinter waiting window')
-    parser.add_argument('--dont-show', action='store_true',
-            help='Skips showing the plots')
-    parser.add_argument('--worker-info', nargs=2,
-            help='Worker id and total number of parallel workers. Only 3D video plotting now')
-
-    # Different analyses for separate specimens
-
-    parser.add_argument('-A', '--analysis', nargs=1,
-            choices=analyses.keys(),
-            help='Analysis method or action. Allowed analyses are '+', '.join(analyses.keys()))
+            with_rois           Specimens with ROIs selected
+            with_movements      Specimens with movements measured
+            with_correction     Specimens with antenna_level (zero level) correction
+        
+        For example, if you want the specimens with movements but without antenna_level corrections
+        and you won't care about ROIs, set
+            with_rois=None, with_movements=True, with_correction=False
+
+        '''
+        specimens = []
+        for data_directory in self.data_directory:
+            specimens.extend( [fn for fn in os.listdir(data_directory) if os.path.isdir(os.path.join(data_directory, fn))] )
+        
+        if with_rois is not None:
+            specimens = [specimen for specimen in specimens if self.get_manalyser(specimen, no_data_load=True).are_rois_selected() == with_rois]
+        
+        if with_movements is not None:
+            specimens = [specimen for specimen in specimens if self.get_manalyser(specimen, no_data_load=True).is_measured() == with_movements]
+        
+        if with_correction is not None:
+            specimens = [specimen for specimen in specimens if self.get_manalyser(specimen, no_data_load=True).get_antenna_level_correction() is not False]
 
-    args = parser.parse_args(custom_args)
+        return sorted(specimens)
     
 
+    def get_specimen_fullpath(self, specimen_name=None):
+        '''
+        Returns the full path of a specimen (datadir + specimen_patch)
+        
+        Arguments
+        ---------
+        specimen_namse : string or None
+            If None use self.current_specimen
+        '''
+        if specimen_name is None:
+            specimen_name = self.current_specimen
 
+        for directory in self.data_directory:
+            if specimen_name in self._folders[directory]:
+                return os.path.join(directory, specimen_name)
 
-    if args.tk_waiting_window:
-        waiting_window = WaitingWindow('terminal.py', 'When ready, this window closes.')
+        raise ValueError("no specimen with name {}".format(specimen_name))
 
-    if args.worker_info:
-        analyser_commands.I_WORKER = int(args.worker_info[0])
-        analyser_commands.N_WORKERS = int(args.worker_info[1])
-
-    # Getting the data directory
-    # --------------------------
-    if args.data_directory:
-        print('Using data directory {}'.format(args.data_directory[0]))
-        
-        data_directories = args.data_directory
-    else:
-        data_directories = input('Data directory >> ')
-    
-    # Check that the data directory exists
-    for directory in data_directories:
-        if not os.path.isdir(directory):
-            raise ValueError("{} is not a directory".format(directory))
-
-    # {specimen name : [image_folder_1, ...]}
-    wanted_imagefolders = {}
-
-    # Getting the specimens
-    # ---------------------
-    directory_groups = []
-    if args.specimens:
-        
-        for group in args.specimens:
-            print('Using specimens {}'.format(group))
-            
-            if group == 'none':
-                directory_groups.append(None)
-                continue
 
-            if ':' in group:
-                specimen_separator = ':'
-            else:
-                specimen_separator = ','
+    def _configure_analyser(self, analyser):
+        if self.active_analysis:
+            analyser.active_analysis = self.active_analysis
+        return analyser
 
-            if ';' in group:
-                
-                for specimen in group.split(specimen_separator):
-                    if ';' in specimen:
-                        splitted = specimen.split(';')
-                        wanted_imagefolders[splitted[0]] = splitted[1:]
-                
-                # Remove specified imagefolders
-                group = ','.join([z.split(';')[0] for z in group.split(specimen_separator)])
-            
-            
-            # dont commit me
-            group = group.replace(':', ',')
-            
-            
-            directories = []
-            for directory in data_directories:
-                selector = DrosoSelect(datadir=directory)
-                directories.extend( selector.parse_specimens(group) )
-            directory_groups.append(directories)
-    else:
-        selector = DrosoSelect(datadir=data_directories[0])
-        directories = selector.ask_user()
-     
-            
-    # Setting up analysers
-    # ---------------------
-    
-    if not args.type:
-        args.type = ['motion' for i in directory_groups]
 
-    analyser_groups = []
+    def get_manalyser(self, specimen_name, **kwargs):
+        '''
+        Gets manalyser for the specimen specified by the given name.
+        '''
+        for directory in self.data_directory:
+            if specimen_name in self._folders[directory]:
+                break
+
+        analyser = self.analyser_class(directory, specimen_name, **kwargs)
+
+        return self._configure_analyser(analyser)
     
-    for i_group, directories in enumerate(directory_groups):
 
+    def get_manalysers(self, specimen_names, **kwargs):
+        '''
+        Like get_manalyser but returns a list of analyser objects and also
+        checks for specimen groups if a specimen cannot be found.
+        '''
         analysers = []
-        Analyser = Analysers[args.type[i_group]]
-        
-        print('Using {}'.format(Analyser.__name__))
+        for name in specimen_names:
+            try:
+                ans = [self.get_manalyser(name, **kwargs)]
+            except FileNotFoundError:
+                ans = [self.get_manalyser(n, **kwargs) for n in self.groups.groups.get(name, [])]
+                
+                # Try again and load
+                if ans is []:
+                    self.groups.load_groups()
+                    ans = [self.get_manalyser(n, **kwargs) for n in self.groups.groups.get(name, [])]
+            
+            if ans is []:
+                raise FileNotFoundError('Cannot find specimen {}'.format(name))
+            
+            for an in ans:
+                analysers.append( self._configure_analyser(an) )
+
+        return analysers
+
+
+    def adm_subprocess(self, specimens, terminal_args, open_terminal=False):
+        '''
+        Invokes drosom/terminal.py
+        
+        Arguments
+        ---------
+        specimens : list of string
+            List of specimen names or 'current'
+        terminal_args : string
+            Agruments passed to the plotter
+        open_terminal : bool
+            If true open in a cmd window (on Windows) or lxterm (on Linux)
+        '''
+        
+        # 1) Find python executable and wrap the filename by quation marks if spaces present
+        python = sys.executable
+        if ' ' in python:
+            python = '"' + python + '"'
+
+       
+        # 2) Find the full path to the adm Python file in the gonio root
+        pyfile = os.path.join(CODE_ROOTDIR, 'drosom/terminal.py')
         
-        if directories is None:
-            analysers.append(Analyser(None, None))
+        # Check for spaces in the filename. If there are spaces in the filename,
+        # we have to encapsulate the filename by quation marks
+        if ' ' in pyfile:
+            pyfile = '"' + pyfile + '"'
+
+        # 3) Get the specimen directoires (full paths separated by space)
+        if specimens == 'current':
+            specimen_names = self.analyser.folder
         else:
+            specimen_names = ':'.join(specimens)
+            if not ':' in specimen_names:
+                specimen_names += ':'
+        
+        if self.active_analysis not in ['default', '', None]:
+            terminal_args += ' --active-analysis '+ self.active_analysis
+
+        arguments = '-D "{}" -S "{}" {}'.format(' '.join(self.data_directory), specimen_names, terminal_args)
+        
+        if self.analyser_class is MAnalyser:
+            pass
+        elif self.analyser_class is OAnalyser:
+            arguments = '--type orientation ' + arguments
+        elif self.analyser_class is TAnalyser:
+            arguments = '--type transmittance ' + arguments
+        else:
+            raise NotImplementedError
 
-            for directory in directories: 
-                
-                path, folder_name = os.path.split(directory)
-                analyser = Analyser(path, folder_name) 
-                
-                if args.active_analysis:
-                    analyser.active_analysis = args.active_analysis
-                
-                analysers.append(analyser)
- 
-        # Ask ROIs if not selected
-        for analyser in analysers:
-            if analyser.are_rois_selected() == False or args.reselect_rois:
-                analyser.select_ROIs()
-
-        # Analyse movements if not analysed, othewise load these
-        for analyser in analysers:
-            if analyser.is_measured() == False or args.recalculate_movements:
-                analyser.measure_movement(eye='left')
-                analyser.measure_movement(eye='right')
-            analyser.load_analysed_movements()
-        
-        
-        if args.reverse_directions:
-            for analyser in analysers:
-                analyser.receptive_fields = True
+        command = '{} {} {} &'.format(python, pyfile, arguments)
         
-       
-
-        if args.average:
-            
-            if len(analysers) >= 2:
-
-                avg_analyser = MAverager(analysers)
-                avg_analyser.setInterpolationSteps(5,5)
-                
-                if args.short_name:
-                    avg_analyser.set_short_name(args.short_name[0])
-                           
-                analysers = avg_analyser
+        if open_terminal:
+            if platform.system() == 'Linux':
+                command = 'lxterm -e ' + command
+            elif platform.system() == 'Windows':
+                command = 'start /wait ' + command
             else:
-                analysers = analysers[0]
-        else:
-            if len(analysers) == 1:
-                analysers = analysers[0]
-
-        analyser_groups.append(analysers)
-    
+                raise OSError('Operating system not supported by gonio?')
 
-    function = analyses[args.analysis[0]]
-    
-    print(analyser_groups)
-    
-    kwargs = {}
-    if wanted_imagefolders:
-        kwargs['wanted_imagefolders'] = wanted_imagefolders
-    
-    if function in MULTIANALYSER_CMDS.values():
-        for analysers in analyser_groups:
-            function(analysers, **kwargs)
-    elif args.average or function in DUALANALYSER_CMDS.values():
-        function(*analyser_groups, **kwargs)
-    else:
-        for analysers in analyser_groups:
-            if not isinstance(analysers, list):
-                analysers = [analysers]
-            for analyser in analysers:
-                function(analyser, **kwargs)
-
-    if args.tk_waiting_window:
-        waiting_window.close()
+        print(command)
+        
+        subprocess.run(command, shell=True)
 
-    if not args.dont_show:
-        plt.show()
 
+    def update_gui(self, changed_specimens=False):
+        raise ValueError("GUI should overload update_gui method in Core core.py")
 
-if __name__ == "__main__":
-    main()
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosom/transmittance_analysis.py` & `gonio-analysis-0.7.0/gonioanalysis/drosom/transmittance_analysis.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosox/analysing.py` & `gonio-analysis-0.7.0/gonioanalysis/drosox/analysing.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosox/loading.py` & `gonio-analysis-0.7.0/gonioanalysis/drosox/loading.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosox/plotting.py` & `gonio-analysis-0.7.0/gonioanalysis/drosox/plotting.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/drosox/terminal.py` & `gonio-analysis-0.7.0/gonioanalysis/drosox/terminal.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/image_tools.py` & `gonio-analysis-0.7.0/gonioanalysis/image_tools.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/dpp.tif` & `gonio-analysis-0.7.0/gonioanalysis/images/dpp.tif`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/droso_roll.png` & `gonio-analysis-0.7.0/gonioanalysis/images/droso_roll.png`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/from_mikko.png` & `gonio-analysis-0.7.0/gonioanalysis/images/from_mikko.png`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/from_mikko_annotated.png` & `gonio-analysis-0.7.0/gonioanalysis/images/from_mikko_annotated.png`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/mikkos_alternative_fly.png` & `gonio-analysis-0.7.0/gonioanalysis/images/mikkos_alternative_fly.png`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/rotation_roll.png` & `gonio-analysis-0.7.0/gonioanalysis/images/rotation_roll.png`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/rotation_yaw.png` & `gonio-analysis-0.7.0/gonioanalysis/images/rotation_yaw.png`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/images/side_aligning_pupil_antenna_whiteBG.jpg` & `gonio-analysis-0.7.0/gonioanalysis/images/side_aligning_pupil_antenna_whiteBG.jpg`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/rotary_encoders.py` & `gonio-analysis-0.7.0/gonioanalysis/rotary_encoders.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/settings.py` & `gonio-analysis-0.7.0/gonioanalysis/settings.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/tkgui/examine.py` & `gonio-analysis-0.7.0/gonioanalysis/tkgui/examine.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/tkgui/menu_commands.py` & `gonio-analysis-0.7.0/gonioanalysis/tkgui/menu_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,28 @@
 
 import gonioanalysis
 from gonioanalysis.directories import USER_HOMEDIR, ANALYSES_SAVEDIR
 from gonioanalysis.droso import SpecimenGroups
 from gonioanalysis.drosom import linked_data
 from gonioanalysis.drosom import kinematics
 from gonioanalysis.drosom import sinesweep
+from gonioanalysis.drosom import export
 from gonioanalysis.drosom.reports.left_right import left_right_displacements, lrfiles_summarise
 from gonioanalysis.drosom.reports.repeats import mean_repeats, repeat_stds
 from gonioanalysis.drosom.reports.stats import response_magnitudes
 from gonioanalysis.tkgui import settings
 from gonioanalysis.tkgui.run_measurement import MeasurementWindow
 from gonioanalysis.tkgui.widgets import (
         select_specimens,
         select_specimen_groups,
         ZeroCorrect,
         CompareVectormaps,
         ImagefolderMultisel,
         )
-        
+
 
 
 
 def ask_string(title, prompt, tk_parent):
     '''
     Asks the user for a string.
     '''
@@ -320,23 +321,20 @@
         self.core.adm_subprocess('current', '-A vectormap')
 
 
     def vectormap_DASH_rotating_video(self):
         self.core.adm_subprocess('current', '--tk_waiting_window -A vectormap_video')
 
     
-    def vectormap_DASH_export_npy(self):
+    def vectormap_DASH_export(self):
         analysername = self.core.analyser.get_specimen_name()
-        fn = tk.filedialog.asksaveasfilename(initialfile=analysername, defaultextension='.npy')
+        fn = tk.filedialog.asksaveasfilename(initialfile=analysername, defaultextension='.npy', filetypes=export.FILETYPES)
         if fn:
-            base = fn.rstrip('.npy')
-            for eye in ['left', 'right']:
-                d3_vectors = self.core.analyser.get_3d_vectors(eye)
-                np.save(base+'_'+eye+'.npy', d3_vectors)
-
+            self.core.adm_subprocess('current', f'-A export_vectormap --output "{fn}"')
+            
     
     def mean_displacement_over_time(self):
         self.core.adm_subprocess('current', '-A magtrace')
 
 
     def mean_latency_by_sigmoidal_fit(self):
         results_string = ''
@@ -356,14 +354,15 @@
 
     def _force_order(self):
         return ['measure_movements_DASH_list_all', 'measure_movements_DASH_list_only_unmeasured',
                 'measure_movements_DASH_in_absolute_coordinates',
                 '.',
                 'averaged_vectormap_DASH_interactive_plot', 'averaged_vectormap_DASH_rotating_video',
                 'averaged_vectormap_DASH_rotating_video_DASH_set_title',
+                'averaged_vectormap_DASH_export',
                 '.',
                 'compare_vectormaps',
                 '.',
                 'comparision_to_optic_flow_DASH_video',
                 '.',
                 'export_LR_displacement_CSV',
                 'export_LR_displacement_CSV_DASH_strong_weak_eye_division',
@@ -429,16 +428,25 @@
 
 
         select_specimens(self.core, run_workers, with_movements=True) 
         
 
     def averaged_vectormap_DASH_rotating_video_DASH_set_title(self):
         ask_string('Set title', 'Give video title', lambda title: select_specimens(self.core, lambda specimens: self.core.adm_subprocess(specimens, '--tk_waiting_window --average --short-name {} -A vectormap_video'.format(title)), with_movements=True)) 
+ 
+
+    def averaged_vectormap_DASH_export(self):
+        def target(specimens):
+            fn = tk.filedialog.asksaveasfilename(initialfile='average', defaultextension='.npy')
+            if fn:
+                self.core.adm_subprocess(specimens, f'--average -A export_vectormap --output {fn}')
+        select_specimens(self.core, target)
         
 
+
     def compare_vectormaps(self):
         popup(self.tk_root, CompareVectormaps, args=[self.core],
                 title='Vectormap comparison')
        
 
     def comparision_to_optic_flow_DASH_video(self): 
         select_specimens(self.core, lambda specimens: self.core.adm_subprocess(specimens, '--tk_waiting_window --average -A flow_analysis_pitch'), with_movements=True)
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/tkgui/plotting.py` & `gonio-analysis-0.7.0/gonioanalysis/tkgui/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,24 +124,23 @@
         
         try:
             self.slider_ax
         except AttributeError:
             self.slider_ax = fig.add_axes([0.2, 0.01, 0.6, 0.05])
         
         # Get a list of image filenames and how many
-        image_fns = self.core.analyser.list_images(self.selected_recording)
+        image_fns = self.core.analyser.list_images(self.selected_recording, absolute_path=True)
         self.N_repeats = len(image_fns)
 
         if self.i_repeat:
             i_frame = self.i_repeat
         else:
             i_frame = 0
         
-        image_fn = os.path.join(self.core.analyser.get_specimen_directory(), self.selected_recording, image_fns[i_frame])
-        
+        image_fn = image_fns[i_frame]
         self.image = tifffile.TiffFile(image_fn).asarray(key=0)
 
         try:
             self.range_slider
         except AttributeError:
             self.range_slider = matplotlib.widgets.Slider(self.slider_ax, 'Range %' , 0, 100, valinit=90, valstep=1)
             self.range_slider.on_changed(self.update_ROI_plot)
```

### Comparing `gonio-analysis-0.6.0/gonioanalysis/tkgui/run_measurement.py` & `gonio-analysis-0.7.0/gonioanalysis/tkgui/run_measurement.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/gonioanalysis/tkgui/widgets.py` & `gonio-analysis-0.7.0/gonioanalysis/tkgui/widgets.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/scripts/add_gridlines.py` & `gonio-analysis-0.7.0/scripts/add_gridlines.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/scripts/create_alr_data.py` & `gonio-analysis-0.7.0/scripts/create_alr_data.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/scripts/drosox_spin.py` & `gonio-analysis-0.7.0/scripts/drosox_spin.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/scripts/framepuller.py` & `gonio-analysis-0.7.0/scripts/framepuller.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/scripts/optimal_sampling.py` & `gonio-analysis-0.7.0/scripts/optimal_sampling.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/scripts/plot_spatial_calibration.py` & `gonio-analysis-0.7.0/scripts/plot_spatial_calibration.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/scripts/videowrapper.py` & `gonio-analysis-0.7.0/scripts/videowrapper.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/setup.py` & `gonio-analysis-0.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,32 +7,38 @@
 exec(open("gonioanalysis/version.py").read())
 
 install_requires = [
         'numpy',
         'scipy',
         'tifffile',
         'matplotlib',
-        'tk-steroids>=0.6.0',
+        'tk-steroids>=0.7.1',
         'roimarker>=0.2.0',
-        'movemeter>=0.4.0',
+        'movemeter>=0.5.0',
         'python-biosystfiles',
         ]
 
 
 setuptools.setup(
     name="gonio-analysis",
     version=__version__,
     author="Joni Kemppainen",
-    author_email="jjtkemppainen1@sheffield.ac.uk",
+    author_email="joni.kemppainen@windowslive.com",
     description="Spatial motion analysis program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jkemppainen/gonio-analysis",
     packages=setuptools.find_packages(),
     install_requires=install_requires, 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3) ",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.0',
+    # Used language features that require Python 3.6 or newer
+    #   - fstrings
+    #
+    #
+    # Python 3.8 final version supporting Windows 7
+    # Python 3.4 final version supporting Windows XP
+    python_requires='>=3.6',
 )
```

### Comparing `gonio-analysis-0.6.0/tests/test_terminal.py` & `gonio-analysis-0.7.0/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/windows_installer/get_tkdeps.py` & `gonio-analysis-0.7.0/windows_installer/get_tkdeps.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/windows_installer/logo_colored.ico` & `gonio-analysis-0.7.0/windows_installer/logo_colored.ico`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/windows_installer/make_installer.py` & `gonio-analysis-0.7.0/windows_installer/make_installer.py`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/windows_installer/movemeter_logo.ico` & `gonio-analysis-0.7.0/windows_installer/movemeter_logo.ico`

 * *Files identical despite different names*

### Comparing `gonio-analysis-0.6.0/windows_installer/pynsist_template.cfg` & `gonio-analysis-0.7.0/windows_installer/pynsist_template.cfg`

 * *Files identical despite different names*

