# Comparing `tmp/darshan-3.4.3.0.tar.gz` & `tmp/darshan-3.4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darshan-3.4.3.0.tar", last modified: Mon Jun 12 20:20:56 2023, max compression
+gzip compressed data, was "darshan-3.4.4.0.tar", last modified: Tue Aug  8 00:12:28 2023, max compression
```

## Comparing `darshan-3.4.3.0.tar` & `darshan-3.4.4.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.316522 darshan-3.4.3.0/
--rw-rw-r--   0 shane     (1000) shane     (1000)      213 2022-10-26 18:33:05.000000 darshan-3.4.3.0/MANIFEST.in
--rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-06-12 20:20:56.316522 darshan-3.4.3.0/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     2115 2023-06-12 18:17:58.000000 darshan-3.4.3.0/README.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.276521 darshan-3.4.3.0/darshan/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1221 2023-06-12 14:45:06.000000 darshan-3.4.3.0/darshan/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)       64 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/__main__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.280521 darshan-3.4.3.0/darshan/backend/
--rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/backend/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6193 2023-02-08 22:31:13.000000 darshan-3.4.3.0/darshan/backend/api_def_c.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3694 2022-05-04 14:43:41.000000 darshan-3.4.3.0/darshan/backend/apmpi.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1928 2022-05-04 14:43:41.000000 darshan-3.4.3.0/darshan/backend/apss.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2305 2022-05-04 14:43:41.000000 darshan-3.4.3.0/darshan/backend/apxc.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    22874 2023-04-19 16:40:28.000000 darshan-3.4.3.0/darshan/backend/cffi_backend.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/cli/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5545 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)       73 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/cli/__main__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2313 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/cli/base.html
--rw-rw-r--   0 shane     (1000) shane     (1000)      966 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/info.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1028 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/name_records.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     7563 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/cli/style.css
--rw-rw-r--   0 shane     (1000) shane     (1000)    29267 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/cli/summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      920 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/to_json.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/datatypes/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/datatypes/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3814 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/datatypes/heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     7635 2023-04-13 22:44:27.000000 darshan-3.4.3.0/darshan/discover_darshan.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/examples/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/examples/darshan-graph/
--rw-rw-r--   0 shane     (1000) shane     (1000)      279 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/Makefile
--rw-rw-r--   0 shane     (1000) shane     (1000)     1676 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/app.c
--rw-rw-r--   0 shane     (1000) shane     (1000)     3882 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/app_rw_mpiio.c
--rw-rw-r--   0 shane     (1000) shane     (1000)     2498 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1070 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1079 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1068 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1069 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1072 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan
--rwxrwxr-x   0 shane     (1000) shane     (1000)      717 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/run.sh
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.288521 darshan-3.4.3.0/darshan/examples/example_logs/
--rw-rw-r--   0 shane     (1000) shane     (1000)      286 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    98998 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/dxt.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/example.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     3967 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/ior_hdf5_example.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/noposix.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/sample-badost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1992 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.288521 darshan-3.4.3.0/darshan/examples/tutorial/
--rw-rw-r--   0 shane     (1000) shane     (1000)      103 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/tutorial/hello.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      216 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/tutorial/plot.py
--rwxrwxr-x   0 shane     (1000) shane     (1000)      596 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/tutorial/tojson.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.288521 darshan-3.4.3.0/darshan/experimental/
--rw-rw-r--   0 shane     (1000) shane     (1000)      134 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.292521 darshan-3.4.3.0/darshan/experimental/aggregators/
--rw-rw-r--   0 shane     (1000) shane     (1000)      407 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4560 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/aggregators/agg_ioops.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2950 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_dxttimeline.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1749 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_sankey.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1335 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_time_summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     5726 2022-11-02 17:48:53.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_timeline.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1476 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/aggregators/mod_agg_iohist.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      637 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/name_records_summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6951 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/print_module_records.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1211 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/records_as_dict.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      516 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/summarize.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.292521 darshan-3.4.3.0/darshan/experimental/operations/
--rw-rw-r--   0 shane     (1000) shane     (1000)     2303 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/operations/filter.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2405 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/operations/merge.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3187 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/operations/reduce.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.296521 darshan-3.4.3.0/darshan/experimental/plots/
--rw-rw-r--   0 shane     (1000) shane     (1000)      251 2023-04-19 16:40:28.000000 darshan-3.4.3.0/darshan/experimental/plots/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    26333 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/data_access_by_filesystem.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    14559 2023-04-13 22:44:27.000000 darshan-3.4.3.0/darshan/experimental/plots/heatmap_handling.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2765 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_access_histogram.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4340 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_common_access_table.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    14759 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4145 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap2.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6297 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_io_cost.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6638 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_opcounts.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1982 2023-04-19 16:40:28.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_posix_access_pattern.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     5204 2022-12-19 21:37:30.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_posix_io_pattern.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.296521 darshan-3.4.3.0/darshan/experimental/transforms/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5626 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/transforms/dxt2png.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.300521 darshan-3.4.3.0/darshan/lib/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3741 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/lib/accum.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2901 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/log_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    35880 2023-02-15 21:55:53.000000 darshan-3.4.3.0/darshan/report.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.304521 darshan-3.4.3.0/darshan/tests/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      533 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/conftest.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.308521 darshan-3.4.3.0/darshan/tests/input/
--rw-rw-r--   0 shane     (1000) shane     (1000)      313 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/match_dotout.dot
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/match_jsonout.json
--rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/noposix.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1441 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/noposixopens.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample-badost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     6631 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample-dxt-simple.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    10717 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample-goodost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11523 2023-02-15 21:55:53.000000 darshan-3.4.3.0/darshan/tests/test_cffi_misc.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    32921 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/tests/test_data_access_by_filesystem.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      567 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_error.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    22010 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_heatmap_handling.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8314 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/tests/test_lib_accum.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2064 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_log_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1653 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_moddxt.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1116 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_modmpiio.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1107 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_modposix.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1144 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_modstdio.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8550 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_plot_common_access_table.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    16837 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_plot_dxt_heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    13048 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/tests/test_plot_exp_common.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    10752 2023-02-15 21:55:53.000000 darshan-3.4.3.0/darshan/tests/test_plot_io_cost.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    24120 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_report.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      563 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_report_copy.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    25957 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/tests/test_summary.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.276521 darshan-3.4.3.0/darshan.egg-info/
--rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     5035 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/SOURCES.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/dependency_links.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/not-zip-safe
--rw-rw-r--   0 shane     (1000) shane     (1000)       51 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/requires.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        8 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/top_level.txt
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.312521 darshan-3.4.3.0/docs/
--rw-rw-r--   0 shane     (1000) shane     (1000)      610 2022-10-26 18:33:05.000000 darshan-3.4.3.0/docs/Makefile
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.272521 darshan-3.4.3.0/docs/api/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.312521 darshan-3.4.3.0/docs/api/pydarshan/
--rw-rw-r--   0 shane     (1000) shane     (1000)      951 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.backend.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      740 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.cli.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      328 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.datatypes.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      179 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.examples.example_logs.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.examples.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2573 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.aggregators.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2015 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.plots.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      272 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      742 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      147 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.tests.input.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     3341 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.tests.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)       62 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/modules.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.272521 darshan-3.4.3.0/docs/build/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.272521 darshan-3.4.3.0/docs/build/html/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.316522 darshan-3.4.3.0/docs/build/html/_static/
--rw-rw-r--   0 shane     (1000) shane     (1000)      286 2023-06-06 18:59:29.000000 darshan-3.4.3.0/docs/build/html/_static/file.png
--rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-06-06 18:59:29.000000 darshan-3.4.3.0/docs/build/html/_static/minus.png
--rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-06-06 18:59:29.000000 darshan-3.4.3.0/docs/build/html/_static/plus.png
--rwxrwxr-x   0 shane     (1000) shane     (1000)     5230 2022-10-26 18:33:05.000000 darshan-3.4.3.0/docs/conf.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      669 2023-05-31 18:10:46.000000 darshan-3.4.3.0/docs/index.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2097 2023-05-31 18:10:46.000000 darshan-3.4.3.0/docs/install.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      771 2022-10-26 18:33:05.000000 darshan-3.4.3.0/docs/make.bat
--rw-rw-r--   0 shane     (1000) shane     (1000)       27 2022-12-01 18:54:58.000000 darshan-3.4.3.0/docs/readme.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     3682 2023-05-31 18:10:46.000000 darshan-3.4.3.0/docs/usage.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     1353 2023-02-16 19:35:59.000000 darshan-3.4.3.0/pyproject.toml
--rw-rw-r--   0 shane     (1000) shane     (1000)      480 2023-06-12 20:20:56.316522 darshan-3.4.3.0/setup.cfg
--rw-rw-r--   0 shane     (1000) shane     (1000)     2850 2023-06-12 14:45:06.000000 darshan-3.4.3.0/setup.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.302298 darshan-3.4.4.0/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      213 2022-10-26 18:33:05.000000 darshan-3.4.4.0/MANIFEST.in
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-08-08 00:12:28.302298 darshan-3.4.4.0/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2115 2023-08-01 19:58:29.000000 darshan-3.4.4.0/README.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.174293 darshan-3.4.4.0/darshan/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1221 2023-08-07 22:14:06.000000 darshan-3.4.4.0/darshan/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)       64 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/__main__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.178293 darshan-3.4.4.0/darshan/backend/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/backend/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6193 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/backend/api_def_c.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3694 2022-05-04 14:43:41.000000 darshan-3.4.4.0/darshan/backend/apmpi.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1928 2022-05-04 14:43:41.000000 darshan-3.4.4.0/darshan/backend/apss.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2305 2022-05-04 14:43:41.000000 darshan-3.4.4.0/darshan/backend/apxc.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    22874 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/backend/cffi_backend.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/cli/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5545 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)       73 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/cli/__main__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2313 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/cli/base.html
+-rw-rw-r--   0 shane     (1000) shane     (1000)      966 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/info.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1028 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/name_records.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     7563 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/cli/style.css
+-rw-rw-r--   0 shane     (1000) shane     (1000)    29267 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/cli/summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      920 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/cli/to_json.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/datatypes/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/datatypes/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3814 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/datatypes/heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     7635 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/discover_darshan.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/examples/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.182293 darshan-3.4.4.0/darshan/examples/darshan-graph/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      279 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/Makefile
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1676 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/app.c
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3882 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/app_rw_mpiio.c
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2498 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1070 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1079 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1068 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1069 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1072 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      717 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/darshan-graph/run.sh
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.214294 darshan-3.4.4.0/darshan/examples/example_logs/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      286 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    98998 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/dxt.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/example.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3967 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/ior_hdf5_example.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/noposix.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/sample-badost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1992 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.218294 darshan-3.4.4.0/darshan/examples/tutorial/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      103 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/tutorial/hello.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      216 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/tutorial/plot.py
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      596 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/examples/tutorial/tojson.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.218294 darshan-3.4.4.0/darshan/experimental/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      134 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.222295 darshan-3.4.4.0/darshan/experimental/aggregators/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      407 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4560 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/aggregators/agg_ioops.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2950 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_dxttimeline.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1749 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_sankey.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1335 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_time_summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5726 2022-11-02 17:48:53.000000 darshan-3.4.4.0/darshan/experimental/aggregators/create_timeline.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1476 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/aggregators/mod_agg_iohist.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      637 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/name_records_summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6951 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/print_module_records.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1211 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/records_as_dict.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      516 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/aggregators/summarize.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.226295 darshan-3.4.4.0/darshan/experimental/operations/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2303 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/operations/filter.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2405 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/operations/merge.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3187 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/operations/reduce.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.238295 darshan-3.4.4.0/darshan/experimental/plots/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      251 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    26333 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/data_access_by_filesystem.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    14559 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/heatmap_handling.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2765 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_access_histogram.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4340 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_common_access_table.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    14759 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4145 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap2.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6297 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_io_cost.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6638 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_opcounts.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1982 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_posix_access_pattern.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5204 2022-12-19 21:37:30.000000 darshan-3.4.4.0/darshan/experimental/plots/plot_posix_io_pattern.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.238295 darshan-3.4.4.0/darshan/experimental/transforms/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5626 2022-10-26 18:33:05.000000 darshan-3.4.4.0/darshan/experimental/transforms/dxt2png.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.242295 darshan-3.4.4.0/darshan/lib/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3741 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/lib/accum.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2901 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/log_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    35880 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/report.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.254296 darshan-3.4.4.0/darshan/tests/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      533 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/conftest.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.294297 darshan-3.4.4.0/darshan/tests/input/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      313 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/match_dotout.dot
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/match_jsonout.json
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/noposix.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1441 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/noposixopens.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample-badost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6631 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample-dxt-simple.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    10717 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample-goodost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/input/sample.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11523 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_cffi_misc.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    32921 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_data_access_by_filesystem.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      567 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_error.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    22010 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_heatmap_handling.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8314 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_lib_accum.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2064 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_log_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1653 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_moddxt.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1116 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_modmpiio.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1107 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_modposix.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1144 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_modstdio.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8550 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_common_access_table.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16837 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_dxt_heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    13048 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_exp_common.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    10752 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_plot_io_cost.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    24120 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_report.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      563 2022-11-22 21:37:27.000000 darshan-3.4.4.0/darshan/tests/test_report_copy.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    25957 2023-08-01 19:58:29.000000 darshan-3.4.4.0/darshan/tests/test_summary.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.174293 darshan-3.4.4.0/darshan.egg-info/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5035 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/SOURCES.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/dependency_links.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/not-zip-safe
+-rw-rw-r--   0 shane     (1000) shane     (1000)       51 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/requires.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        8 2023-08-08 00:12:28.000000 darshan-3.4.4.0/darshan.egg-info/top_level.txt
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.298298 darshan-3.4.4.0/docs/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      610 2022-10-26 18:33:05.000000 darshan-3.4.4.0/docs/Makefile
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.170292 darshan-3.4.4.0/docs/api/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.302298 darshan-3.4.4.0/docs/api/pydarshan/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      951 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.backend.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      740 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.cli.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      328 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.datatypes.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      179 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.examples.example_logs.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.examples.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2573 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.aggregators.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2015 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.plots.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      272 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      742 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      147 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.tests.input.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3341 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/darshan.tests.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)       62 2022-12-16 21:58:31.000000 darshan-3.4.4.0/docs/api/pydarshan/modules.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.170292 darshan-3.4.4.0/docs/build/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.170292 darshan-3.4.4.0/docs/build/html/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-08-08 00:12:28.302298 darshan-3.4.4.0/docs/build/html/_static/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      286 2023-08-05 14:28:56.000000 darshan-3.4.4.0/docs/build/html/_static/file.png
+-rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-08-05 14:28:56.000000 darshan-3.4.4.0/docs/build/html/_static/minus.png
+-rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-08-05 14:28:56.000000 darshan-3.4.4.0/docs/build/html/_static/plus.png
+-rwxrwxr-x   0 shane     (1000) shane     (1000)     5230 2022-10-26 18:33:05.000000 darshan-3.4.4.0/docs/conf.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      669 2023-08-01 19:58:29.000000 darshan-3.4.4.0/docs/index.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2097 2023-08-01 19:58:29.000000 darshan-3.4.4.0/docs/install.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      771 2022-10-26 18:33:05.000000 darshan-3.4.4.0/docs/make.bat
+-rw-rw-r--   0 shane     (1000) shane     (1000)       27 2022-12-01 18:54:58.000000 darshan-3.4.4.0/docs/readme.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3682 2023-08-01 19:58:29.000000 darshan-3.4.4.0/docs/usage.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1353 2023-08-01 19:58:29.000000 darshan-3.4.4.0/pyproject.toml
+-rw-rw-r--   0 shane     (1000) shane     (1000)      480 2023-08-08 00:12:28.302298 darshan-3.4.4.0/setup.cfg
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2850 2023-08-07 22:14:06.000000 darshan-3.4.4.0/setup.py
```

### Comparing `darshan-3.4.3.0/PKG-INFO` & `darshan-3.4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darshan
-Version: 3.4.3.0
+Version: 3.4.4.0
 Summary: Python tools to interact with darshan log records of HPC applications.
 Home-page: https://www.mcs.anl.gov/research/projects/darshan/
 Author: 
 Author-email: 
 Keywords: darshan
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `darshan-3.4.3.0/README.rst` & `darshan-3.4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/__init__.py` & `darshan-3.4.4.0/darshan/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 PyDarshan provides direct log access for reading binary Darshan logs.
 PyDarshan also provides a suite of analysis utilities.
 """
 
-__version__ = '3.4.3.0'
-__darshanutil_version__ = '3.4.3'
+__version__ = '3.4.4.0'
+__darshanutil_version__ = '3.4.4'
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 options = {} # type: ignore
```

### Comparing `darshan-3.4.3.0/darshan/backend/api_def_c.py` & `darshan-3.4.4.0/darshan/backend/api_def_c.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/backend/apmpi.py` & `darshan-3.4.4.0/darshan/backend/apmpi.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/backend/apss.py` & `darshan-3.4.4.0/darshan/backend/apss.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/backend/apxc.py` & `darshan-3.4.4.0/darshan/backend/apxc.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/backend/cffi_backend.py` & `darshan-3.4.4.0/darshan/backend/cffi_backend.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/cli/__init__.py` & `darshan-3.4.4.0/darshan/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/cli/base.html` & `darshan-3.4.4.0/darshan/cli/base.html`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/cli/info.py` & `darshan-3.4.4.0/darshan/cli/info.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/cli/name_records.py` & `darshan-3.4.4.0/darshan/cli/name_records.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/cli/style.css` & `darshan-3.4.4.0/darshan/cli/style.css`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/cli/summary.py` & `darshan-3.4.4.0/darshan/cli/summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/cli/to_json.py` & `darshan-3.4.4.0/darshan/cli/to_json.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/datatypes/heatmap.py` & `darshan-3.4.4.0/darshan/datatypes/heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/discover_darshan.py` & `darshan-3.4.4.0/darshan/discover_darshan.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/app.c` & `darshan-3.4.4.0/darshan/examples/darshan-graph/app.c`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/app_rw_mpiio.c` & `darshan-3.4.4.0/darshan/examples/darshan-graph/app_rw_mpiio.c`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan` & `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan` & `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.4.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/darshan-graph/run.sh` & `darshan-3.4.4.0/darshan/examples/darshan-graph/run.sh`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/example_logs/dxt.darshan` & `darshan-3.4.4.0/darshan/examples/example_logs/dxt.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/example_logs/example.darshan` & `darshan-3.4.4.0/darshan/examples/example_logs/example.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/example_logs/ior_hdf5_example.darshan` & `darshan-3.4.4.0/darshan/examples/example_logs/ior_hdf5_example.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/example_logs/noposix.darshan` & `darshan-3.4.4.0/darshan/examples/example_logs/noposix.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/example_logs/sample-badost.darshan` & `darshan-3.4.4.0/darshan/examples/example_logs/sample-badost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan` & `darshan-3.4.4.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/examples/tutorial/tojson.py` & `darshan-3.4.4.0/darshan/examples/tutorial/tojson.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/agg_ioops.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/agg_ioops.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/create_dxttimeline.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/create_dxttimeline.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/create_sankey.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/create_sankey.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/create_time_summary.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/create_time_summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/create_timeline.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/create_timeline.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/mod_agg_iohist.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/mod_agg_iohist.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/name_records_summary.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/name_records_summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/print_module_records.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/print_module_records.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/records_as_dict.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/records_as_dict.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/aggregators/summarize.py` & `darshan-3.4.4.0/darshan/experimental/aggregators/summarize.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/operations/filter.py` & `darshan-3.4.4.0/darshan/experimental/operations/filter.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/operations/merge.py` & `darshan-3.4.4.0/darshan/experimental/operations/merge.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/operations/reduce.py` & `darshan-3.4.4.0/darshan/experimental/operations/reduce.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/data_access_by_filesystem.py` & `darshan-3.4.4.0/darshan/experimental/plots/data_access_by_filesystem.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/heatmap_handling.py` & `darshan-3.4.4.0/darshan/experimental/plots/heatmap_handling.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_access_histogram.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_access_histogram.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_common_access_table.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_common_access_table.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap2.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_dxt_heatmap2.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_io_cost.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_io_cost.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_opcounts.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_opcounts.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_posix_access_pattern.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_posix_access_pattern.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/plots/plot_posix_io_pattern.py` & `darshan-3.4.4.0/darshan/experimental/plots/plot_posix_io_pattern.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/experimental/transforms/dxt2png.py` & `darshan-3.4.4.0/darshan/experimental/transforms/dxt2png.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/lib/accum.py` & `darshan-3.4.4.0/darshan/lib/accum.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/log_utils.py` & `darshan-3.4.4.0/darshan/log_utils.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/report.py` & `darshan-3.4.4.0/darshan/report.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/conftest.py` & `darshan-3.4.4.0/darshan/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/input/noposix.darshan` & `darshan-3.4.4.0/darshan/tests/input/noposix.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/input/noposixopens.darshan` & `darshan-3.4.4.0/darshan/tests/input/noposixopens.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/input/sample-badost.darshan` & `darshan-3.4.4.0/darshan/tests/input/sample-badost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/input/sample-dxt-simple.darshan` & `darshan-3.4.4.0/darshan/tests/input/sample-dxt-simple.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/input/sample-goodost.darshan` & `darshan-3.4.4.0/darshan/tests/input/sample-goodost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/input/sample.darshan` & `darshan-3.4.4.0/darshan/tests/input/sample.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_cffi_misc.py` & `darshan-3.4.4.0/darshan/tests/test_cffi_misc.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_data_access_by_filesystem.py` & `darshan-3.4.4.0/darshan/tests/test_data_access_by_filesystem.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_error.py` & `darshan-3.4.4.0/darshan/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_heatmap_handling.py` & `darshan-3.4.4.0/darshan/tests/test_heatmap_handling.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_lib_accum.py` & `darshan-3.4.4.0/darshan/tests/test_lib_accum.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_log_utils.py` & `darshan-3.4.4.0/darshan/tests/test_log_utils.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_moddxt.py` & `darshan-3.4.4.0/darshan/tests/test_moddxt.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_modmpiio.py` & `darshan-3.4.4.0/darshan/tests/test_modmpiio.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_modposix.py` & `darshan-3.4.4.0/darshan/tests/test_modposix.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_modstdio.py` & `darshan-3.4.4.0/darshan/tests/test_modstdio.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_plot_common_access_table.py` & `darshan-3.4.4.0/darshan/tests/test_plot_common_access_table.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_plot_dxt_heatmap.py` & `darshan-3.4.4.0/darshan/tests/test_plot_dxt_heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_plot_exp_common.py` & `darshan-3.4.4.0/darshan/tests/test_plot_exp_common.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_plot_io_cost.py` & `darshan-3.4.4.0/darshan/tests/test_plot_io_cost.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_report.py` & `darshan-3.4.4.0/darshan/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_report_copy.py` & `darshan-3.4.4.0/darshan/tests/test_report_copy.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan/tests/test_summary.py` & `darshan-3.4.4.0/darshan/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/darshan.egg-info/PKG-INFO` & `darshan-3.4.4.0/darshan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darshan
-Version: 3.4.3.0
+Version: 3.4.4.0
 Summary: Python tools to interact with darshan log records of HPC applications.
 Home-page: https://www.mcs.anl.gov/research/projects/darshan/
 Author: 
 Author-email: 
 Keywords: darshan
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `darshan-3.4.3.0/darshan.egg-info/SOURCES.txt` & `darshan-3.4.4.0/darshan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/Makefile` & `darshan-3.4.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/api/pydarshan/darshan.backend.rst` & `darshan-3.4.4.0/docs/api/pydarshan/darshan.backend.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/api/pydarshan/darshan.cli.rst` & `darshan-3.4.4.0/docs/api/pydarshan/darshan.cli.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.aggregators.rst` & `darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.aggregators.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.plots.rst` & `darshan-3.4.4.0/docs/api/pydarshan/darshan.experimental.plots.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/api/pydarshan/darshan.rst` & `darshan-3.4.4.0/docs/api/pydarshan/darshan.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/api/pydarshan/darshan.tests.rst` & `darshan-3.4.4.0/docs/api/pydarshan/darshan.tests.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/conf.py` & `darshan-3.4.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/index.rst` & `darshan-3.4.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/install.rst` & `darshan-3.4.4.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/make.bat` & `darshan-3.4.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/docs/usage.rst` & `darshan-3.4.4.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/pyproject.toml` & `darshan-3.4.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `darshan-3.4.3.0/setup.py` & `darshan-3.4.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     include_package_data=True,
     keywords="darshan",
     name="darshan",
     packages=find_packages(include=["darshan"]),
     setup_requires=setup_requirements,
     tests_require=test_requirements,
     url='https://www.mcs.anl.gov/research/projects/darshan/',
-    version='3.4.3.0',
+    version='3.4.4.0',
     zip_safe=False,
     package_data={"": ["*.darshan"],
                   "darshan": ["cli/style.css",
                               "cli/base.html",
                               "examples/example_logs/*",
                               "examples/darshan-graph/*",
                               "tests/input/*"]},
```

