# Comparing `tmp/ReadROOT-2.4.0.tar.gz` & `tmp/ReadROOT-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadROOT-2.4.0.tar", last modified: Mon Aug  7 16:48:11 2023, max compression
+gzip compressed data, was "ReadROOT-2.4.1.tar", last modified: Tue Aug  8 15:28:44 2023, max compression
```

## Comparing `ReadROOT-2.4.0.tar` & `ReadROOT-2.4.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 16:48:11.817793 ReadROOT-2.4.0/
--rw-rw-rw-   0        0        0    16128 2023-02-15 23:51:19.000000 ReadROOT-2.4.0/ErrorPropagation.py
--rw-rw-rw-   0        0        0     5152 2023-06-14 20:31:08.000000 ReadROOT-2.4.0/IOClasses.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:48:11.662942 ReadROOT-2.4.0/Images/
--rw-rw-rw-   0        0        0     1802 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/Calculate.png
--rw-rw-rw-   0        0        0     2340 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/Clear.png
-drwxrwxrwx   0        0        0        0 2023-08-07 16:48:11.707922 ReadROOT-2.4.0/Images/CoMPASS/
--rw-rw-rw-   0        0        0     2712 2023-05-23 14:31:42.000000 ReadROOT-2.4.0/Images/CoMPASS/Coincidence.png
--rw-rw-rw-   0        0        0     2292 2023-05-23 14:18:04.000000 ReadROOT-2.4.0/Images/CoMPASS/Discriminator.png
--rw-rw-rw-   0        0        0     2492 2023-05-23 14:27:57.000000 ReadROOT-2.4.0/Images/CoMPASS/EnergyCalibration.png
--rw-rw-rw-   0        0        0     2492 2023-05-23 14:13:06.000000 ReadROOT-2.4.0/Images/CoMPASS/Input.png
--rw-rw-rw-   0        0        0     2547 2023-05-23 14:32:49.000000 ReadROOT-2.4.0/Images/CoMPASS/Misc.png
--rw-rw-rw-   0        0        0     1089 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/CoMPASS/OpenGraph.png
--rw-rw-rw-   0        0        0     2499 2023-05-23 14:20:06.000000 ReadROOT-2.4.0/Images/CoMPASS/QDC.png
--rw-rw-rw-   0        0        0     2282 2023-05-23 14:25:56.000000 ReadROOT-2.4.0/Images/CoMPASS/Rejections.png
--rw-rw-rw-   0        0        0     2472 2023-05-23 14:23:25.000000 ReadROOT-2.4.0/Images/CoMPASS/Spectra.png
--rw-rw-rw-   0        0        0     2264 2023-05-23 14:29:40.000000 ReadROOT-2.4.0/Images/CoMPASS/Sync.png
--rw-rw-rw-   0        0        0    15934 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/CoMPASS/icon64x64.ico
--rw-rw-rw-   0        0        0     3193 2023-06-14 13:48:49.000000 ReadROOT-2.4.0/Images/CoMPASS/icon64x64.png
--rw-rw-rw-   0        0        0     1734 2023-06-12 19:05:08.000000 ReadROOT-2.4.0/Images/CompClear.png
--rw-rw-rw-   0        0        0     1452 2023-06-08 20:53:51.000000 ReadROOT-2.4.0/Images/Disabled0.png
--rw-rw-rw-   0        0        0     1201 2023-06-08 20:54:19.000000 ReadROOT-2.4.0/Images/Disabled1.png
--rw-rw-rw-   0        0        0     1515 2023-06-08 20:54:35.000000 ReadROOT-2.4.0/Images/Disabled2.png
--rw-rw-rw-   0        0        0     1566 2023-06-08 20:54:54.000000 ReadROOT-2.4.0/Images/Disabled3.png
--rw-rw-rw-   0        0        0     1583 2023-06-21 19:30:21.000000 ReadROOT-2.4.0/Images/DisabledSelect.png
--rw-rw-rw-   0        0        0     1994 2023-06-14 14:36:16.000000 ReadROOT-2.4.0/Images/DisabledSelectROI.png
--rw-rw-rw-   0        0        0     1646 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/EnergyHist.png
--rw-rw-rw-   0        0        0     1106 2023-06-12 18:27:14.000000 ReadROOT-2.4.0/Images/EnergyvsEnergyHist.png
-drwxrwxrwx   0        0        0        0 2023-08-07 16:48:11.739877 ReadROOT-2.4.0/Images/Log/
--rw-rw-rw-   0        0        0      551 2023-07-04 16:52:34.000000 ReadROOT-2.4.0/Images/Log/0.png
--rw-rw-rw-   0        0        0      476 2023-07-04 16:45:55.000000 ReadROOT-2.4.0/Images/Log/1.png
--rw-rw-rw-   0        0        0      761 2023-07-04 16:46:51.000000 ReadROOT-2.4.0/Images/Log/2.png
--rw-rw-rw-   0        0        0      818 2023-07-04 18:15:22.000000 ReadROOT-2.4.0/Images/Log/3.png
--rw-rw-rw-   0        0        0      620 2023-07-04 18:16:09.000000 ReadROOT-2.4.0/Images/Log/4.png
--rw-rw-rw-   0        0        0      835 2023-07-04 18:16:54.000000 ReadROOT-2.4.0/Images/Log/5.png
--rw-rw-rw-   0        0        0      747 2023-07-04 18:17:44.000000 ReadROOT-2.4.0/Images/Log/6.png
--rw-rw-rw-   0        0        0      635 2023-07-04 18:18:20.000000 ReadROOT-2.4.0/Images/Log/7.png
--rw-rw-rw-   0        0        0      822 2023-07-04 18:18:59.000000 ReadROOT-2.4.0/Images/Log/8.png
--rw-rw-rw-   0        0        0      971 2023-07-04 18:24:12.000000 ReadROOT-2.4.0/Images/Log/9+.png
--rw-rw-rw-   0        0        0      747 2023-07-04 18:19:41.000000 ReadROOT-2.4.0/Images/Log/9.png
--rw-rw-rw-   0        0        0     4514 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/MCS Graph.png
--rw-rw-rw-   0        0        0     1322 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/Off0.png
--rw-rw-rw-   0        0        0      937 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/Off1.png
--rw-rw-rw-   0        0        0     1343 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/Off2.png
--rw-rw-rw-   0        0        0     1370 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/Off3.png
--rw-rw-rw-   0        0        0      860 2023-06-21 19:30:00.000000 ReadROOT-2.4.0/Images/OffSelect.png
--rw-rw-rw-   0        0        0     1718 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/OffSelectROI.png
--rw-rw-rw-   0        0        0     1335 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/On0.png
--rw-rw-rw-   0        0        0      926 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/On1.png
--rw-rw-rw-   0        0        0     1336 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/On2.png
--rw-rw-rw-   0        0        0     1366 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/On3.png
--rw-rw-rw-   0        0        0      589 2023-06-21 19:29:10.000000 ReadROOT-2.4.0/Images/OnSelect.png
--rw-rw-rw-   0        0        0     1737 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/OnSelectROI.png
--rw-rw-rw-   0        0        0     1099 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/OpenFolder.png
--rw-rw-rw-   0        0        0     1267 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/OpenFolderCompass.png
--rw-rw-rw-   0        0        0     1224 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/PSDHist.png
--rw-rw-rw-   0        0        0     1450 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/PSDvsEnergyHist.png
--rw-rw-rw-   0        0        0     1927 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/Plot.png
--rw-rw-rw-   0        0        0     1242 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/PlotCompass.png
--rw-rw-rw-   0        0        0     1404 2023-06-20 18:31:47.000000 ReadROOT-2.4.0/Images/SaveCompass.png
--rw-rw-rw-   0        0        0     1461 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/SaveImage.png
--rw-rw-rw-   0        0        0     2076 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/TOFHist.png
--rw-rw-rw-   0        0        0     1140 2023-06-12 18:27:54.000000 ReadROOT-2.4.0/Images/TOFvsEnergyHist.png
--rw-rw-rw-   0        0        0     1447 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/Images/TimeHist.png
--rw-rw-rw-   0        0        0      947 2023-05-17 22:43:58.000000 ReadROOT-2.4.0/Images/axis.png
--rw-rw-rw-   0        0        0      463 2023-06-02 19:16:56.000000 ReadROOT-2.4.0/Images/collapsed.png
--rw-rw-rw-   0        0        0      689 2023-05-17 22:35:31.000000 ReadROOT-2.4.0/Images/delete.png
--rw-rw-rw-   0        0        0      458 2023-06-02 19:17:19.000000 ReadROOT-2.4.0/Images/expanded.png
--rw-rw-rw-   0        0        0     1010 2023-05-17 19:25:44.000000 ReadROOT-2.4.0/Images/file_config.png
--rw-rw-rw-   0        0        0      667 2023-05-17 22:56:43.000000 ReadROOT-2.4.0/Images/grid.png
--rw-rw-rw-   0        0        0     1546 2023-05-23 15:50:13.000000 ReadROOT-2.4.0/Images/histogram.png
--rw-rw-rw-   0        0        0      999 2023-05-17 20:52:54.000000 ReadROOT-2.4.0/Images/info.png
--rw-rw-rw-   0        0        0      344 2023-05-17 22:44:20.000000 ReadROOT-2.4.0/Images/line.png
--rw-rw-rw-   0        0        0      647 2023-05-17 22:35:02.000000 ReadROOT-2.4.0/Images/save.png
--rw-rw-rw-   0        0        0     1712 2023-05-17 22:24:15.000000 ReadROOT-2.4.0/Images/settings.png
--rw-rw-rw-   0        0        0     2094 2023-06-14 14:54:21.000000 ReadROOT-2.4.0/Images/start.png
--rw-rw-rw-   0        0        0     1992 2023-06-14 14:53:58.000000 ReadROOT-2.4.0/Images/stop.png
--rw-rw-rw-   0        0        0     1262 2023-05-23 15:51:24.000000 ReadROOT-2.4.0/Images/time.png
--rw-rw-rw-   0        0        0     2703 2023-08-07 16:48:11.815943 ReadROOT-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    10706 2023-08-07 16:45:33.000000 ReadROOT-2.4.0/QtClasses.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:48:11.799074 ReadROOT-2.4.0/ReadROOT.egg-info/
--rw-rw-rw-   0        0        0     2703 2023-08-07 16:48:11.000000 ReadROOT-2.4.0/ReadROOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2143 2023-08-07 16:48:11.000000 ReadROOT-2.4.0/ReadROOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 16:48:11.000000 ReadROOT-2.4.0/ReadROOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2023-08-07 16:48:11.000000 ReadROOT-2.4.0/ReadROOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-07 16:48:11.000000 ReadROOT-2.4.0/ReadROOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7245 2023-06-08 18:12:55.000000 ReadROOT-2.4.0/ValidInputs.py
--rw-rw-rw-   0        0        0    12005 2023-07-27 16:06:43.000000 ReadROOT-2.4.0/XML_Parser.py
--rw-rw-rw-   0        0        0     4230 2023-08-07 16:48:03.000000 ReadROOT-2.4.0/__init__.py
--rw-rw-rw-   0        0        0      881 2023-07-19 17:15:14.000000 ReadROOT-2.4.0/config.json
--rw-rw-rw-   0        0        0    44649 2023-08-07 16:34:06.000000 ReadROOT-2.4.0/discord.mp3
--rw-rw-rw-   0        0        0     7798 2022-12-02 19:45:45.000000 ReadROOT-2.4.0/funcs.cpp
--rw-rw-rw-   0        0        0     1624 2023-07-19 17:10:42.000000 ReadROOT-2.4.0/funcs.hpp
-drwxrwxrwx   0        0        0        0 2023-08-07 16:48:11.804985 ReadROOT-2.4.0/merge/
--rw-rw-rw-   0        0        0      106 2023-06-19 15:42:39.000000 ReadROOT-2.4.0/merge/__init__.py
--rw-rw-rw-   0        0        0     6327 2023-07-19 16:22:00.000000 ReadROOT-2.4.0/merge/merge_root_files.py
--rw-rw-rw-   0        0        0    31747 2023-07-03 15:57:45.000000 ReadROOT-2.4.0/read_root.py
--rw-rw-rw-   0        0        0    79395 2023-06-14 15:45:35.000000 ReadROOT-2.4.0/read_root_gui.py
--rw-rw-rw-   0        0        0    89839 2023-08-07 16:48:03.000000 ReadROOT-2.4.0/read_root_gui_v2.py
--rw-rw-rw-   0        0        0     1222 2023-08-07 16:47:51.000000 ReadROOT-2.4.0/reload.py
--rw-rw-rw-   0        0        0     3531 2023-07-12 14:25:15.000000 ReadROOT-2.4.0/root_plotter.py
--rw-rw-rw-   0        0        0       42 2023-08-07 16:48:11.818541 ReadROOT-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1487 2023-08-07 16:48:03.000000 ReadROOT-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:48:11.812322 ReadROOT-2.4.0/test/
--rw-rw-rw-   0        0        0       19 2023-05-25 14:27:41.000000 ReadROOT-2.4.0/test/test.py
--rw-rw-rw-   0        0        0     2864 2023-06-14 19:53:55.000000 ReadROOT-2.4.0/test/test_cpp.py
--rw-rw-rw-   0        0        0      356 2023-07-19 17:10:42.000000 ReadROOT-2.4.0/wrap.cpp
+drwxrwxrwx   0        0        0        0 2023-08-08 15:28:44.340235 ReadROOT-2.4.1/
+-rw-rw-rw-   0        0        0    16128 2023-02-15 23:51:19.000000 ReadROOT-2.4.1/ErrorPropagation.py
+-rw-rw-rw-   0        0        0     5152 2023-06-14 20:31:08.000000 ReadROOT-2.4.1/IOClasses.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:28:43.766804 ReadROOT-2.4.1/Images/
+-rw-rw-rw-   0        0        0     1802 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/Calculate.png
+-rw-rw-rw-   0        0        0     2340 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/Clear.png
+drwxrwxrwx   0        0        0        0 2023-08-08 15:28:43.833732 ReadROOT-2.4.1/Images/CoMPASS/
+-rw-rw-rw-   0        0        0     2712 2023-05-23 14:31:42.000000 ReadROOT-2.4.1/Images/CoMPASS/Coincidence.png
+-rw-rw-rw-   0        0        0     2292 2023-05-23 14:18:04.000000 ReadROOT-2.4.1/Images/CoMPASS/Discriminator.png
+-rw-rw-rw-   0        0        0     2492 2023-05-23 14:27:57.000000 ReadROOT-2.4.1/Images/CoMPASS/EnergyCalibration.png
+-rw-rw-rw-   0        0        0     2492 2023-05-23 14:13:06.000000 ReadROOT-2.4.1/Images/CoMPASS/Input.png
+-rw-rw-rw-   0        0        0     2547 2023-05-23 14:32:49.000000 ReadROOT-2.4.1/Images/CoMPASS/Misc.png
+-rw-rw-rw-   0        0        0     1089 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/CoMPASS/OpenGraph.png
+-rw-rw-rw-   0        0        0     2499 2023-05-23 14:20:06.000000 ReadROOT-2.4.1/Images/CoMPASS/QDC.png
+-rw-rw-rw-   0        0        0     2282 2023-05-23 14:25:56.000000 ReadROOT-2.4.1/Images/CoMPASS/Rejections.png
+-rw-rw-rw-   0        0        0     2472 2023-05-23 14:23:25.000000 ReadROOT-2.4.1/Images/CoMPASS/Spectra.png
+-rw-rw-rw-   0        0        0     2264 2023-05-23 14:29:40.000000 ReadROOT-2.4.1/Images/CoMPASS/Sync.png
+-rw-rw-rw-   0        0        0    15934 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/CoMPASS/icon64x64.ico
+-rw-rw-rw-   0        0        0     3193 2023-06-14 13:48:49.000000 ReadROOT-2.4.1/Images/CoMPASS/icon64x64.png
+-rw-rw-rw-   0        0        0     1734 2023-06-12 19:05:08.000000 ReadROOT-2.4.1/Images/CompClear.png
+-rw-rw-rw-   0        0        0     1452 2023-06-08 20:53:51.000000 ReadROOT-2.4.1/Images/Disabled0.png
+-rw-rw-rw-   0        0        0     1201 2023-06-08 20:54:19.000000 ReadROOT-2.4.1/Images/Disabled1.png
+-rw-rw-rw-   0        0        0     1515 2023-06-08 20:54:35.000000 ReadROOT-2.4.1/Images/Disabled2.png
+-rw-rw-rw-   0        0        0     1566 2023-06-08 20:54:54.000000 ReadROOT-2.4.1/Images/Disabled3.png
+-rw-rw-rw-   0        0        0     1583 2023-06-21 19:30:21.000000 ReadROOT-2.4.1/Images/DisabledSelect.png
+-rw-rw-rw-   0        0        0     1994 2023-06-14 14:36:16.000000 ReadROOT-2.4.1/Images/DisabledSelectROI.png
+-rw-rw-rw-   0        0        0     1646 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/EnergyHist.png
+-rw-rw-rw-   0        0        0     1106 2023-06-12 18:27:14.000000 ReadROOT-2.4.1/Images/EnergyvsEnergyHist.png
+drwxrwxrwx   0        0        0        0 2023-08-08 15:28:44.130289 ReadROOT-2.4.1/Images/Log/
+-rw-rw-rw-   0        0        0      551 2023-07-04 16:52:34.000000 ReadROOT-2.4.1/Images/Log/0.png
+-rw-rw-rw-   0        0        0      476 2023-07-04 16:45:55.000000 ReadROOT-2.4.1/Images/Log/1.png
+-rw-rw-rw-   0        0        0      761 2023-07-04 16:46:51.000000 ReadROOT-2.4.1/Images/Log/2.png
+-rw-rw-rw-   0        0        0      818 2023-07-04 18:15:22.000000 ReadROOT-2.4.1/Images/Log/3.png
+-rw-rw-rw-   0        0        0      620 2023-07-04 18:16:09.000000 ReadROOT-2.4.1/Images/Log/4.png
+-rw-rw-rw-   0        0        0      835 2023-07-04 18:16:54.000000 ReadROOT-2.4.1/Images/Log/5.png
+-rw-rw-rw-   0        0        0      747 2023-07-04 18:17:44.000000 ReadROOT-2.4.1/Images/Log/6.png
+-rw-rw-rw-   0        0        0      635 2023-07-04 18:18:20.000000 ReadROOT-2.4.1/Images/Log/7.png
+-rw-rw-rw-   0        0        0      822 2023-07-04 18:18:59.000000 ReadROOT-2.4.1/Images/Log/8.png
+-rw-rw-rw-   0        0        0      971 2023-07-04 18:24:12.000000 ReadROOT-2.4.1/Images/Log/9+.png
+-rw-rw-rw-   0        0        0      747 2023-07-04 18:19:41.000000 ReadROOT-2.4.1/Images/Log/9.png
+-rw-rw-rw-   0        0        0     4514 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/MCS Graph.png
+-rw-rw-rw-   0        0        0     1322 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/Off0.png
+-rw-rw-rw-   0        0        0      937 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/Off1.png
+-rw-rw-rw-   0        0        0     1343 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/Off2.png
+-rw-rw-rw-   0        0        0     1370 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/Off3.png
+-rw-rw-rw-   0        0        0      860 2023-06-21 19:30:00.000000 ReadROOT-2.4.1/Images/OffSelect.png
+-rw-rw-rw-   0        0        0     1718 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/OffSelectROI.png
+-rw-rw-rw-   0        0        0     1335 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/On0.png
+-rw-rw-rw-   0        0        0      926 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/On1.png
+-rw-rw-rw-   0        0        0     1336 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/On2.png
+-rw-rw-rw-   0        0        0     1366 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/On3.png
+-rw-rw-rw-   0        0        0      589 2023-06-21 19:29:10.000000 ReadROOT-2.4.1/Images/OnSelect.png
+-rw-rw-rw-   0        0        0     1737 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/OnSelectROI.png
+-rw-rw-rw-   0        0        0     1099 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/OpenFolder.png
+-rw-rw-rw-   0        0        0     1267 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/OpenFolderCompass.png
+-rw-rw-rw-   0        0        0     1224 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/PSDHist.png
+-rw-rw-rw-   0        0        0     1450 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/PSDvsEnergyHist.png
+-rw-rw-rw-   0        0        0     1927 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/Plot.png
+-rw-rw-rw-   0        0        0     1242 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/PlotCompass.png
+-rw-rw-rw-   0        0        0     1404 2023-06-20 18:31:47.000000 ReadROOT-2.4.1/Images/SaveCompass.png
+-rw-rw-rw-   0        0        0     1461 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/SaveImage.png
+-rw-rw-rw-   0        0        0     2076 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/TOFHist.png
+-rw-rw-rw-   0        0        0     1140 2023-06-12 18:27:54.000000 ReadROOT-2.4.1/Images/TOFvsEnergyHist.png
+-rw-rw-rw-   0        0        0     1447 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/Images/TimeHist.png
+-rw-rw-rw-   0        0        0      947 2023-05-17 22:43:58.000000 ReadROOT-2.4.1/Images/axis.png
+-rw-rw-rw-   0        0        0      463 2023-06-02 19:16:56.000000 ReadROOT-2.4.1/Images/collapsed.png
+-rw-rw-rw-   0        0        0      689 2023-05-17 22:35:31.000000 ReadROOT-2.4.1/Images/delete.png
+-rw-rw-rw-   0        0        0      458 2023-06-02 19:17:19.000000 ReadROOT-2.4.1/Images/expanded.png
+-rw-rw-rw-   0        0        0     1010 2023-05-17 19:25:44.000000 ReadROOT-2.4.1/Images/file_config.png
+-rw-rw-rw-   0        0        0      667 2023-05-17 22:56:43.000000 ReadROOT-2.4.1/Images/grid.png
+-rw-rw-rw-   0        0        0     1546 2023-05-23 15:50:13.000000 ReadROOT-2.4.1/Images/histogram.png
+-rw-rw-rw-   0        0        0      999 2023-05-17 20:52:54.000000 ReadROOT-2.4.1/Images/info.png
+-rw-rw-rw-   0        0        0      344 2023-05-17 22:44:20.000000 ReadROOT-2.4.1/Images/line.png
+-rw-rw-rw-   0        0        0      647 2023-05-17 22:35:02.000000 ReadROOT-2.4.1/Images/save.png
+-rw-rw-rw-   0        0        0     1712 2023-05-17 22:24:15.000000 ReadROOT-2.4.1/Images/settings.png
+-rw-rw-rw-   0        0        0     2094 2023-06-14 14:54:21.000000 ReadROOT-2.4.1/Images/start.png
+-rw-rw-rw-   0        0        0     1992 2023-06-14 14:53:58.000000 ReadROOT-2.4.1/Images/stop.png
+-rw-rw-rw-   0        0        0     1262 2023-05-23 15:51:24.000000 ReadROOT-2.4.1/Images/time.png
+-rw-rw-rw-   0        0        0     2703 2023-08-08 15:28:44.338124 ReadROOT-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10706 2023-08-07 16:45:33.000000 ReadROOT-2.4.1/QtClasses.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:28:44.222804 ReadROOT-2.4.1/ReadROOT.egg-info/
+-rw-rw-rw-   0        0        0     2703 2023-08-08 15:28:42.000000 ReadROOT-2.4.1/ReadROOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2143 2023-08-08 15:28:42.000000 ReadROOT-2.4.1/ReadROOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 15:28:42.000000 ReadROOT-2.4.1/ReadROOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2023-08-08 15:28:42.000000 ReadROOT-2.4.1/ReadROOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 15:28:42.000000 ReadROOT-2.4.1/ReadROOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7245 2023-06-08 18:12:55.000000 ReadROOT-2.4.1/ValidInputs.py
+-rw-rw-rw-   0        0        0    12005 2023-07-27 16:06:43.000000 ReadROOT-2.4.1/XML_Parser.py
+-rw-rw-rw-   0        0        0     4230 2023-08-08 15:28:35.000000 ReadROOT-2.4.1/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-07-19 17:15:14.000000 ReadROOT-2.4.1/config.json
+-rw-rw-rw-   0        0        0    44649 2023-08-07 16:34:06.000000 ReadROOT-2.4.1/discord.mp3
+-rw-rw-rw-   0        0        0     7798 2022-12-02 19:45:45.000000 ReadROOT-2.4.1/funcs.cpp
+-rw-rw-rw-   0        0        0     1624 2023-07-19 17:10:42.000000 ReadROOT-2.4.1/funcs.hpp
+drwxrwxrwx   0        0        0        0 2023-08-08 15:28:44.284202 ReadROOT-2.4.1/merge/
+-rw-rw-rw-   0        0        0      106 2023-06-19 15:42:39.000000 ReadROOT-2.4.1/merge/__init__.py
+-rw-rw-rw-   0        0        0     6327 2023-07-19 16:22:00.000000 ReadROOT-2.4.1/merge/merge_root_files.py
+-rw-rw-rw-   0        0        0    31747 2023-07-03 15:57:45.000000 ReadROOT-2.4.1/read_root.py
+-rw-rw-rw-   0        0        0    79395 2023-06-14 15:45:35.000000 ReadROOT-2.4.1/read_root_gui.py
+-rw-rw-rw-   0        0        0    90687 2023-08-08 15:28:35.000000 ReadROOT-2.4.1/read_root_gui_v2.py
+-rw-rw-rw-   0        0        0     1222 2023-08-08 15:28:33.000000 ReadROOT-2.4.1/reload.py
+-rw-rw-rw-   0        0        0     3531 2023-07-12 14:25:15.000000 ReadROOT-2.4.1/root_plotter.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 15:28:44.341560 ReadROOT-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1487 2023-08-08 15:28:35.000000 ReadROOT-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 15:28:44.330280 ReadROOT-2.4.1/test/
+-rw-rw-rw-   0        0        0       19 2023-05-25 14:27:41.000000 ReadROOT-2.4.1/test/test.py
+-rw-rw-rw-   0        0        0     2864 2023-06-14 19:53:55.000000 ReadROOT-2.4.1/test/test_cpp.py
+-rw-rw-rw-   0        0        0      356 2023-07-19 17:10:42.000000 ReadROOT-2.4.1/wrap.cpp
```

### Comparing `ReadROOT-2.4.0/ErrorPropagation.py` & `ReadROOT-2.4.1/ErrorPropagation.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/IOClasses.py` & `ReadROOT-2.4.1/IOClasses.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Calculate.png` & `ReadROOT-2.4.1/Images/Calculate.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Clear.png` & `ReadROOT-2.4.1/Images/Clear.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/Coincidence.png` & `ReadROOT-2.4.1/Images/CoMPASS/Coincidence.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/Discriminator.png` & `ReadROOT-2.4.1/Images/CoMPASS/Discriminator.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/EnergyCalibration.png` & `ReadROOT-2.4.1/Images/CoMPASS/EnergyCalibration.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/Input.png` & `ReadROOT-2.4.1/Images/CoMPASS/Input.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/Misc.png` & `ReadROOT-2.4.1/Images/CoMPASS/Misc.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/OpenGraph.png` & `ReadROOT-2.4.1/Images/CoMPASS/OpenGraph.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/QDC.png` & `ReadROOT-2.4.1/Images/CoMPASS/QDC.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/Rejections.png` & `ReadROOT-2.4.1/Images/CoMPASS/Rejections.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/Spectra.png` & `ReadROOT-2.4.1/Images/CoMPASS/Spectra.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/Sync.png` & `ReadROOT-2.4.1/Images/CoMPASS/Sync.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/icon64x64.ico` & `ReadROOT-2.4.1/Images/CoMPASS/icon64x64.ico`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CoMPASS/icon64x64.png` & `ReadROOT-2.4.1/Images/CoMPASS/icon64x64.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/CompClear.png` & `ReadROOT-2.4.1/Images/CompClear.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Disabled0.png` & `ReadROOT-2.4.1/Images/Disabled0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Disabled1.png` & `ReadROOT-2.4.1/Images/Disabled1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Disabled2.png` & `ReadROOT-2.4.1/Images/Disabled2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Disabled3.png` & `ReadROOT-2.4.1/Images/Disabled3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/DisabledSelect.png` & `ReadROOT-2.4.1/Images/DisabledSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/DisabledSelectROI.png` & `ReadROOT-2.4.1/Images/DisabledSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/EnergyHist.png` & `ReadROOT-2.4.1/Images/EnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/EnergyvsEnergyHist.png` & `ReadROOT-2.4.1/Images/EnergyvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/0.png` & `ReadROOT-2.4.1/Images/Log/0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/2.png` & `ReadROOT-2.4.1/Images/Log/2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/3.png` & `ReadROOT-2.4.1/Images/Log/3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/4.png` & `ReadROOT-2.4.1/Images/Log/4.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/5.png` & `ReadROOT-2.4.1/Images/Log/5.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/6.png` & `ReadROOT-2.4.1/Images/Log/6.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/7.png` & `ReadROOT-2.4.1/Images/Log/7.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/8.png` & `ReadROOT-2.4.1/Images/Log/8.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/9+.png` & `ReadROOT-2.4.1/Images/Log/9+.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Log/9.png` & `ReadROOT-2.4.1/Images/Log/9.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/MCS Graph.png` & `ReadROOT-2.4.1/Images/MCS Graph.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Off0.png` & `ReadROOT-2.4.1/Images/Off0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Off1.png` & `ReadROOT-2.4.1/Images/Off1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Off2.png` & `ReadROOT-2.4.1/Images/Off2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Off3.png` & `ReadROOT-2.4.1/Images/Off3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/OffSelect.png` & `ReadROOT-2.4.1/Images/OffSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/OffSelectROI.png` & `ReadROOT-2.4.1/Images/OffSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/On0.png` & `ReadROOT-2.4.1/Images/On0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/On1.png` & `ReadROOT-2.4.1/Images/On1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/On2.png` & `ReadROOT-2.4.1/Images/On2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/On3.png` & `ReadROOT-2.4.1/Images/On3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/OnSelect.png` & `ReadROOT-2.4.1/Images/OnSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/OnSelectROI.png` & `ReadROOT-2.4.1/Images/OnSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/OpenFolder.png` & `ReadROOT-2.4.1/Images/OpenFolder.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/OpenFolderCompass.png` & `ReadROOT-2.4.1/Images/OpenFolderCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/PSDHist.png` & `ReadROOT-2.4.1/Images/PSDHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/PSDvsEnergyHist.png` & `ReadROOT-2.4.1/Images/PSDvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/Plot.png` & `ReadROOT-2.4.1/Images/Plot.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/PlotCompass.png` & `ReadROOT-2.4.1/Images/PlotCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/SaveCompass.png` & `ReadROOT-2.4.1/Images/SaveCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/SaveImage.png` & `ReadROOT-2.4.1/Images/SaveImage.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/TOFHist.png` & `ReadROOT-2.4.1/Images/TOFHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/TOFvsEnergyHist.png` & `ReadROOT-2.4.1/Images/TOFvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/TimeHist.png` & `ReadROOT-2.4.1/Images/TimeHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/axis.png` & `ReadROOT-2.4.1/Images/axis.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/delete.png` & `ReadROOT-2.4.1/Images/delete.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/file_config.png` & `ReadROOT-2.4.1/Images/file_config.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/grid.png` & `ReadROOT-2.4.1/Images/grid.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/histogram.png` & `ReadROOT-2.4.1/Images/histogram.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/info.png` & `ReadROOT-2.4.1/Images/info.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/save.png` & `ReadROOT-2.4.1/Images/save.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/settings.png` & `ReadROOT-2.4.1/Images/settings.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/start.png` & `ReadROOT-2.4.1/Images/start.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/stop.png` & `ReadROOT-2.4.1/Images/stop.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/Images/time.png` & `ReadROOT-2.4.1/Images/time.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/PKG-INFO` & `ReadROOT-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ReadROOT
-Version: 2.4.0
+Version: 2.4.1
 Summary: Easy GUI made to read ROOT files created by the CoMPASS software distribued by CAEN.
 Home-page: https://github.com/Chujo58/ReadROOT
 Author: Chloé Legué
 Author-email: chloe.legue@mail.mcgill.ca
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 **Created by :** Chloe Legue
 
-**Current version date :** 2023/08/07
+**Current version date :** 2023/08/08
 
 <p align=center>
 <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.11-green.svg"></a>
 <a target="_blank" href="https://pypi.org/project/ReadROOT/" title="PyPI version"><img src="https://img.shields.io/pypi/v/ReadROOT?logo=pypi"></a>
 </p>
 
 ReadROOT is an easy GUI made to read ROOT files created by the CoMPASS software distributed by CAEN. This GUI will also allow the user to plot the different graphs from the CoMPASS software.
```

### Comparing `ReadROOT-2.4.0/QtClasses.py` & `ReadROOT-2.4.1/QtClasses.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/ReadROOT.egg-info/PKG-INFO` & `ReadROOT-2.4.1/ReadROOT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ReadROOT
-Version: 2.4.0
+Version: 2.4.1
 Summary: Easy GUI made to read ROOT files created by the CoMPASS software distribued by CAEN.
 Home-page: https://github.com/Chujo58/ReadROOT
 Author: Chloé Legué
 Author-email: chloe.legue@mail.mcgill.ca
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 **Created by :** Chloe Legue
 
-**Current version date :** 2023/08/07
+**Current version date :** 2023/08/08
 
 <p align=center>
 <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.11-green.svg"></a>
 <a target="_blank" href="https://pypi.org/project/ReadROOT/" title="PyPI version"><img src="https://img.shields.io/pypi/v/ReadROOT?logo=pypi"></a>
 </p>
 
 ReadROOT is an easy GUI made to read ROOT files created by the CoMPASS software distributed by CAEN. This GUI will also allow the user to plot the different graphs from the CoMPASS software.
```

### Comparing `ReadROOT-2.4.0/ReadROOT.egg-info/SOURCES.txt` & `ReadROOT-2.4.1/ReadROOT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/ValidInputs.py` & `ReadROOT-2.4.1/ValidInputs.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/XML_Parser.py` & `ReadROOT-2.4.1/XML_Parser.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/__init__.py` & `ReadROOT-2.4.1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, sys, matplotlib, json, difflib
 running_directory = os.getcwd() #This is to make the relative import work!
 path = os.path.dirname(os.path.abspath(__file__))
 os.chdir(path)
 sys.path.append(path) #FOR C++ TO WORK!
 
-__version__ = '2.4.0'
+__version__ = '2.4.1'
 
 from . import read_root
 from . import read_root_gui
 from . import read_root_gui_v2
 from . import IOClasses
 from . import QtClasses
 from . import root_plotter
```

### Comparing `ReadROOT-2.4.0/config.json` & `ReadROOT-2.4.1/config.json`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/discord.mp3` & `ReadROOT-2.4.1/discord.mp3`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/funcs.cpp` & `ReadROOT-2.4.1/funcs.cpp`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/funcs.hpp` & `ReadROOT-2.4.1/funcs.hpp`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/merge/merge_root_files.py` & `ReadROOT-2.4.1/merge/merge_root_files.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/read_root.py` & `ReadROOT-2.4.1/read_root.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/read_root_gui.py` & `ReadROOT-2.4.1/read_root_gui.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/read_root_gui_v2.py` & `ReadROOT-2.4.1/read_root_gui_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #----------------------------------------------------------------------------
 # Created by : Chloé Legué
-# Current version date : 2023/08/07
-# Version = 2.4.0
+# Current version date : 2023/08/08
+# Version = 2.4.1
 #----------------------------------------------------------------------------
 """
 This code was made for the coincidence experiment at McGill University. 
 
 The code allows the user to choose a folder containing the results saved from the CoMPASS software from CAEN. This code should be used with the CAEN DT5751, or any other digitizer from CAEN that work in the same way.
 
 This code is able to reproduce the important graphs that the CoMPASS software makes like MCS Graph, Energy Histogram and TOF Histogram. Other graphs can be added if needed.
@@ -565,14 +565,16 @@
 
 
         #Make the plotting region
         self.inner_left = grid_left.place_object(g.GridLayout(False), alignment=0).set_width(int(40*self.ratio))
         inner_right = grid_left.place_object(g.GridLayout(False), alignment=0)
         
         #Add the buttons for the different plots:
+        self.previous_graph_btn = None #To keep track of what was the last graph button selected.
+
         self.energy_btn = self.make_comp_btn(self.inner_left, "New Energy Histogram", "Images/EnergyHist.png", column=1, row=1)
         self.energy_btn.signal_toggled.connect(self.plot_selection)
 
         self.psd_btn = self.make_comp_btn(self.inner_left, "New PSD Histogram", "Images/PSDHist.png", column=1, row=2)
         self.psd_btn.signal_toggled.connect(self.plot_selection)
         
         self.time_btn = self.make_comp_btn(self.inner_left, "New Time Histogram", "Images/TimeHist.png", column=1, row=3)
@@ -600,14 +602,16 @@
         self.plot_btn = self.inner_left.place_object(g.Button(" ", tip="Plot the graph/histogram selected above"), alignment=0, column=1, row=10).set_height(int(35*self.ratio)).set_width(int(35*self.ratio))
         self.plot_btn.set_style_unchecked(style="image: url(Images/PlotCompass.png)")
         self.plot_btn.signal_clicked.connect(self.plot_graphs)
 
         self.clear_btn = self.make_comp_btn(self.inner_left, "Clear plot", "Images/CompClear.png", column=1, row=11)
         self.clear_btn.signal_toggled.connect(self.clear)
 
+        self.graph_buttons = [self.energy_btn, self.psd_btn, self.time_btn, self.tof_btn, self.psdvse_btn, self.evse_btn, self.tofvse_btn, self.mcs_btn]
+
         #Adding the databox and the plot
         # inner_right.new_autorow()
         plot_region = inner_right.place_object(pg.PlotWidget(), alignment=0)
         plot_region.setBackground("black") if self.dark_theme_on else plot_region.setBackground("white")
         self.plot = plot_region.getPlotItem()
 
     def make_plot_settings(self, parent):
@@ -659,16 +663,16 @@
         parent.expand()
 
     def make_collapsible_section(self, parent):
         collapse_grid_layout = g.GridLayout(False)
         self.old_range = 500
         self.old_min = 0
 
-        self.previous_start_btn = None
-        self.previous_stop_btn = None
+        self.previous_start_btn = None #To keep track of what was the last start channel button selected
+        self.previous_stop_btn = None #To keep track of what was the last stop channel buttons selected.
         
         # Calculate TOF button theme:
         light_theme = """
             QPushButton{
                 border: 2px solid rgb(193,193,193);
                 border-radius: 5px;
                 background-color: qlineargradient(x1:0, y1:0, x2: 1, y2: 1, stop:0 rgb(120,225,252), stop:1 rgb(119,119,170));
@@ -999,21 +1003,21 @@
         self.buttons_files = {}
         
         for file in self.files:
             for index, (key, label) in enumerate(xml_labels.items()):
                 if label in file:
                     self.buttons_files[key] = file
 
-    def toggle_others_out(self, selected_button, buttons_list):
+    def toggle_others_out(self, selected_button: g.Button, buttons_list: list):
         for button in buttons_list:
             if button is selected_button:
                 continue
             button.set_checked(False)
 
-    def find_checked_button(self, buttons_list, previous_btn):
+    def find_checked_button(self, buttons_list: list, previous_btn: g.Button):
         for button in buttons_list:
             if button.is_checked() and button is not previous_btn:
                 return button
 
     def channel_toggling(self, *a):
         # #General channel buttons:
         checked_btn = self.find_checked_button(self.buttons_list, self.previous_btn)
@@ -1031,14 +1035,21 @@
     def stop_channel_toggling(self, *a):
         #TOF stop channel buttons:
         checked_stop_btn = self.find_checked_button(self.stop_buttons_list, self.previous_stop_btn)
         if checked_stop_btn is not self.previous_stop_btn:
             self.toggle_others_out(checked_stop_btn, self.stop_buttons_list)
             self.previous_stop_btn = checked_stop_btn
 
+    def graph_button_toggling(self, *a):
+        #Graph buttons:
+        checked_graph_btn = self.find_checked_button(self.graph_buttons, self.previous_graph_btn)
+        if checked_graph_btn is not self.previous_graph_btn:
+            self.toggle_others_out(checked_graph_btn, self.graph_buttons)
+            self.previous_graph_btn = checked_graph_btn
+
     def load_graph_options(self):
         self.change_title()
         self.change_legend()
         self.change_grid()
         self.change_labels()
         self.change_log()
                 
@@ -1716,15 +1727,17 @@
             self.worker.finished.connect(lambda: self.disable_all_buttons(self.states))
             self.load_states = False
 
         if not hasattr(self, "load_states") and a[0]:
             self.logs.add_log("Did you properly load your folder?")
 
         if a[0]:
-            try: self.disable_all_buttons(self.states)
+            try: 
+                self.disable_all_buttons(self.states)
+                self.graph_button_toggling()
             except: pass
         else:
             self.enable_all_buttons()
 
 
     def update_states(self, *a):
         self.states[a[0][0]] = a[0][1]
```

### Comparing `ReadROOT-2.4.0/reload.py` & `ReadROOT-2.4.1/reload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 import time, shutil, os
 version_date = datetime.now().strftime('%Y/%m/%d')
-version_number = "2.4.0"
+version_number = "2.4.1"
 
 with open("READme.md", "r") as f:
     read_me = f.readlines()
 
 with open("setup.py", "r") as f:
     setup = f.readlines()
```

### Comparing `ReadROOT-2.4.0/root_plotter.py` & `ReadROOT-2.4.1/root_plotter.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.4.0/setup.py` & `ReadROOT-2.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 from setuptools import setup
 
 description = open("READme.md").read()
 
 setup(
     name = "ReadROOT",
```

### Comparing `ReadROOT-2.4.0/test/test_cpp.py` & `ReadROOT-2.4.1/test/test_cpp.py`

 * *Files identical despite different names*

