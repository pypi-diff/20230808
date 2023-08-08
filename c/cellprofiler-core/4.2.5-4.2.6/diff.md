# Comparing `tmp/cellprofiler-core-4.2.5.tar.gz` & `tmp/cellprofiler-core-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellprofiler-core-4.2.5.tar", last modified: Wed Dec 14 18:52:49 2022, max compression
+gzip compressed data, was "cellprofiler-core-4.2.6.tar", last modified: Tue Aug  8 15:00:38 2023, max compression
```

## Comparing `cellprofiler-core-4.2.5.tar` & `cellprofiler-core-4.2.6.tar`

### file list

```diff
@@ -1,611 +1,611 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      493 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.900687 cellprofiler-core-4.2.5/cellprofiler_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.904687 cellprofiler-core-4.2.5/cellprofiler_core/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30285 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/_worker_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.904687 cellprofiler-core-4.2.5/cellprofiler_core/analysis/event/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/event/_finished.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/event/_paused.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/event/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/event/_resumed.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/event/_started.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.904687 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_ack.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_debug_cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_dictionary_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_exception_please_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_image_set_success.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_image_set_success_with_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_no_work.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_omero_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_server_exited.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_shared_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/_work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.908687 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_analysis_cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_debug_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_debug_waiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_display_post_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_display_post_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_exception_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_initial_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_measurements_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_omero_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_pipeline_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_shared_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.908687 cellprofiler-core-4.2.5/cellprofiler_core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/commands/_pipeline_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/commands/_worker_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.912687 cellprofiler-core-4.2.5/cellprofiler_core/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.912687 cellprofiler-core-4.2.5/cellprofiler_core/constants/module/
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/module/_identify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.912687 cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/images.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/constants/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.912687 cellprofiler-core-4.2.5/cellprofiler_core/image/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/_grayscale_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/_image_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/_image_set_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/_rgb_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.912687 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/_abstract_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/_callback_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/_vanilla_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.916687 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/_file_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/_flex_frame_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/_movie_frame_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.916687 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_color_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_mask_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_objects_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_url_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.916687 cellprofiler-core-4.2.5/cellprofiler_core/measurement/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71679 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/measurement/_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/measurement/_metadata_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/measurement/_relationship_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.916687 cellprofiler-core-4.2.5/cellprofiler_core/module/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/_identify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38204 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/_plugin_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.920687 cellprofiler-core-4.2.5/cellprofiler_core/module/image_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/image_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/image_segmentation/_image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/module/image_segmentation/_object_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.920687 cellprofiler-core-4.2.5/cellprofiler_core/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30948 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/align.py
--rw-r--r--   0 runner    (1001) docker     (123)    33452 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/inject_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/injectimage.py
--rw-r--r--   0 runner    (1001) docker     (123)    61221 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/loaddata.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/measurementfixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    69915 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)   104716 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/namesandtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/modules/setting_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.920687 cellprofiler-core-4.2.5/cellprofiler_core/object/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/object/_object_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    17585 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/object/_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/object/_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.924687 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_image_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_image_set_channel_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)   100895 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.924687 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_image_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_measurement_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_object_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.928687 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_end_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_file_walk_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_file_walk_started.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_ipd_load_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_load_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_module_added.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_module_disabled.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_module_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_module_enabled.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_module_moved.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_module_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_module_show_window.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_pipeline_cleared.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_pipeline_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_prepare_run_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_urls_added.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_urls_removed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.928687 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/run_exception/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/run_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/run_exception/_post_run_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/run_exception/_prepare_run_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/run_exception/_run_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.928687 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/io/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/io/_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/pipeline/io/_v6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.928687 cellprofiler-core-4.2.5/cellprofiler_core/preferences/
--rw-r--r--   0 runner    (1001) docker     (123)    63252 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/preferences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/preferences/_headless_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.932687 cellprofiler-core-4.2.5/cellprofiler_core/setting/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_binary_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_delete_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_divider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_do_things.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_figure_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_file_collection_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_hidden_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_html_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_image_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_path_list_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_regexp_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_settings_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_structuring_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_tree_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/_validation_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.932687 cellprofiler-core-4.2.5/cellprofiler_core/setting/change_setting_event/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/change_setting_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/change_setting_event/_after_change_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/change_setting_event/_change_setting_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.932687 cellprofiler-core-4.2.5/cellprofiler_core/setting/choice/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/choice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/choice/_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/choice/_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/choice/_custom_choice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.936687 cellprofiler-core-4.2.5/cellprofiler_core/setting/do_something/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/do_something/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/do_something/_do_something.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/do_something/_image_set_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/do_something/_path_list_refresh_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/do_something/_remove_setting_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.936687 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_compound_filter_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_directory_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_does_not_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_does_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_extension_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_file_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_filter_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_image_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_metadata_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_regexp_filter_predicate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.936687 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_image_name_subscriber_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_measurement_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_object_subscriber_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_subdirectory_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.940687 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/_float_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.940687 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/integer_range/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/integer_range/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/range/integer_range/_integer_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.940687 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/_grid_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/_label_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.940687 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.940687 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/list_subscriber/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/list_subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/list_subscriber/_image_list_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/list_subscriber/_label_list_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.940687 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.944687 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/_character.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.944687 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/_grid_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.944687 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/_crop_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/_file_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/_outline_image_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.944687 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.944687 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/integer/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/integer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/integer/_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/integer/_odd_integer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.944687 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/pathname/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/pathname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/pathname/_pathname.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/setting/text/pathname/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/module/identify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/modules/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)   113440 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/hdf5_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/pathname.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/utf16encode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/_analysis_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/_boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/_communicable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/_lock_status_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/_upstream_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.948687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_boundary_exited.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_upstream_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.952687 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/request/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/request/_lock_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/request/_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.952687 cellprofiler-core-4.2.5/cellprofiler_core/worker/
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/worker/_pipeline_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)    22680 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/worker/_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.952687 cellprofiler-core-4.2.5/cellprofiler_core/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/workspace/_disposition_changed_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    21566 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/cellprofiler_core/workspace/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.904687 cellprofiler-core-4.2.5/cellprofiler_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2022-12-14 18:52:48.000000 cellprofiler-core-4.2.5/cellprofiler_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25254 2022-12-14 18:52:48.000000 cellprofiler-core-4.2.5/cellprofiler_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 18:52:48.000000 cellprofiler-core-4.2.5/cellprofiler_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 18:52:48.000000 cellprofiler-core-4.2.5/cellprofiler_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-14 18:52:48.000000 cellprofiler-core-4.2.5/cellprofiler_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-14 18:52:48.000000 cellprofiler-core-4.2.5/cellprofiler_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.900687 cellprofiler-core-4.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.952687 cellprofiler-core-4.2.5/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69010 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/analysis/test_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.952687 cellprofiler-core-4.2.5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.956687 cellprofiler-core-4.2.5/tests/core/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.956687 cellprofiler-core-4.2.5/tests/core/image/abstract_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.956687 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/test__file_image.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/test__flex_frame_image.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/test__movie_frame_image.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/test__stk_frame_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.960687 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/url/test__color_image.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/url/test__mask_image.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/url/test__monochrome_image.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/url/test__objects_image.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/url/test__url_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/test__abstract_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/test__callback_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/abstract_image/test__vanilla_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/test__grayscale_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/test__image.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/test__image_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/test__image_set_list.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/image/test__rgb_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.960687 cellprofiler-core-4.2.5/tests/core/measurement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/measurement/test__measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/measurement/test__metadata_group.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/measurement/test__relationship_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.960687 cellprofiler-core-4.2.5/tests/core/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.960687 cellprofiler-core-4.2.5/tests/core/module/image_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/image_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/image_segmentation/test__image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/image_segmentation/test__object_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/test__identify.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/test__image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/test__module.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/module/test__plugin_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.964687 cellprofiler-core-4.2.5/tests/core/object/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/object/test__object_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/object/test__objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/object/test__segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.964687 cellprofiler-core-4.2.5/tests/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.964687 cellprofiler-core-4.2.5/tests/core/pipeline/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/dependency/test__dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/dependency/test__image_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/dependency/test__measurement_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/dependency/test__object_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.968687 cellprofiler-core-4.2.5/tests/core/pipeline/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.968687 cellprofiler-core-4.2.5/tests/core/pipeline/event/run_exception/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/run_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/run_exception/test__post_run_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/run_exception/test__prepare_run_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/run_exception/test__run_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__end_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__event.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__file_walk_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__file_walk_started.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__ipd_load_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__load_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__module_added.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__module_disabled.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__module_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__module_enabled.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__module_moved.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__module_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__module_show_window.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__pipeline_cleared.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__pipeline_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__prepare_run_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__urls_added.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/event/test__urls_removed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.968687 cellprofiler-core-4.2.5/tests/core/pipeline/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/test__image_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/test__image_set_channel_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/test__listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/pipeline/test__pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.972687 cellprofiler-core-4.2.5/tests/core/setting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.976687 cellprofiler-core-4.2.5/tests/core/setting/change_setting_event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/change_setting_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/change_setting_event/test__after_change_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/change_setting_event/test__before_change_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/change_setting_event/test__change_setting_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.976687 cellprofiler-core-4.2.5/tests/core/setting/choice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/choice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/choice/test__choice.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/choice/test__colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/choice/test__custom_choice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.976687 cellprofiler-core-4.2.5/tests/core/setting/do_something/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/do_something/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/do_something/test__do_something.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/do_something/test__image_set_display.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/do_something/test__path_list_refresh_button.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/do_something/test__remove_setting_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.980687 cellprofiler-core-4.2.5/tests/core/setting/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__compound_filter_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__directory_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__does_not_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__does_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__extension_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__file_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__filter_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__image_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__metadata_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/filter/test__regexp_filter_predicate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.980687 cellprofiler-core-4.2.5/tests/core/setting/multichoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/multichoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/multichoice/test__image_name_subscriber_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/multichoice/test__measurement_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/multichoice/test__multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/multichoice/test__object_subscriber_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/multichoice/test__subdirectory_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/multichoice/test__subscriber_multichoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.980687 cellprofiler-core-4.2.5/tests/core/setting/range/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/range/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.980687 cellprofiler-core-4.2.5/tests/core/setting/range/integer_range/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/range/integer_range/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/range/integer_range/test__integer_or_unbounded_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/range/integer_range/test__integer_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/range/test__float_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/range/test__range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.980687 cellprofiler-core-4.2.5/tests/core/setting/subscriber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.984687 cellprofiler-core-4.2.5/tests/core/setting/subscriber/image_subscriber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/image_subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/image_subscriber/test__crop_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/image_subscriber/test__file_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/image_subscriber/test__image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/image_subscriber/test__outline_image_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.984687 cellprofiler-core-4.2.5/tests/core/setting/subscriber/list_subscriber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/list_subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/list_subscriber/test__image_list_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/list_subscriber/test__label_list_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/list_subscriber/test__list_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/test__grid_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/test__label_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/subscriber/test__subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__binary_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__color.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__delete_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__divider.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__do_things.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__figure_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__file_collection_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__hidden_count.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__html_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__image_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__path_list_display.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__regexp_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__settings_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__structuring_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__table.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__tree_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/test__validation_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.984687 cellprofiler-core-4.2.5/tests/core/setting/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.984687 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.984687 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.988687 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/image_name/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/image_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/image_name/test__crop_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/image_name/test__external_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/image_name/test__file_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/image_name/test__image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/image_name/test__outline_image_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/test__grid_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/test__label_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/name/test__name.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/alphanumeric/test__alphanumeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.988687 cellprofiler-core-4.2.5/tests/core/setting/text/number/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/number/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.988687 cellprofiler-core-4.2.5/tests/core/setting/text/number/integer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/number/integer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/number/integer/test__integer.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/number/integer/test__odd_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/number/test__float.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/number/test__number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.988687 cellprofiler-core-4.2.5/tests/core/setting/text/pathname/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/pathname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/pathname/test__pathname.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/pathname/test__url.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/test__directory.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/test__filename.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/setting/text/test__text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.988687 cellprofiler-core-4.2.5/tests/core/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/worker/test__pipeline_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/worker/test__worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.988687 cellprofiler-core-4.2.5/tests/core/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/workspace/test__disposition_changed_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/core/workspace/test__workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.992687 cellprofiler-core-4.2.5/tests/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/image/test_image_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/image/test_image_set_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.992687 cellprofiler-core-4.2.5/tests/measurement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56902 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/measurement/test_measurements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.992687 cellprofiler-core-4.2.5/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10221 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/module/test_image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/module/test_object_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.992687 cellprofiler-core-4.2.5/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    28484 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41457 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/test_injectimage.py
--rw-r--r--   0 runner    (1001) docker     (123)    37147 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/test_loaddata.py
--rw-r--r--   0 runner    (1001) docker     (123)    36806 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    91427 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/modules/test_namesandtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/tests/object/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39054 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/object/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/object/test_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/pipeline/test_image_plane_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    57252 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/pipeline/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/tests/preferences/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/preferences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/preferences/test_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/tests/setting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/setting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/setting/test_namesubscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    14612 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/setting/test_setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46839 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/worker/test_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:48.996688 cellprofiler-core-4.2.5/tests/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2022-12-14 18:52:34.000000 cellprofiler-core-4.2.5/tests/workspace/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.287566 cellprofiler-core-4.2.6/cellprofiler_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.287566 cellprofiler-core-4.2.6/cellprofiler_core/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/_worker_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.287566 cellprofiler-core-4.2.6/cellprofiler_core/analysis/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/event/_finished.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/event/_paused.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/event/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/event/_resumed.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/event/_started.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.287566 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_ack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_debug_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_dictionary_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_exception_please_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_image_set_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_image_set_success_with_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_no_work.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_omero_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_server_exited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_shared_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/_work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_analysis_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_debug_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_debug_waiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_display_post_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_display_post_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_exception_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_initial_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_measurements_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_omero_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_pipeline_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_shared_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/commands/_pipeline_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/commands/_worker_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/constants/module/
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/module/_identify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/constants/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/_grayscale_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/_image_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/_image_set_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/_rgb_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/_abstract_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/_callback_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/_vanilla_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/_file_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/_flex_frame_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/_movie_frame_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_color_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_mask_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_objects_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_url_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/measurement/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71679 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/measurement/_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/measurement/_metadata_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/measurement/_relationship_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.291566 cellprofiler-core-4.2.6/cellprofiler_core/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/_identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/_image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38204 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/_plugin_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.299566 cellprofiler-core-4.2.6/cellprofiler_core/module/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/image_segmentation/_image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/module/image_segmentation/_object_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.299566 cellprofiler-core-4.2.6/cellprofiler_core/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30948 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/inject_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/injectimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61221 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/loaddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/measurementfixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69915 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104716 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/namesandtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/modules/setting_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.299566 cellprofiler-core-4.2.6/cellprofiler_core/object/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/object/_object_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17585 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/object/_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/object/_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.299566 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_image_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_image_set_channel_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100895 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.299566 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_image_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_measurement_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_object_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.307566 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_end_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_file_walk_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_file_walk_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_ipd_load_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_load_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_module_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_module_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_module_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_module_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_module_moved.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_module_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_module_show_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_pipeline_cleared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_pipeline_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_prepare_run_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_urls_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_urls_removed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.311565 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/run_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/run_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/run_exception/_post_run_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/run_exception/_prepare_run_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/run_exception/_run_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.311565 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/io/_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/pipeline/io/_v6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.311565 cellprofiler-core-4.2.6/cellprofiler_core/preferences/
+-rw-r--r--   0 runner    (1001) docker     (123)    63252 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/preferences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/preferences/_headless_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.315566 cellprofiler-core-4.2.6/cellprofiler_core/setting/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_binary_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_delete_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_do_things.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_figure_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_file_collection_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_hidden_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_html_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_image_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_path_list_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_regexp_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_settings_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_structuring_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_tree_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/_validation_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.315566 cellprofiler-core-4.2.6/cellprofiler_core/setting/change_setting_event/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/change_setting_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/change_setting_event/_after_change_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/change_setting_event/_change_setting_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/choice/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/choice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/choice/_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/choice/_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/choice/_custom_choice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/do_something/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/do_something/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/do_something/_do_something.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/do_something/_image_set_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/do_something/_path_list_refresh_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/do_something/_remove_setting_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_compound_filter_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_directory_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_does_not_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_does_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_extension_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_file_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_filter_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_image_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_metadata_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_regexp_filter_predicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_image_name_subscriber_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_measurement_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_object_subscriber_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_subdirectory_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/_float_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/integer_range/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/integer_range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/range/integer_range/_integer_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/_grid_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/_label_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.319566 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/list_subscriber/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/list_subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/list_subscriber/_image_list_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/list_subscriber/_label_list_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/_character.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/_grid_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/_crop_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/_file_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/_outline_image_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/integer/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/integer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/integer/_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/integer/_odd_integer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/pathname/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/pathname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/pathname/_pathname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/setting/text/pathname/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.323566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/module/identify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/modules/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113440 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/hdf5_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/pathname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/utf16encode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/_analysis_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/_boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/_communicable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/_lock_status_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/_upstream_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_boundary_exited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_upstream_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/request/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/request/_lock_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/request/_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/worker/_pipeline_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22680 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/worker/_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/cellprofiler_core/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/workspace/_disposition_changed_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21566 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/cellprofiler_core/workspace/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.287566 cellprofiler-core-4.2.6/cellprofiler_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 15:00:38.000000 cellprofiler-core-4.2.6/cellprofiler_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25254 2023-08-08 15:00:38.000000 cellprofiler-core-4.2.6/cellprofiler_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:00:38.000000 cellprofiler-core-4.2.6/cellprofiler_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:00:38.000000 cellprofiler-core-4.2.6/cellprofiler_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-08 15:00:38.000000 cellprofiler-core-4.2.6/cellprofiler_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 15:00:38.000000 cellprofiler-core-4.2.6/cellprofiler_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.283566 cellprofiler-core-4.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69010 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/analysis/test_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/tests/core/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/tests/core/image/abstract_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.327566 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/test__file_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/test__flex_frame_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/test__movie_frame_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/test__stk_frame_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.331566 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/url/test__color_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/url/test__mask_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/url/test__monochrome_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/url/test__objects_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/url/test__url_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/test__abstract_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/test__callback_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/abstract_image/test__vanilla_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/test__grayscale_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/test__image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/test__image_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/test__image_set_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/image/test__rgb_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.331566 cellprofiler-core-4.2.6/tests/core/measurement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/measurement/test__measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/measurement/test__metadata_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/measurement/test__relationship_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.331566 cellprofiler-core-4.2.6/tests/core/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.331566 cellprofiler-core-4.2.6/tests/core/module/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/image_segmentation/test__image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/image_segmentation/test__object_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/test__identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/test__image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/test__module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/module/test__plugin_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.331566 cellprofiler-core-4.2.6/tests/core/object/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/object/test__object_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/object/test__objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/object/test__segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.331566 cellprofiler-core-4.2.6/tests/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.331566 cellprofiler-core-4.2.6/tests/core/pipeline/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/dependency/test__dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/dependency/test__image_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/dependency/test__measurement_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/dependency/test__object_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.335566 cellprofiler-core-4.2.6/tests/core/pipeline/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.335566 cellprofiler-core-4.2.6/tests/core/pipeline/event/run_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/run_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/run_exception/test__post_run_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/run_exception/test__prepare_run_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/run_exception/test__run_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__end_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__event.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__file_walk_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__file_walk_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__ipd_load_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__load_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__module_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__module_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__module_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__module_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__module_moved.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__module_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__module_show_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__pipeline_cleared.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__pipeline_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__prepare_run_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__urls_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/event/test__urls_removed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.335566 cellprofiler-core-4.2.6/tests/core/pipeline/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/test__image_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/test__image_set_channel_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/test__listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/pipeline/test__pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.335566 cellprofiler-core-4.2.6/tests/core/setting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.335566 cellprofiler-core-4.2.6/tests/core/setting/change_setting_event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/change_setting_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/change_setting_event/test__after_change_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/change_setting_event/test__before_change_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/change_setting_event/test__change_setting_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.335566 cellprofiler-core-4.2.6/tests/core/setting/choice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/choice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/choice/test__choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/choice/test__colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/choice/test__custom_choice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.335566 cellprofiler-core-4.2.6/tests/core/setting/do_something/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/do_something/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/do_something/test__do_something.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/do_something/test__image_set_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/do_something/test__path_list_refresh_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/do_something/test__remove_setting_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__compound_filter_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__directory_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__does_not_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__does_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__extension_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__file_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__filter_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__image_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__metadata_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/filter/test__regexp_filter_predicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/multichoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/multichoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/multichoice/test__image_name_subscriber_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/multichoice/test__measurement_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/multichoice/test__multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/multichoice/test__object_subscriber_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/multichoice/test__subdirectory_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/multichoice/test__subscriber_multichoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/range/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/range/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/range/integer_range/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/range/integer_range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/range/integer_range/test__integer_or_unbounded_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/range/integer_range/test__integer_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/range/test__float_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/range/test__range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/subscriber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/subscriber/image_subscriber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/image_subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/image_subscriber/test__crop_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/image_subscriber/test__file_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/image_subscriber/test__image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/image_subscriber/test__outline_image_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/subscriber/list_subscriber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/list_subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/list_subscriber/test__image_list_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/list_subscriber/test__label_list_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/list_subscriber/test__list_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/test__grid_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/test__label_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/subscriber/test__subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__binary_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__delete_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__do_things.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__figure_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__file_collection_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__hidden_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__html_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__image_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__path_list_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__regexp_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__settings_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__structuring_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__tree_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/test__validation_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.339566 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/image_name/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/image_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/image_name/test__crop_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/image_name/test__external_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/image_name/test__file_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/image_name/test__image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/image_name/test__outline_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/test__grid_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/test__label_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/name/test__name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/alphanumeric/test__alphanumeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/core/setting/text/number/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/number/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/core/setting/text/number/integer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/number/integer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/number/integer/test__integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/number/integer/test__odd_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/number/test__float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/number/test__number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/core/setting/text/pathname/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/pathname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/pathname/test__pathname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/pathname/test__url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/test__directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/test__filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/setting/text/test__text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/core/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/worker/test__pipeline_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/worker/test__worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/core/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/workspace/test__disposition_changed_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-08 15:00:27.000000 cellprofiler-core-4.2.6/tests/core/workspace/test__workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/image/test_image_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/image/test_image_set_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/measurement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56902 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/measurement/test_measurements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/module/test_image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/module/test_object_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.343566 cellprofiler-core-4.2.6/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41457 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/test_injectimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37147 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/test_loaddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36806 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91427 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/modules/test_namesandtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/tests/object/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39054 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/object/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/object/test_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/pipeline/test_image_plane_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57252 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/pipeline/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/tests/preferences/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/preferences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/preferences/test_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/tests/setting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/setting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/setting/test_namesubscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14612 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/setting/test_setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/worker/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:38.347566 cellprofiler-core-4.2.6/tests/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-08 15:00:28.000000 cellprofiler-core-4.2.6/tests/workspace/test_workspace.py
```

### Comparing `cellprofiler-core-4.2.5/LICENSE` & `cellprofiler-core-4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/__main__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/__main__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/analysis/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/analysis/_analysis.py` & `cellprofiler-core-4.2.6/cellprofiler_core/analysis/_analysis.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/analysis/_runner.py` & `cellprofiler-core-4.2.6/cellprofiler_core/analysis/_runner.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/analysis/_worker_runner.py` & `cellprofiler-core-4.2.6/cellprofiler_core/analysis/_worker_runner.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/analysis/reply/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/analysis/reply/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/analysis/request/_exception_report.py` & `cellprofiler-core-4.2.6/cellprofiler_core/analysis/request/_exception_report.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/commands/_pipeline_command.py` & `cellprofiler-core-4.2.6/cellprofiler_core/commands/_pipeline_command.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/measurement.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/module/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/module/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/module/_identify.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/module/_identify.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/load_data.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/load_data.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/modules/metadata.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/modules/metadata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/pipeline.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/constants/setting.py` & `cellprofiler-core-4.2.6/cellprofiler_core/constants/setting.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/_grayscale_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/_grayscale_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/_image_set.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/_image_set.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/_image_set_list.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/_image_set_list.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/_abstract_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/_abstract_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/_callback_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/_callback_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/_vanilla_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/_vanilla_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/_file_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/_file_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_color_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_color_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_mask_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_mask_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_objects_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_objects_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/image/abstract_image/file/url/_url_image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/image/abstract_image/file/url/_url_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/measurement/_measurements.py` & `cellprofiler-core-4.2.6/cellprofiler_core/measurement/_measurements.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/measurement/_metadata_group.py` & `cellprofiler-core-4.2.6/cellprofiler_core/measurement/_metadata_group.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/module/_identify.py` & `cellprofiler-core-4.2.6/cellprofiler_core/module/_identify.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/module/_image_processing.py` & `cellprofiler-core-4.2.6/cellprofiler_core/module/_image_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/module/_module.py` & `cellprofiler-core-4.2.6/cellprofiler_core/module/_module.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/module/_plugin_importer.py` & `cellprofiler-core-4.2.6/cellprofiler_core/module/_plugin_importer.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/module/image_segmentation/_image_segmentation.py` & `cellprofiler-core-4.2.6/cellprofiler_core/module/image_segmentation/_image_segmentation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/module/image_segmentation/_object_processing.py` & `cellprofiler-core-4.2.6/cellprofiler_core/module/image_segmentation/_object_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/align.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/align.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/groups.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/groups.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/images.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/images.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/inject_objects.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/inject_objects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/injectimage.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/injectimage.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/loaddata.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/loaddata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/measurementfixture.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/measurementfixture.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/metadata.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/metadata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/namesandtypes.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/namesandtypes.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/modules/setting_validation.py` & `cellprofiler-core-4.2.6/cellprofiler_core/modules/setting_validation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/object/_object_set.py` & `cellprofiler-core-4.2.6/cellprofiler_core/object/_object_set.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/object/_objects.py` & `cellprofiler-core-4.2.6/cellprofiler_core/object/_objects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/object/_segmentation.py` & `cellprofiler-core-4.2.6/cellprofiler_core/object/_segmentation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_image_plane.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_image_plane.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_image_set_channel_descriptor.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_image_set_channel_descriptor.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_listener.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_listener.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/_pipeline.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_dependency.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_image_dependency.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_image_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_measurement_dependency.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_measurement_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/dependency/_object_dependency.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/dependency/_object_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/_event.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/_event.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/event/run_exception/_run_exception.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/event/run_exception/_run_exception.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/io/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/io/_v5.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/io/_v5.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/pipeline/io/_v6.py` & `cellprofiler-core-4.2.6/cellprofiler_core/pipeline/io/_v6.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/preferences/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/preferences/_headless_configuration.py` & `cellprofiler-core-4.2.6/cellprofiler_core/preferences/_headless_configuration.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_binary.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_binary.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_binary_matrix.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_binary_matrix.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_color.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_color.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_coordinates.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_coordinates.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_data_types.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_data_types.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_do_things.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_do_things.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_figure_subscriber.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_figure_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_file_collection_display.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_file_collection_display.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_hidden_count.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_hidden_count.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_html_text.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_html_text.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_image_plane.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_image_plane.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_joiner.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_joiner.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_measurement.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_regexp_text.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_regexp_text.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_setting.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_setting.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_settings_group.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_settings_group.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_structuring_element.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_structuring_element.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_table.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_table.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_tree_choice.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_tree_choice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/_validation_error.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/_validation_error.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/choice/_choice.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/choice/_choice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/choice/_custom_choice.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/choice/_custom_choice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/do_something/_do_something.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/do_something/_do_something.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_directory_predicate.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_directory_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_extension_predicate.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_extension_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_file_predicate.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_file_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_filter.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_filter.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_filter_predicate.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_filter_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_image_predicate.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_image_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_metadata_predicate.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_metadata_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/filter/_regexp_filter_predicate.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/filter/_regexp_filter_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_measurement_multichoice.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_measurement_multichoice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_multichoice.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_multichoice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_subdirectory_filter.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_subdirectory_filter.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/range/_float_range.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/range/_float_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/range/_range.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/range/_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/range/integer_range/_integer_range.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/range/integer_range/_integer_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/_subscriber.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/_directory.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/_directory.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/_filename.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/_filename.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/_character.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/_character.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/_name.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/_name.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/number/_number.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/number/_number.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/setting/text/pathname/_pathname.py` & `cellprofiler-core-4.2.6/cellprofiler_core/setting/text/pathname/_pathname.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/analysis.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/analysis.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/module/identify.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/module/identify.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/modules/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/modules/load_data.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/modules/load_data.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/object.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/object.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/core/pipeline.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/grid.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/grid.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/hdf5_dict.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/hdf5_dict.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/image.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/java.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/java.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/legacy.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/legacy.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/measurement.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/pathname.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/pathname.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/utf16encode.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/utf16encode.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/_analysis_context.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/_analysis_context.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/_boundary.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/_boundary.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/_communicable.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/_communicable.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/utilities/zmq/communicable/request/_request.py` & `cellprofiler-core-4.2.6/cellprofiler_core/utilities/zmq/communicable/request/_request.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/worker/__init__.py` & `cellprofiler-core-4.2.6/cellprofiler_core/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/worker/_pipeline_event_listener.py` & `cellprofiler-core-4.2.6/cellprofiler_core/worker/_pipeline_event_listener.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/worker/_worker.py` & `cellprofiler-core-4.2.6/cellprofiler_core/worker/_worker.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core/workspace/_workspace.py` & `cellprofiler-core-4.2.6/cellprofiler_core/workspace/_workspace.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/cellprofiler_core.egg-info/SOURCES.txt` & `cellprofiler-core-4.2.6/cellprofiler_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/setup.py` & `cellprofiler-core-4.2.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "twine==3.1.1",
         ],
         "test": ["pytest==5.4.1"],
         "wx": ["wxPython==4.1.0"],
     },
     install_requires=[
         "boto3>=1.12.28",
-        "centrosome==1.2.1",
+        "centrosome==1.2.2",
         "docutils==0.15.2",
         "h5py~=3.6.0",
         "matplotlib>=3.1.3",
         "numpy>=1.18.2",
         "prokaryote==2.4.4",
         "psutil>=5.7.0",
         "python-bioformats==4.0.7",
@@ -37,10 +37,10 @@
     ],
     license="BSD",
     name="cellprofiler-core",
     package_data={"cellprofiler_core": ["py.typed"]},
     packages=setuptools.find_packages(exclude=["tests"]),
     python_requires=">=3.8",
     url="https://github.com/CellProfiler/core",
-    version="4.2.5",
+    version="4.2.6",
     zip_safe=False,
 )
```

### Comparing `cellprofiler-core-4.2.5/tests/analysis/test_analysis.py` & `cellprofiler-core-4.2.6/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/image/abstract_image/file/test__file_image.py` & `cellprofiler-core-4.2.6/tests/core/image/abstract_image/file/test__file_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/image/test__image.py` & `cellprofiler-core-4.2.6/tests/core/image/test__image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/measurement/test__measurements.py` & `cellprofiler-core-4.2.6/tests/core/measurement/test__measurements.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/module/test__module.py` & `cellprofiler-core-4.2.6/tests/core/module/test__module.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/object/test__objects.py` & `cellprofiler-core-4.2.6/tests/core/object/test__objects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/pipeline/test__pipeline.py` & `cellprofiler-core-4.2.6/tests/core/pipeline/test__pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/setting/range/integer_range/test__integer_or_unbounded_range.py` & `cellprofiler-core-4.2.6/tests/core/setting/range/integer_range/test__integer_or_unbounded_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/setting/range/test__range.py` & `cellprofiler-core-4.2.6/tests/core/setting/range/test__range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/setting/test__file_collection_display.py` & `cellprofiler-core-4.2.6/tests/core/setting/test__file_collection_display.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/setting/test__measurement.py` & `cellprofiler-core-4.2.6/tests/core/setting/test__measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/setting/text/number/test__number.py` & `cellprofiler-core-4.2.6/tests/core/setting/text/number/test__number.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/setting/text/test__directory.py` & `cellprofiler-core-4.2.6/tests/core/setting/text/test__directory.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/worker/test__worker.py` & `cellprofiler-core-4.2.6/tests/core/worker/test__worker.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/core/workspace/test__workspace.py` & `cellprofiler-core-4.2.6/tests/core/workspace/test__workspace.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/image/test_image.py` & `cellprofiler-core-4.2.6/tests/image/test_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/image/test_image_set.py` & `cellprofiler-core-4.2.6/tests/image/test_image_set.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/image/test_image_set_list.py` & `cellprofiler-core-4.2.6/tests/image/test_image_set_list.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/measurement/test_measurements.py` & `cellprofiler-core-4.2.6/tests/measurement/test_measurements.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/module/test_image_segmentation.py` & `cellprofiler-core-4.2.6/tests/module/test_image_segmentation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/module/test_object_processing.py` & `cellprofiler-core-4.2.6/tests/module/test_object_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/__init__.py` & `cellprofiler-core-4.2.6/tests/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/test_align.py` & `cellprofiler-core-4.2.6/tests/modules/test_align.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/test_groups.py` & `cellprofiler-core-4.2.6/tests/modules/test_groups.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/test_images.py` & `cellprofiler-core-4.2.6/tests/modules/test_images.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/test_injectimage.py` & `cellprofiler-core-4.2.6/tests/modules/test_injectimage.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/test_loaddata.py` & `cellprofiler-core-4.2.6/tests/modules/test_loaddata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/test_metadata.py` & `cellprofiler-core-4.2.6/tests/modules/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/modules/test_namesandtypes.py` & `cellprofiler-core-4.2.6/tests/modules/test_namesandtypes.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/object/test_objects.py` & `cellprofiler-core-4.2.6/tests/object/test_objects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/object/test_segmentation.py` & `cellprofiler-core-4.2.6/tests/object/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/pipeline/test_image_plane_details.py` & `cellprofiler-core-4.2.6/tests/pipeline/test_image_plane_details.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/pipeline/test_pipeline.py` & `cellprofiler-core-4.2.6/tests/pipeline/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/preferences/test_preferences.py` & `cellprofiler-core-4.2.6/tests/preferences/test_preferences.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/setting/test_namesubscriber.py` & `cellprofiler-core-4.2.6/tests/setting/test_namesubscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/setting/test_setting.py` & `cellprofiler-core-4.2.6/tests/setting/test_setting.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/worker/test_worker.py` & `cellprofiler-core-4.2.6/tests/worker/test_worker.py`

 * *Files identical despite different names*

### Comparing `cellprofiler-core-4.2.5/tests/workspace/test_workspace.py` & `cellprofiler-core-4.2.6/tests/workspace/test_workspace.py`

 * *Files identical despite different names*

