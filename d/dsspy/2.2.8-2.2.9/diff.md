# Comparing `tmp/dsspy-2.2.8.tar.gz` & `tmp/dsspy-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PyDSS/PyDSS/dist/.tmp-krmgk6bg/dsspy-2.2.8.tar", last modified: Fri Jul 21 22:57:44 2023, max compression
+gzip compressed data, was "/home/runner/work/PyDSS/PyDSS/dist/.tmp-aahuds1a/dsspy-2.2.9.tar", last modified: Tue Aug  8 19:37:52 2023, max compression
```

## Comparing `dsspy-2.2.8.tar` & `dsspy-2.2.9.tar`

### file list

```diff
@@ -1,220 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-21 22:57:35.000000 dsspy-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-21 22:57:44.000000 dsspy-2.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/Extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/Extensions/MonteCarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/Extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3014 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/NetworkModifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/ProfileManager/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/ProfileInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/base_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/MongoDB.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/h5.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ResultData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/SolveMode.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/src/app/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/DataWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/HDF5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/JSON_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/Tester.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/arrow_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/pydss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/src/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/create_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/apps/data_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/add_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/create_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/edit_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/pydss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/run_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dataset_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/ExportMode-byClass.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/ExportMode-byElement.toml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/Exports.toml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/Subscriptions.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/Monte_Carlo/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/Monte_Carlo/MonteCarloSettings.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/Monte_Carlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/plots.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/FaultController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/GenController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/MotorStall.toml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/PvController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/SocketController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/StorageController.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/xfmrController.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/FrequencySweep.toml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/Histogram.toml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/NetworkGraph.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/Table.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/ThreeDim.toml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/TimeSeries.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/Topology.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/VoltageDistance.toml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/XY.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2297 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssBus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssCircuit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6380 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssElement.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssElementFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    30519 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssObjectBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/element_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/element_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/export_list_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/get_snapshot_timepoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/helics_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    44407 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/modes/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/Dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/QSTS.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/Snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/naerm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/node_voltage_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyContrReader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyControllers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/FaultController.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/GenController.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/HybridController.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/MotorStall.py
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvController.py
--rw-r--r--   0 runner    (1001) docker     (123)    24135 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/SocketController.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/StorageController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/ThermostaticLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/xfmrController.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/pyController.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/pyControllerAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyDSS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyLogger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1428 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlotReader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPlots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/FrequencySweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/Histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/NetworkGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/Table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/ThreeDim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/Topology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/VoltageDistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/XY.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/pyPlotAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/pyPlots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py
--rw-r--r--   0 runner    (1001) docker     (123)    20893 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocessAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyResults.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pydss_fs_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30773 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pydss_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    38195 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pydss_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/capacitor_change_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/feeder_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/pv_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/reg_control_tap_number_change_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/thermal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/voltage_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/simulation_input_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/storage_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/thermal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/unitDefinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/dss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/pydss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/simulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/timing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/value_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:57:44.000000 dsspy-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-21 22:57:35.000000 dsspy-2.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_auto_snapshot_time_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_custom_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_dataset_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_element_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_export_list_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_independent_controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_opendss_export_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_opendss_export_powers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_pv_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_pydss_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_pydss_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_space_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-08 19:37:40.000000 dsspy-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 19:37:52.000000 dsspy-2.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/Extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/Extensions/MonteCarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/Extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3014 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/NetworkModifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/ProfileManager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ProfileManager/ProfileInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ProfileManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ProfileManager/base_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ProfileManager/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/ProfileManager/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ProfileManager/hooks/MongoDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ProfileManager/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ProfileManager/hooks/h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/ResultData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/SolveMode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/api/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/api/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/api/src/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/app/DataWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/app/HDF5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/app/JSON_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/app/Tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/app/arrow_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/app/pydss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/api/src/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/web/create_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/web/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/api/src/web/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/apps/data_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/add_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/create_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/edit_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/pydss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/cli/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dataset_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/defaults/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/defaults/ExportLists/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/ExportLists/ExportMode-byClass.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/ExportLists/ExportMode-byElement.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/ExportLists/Exports.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/ExportLists/Subscriptions.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/ExportLists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:51.000000 dsspy-2.2.9/PyDSS/defaults/Monte_Carlo/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/Monte_Carlo/MonteCarloSettings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/Monte_Carlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/plots.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/FaultController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/GenController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/MotorStall.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/MotorStallSimple.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/PvController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/PvDynamic.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/PvFrequencyRideThru.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/SocketController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/StorageController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/ThermostaticLoad.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyControllerList/xfmrController.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/FrequencySweep.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/Histogram.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/NetworkGraph.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/Table.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/ThreeDim.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/TimeSeries.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/Topology.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/VoltageDistance.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/XY.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/defaults/pyPlotList/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2297 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dssBus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dssCircuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6380 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dssElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dssElementFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30519 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dssInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dssObjectBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/dssTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/element_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/element_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/export_list_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/get_snapshot_timepoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/helics_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44407 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/modes/Dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/modes/QSTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/modes/Snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/modes/solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/naerm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/node_voltage_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyContrReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyControllers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/FaultController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/GenController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/MotorStall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/MotorStallSimple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/PvController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/PvDynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/PvFrequencyRideThru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24135 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/Settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/SocketController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/StorageController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/ThermostaticLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/Controllers/xfmrController.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/pyController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyControllers/pyControllerAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyDSS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyLogger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1428 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlotReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyPlots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/FrequencySweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/Histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/NetworkGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/ThreeDim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/Topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/VoltageDistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/XY.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/Plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/pyPlotAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPlots/pyPlots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/pyPostprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyPostprocessor/pyPostprocessAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pyResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pydss_fs_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30773 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pydss_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38195 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/pydss_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/capacitor_change_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/feeder_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/pv_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/reg_control_tap_number_change_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/thermal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/reports/voltage_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/simulation_input_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/storage_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/thermal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/unitDefinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/PyDSS/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/utils/dss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/utils/pydss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/utils/simulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/utils/timing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-08-08 19:37:40.000000 dsspy-2.2.9/PyDSS/value_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/dsspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 19:37:51.000000 dsspy-2.2.9/dsspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-08-08 19:37:51.000000 dsspy-2.2.9/dsspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:37:51.000000 dsspy-2.2.9/dsspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 19:37:51.000000 dsspy-2.2.9/dsspy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-08 19:37:51.000000 dsspy-2.2.9/dsspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 19:37:51.000000 dsspy-2.2.9/dsspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:37:52.000000 dsspy-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-08 19:37:40.000000 dsspy-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:37:52.000000 dsspy-2.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_auto_snapshot_time_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_custom_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_dataset_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_element_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_export_list_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_independent_controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_opendss_export_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_opendss_export_powers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_pv_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_pydss_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_pydss_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 19:37:40.000000 dsspy-2.2.9/tests/test_space_estimation.py
```

### Comparing `dsspy-2.2.8/LICENSE` & `dsspy-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PKG-INFO` & `dsspy-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsspy
-Version: 2.2.8
+Version: 2.2.9
 Summary: A high-level python interface for OpenDSS
 Home-page: http://www.github.com/nrel/pydss
 Author: Aadil Latif
 Author-email: Aadil.Latif@nrel.gov
 License: BSD 3 clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `dsspy-2.2.8/PyDSS/Extensions/MonteCarlo.py` & `dsspy-2.2.9/PyDSS/Extensions/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/NetworkModifier.py` & `dsspy-2.2.9/PyDSS/NetworkModifier.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/ProfileManager/ProfileInterface.py` & `dsspy-2.2.9/PyDSS/ProfileManager/ProfileInterface.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/ProfileManager/base_definitions.py` & `dsspy-2.2.9/PyDSS/ProfileManager/base_definitions.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/ProfileManager/hooks/MongoDB.py` & `dsspy-2.2.9/PyDSS/ProfileManager/hooks/MongoDB.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/ProfileManager/hooks/h5.py` & `dsspy-2.2.9/PyDSS/ProfileManager/hooks/h5.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/ResultData.py` & `dsspy-2.2.9/PyDSS/ResultData.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/SolveMode.py` & `dsspy-2.2.9/PyDSS/SolveMode.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/server.py` & `dsspy-2.2.9/PyDSS/api/server.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/app/DataWriter.py` & `dsspy-2.2.9/PyDSS/api/src/app/DataWriter.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/app/HDF5.py` & `dsspy-2.2.9/PyDSS/api/src/app/HDF5.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/app/JSON_writer.py` & `dsspy-2.2.9/PyDSS/api/src/app/JSON_writer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/app/Tester.py` & `dsspy-2.2.9/PyDSS/api/src/app/Tester.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/app/arrow_writer.py` & `dsspy-2.2.9/PyDSS/api/src/app/arrow_writer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/app/pydss.py` & `dsspy-2.2.9/PyDSS/api/src/app/pydss.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/web/handler.py` & `dsspy-2.2.9/PyDSS/api/src/web/handler.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/api/src/web/parser.py` & `dsspy-2.2.9/PyDSS/api/src/web/parser.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/apps/data_viewer.py` & `dsspy-2.2.9/PyDSS/apps/data_viewer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/add_post_process.py` & `dsspy-2.2.9/PyDSS/cli/add_post_process.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/controllers.py` & `dsspy-2.2.9/PyDSS/cli/controllers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/convert.py` & `dsspy-2.2.9/PyDSS/cli/convert.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/create_project.py` & `dsspy-2.2.9/PyDSS/cli/create_project.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/edit_scenario.py` & `dsspy-2.2.9/PyDSS/cli/edit_scenario.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/export.py` & `dsspy-2.2.9/PyDSS/cli/export.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/extract.py` & `dsspy-2.2.9/PyDSS/cli/extract.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/pydss.py` & `dsspy-2.2.9/PyDSS/cli/pydss.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/reports.py` & `dsspy-2.2.9/PyDSS/cli/reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/run.py` & `dsspy-2.2.9/PyDSS/cli/run.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/cli/run_server.py` & `dsspy-2.2.9/PyDSS/cli/run_server.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/config_data.py` & `dsspy-2.2.9/PyDSS/config_data.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/controllers.py` & `dsspy-2.2.9/PyDSS/controllers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/dataset_buffer.py` & `dsspy-2.2.9/PyDSS/dataset_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Contains DatasetBuffer"""
 
+from cmath import nan
 import logging
 
 import numpy as np
 import pandas as pd
 
 from PyDSS.common import DatasetPropertyType
 from PyDSS.exceptions import InvalidConfiguration
 from PyDSS.utils.utils import make_timestamps
 
 
+
 KiB = 1024
 MiB = KiB * KiB
 GiB = MiB * MiB
 
 # The optimal number of chunks to store in memory will vary widely.
 # The h5py docs recommend keeping chunk byte sizes between 10 KiB - 1 MiB.
 # It needs to be larger than the biggest possible row and also cover enough
@@ -139,14 +141,15 @@
 
         """
         size_row = self._buf.size * self._buf.itemsize / len(self._buf)
         return size_row * self._max_size
 
     def write_value(self, value):
         """Write the value to the internal buffer, flushing when full."""
+
         self._buf[self._buf_index] = value
         self._buf_index += 1
         if self._buf_index == self.chunk_count:
             self.flush_data()
 
     def write_data(self, values):
         """Write the data to the dataset."""
```

### Comparing `dsspy-2.2.8/PyDSS/defaults/ExportLists/ExportMode-byClass.toml` & `dsspy-2.2.9/PyDSS/defaults/ExportLists/ExportMode-byClass.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/defaults/ExportLists/Exports.toml` & `dsspy-2.2.9/PyDSS/defaults/ExportLists/Exports.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/defaults/plots.toml` & `dsspy-2.2.9/PyDSS/defaults/plots.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml` & `dsspy-2.2.9/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/defaults/pyControllerList/StorageController.toml` & `dsspy-2.2.9/PyDSS/defaults/pyControllerList/StorageController.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/dssBus.py` & `dsspy-2.2.9/PyDSS/dssBus.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/dssCircuit.py` & `dsspy-2.2.9/PyDSS/dssCircuit.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/dssElement.py` & `dsspy-2.2.9/PyDSS/dssElement.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/dssInstance.py` & `dsspy-2.2.9/PyDSS/dssInstance.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/dssObjectBase.py` & `dsspy-2.2.9/PyDSS/dssObjectBase.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/dssTransformer.py` & `dsspy-2.2.9/PyDSS/dssTransformer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/element_fields.py` & `dsspy-2.2.9/PyDSS/element_fields.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/element_options.py` & `dsspy-2.2.9/PyDSS/element_options.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/exceptions.py` & `dsspy-2.2.9/PyDSS/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/export_list_reader.py` & `dsspy-2.2.9/PyDSS/export_list_reader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/get_snapshot_timepoints.py` & `dsspy-2.2.9/PyDSS/get_snapshot_timepoints.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/helics_interface.py` & `dsspy-2.2.9/PyDSS/helics_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,18 +146,22 @@
                     value = helics.helicsInputGetString(sub_info['Subscription'])
                 elif sub_info['Data type'].lower() == 'boolean':
                     value = helics.helicsInputGetBoolean(sub_info['Subscription'])
                 elif sub_info['Data type'].lower() == 'integer':
                     value = helics.helicsInputGetInteger(sub_info['Subscription'])
 
                 if value and value != 0:
+                    if value > 1e6 or value < -1e6:
+                        # #print("YO HERE")
+                        value = 1.0 
+                    
                     value = value * sub_info['Multiplier']
-
                     dssElement = self._objects_by_element[element_name]
-                    dssElement.SetParameter(sub_info['Property'], value)
+                    # #print(sub_info['Property'], value)
+                    dssElement.SetParameter(sub_info['Property'], value) 
 
                     self._logger.info('Value for "{}.{}" changed to "{}"'.format(
                         element_name,
                         sub_info['Property'],
                         value * sub_info['Multiplier']
                     ))
```

### Comparing `dsspy-2.2.8/PyDSS/loggers.py` & `dsspy-2.2.9/PyDSS/loggers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/metrics.py` & `dsspy-2.2.9/PyDSS/metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/modes/Dynamic.py` & `dsspy-2.2.9/PyDSS/modes/Dynamic.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/modes/QSTS.py` & `dsspy-2.2.9/PyDSS/modes/QSTS.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/modes/Snapshot.py` & `dsspy-2.2.9/PyDSS/modes/Snapshot.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/modes/solver_base.py` & `dsspy-2.2.9/PyDSS/modes/solver_base.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/naerm.py` & `dsspy-2.2.9/PyDSS/naerm.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,8 @@
     except Exception as e:
         return 'Failed'
 
 
 if __name__ == '__main__':
 
     name = 'PyDSS_x/circuit/heco19021/power_real/double'
-    print(get_naerm_value([34,45],'PyDSS_x/circuit/heco19021/power_imag/double' ))
+    #print(get_naerm_value([34,45],'PyDSS_x/circuit/heco19021/power_imag/double' ))
```

### Comparing `dsspy-2.2.8/PyDSS/node_voltage_metrics.py` & `dsspy-2.2.9/PyDSS/node_voltage_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyContrReader.py` & `dsspy-2.2.9/PyDSS/pyContrReader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/FaultController.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/FaultController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/GenController.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/GenController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/HybridController.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/MotorStall.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,230 +1,173 @@
-from  PyDSS.pyControllers.pyControllerAbstract import ControllerAbstract
+#Algebraic model for Type D motor - Residential air conditioner
+'''
+author: Kapil Duwadi
+Version: 1.0
+'''
+
+from PyDSS.pyControllers.pyControllerAbstract import ControllerAbstract
+import matplotlib.pyplot as plt
+import scipy.signal as signal
+import numpy as np
+import random
 import math
+import os
 
-class HybridController(ControllerAbstract):
-    TimeChange = False
-    Time = (-1, 0)
-
-    oldPcalc = 0
-    oldQcalc = 0
-    #dPOld = 0
-    #dQOld = 0
-
-    __vDisconnected = False
-    __pDisconnected = False
-
-    def __init__(self, PvObj, Settings, dssInstance, ElmObjectList, dssSolver):
-        super(HybridController).__init__(PvObj, Settings, dssInstance, ElmObjectList, dssSolver)
-        self.__ElmObjectList = ElmObjectList
-        self.ControlDict = {
-            'None'           : lambda: 0,
-            'CPF'            : self.CPFcontrol,
-            'VPF'            : self.VPFcontrol,
-            'VVar'           : self.VVARcontrol,
-            'VW'             : self.VWcontrol,
-            'Cutoff'         : self.CutoffControl,
-        }
-
-        self.__ControlledElm = PvObj
-        Class, Name = self.__ControlledElm.GetInfo()
-        self.__Name = 'pyCont_' + Class + '_' + Name
-        if '_' in Name:
-            self.Phase = Name.split('_')[1]
-        else:
-            self.Phase = None
-        self.__ElmObjectList = ElmObjectList
-        self.__ControlledElm = PvObj
-        self.__dssInstance = dssInstance
-        self.__dssSolver = dssSolver
+class MotorStall(ControllerAbstract):
+    """The controller locks a regulator in the event of reverse power flow. Subclass of the :class:`PyDSS.pyControllers.
+    pyControllerAbstract.ControllerAbstract` abstract class.
+
+        :param RegulatorObj: A :class:`PyDSS.dssElement.dssElement` object that wraps around an OpenDSS 'Regulator' element
+        :type FaultObj: class:`PyDSS.dssElement.dssElement`
+        :param Settings: A dictionary that defines the settings for the PvController.
+        :type Settings: dict
+        :param dssInstance: An :class:`opendssdirect` instance
+        :type dssInstance: :class:`opendssdirect`
+        :param ElmObjectList: Dictionary of all dssElement, dssBus and dssCircuit objects
+        :type ElmObjectList: dict
+        :param dssSolver: An instance of one of the classed defined in :mod:`PyDSS.SolveMode`.
+        :type dssSolver: :mod:`PyDSS.SolveMode`
+        :raises: AssertionError if 'RegulatorObj' is not a wrapped OpenDSS Regulator element
+
+    """
+        
+    def __init__(self, MotorObj, Settings, dssInstance, ElmObjectList, dssSolver):
+        super(MotorStall, self).__init__(MotorObj, Settings, dssInstance, ElmObjectList, dssSolver)
+        self._class, self._name = MotorObj.GetInfo()
+        assert self._class == "Load", "Motor stall model can only be used with load models"
+        assert MotorObj.NumPhases == 1, "Motor stall model can only be used with single phase loads"
+        
+        self.name = "Controller-{}-{}".format(self._class, self._name)
+        self._ControlledElm = MotorObj
         self.__Settings = Settings
-
-        self.update = [self.ControlDict[Settings['Control' + str(i)]] for i in [1, 2, 3]]
-
+        self.__dssSolver = dssSolver
+        self.__dssInstance = dssInstance
+        self.mode = 3
+        self.model_mode = self._ControlledElm.SetParameter('model', self.mode) # 3 - motor, 1 - Standard constant P+jQ
+        self._ControlledElm.SetParameter('vminpu', 0.0)
+
+        self.kw = self.__Settings['ratedKW']
+        S = self.kw / self.__Settings['ratedPF']
+        self.kvar = math.sqrt(S**2 - self.kw**2)
+        mode = 2
+        
+        if mode == 1:
+            self.kw_rated = self._ControlledElm.SetParameter('kw', self.kw)
+            self.kvar_rated = self._ControlledElm.SetParameter('kvar', self.kvar)        
+        elif mode == 2:
+            self.kw_rated = self._ControlledElm.GetParameter('kw')
+            self.kvar_rated = self._ControlledElm.GetParameter('kvar')
+        self.kva_rated = (self.kw_rated**2 + self.kvar_rated**2)**0.5
+            
+        self.stall_time_start = 0
+        self.stall = False
+        self.disconnected =False
+        self.Tdisconnect_start = 0
+        
+        self.R_stall_pu = self.__Settings['R_stall_pu']
+        self.kvbase = self._ControlledElm.sBus[0].GetVariable("kVBase")
+        self.Ibase = 1e3 * self.kva_rated /1e3 * self.kvbase
+
+        self.dt = dssSolver.GetStepResolutionSeconds()
+        self.H = signal.TransferFunction([1], [self.__Settings['Tth'], 1])
+        self.R = signal.TransferFunction([1], [self.__Settings['Trestart'], 1])
+        
+        self.U = [0, 0]
+        self.T = [0, self.dt]
+        self.X = 0
+
+        self.rU = [0, 0]
+        self.rT = [0, self.dt]
+        self.rX = 0
+        self.v = 0
         return
-
-    def Update(self, Priority, Time, Update):
-        self.TimeChange = self.Time != (Priority, Time)
-        self.Time = (Priority, Time)
-        # Ppv = -sum(self.__ControlledElm.GetVariable('Powers')[::2]) / self.__Prated
-        # if self.__pDisconnected:
-        #     if Ppv < self.__cutin:
-        #         return 0
-        #     else:
-        #         self.__pDisconnected = False
-        # else:
-        #     if Ppv < self.__cutout:
-        #         self.__pDisconnected = True
-        #         self.__ControlledElm.SetParameter('pf', 1)
-        #         return 0
-        return self.update[Priority]()
-
-    def VWcontrol(self):
-        uMinC = self.__Settings['uMinC']
-        uMaxC = self.__Settings['uMaxC']
-        Pmin  = self.__Settings['PminVW'] / 100
-
-        uIn = max(self.__ControlledElm.sBus[0].GetVariable('puVmagAngle')[::2])
-        Ppv = -sum(self.__ControlledElm.GetVariable('Powers')[::2]) / self.__Srated
-        Qpv = -sum(self.__ControlledElm.GetVariable('Powers')[1::2]) / self.__Srated
-        #PpvoutPU = Ppv / self.__Prated
-
-        Plim = (1 - Qpv ** 2) ** 0.5 if self.__Settings['VWtype'] == 'Available Power' else 1
-        m = (1 - Pmin) / (uMinC - uMaxC)
-        #m = (Plim - Pmin) / (uMinC - uMaxC)
-        c = ((Pmin * uMinC) - uMaxC) / (uMinC - uMaxC)
-
-        if uIn < uMinC:
-            Pcalc = Plim
-        elif uIn < uMaxC and uIn > uMinC:
-            Pcalc = min(m * uIn + c, Plim)
-        else:
-            Pcalc = Pmin
-
-        if Ppv > Pcalc or (Ppv > 0 and self.Pmppt < 100):
-            # adding heavy ball term to improve convergence
-            dP = (Ppv - Pcalc) * 0.5 / self.__dampCoef + (self.oldPcalc - Ppv) * 0.1 / self.__dampCoef
-            Pcalc = Ppv - dP
-            self.Pmppt = min(self.Pmppt * Pcalc / Ppv, 100)
-            self.__ControlledElm.SetParameter('%Pmpp', self.Pmppt)
-            self.pf = math.cos(math.atan(Qpv / Pcalc))
-            if Qpv < 0:
-                self.pf = -self.pf
-            self.__ControlledElm.SetParameter('pf', self.pf)
-        else:
-            dP = 0
-
-        Error = abs(dP)
-        self.oldPcalc = Ppv
-        return Error
-
-    def CutoffControl(self):
-        uIn = max(self.__ControlledElm.sBus[0].GetVariable('puVmagAngle')[::2])
-        uCut = self.__Settings['%UCutoff']
-        if uIn >= uCut:
-            self.__ControlledElm.SetParameter('%Pmpp', 0)
-            self.__ControlledElm.SetParameter('pf', 1)
-            if self.__vDisconnected:
-                return 0
-            else:
-                self.__vDisconnected = True
-                return self.__Prated
-
-        if self.TimeChange and self.__vDisconnected and uIn < uCut:
-            self.__ControlledElm.SetParameter('%Pmpp', self.Pmppt)
-            self.__ControlledElm.SetParameter('pf', self.pf)
-            self.__vDisconnected = False
-            return self.__Prated
-
-        return 0
-
-
-    def CPFcontrol(self):
-        PF = self.__Settings['pf']
-        self.__dssSolver.reSolve()
-
-        self.__ControlledElm.SetParameter('irradiance', 1)
-        self.__ControlledElm.SetParameter('pf', -PF)
-
-        Error = PF + float(self.__ControlledElm.GetParameter('pf'))
-
-        Pirr = float(self.__ControlledElm.GetParameter('irradiance'))
-        self.__ControlledElm.SetParameter('irradiance', Pirr * (1 + Error * 3))
-        self.__ControlledElm.SetParameter('pf', str(-PF))
-
-        return Error
-
-    def VPFcontrol(self):
-        Pmin = self.__Settings['Pmin']
-        Pmax = self.__Settings['Pmax']
-        PFmin = self.__Settings['pfMin']
-        PFmax = self.__Settings['pfMax']
-        self.__dssSolver.reSolve()
-        Pcalc = abs(sum(-(float(x)) for x in self.__ControlledElm.GetVariable('Powers')[0::2])) / self.__Srated
-        if Pcalc > 0:
-            if Pcalc < Pmin:
-                PF = PFmax
-            elif Pcalc > Pmax:
-                PF = PFmin
+    
+    def Name(self):
+        return self.name
+
+    def ControlledElement(self):
+        return "{}.{}".format(self._class, self._name)
+
+    def debugInfo(self):
+        return 
+
+    def Update(self, Priority, Time, UpdateResults):
+        
+        self.t = self.__dssSolver.GetTotalSeconds()
+        self.current_pu = self._ControlledElm.GetVariable('CurrentsMagAng')[0] / self.Ibase
+        self.voltage = self._ControlledElm.GetVariable('VoltagesMagAng')[0]
+        self.p = self._ControlledElm.GetVariable('Powers')[0]
+        self.q = self._ControlledElm.GetVariable('Powers')[1]
+        self.voltage_pu = self._ControlledElm.sBus[0].GetVariable("puVmagAngle")[0]
+
+        if Priority == 0:
+            
+            u = self.current_pu ** 2 * self.R_stall_pu       
+          
+            CompLF = self.p / self.kw_rated
+            CompPF = 1#self.p / (self.p**2 + self.q**2)**0.5
+            
+            V_stall_adj = self.__Settings['Vstall']*(1 + self.__Settings['LFadj'] * (CompLF-1))
+            V_break_adj = self.__Settings['Vbreak']*(1 + self.__Settings['LFadj'] * (CompLF-1))
+            
+            P0 = 1 - self.__Settings['Kp1'] * (1-V_break_adj)**self.__Settings['Np1']
+            Q0 = ((1 - CompPF**2)**0.5 / CompPF)-self.__Settings['Kq1']*(1-V_break_adj)**self.__Settings['Nq1']
+            
+            p_run_pu = P0 + self.__Settings['Kp1']*(self.voltage_pu-V_break_adj)**self.__Settings['Np1']
+            q_run_pu = Q0 + self.__Settings['Kq1']*(self.voltage_pu-V_break_adj)**self.__Settings['Nq1']
+            
+            p_stall_pu = P0 + self.__Settings['Kp2'] * (V_break_adj - self.voltage_pu)**self.__Settings['Np2']
+            q_stall_pu = Q0 + self.__Settings['Kq2'] * (V_break_adj - self.voltage_pu)**self.__Settings['Nq2']
+           
+            if self.voltage_pu < V_stall_adj and self.stall and self.model_mode == self.mode:
+                self.stall_time = self.__dssSolver.GetTotalSeconds() - self.stall_time_start
+                if self.stall_time > self.__Settings['Tstall']:
+                    self._ControlledElm.SetParameter('kw', self.kw_rated * self.__Settings['Pfault'] )#* abs(p_stall_pu))
+                    self._ControlledElm.SetParameter('kvar', self.kvar_rated * self.__Settings['Qfault']) #*  abs(p_stall_pu))
+                    self.model_mode = self._ControlledElm.SetParameter('model', 2)
+                      
+            if self.voltage_pu < V_stall_adj and not self.stall:
+                self.stall_time_start = self.__dssSolver.GetTotalSeconds()
+                self.stall = True
+            
+            u = 1 if self.model_mode == 2 else 0
+            
+            self.T = np.array([self.T[-1], self.t])
+            self.U = np.array([self.U[-1], u])
+            tout, yout, xout = signal.lsim2(self.H, self.U, self.T, self.X)
+            self.X = xout[-1]
+            theeta = yout[-1]
+            
+            if theeta < self.__Settings['Tth1t']:
+                Kth = 1
+            elif theeta > self.__Settings['Tth2t']:
+                Kth = 0
             else:
-                m = (PFmax - PFmin) / (Pmin - Pmax)
-                c = (PFmin * Pmin - PFmax * Pmax) / (Pmin - Pmax)
-                PF = Pcalc * m + c
-        else:
-            PF = PFmax
-
-        self.__ControlledElm.SetParameter('irradiance', 1)
-        self.__ControlledElm.SetParameter('pf', str(-PF))
-        self.__dssSolver.reSolve()
-
-        for i in range(10):
-            Error = PF + float(self.__ControlledElm.GetParameter('pf'))
-            if abs(Error) < 1E-4:
-                break
-            Pirr = float(self.__ControlledElm.GetParameter('irradiance'))
-            self.__ControlledElm.SetParameter('pf', str(-PF))
-            self.__ControlledElm.SetParameter('irradiance', Pirr * (1 + Error*1.5))
-            self.__dssSolver.reSolve()
-
+                m = 1 / (self.__Settings['Tth1t'] - self.__Settings['Tth2t'])
+                c = - m * self.__Settings['Tth2t']
+                Kth = m * theeta + c
+            
+            if self.model_mode == 2:
+                p_stall = self.kw_rated * self.__Settings['Pfault'] #* abs(p_stall_pu)
+                q_stall = self.kvar_rated * self.__Settings['Qfault'] #* abs(p_stall_pu)
+                
+                self._ControlledElm.SetParameter('kw', p_stall * Kth)
+                self._ControlledElm.SetParameter('kvar', q_stall * Kth)
+
+            if Kth==0 and self.voltage_pu > self.__Settings['Vrstrt']:
+                self.v = 1
+                
+            self.rT = np.array([self.rT[-1], self.t])
+            self.rU = np.array([self.rU[-1], self.v])
+            _, yout_r, xout_r = signal.lsim2(self.R, self.rU, self.rT, self.rX)
+            self.rX = xout_r[-1]
+            reconnect = yout_r[-1]
+
+            if reconnect > 0:
+                self.model_mode = self._ControlledElm.SetParameter('model', self.mode)
+                self._ControlledElm.SetParameter('kw', self.kw_rated * reconnect)
+                self._ControlledElm.SetParameter('kvar', self.kvar_rated * reconnect)
+                self.stall = False
+         
+        self.model_mode_old = self.model_mode
         return 0
 
-    def VVARcontrol(self):
-        uMin = self.__Settings['uMin']
-        uMax = self.__Settings['uMax']
-        pfLim = self.__Settings['PFlim']
-        uDbMin = self.__Settings['uDbMin']
-        uDbMax = self.__Settings['uDbMax']
-        Priority = self.__Settings['Priority']
-
-        uIn = max(self.__ControlledElm.sBus[0].GetVariable('puVmagAngle')[::2])
-
-        m1 = self.QlimPU / (uMin - uDbMin)
-        m2 = self.QlimPU / (uDbMax - uMax)
-        c1 = self.QlimPU * uDbMin / (uDbMin - uMin)
-        c2 = self.QlimPU * uDbMax / (uMax - uDbMax)
-
-        Ppv = abs(sum(self.__ControlledElm.GetVariable('Powers')[::2]))
-        Pcalc = Ppv / self.__Srated
-        Qpv = -sum(self.__ControlledElm.GetVariable('Powers')[1::2])
-        Qpv = Qpv / self.__Srated
-
-        Qcalc = 0
-        if uIn <= uMin:
-            Qcalc = self.QlimPU
-        elif uIn <= uDbMin and uIn > uMin:
-            Qcalc = uIn * m1 + c1
-        elif uIn <= uDbMax and uIn > uDbMin:
-            Qcalc = 0
-        elif uIn <= uMax and uIn > uDbMax:
-            Qcalc = uIn * m2 + c2
-        elif uIn >= uMax:
-            Qcalc = -self.QlimPU
-
-        # adding heavy ball term to improve convergence
-        Qcalc = Qpv + (Qcalc - Qpv) * 0.5 / self.__dampCoef + (Qpv - self.oldQcalc) * 0.1 / self.__dampCoef
-        dQ = abs(Qcalc - Qpv)
-
-        if Priority == 'Var':
-            Plim = (1 - Qcalc ** 2) ** 0.5
-            if self.TimeChange:
-                self.Pmppt = 100
-            if Pcalc > Plim and self.TimeChange is False:
-                self.Pmppt = Plim / self.__Prated * self.__Srated * 100
-                Pcalc = Plim
-            self.__ControlledElm.SetParameter('%Pmpp', self.Pmppt)
-        else:
-            pass
-
-        if Pcalc > 0:
-            self.pf = math.cos(math.atan(Qcalc / Pcalc))
-            if self.__Settings['Enable PF limit'] and abs(self.pf) < pfLim:
-                self.pf = pfLim
-            if Qcalc < 0:
-                self.pf = -self.pf
-            self.__ControlledElm.SetParameter('pf', self.pf)
-        else:
-            pass
-
-        Error = abs(dQ)
-        self.oldQcalc = Qpv
-
-        return Error
```

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/MotorStall.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/MotorStallSimple.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Version: 1.0
 '''
 
 from PyDSS.pyControllers.pyControllerAbstract import ControllerAbstract
 import random
 import math
 
-class MotorStall(ControllerAbstract):
+class MotorStallSimple(ControllerAbstract):
     """The controller locks a regulator in the event of reverse power flow. Subclass of the :class:`PyDSS.pyControllers.
     pyControllerAbstract.ControllerAbstract` abstract class.
 
                 :param RegulatorObj: A :class:`PyDSS.dssElement.dssElement` object that wraps around an OpenDSS 'Regulator' element
                 :type FaultObj: class:`PyDSS.dssElement.dssElement`
                 :param Settings: A dictionary that defines the settings for the PvController.
                 :type Settings: dict
@@ -24,24 +24,26 @@
                 :type dssSolver: :mod:`PyDSS.SolveMode`
                 :raises: AssertionError if 'RegulatorObj' is not a wrapped OpenDSS Regulator element
 
         """
 
 
     def __init__(self, MotorObj, Settings, dssInstance, ElmObjectList, dssSolver):
-        super(MotorStall, self).__init__(MotorObj, Settings, dssInstance, ElmObjectList, dssSolver)
+        super(MotorStallSimple, self).__init__(MotorObj, Settings, dssInstance, ElmObjectList, dssSolver)
         self._class, self._name = MotorObj.GetInfo()
         self.name = "Controller-{}-{}".format(self._class, self._name)
         self._ControlledElm = MotorObj
         self.__Settings = Settings
         self.__dssSolver = dssSolver
 
         self._ControlledElm.SetParameter('model', 2)
         self._ControlledElm.SetParameter('vminpu', 0.0)
-
+        self._ControlledElm.SetParameter('vlowpu', 0.0)
+        # self.kw = self._ControlledElm.GetParameter('kw')
+        # self.kvar = self._ControlledElm.GetParameter('kvar')
         self.kw = self.__Settings['ratedKW']
         S = self.kw / self.__Settings['ratedPF']
         self.kvar = math.sqrt(S**2 - self.kw**2)
         self._ControlledElm.SetParameter('kw', self.kw)
         self._ControlledElm.SetParameter('kvar', self.kvar)
         self.stall_time_start = 0
         self.stall = False
@@ -57,42 +59,43 @@
         return "{}.{}".format(self._class, self._name)
 
     def debugInfo(self):
         return [self.__Settings['Control{}'.format(i+1)] for i in range(3)]
 
 
     def Update(self, Priority, Time, UpdateResults):
+        assert Priority in [0, 1, 2], "Valid control priorities can range from 0-2."
         if Priority == 0:
             Vbase = self._ControlledElm.sBus[0].GetVariable('kVBase')
             Ve_mags = max(self._ControlledElm.GetVariable('VoltagesMagAng')[::2])/ 120.0
 
+
             if Ve_mags < self.__Settings['Vstall'] and not self.stall:
-                self._ControlledElm.SetParameter('kw', self.kw * self.__Settings['Pfault'])
-                self._ControlledElm.SetParameter('kvar', self.kw * self.__Settings['Qfault'])
+                self._ControlledElm.SetParameter('kw', self.kw * self.__Settings['Pfault'] )
+                self._ControlledElm.SetParameter('kvar', self.kw * self.__Settings['Qfault'] )
                 self._ControlledElm.SetParameter('model', 1)
                 self.stall = True
                 self.stall_time_start = self.__dssSolver.GetTotalSeconds()
                 return 0.1
             return 0
         if Priority == 1:
             if self.stall:
                 self.stall_time = self.__dssSolver.GetTotalSeconds() - self.stall_time_start
                 if self.stall_time > self.__Settings['Tprotection']:
                     self.stall = False
                     self.disconnected = True
                     self._ControlledElm.SetParameter('kw', 0)
                     self._ControlledElm.SetParameter('kvar', 0)
                     self.Tdisconnect_start = self.__dssSolver.GetTotalSeconds()
-                return 0
+                return 0 #self.model_1(Priority)
             return 0
         if Priority == 2:
             if self.disconnected:
                 time = self.__dssSolver.GetTotalSeconds() - self.Tdisconnect_start
                 if time > self.__Settings['Treconnect']:
                     self.disconnected = False
                     self._ControlledElm.SetParameter('kw', self.kw)
                     self._ControlledElm.SetParameter('kvar', self.kvar)
                     self._ControlledElm.SetParameter('model', 2)
                     self._ControlledElm.SetParameter('vminpu', 0.0)
-
         return 0
```

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvController.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/PvController.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         :raises: AssertionError if 'PvObj' is not a wrapped OpenDSS PVSystem element
 
     """
 
     def __init__(self, PvObj, Settings, dssInstance, ElmObjectList, dssSolver):
         """Constructor method
         """
+        
         super(PvController, self).__init__(PvObj, Settings, dssInstance, ElmObjectList, dssSolver)
         self.TimeChange = False
         self.Time = (-1, 0)
-
         self.oldQpv = 0
         self.oldPcalc = 0
 
         self.__vDisconnected = False
         self.__pDisconnected = False
 
         self.__ElmObjectList = ElmObjectList
```

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/SocketController.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/SocketController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/StorageController.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/StorageController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/ThermostaticLoad.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/ThermostaticLoad.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,16 +22,14 @@
         self.__ControlledElm.SetParameter("kw", Settings["kw"])
         self.Prated = LoadObj.GetParameter("kw")
 
 
         self.a = 1 / (Settings["R"] * Settings["C"])
         self.b = Settings["mu"] / Settings["C"]
         self.w = 0
-        self.f = open(r"C:\Users\alatif\Desktop\tcl\results.csv", "w")
-        self.f.write("Tamb,T,State\n")
         return
 
     @property
     def Name(self):
         return self.__Name
 
     def debugInfo(self):
@@ -58,13 +56,11 @@
 
             if self.T > self.Tmax:
                 self.On = True
                 self.__ControlledElm.SetParameter("kw", self.Prated)
             elif self.T < self.Tmin:
                 self.On = False
                 self.__ControlledElm.SetParameter("kw", 0)
-
-            self.f.write(f"{Ta},{self.T},{self.On}" + "\n")
         return 0
 
     def __del__(self):
         self.f.close()
```

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/Controllers/xfmrController.py` & `dsspy-2.2.9/PyDSS/pyControllers/Controllers/xfmrController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyControllers/pyController.py` & `dsspy-2.2.9/PyDSS/pyControllers/pyController.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 
 def Create(ElmName, ControllerType, Settings, ElmObjectList, dssInstance, dssSolver):
 
     assert (ControllerType in ControllerTypes), "Definition for '{}' controller not found. \n " \
                                                 "Please define the controller in ~PyDSS\pyControllers\Controllers".format(
         ControllerType
     )
+
     assert (ElmName in ElmObjectList), "'{}' does not exist in the PyDSS master object dictionary.".format(ElmName)
     relObject = ElmObjectList[ElmName]
+    
     # except:
     #     Index = dssInstance.Circuit.SetActiveElement(ElmName)
     #     if int(Index) >= 0:
     #         ElmObjectList[ElmName] = dssElement(dssInstance)
     #         relObject = ElmObjectList[ElmName]
     # else:
     #     return -1
 
-
     ObjectController = ControllerTypes[ControllerType](relObject, Settings, dssInstance, ElmObjectList, dssSolver)
     return ObjectController
```

### Comparing `dsspy-2.2.8/PyDSS/pyDSS.py` & `dsspy-2.2.9/PyDSS/pyDSS.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyLogger.py` & `dsspy-2.2.9/PyDSS/pyLogger.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlotReader.py` & `dsspy-2.2.9/PyDSS/pyPlotReader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/FrequencySweep.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/FrequencySweep.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/Histogram.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/Histogram.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/NetworkGraph.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/NetworkGraph.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/Table.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/Table.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/ThreeDim.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/ThreeDim.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/TimeSeries.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/Topology.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/Topology.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/VoltageDistance.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/VoltageDistance.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/Plots/XY.py` & `dsspy-2.2.9/PyDSS/pyPlots/Plots/XY.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/pyPlotAbstract.py` & `dsspy-2.2.9/PyDSS/pyPlots/pyPlotAbstract.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPlots/pyPlots.py` & `dsspy-2.2.9/PyDSS/pyPlots/pyPlots.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py` & `dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py` & `dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py` & `dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     return ovrl, affected_buses
 
 
 def form_pvzones(affected_buses, dismat_df, zone_thr):
     """
     Builds PV zones
     """
-    # print('Affected buses:', affected_buses)
+    # #print('Affected buses:', affected_buses)
     ohmy = dismat_df.loc[affected_buses, :].copy()
     zone = list()
     for col in ohmy.columns:
         if min(ohmy.loc[:, col]) <= zone_thr:
             zone.append(col)
 
     return zone
@@ -536,15 +536,15 @@
                 bus1 = dss.Properties.Value("bus1")
                 if bus1 in self.zone:
                     lifo_pv_list.append(pv)
 
         lifo_pv_list = list(lifo_pv_list)
         if self.zone and not lifo_pv_list:
             self.comment = f"No PV system found in the vicinity (radius={self.zone_threshold}) of the thermal overload"
-            # print(comment)
+            # #print(comment)
 
         if self.zone_option == "Yes" and lifo_pv_list:
             self.my_lifo_list = lifo_pv_list + [
                 x for x in self.poa_lifo_ordered_pv_list if not x in lifo_pv_list
             ]
 
         else:
@@ -562,15 +562,15 @@
         self.PV_curtailed = dict()
         self.PV_kW_curtailed = dict()
         self.pvbus_voltage = dict()
         self.solution_status = -1
         self.comment = "RAS"
         total_kVA_deployed = self.pvs_df["kVARated"].sum()
         self.total_init_kW_deployed = 0
-        # print("Total PV KVA deployed: ",total_kVA_deployed)
+        # #print("Total PV KVA deployed: ",total_kVA_deployed)
         self.total_kVA_curtailed = 0
         self.total_kW_curtailed = 0
         self.total_kW_output = 0
         Pct_kW_curtailment = 0
 
         for pv_sys in self.poa_lifo_ordered_pv_list:
             # pv_sys_n = remove_pen(pv_sys)
@@ -590,15 +590,15 @@
         self.zone = []
 
         if self.affected_buses:
 
             self.zone = form_pvzones(
                 self.affected_buses, self.dismat_df, self.zone_threshold
             )
-            # print('zone length:',len(zone))
+            # #print('zone length:',len(zone))
 
         else:
             self.logger.info("No monitored line affected")
 
         self.get_curtailment_candidates()
 
         self.solution_status = 0
@@ -619,15 +619,15 @@
             self.solve_overloads()
 
         if self.solution_status == -1:
             self.comment = "No need to curtail!"
 
         if max(self.PV_curtailed.keys(), key=(lambda k: self.PV_curtailed[k])) == 0:
             self.comment = "Deployment passed without curtailment!"
-            # print(comment)
+            # #print(comment)
             self.solution_status == 0
 
         self.PV_curtailed["Comment"] = self.comment
         Pct_curtailment = self.total_kVA_curtailed * 100 / max(1, total_kVA_deployed)
         self.PV_curtailed["Pct_curtailment"] = Pct_curtailment
 
         Pct_kW_curtailment = (
@@ -635,15 +635,15 @@
         )
         self.PV_kW_curtailed["Pct_kW_curtailment"] = Pct_kW_curtailment
         self.PV_kW_curtailed["Total_PV_kW_deployed"] = self.total_init_kW_deployed
         self.PV_kW_curtailed["Total_PV_kW_curtailed"] = self.total_kW_curtailed
         self.PV_kW_curtailed["Total_PV_kW_output"] = self.total_kW_output
 
         self.PV_kW_curtailed["Comment"] = self.comment
-        # print("Done with 1 poa loop:", Pct_curtailment)
+        # #print("Done with 1 poa loop:", Pct_curtailment)
 
         self.logger.info(f"kW Curtailed: {self.PV_kW_curtailed}")
         self.has_converged = sol.Converged()
         self.error = sol.Convergence()
         # This error is fake for now, find how to get this from Opendssdirect
 
     def run(self, step, stepMax, simulation=None):
```

### Comparing `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py` & `dsspy-2.2.9/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,14 @@
         with open(fpath, "w") as f:
             f.write(json_object)
         url = f"https://nrel.utilidatacloud.com/optimize/{self._uuid}"
         headers = {'Content-type': 'application/json'}
         reply = requests.post(url, data=json_object, verify=False, headers=headers)
         if reply.status_code == 200:
             reply = reply.json()
-            print(reply)
             return reply['recommendations']
         else:
             reply = reply.json()
             self.logger.error(f"Error optimizing the model.{reply['message']}")
             #raise Exception(f"Error optimizing the model.\nReply from the server:\n{reply.text}")
 
     def disable_control_elements(self):
@@ -417,15 +416,15 @@
 
     def poll_api(self, req_type, payload):
         # Initiate http request - kwargs are constructed into a dict and passed as optional parameters
         # Ex (limit=100, sortorder='desc', startdate='1970-10-03', etc)
         r = requests.get(self.url + req_type, headers=self.h, params=payload)
 
         if r.status_code != 200:  # Handle erroneous requests
-            print("Error: " + str(r.status_code))
+            self.logger.error("Error: " + str(r.status_code))
         else:
             r = r.json()
             try:
                 return r['results']  # Most JSON results are nested under 'results' key
             except KeyError:
                 return r  # for non-nested results, return the entire JSON string
```

### Comparing `dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocess.py` & `dsspy-2.2.9/PyDSS/pyPostprocessor/pyPostprocess.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocessAbstract.py` & `dsspy-2.2.9/PyDSS/pyPostprocessor/pyPostprocessAbstract.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pyResults.py` & `dsspy-2.2.9/PyDSS/pyResults.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pydss_fs_interface.py` & `dsspy-2.2.9/PyDSS/pydss_fs_interface.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pydss_project.py` & `dsspy-2.2.9/PyDSS/pydss_project.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/pydss_results.py` & `dsspy-2.2.9/PyDSS/pydss_results.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/registry.py` & `dsspy-2.2.9/PyDSS/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                 ),
             },
         ],
         ControllerType.SOCKET_CONTROLLER.value: [],
         ControllerType.STORAGE_CONTROLLER.value: [],
         ControllerType.XMFR_CONTROLLER.value: [],
         ControllerType.MOTOR_STALL.value: [],
+        ControllerType.MOTOR_STALL_SIMPLE.value: [],
         ControllerType.PV_VOLTAGE_RIDETHROUGH.value: [],
         ControllerType.FAULT_CONTROLLER.value: [],
     },
 }
 
 REQUIRED_CONTROLLER_FIELDS = ("name", "filename")
```

### Comparing `dsspy-2.2.8/PyDSS/reports/capacitor_change_count.py` & `dsspy-2.2.9/PyDSS/reports/capacitor_change_count.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/reports/feeder_losses.py` & `dsspy-2.2.9/PyDSS/reports/feeder_losses.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/reports/pv_reports.py` & `dsspy-2.2.9/PyDSS/reports/pv_reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/reports/reg_control_tap_number_change_count.py` & `dsspy-2.2.9/PyDSS/reports/reg_control_tap_number_change_count.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/reports/reports.py` & `dsspy-2.2.9/PyDSS/reports/reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/reports/thermal_metrics.py` & `dsspy-2.2.9/PyDSS/reports/thermal_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/reports/voltage_metrics.py` & `dsspy-2.2.9/PyDSS/reports/voltage_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/simulation_input_models.py` & `dsspy-2.2.9/PyDSS/simulation_input_models.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/storage_filters.py` & `dsspy-2.2.9/PyDSS/storage_filters.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/thermal_metrics.py` & `dsspy-2.2.9/PyDSS/thermal_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/unitDefinations.py` & `dsspy-2.2.9/PyDSS/unitDefinations.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/utils/dataframe_utils.py` & `dsspy-2.2.9/PyDSS/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/utils/dss_utils.py` & `dsspy-2.2.9/PyDSS/utils/dss_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/utils/pydss_utils.py` & `dsspy-2.2.9/PyDSS/utils/pydss_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/utils/simulation_utils.py` & `dsspy-2.2.9/PyDSS/utils/simulation_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/utils/timing_utils.py` & `dsspy-2.2.9/PyDSS/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/utils/utils.py` & `dsspy-2.2.9/PyDSS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/PyDSS/value_storage.py` & `dsspy-2.2.9/PyDSS/value_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,14 +597,15 @@
 
         Parameters
         ----------
         value : list
             list of ValueStorageBase
 
         """
+        
         if isinstance(values[0].value, list):
             vals = [x for y in values for x in y.value]
         else:
             vals = [x.value for x in values]
 
         self._dataset.write_value(vals)
 
@@ -614,22 +615,24 @@
         Parameters
         ----------
         value : ValueStorageBase
         time_step : int
         elem_index : int
 
         """
+        
         if isinstance(value.value, list):
             vals = [x for x in value.value]
         else:
             vals = value.value
 
         self._dataset.write_value(vals)
         self._time_steps.write_value([time_step, elem_index])
-
+        
+        
     def flush_data(self):
         """Flush any outstanding data to disk."""
         self._dataset.flush_data()
         if self._time_steps is not None:
             self._time_steps.flush_data()
 
     def max_num_bytes(self):
```

### Comparing `dsspy-2.2.8/dsspy.egg-info/PKG-INFO` & `dsspy-2.2.9/dsspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsspy
-Version: 2.2.8
+Version: 2.2.9
 Summary: A high-level python interface for OpenDSS
 Home-page: http://www.github.com/nrel/pydss
 Author: Aadil Latif
 Author-email: Aadil.Latif@nrel.gov
 License: BSD 3 clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `dsspy-2.2.8/dsspy.egg-info/SOURCES.txt` & `dsspy-2.2.9/dsspy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -85,18 +85,22 @@
 PyDSS/defaults/ExportLists/Subscriptions.toml
 PyDSS/defaults/ExportLists/__init__.py
 PyDSS/defaults/Monte_Carlo/MonteCarloSettings.toml
 PyDSS/defaults/Monte_Carlo/__init__.py
 PyDSS/defaults/pyControllerList/FaultController.toml
 PyDSS/defaults/pyControllerList/GenController.toml
 PyDSS/defaults/pyControllerList/MotorStall.toml
+PyDSS/defaults/pyControllerList/MotorStallSimple.toml
 PyDSS/defaults/pyControllerList/PvController.toml
+PyDSS/defaults/pyControllerList/PvDynamic.toml
+PyDSS/defaults/pyControllerList/PvFrequencyRideThru.toml
 PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml
 PyDSS/defaults/pyControllerList/SocketController.toml
 PyDSS/defaults/pyControllerList/StorageController.toml
+PyDSS/defaults/pyControllerList/ThermostaticLoad.toml
 PyDSS/defaults/pyControllerList/__init__.py
 PyDSS/defaults/pyControllerList/xfmrController.toml
 PyDSS/defaults/pyPlotList/FrequencySweep.toml
 PyDSS/defaults/pyPlotList/Histogram.toml
 PyDSS/defaults/pyPlotList/NetworkGraph.toml
 PyDSS/defaults/pyPlotList/Table.toml
 PyDSS/defaults/pyPlotList/ThreeDim.toml
@@ -111,17 +115,19 @@
 PyDSS/modes/__init__.py
 PyDSS/modes/solver_base.py
 PyDSS/pyControllers/__init__.py
 PyDSS/pyControllers/pyController.py
 PyDSS/pyControllers/pyControllerAbstract.py
 PyDSS/pyControllers/Controllers/FaultController.py
 PyDSS/pyControllers/Controllers/GenController.py
-PyDSS/pyControllers/Controllers/HybridController.py
 PyDSS/pyControllers/Controllers/MotorStall.py
+PyDSS/pyControllers/Controllers/MotorStallSimple.py
 PyDSS/pyControllers/Controllers/PvController.py
+PyDSS/pyControllers/Controllers/PvDynamic.py
+PyDSS/pyControllers/Controllers/PvFrequencyRideThru.py
 PyDSS/pyControllers/Controllers/PvVoltageRideThru.py
 PyDSS/pyControllers/Controllers/SocketController.py
 PyDSS/pyControllers/Controllers/StorageController.py
 PyDSS/pyControllers/Controllers/ThermostaticLoad.py
 PyDSS/pyControllers/Controllers/__init__.py
 PyDSS/pyControllers/Controllers/xfmrController.py
 PyDSS/pyControllers/Controllers/Settings/PvControllers.toml
```

### Comparing `dsspy-2.2.8/setup.py` & `dsspy-2.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/common.py` & `dsspy-2.2.9/tests/common.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_auto_snapshot_time_point.py` & `dsspy-2.2.9/tests/test_auto_snapshot_time_point.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_custom_exports.py` & `dsspy-2.2.9/tests/test_custom_exports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_dataset_buffer.py` & `dsspy-2.2.9/tests/test_dataset_buffer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_export_list_reader.py` & `dsspy-2.2.9/tests/test_export_list_reader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_metrics.py` & `dsspy-2.2.9/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_opendss_export_overloads.py` & `dsspy-2.2.9/tests/test_opendss_export_overloads.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_opendss_export_powers.py` & `dsspy-2.2.9/tests/test_opendss_export_powers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_pv_reports.py` & `dsspy-2.2.9/tests/test_pv_reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_pydss_examples.py` & `dsspy-2.2.9/tests/test_pydss_examples.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_pydss_project.py` & `dsspy-2.2.9/tests/test_pydss_project.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_registry.py` & `dsspy-2.2.9/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.8/tests/test_space_estimation.py` & `dsspy-2.2.9/tests/test_space_estimation.py`

 * *Files identical despite different names*

