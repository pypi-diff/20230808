# Comparing `tmp/cg-40.6.2.tar.gz` & `tmp/cg-40.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-40.6.2.tar", last modified: Mon Aug  7 14:29:10 2023, max compression
+gzip compressed data, was "dist/cg-40.6.3.tar", last modified: Tue Aug  8 12:39:42 2023, max compression
```

## Comparing `cg-40.6.2.tar` & `cg-40.6.3.tar`

### file list

```diff
@@ -1,1341 +1,1342 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-07 14:28:59.000000 cg-40.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-07 14:29:10.000000 cg-40.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-07 14:28:59.000000 cg-40.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 14:28:59.000000 cg-40.6.2/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/dragen_demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/db/models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/crunchy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19086 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/lims/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-07 14:28:59.000000 cg-40.6.2/cg/apps/tb/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20219 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/demultiplex/sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/set/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/upload/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/taxprofiler/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-07 14:28:59.000000 cg-40.6.2/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/archiving.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-07 14:28:59.000000 cg-40.6.2/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-07 14:28:59.000000 cg-40.6.2/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-07 14:28:59.000000 cg-40.6.2/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/archive/ddn_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/archive/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/demultiplex/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    18504 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77763 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/templates/mip-dna_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    78381 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/report/templates/rnafusion_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    20643 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/upload/upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26033 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13526 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-07 14:28:59.000000 cg-40.6.2/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/rnafusion/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/rnafusion/command_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/rnafusion/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/taxprofiler/taxprofiler_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-07 14:28:59.000000 cg-40.6.2/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-08-07 14:28:59.000000 cg-40.6.2/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-07 14:28:59.000000 cg-40.6.2/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-07 14:28:59.000000 cg-40.6.2/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18610 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-07 14:28:59.000000 cg-40.6.2/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    31756 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-08-07 14:28:59.000000 cg-40.6.2/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-07 14:28:59.000000 cg-40.6.2/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46349 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-07 14:29:10.000000 cg-40.6.2/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 14:28:59.000000 cg-40.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-07 14:28:59.000000 cg-40.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:29:10.000000 cg-40.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-07 14:28:59.000000 cg-40.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/test_dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/demultiplex/test_sample_sheet_creator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24593 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/lims/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/lims/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-07 14:28:59.000000 cg-40.6.2/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/test_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/upload/test_cli_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-08-07 14:28:59.000000 cg-40.6.2/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    99558 2023-08-07 14:28:59.000000 cg-40.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/spring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/spring/dummy_run_001.spring
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/spring/dummy_run_002.spring
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/170407_ST-E00198_0209_BHHKVCALXX/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/230504_A00689_0804_BHY7FFDRX2/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/CopyComplete.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RTAComplete.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)    79276 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4459 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/run_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/io/example_json.json
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/io/example_xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257895 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1508.28.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257305 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257516 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257046 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1508.28.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257619 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1508.28.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257428 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1508.28.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257569 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1508.28.rnafusion.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   165243 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88532 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/1605.11.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-07 14:28:59.000000 cg-40.6.2/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-07 14:28:59.000000 cg-40.6.2/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-08-07 14:28:59.000000 cg-40.6.2/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-07 14:28:59.000000 cg-40.6.2/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-07 14:28:59.000000 cg-40.6.2/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-07 14:28:59.000000 cg-40.6.2/tests/io/test_io_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-07 14:28:59.000000 cg-40.6.2/tests/io/test_io_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-08-07 14:28:59.000000 cg-40.6.2/tests/io/test_validate_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/archive/test_archive_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/clean/test_clean_flow_cell_run_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/clean/test_remove_old_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    17564 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17797 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/test_rename_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/test_report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/report/test_rnafusion_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/gisaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-07 14:28:59.000000 cg-40.6.2/tests/meta/workflow/test_rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20616 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-07 14:28:59.000000 cg-40.6.2/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-07 14:28:59.000000 cg-40.6.2/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-07 14:28:59.000000 cg-40.6.2/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-07 14:28:59.000000 cg-40.6.2/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-07 14:28:59.000000 cg-40.6.2/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-07 14:28:59.000000 cg-40.6.2/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    33719 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-08-07 14:28:59.000000 cg-40.6.2/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-07 14:28:59.000000 cg-40.6.2/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:10.000000 cg-40.6.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-07 14:28:59.000000 cg-40.6.2/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:42.000000 cg-40.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-08 12:39:28.000000 cg-40.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-08 12:39:42.000000 cg-40.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-08 12:39:28.000000 cg-40.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 12:39:28.000000 cg-40.6.3/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/dragen_demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/db/models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/crunchy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19086 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-08 12:39:28.000000 cg-40.6.3/cg/apps/tb/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20219 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/demultiplex/sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/set/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/upload/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/taxprofiler/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 12:39:28.000000 cg-40.6.3/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/archiving.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 12:39:28.000000 cg-40.6.3/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-08 12:39:28.000000 cg-40.6.3/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-08 12:39:28.000000 cg-40.6.3/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/archive/ddn_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/archive/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/demultiplex/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18504 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77763 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/templates/mip-dna_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    78381 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/report/templates/rnafusion_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20643 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/upload/upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26033 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13526 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-08 12:39:28.000000 cg-40.6.3/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/rnafusion/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/rnafusion/command_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/rnafusion/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/taxprofiler/taxprofiler_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-08 12:39:28.000000 cg-40.6.3/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-08-08 12:39:28.000000 cg-40.6.3/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 12:39:28.000000 cg-40.6.3/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-08 12:39:28.000000 cg-40.6.3/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18610 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-08 12:39:28.000000 cg-40.6.3/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31756 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-08-08 12:39:28.000000 cg-40.6.3/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-08 12:39:28.000000 cg-40.6.3/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46381 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-08 12:39:41.000000 cg-40.6.3/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-08 12:39:28.000000 cg-40.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-08 12:39:28.000000 cg-40.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:39:42.000000 cg-40.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-08 12:39:28.000000 cg-40.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/test_dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/demultiplex/test_sample_sheet_creator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24593 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/lims/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/lims/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 12:39:28.000000 cg-40.6.3/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/test_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/upload/test_cli_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-08-08 12:39:28.000000 cg-40.6.3/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99558 2023-08-08 12:39:28.000000 cg-40.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/ACC11927A5_S1_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/spring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/spring/dummy_run_001.spring
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/spring/dummy_run_002.spring
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/170407_ST-E00198_0209_BHHKVCALXX/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/230504_A00689_0804_BHY7FFDRX2/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/CopyComplete.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RTAComplete.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79276 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4459 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/run_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/io/example_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/io/example_xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257895 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1508.28.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257305 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257516 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257046 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1508.28.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257619 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1508.28.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257428 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1508.28.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257569 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1508.28.rnafusion.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   165243 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88532 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/1605.11.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-08 12:39:28.000000 cg-40.6.3/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-08 12:39:28.000000 cg-40.6.3/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-08-08 12:39:28.000000 cg-40.6.3/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-08 12:39:28.000000 cg-40.6.3/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-08 12:39:28.000000 cg-40.6.3/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-08 12:39:28.000000 cg-40.6.3/tests/io/test_io_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-08 12:39:28.000000 cg-40.6.3/tests/io/test_io_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-08-08 12:39:28.000000 cg-40.6.3/tests/io/test_validate_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/clean/test_clean_flow_cell_run_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/clean/test_remove_old_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    17564 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17797 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/test_rename_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/test_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/report/test_rnafusion_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/gisaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-08 12:39:28.000000 cg-40.6.3/tests/meta/workflow/test_rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20616 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-08 12:39:28.000000 cg-40.6.3/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-08 12:39:28.000000 cg-40.6.3/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 12:39:28.000000 cg-40.6.3/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-08 12:39:28.000000 cg-40.6.3/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-08 12:39:28.000000 cg-40.6.3/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 12:39:28.000000 cg-40.6.3/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:42.000000 cg-40.6.3/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33719 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:42.000000 cg-40.6.3/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:42.000000 cg-40.6.3/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-08-08 12:39:28.000000 cg-40.6.3/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-08 12:39:28.000000 cg-40.6.3/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:41.000000 cg-40.6.3/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:42.000000 cg-40.6.3/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:42.000000 cg-40.6.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-08 12:39:28.000000 cg-40.6.3/tests/utils/test_utils.py
```

### Comparing `cg-40.6.2/PKG-INFO` & `cg-40.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 40.6.2
+Version: 40.6.3
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-40.6.2/README.md` & `cg-40.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/crud/create.py` & `cg-40.6.3/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/crud/delete.py` & `cg-40.6.3/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/crud/find.py` & `cg-40.6.3/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/base.py` & `cg-40.6.3/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/datasource.py` & `cg-40.6.3/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/demux.py` & `cg-40.6.3/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/demux_sample.py` & `cg-40.6.3/cg/apps/cgstats/db/models/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/dragen_demux_sample.py` & `cg-40.6.3/cg/apps/cgstats/db/models/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/sample.py` & `cg-40.6.3/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/support_params.py` & `cg-40.6.3/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/unaligned.py` & `cg-40.6.3/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/db/models/version.py` & `cg-40.6.3/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-40.6.3/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-40.6.3/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/parsers/demux_stats.py` & `cg-40.6.3/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-40.6.3/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-40.6.3/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/parsers/run_info.py` & `cg-40.6.3/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/cgstats/stats.py` & `cg-40.6.3/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/coverage/api.py` & `cg-40.6.3/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/crunchy/crunchy.py` & `cg-40.6.3/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/crunchy/files.py` & `cg-40.6.3/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/crunchy/sbatch.py` & `cg-40.6.3/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/demultiplex_api.py` & `cg-40.6.3/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/demux_report.py` & `cg-40.6.3/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/sample_sheet/create.py` & `cg-40.6.3/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-40.6.3/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/sample_sheet/index.py` & `cg-40.6.3/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/sample_sheet/models.py` & `cg-40.6.3/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-40.6.3/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-40.6.3/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/demultiplex/sbatch.py` & `cg-40.6.3/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/gens.py` & `cg-40.6.3/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/gt.py` & `cg-40.6.3/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/hermes/hermes_api.py` & `cg-40.6.3/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/hermes/models.py` & `cg-40.6.3/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/housekeeper/hk.py` & `cg-40.6.3/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/invoice/render.py` & `cg-40.6.3/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-40.6.3/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-40.6.3/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-40.6.3/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-40.6.3/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/lims/api.py` & `cg-40.6.3/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/lims/batch.py` & `cg-40.6.3/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/lims/order.py` & `cg-40.6.3/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/lims/sample_sheet.py` & `cg-40.6.3/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/loqus.py` & `cg-40.6.3/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/madeline/api.py` & `cg-40.6.3/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/mip/confighandler.py` & `cg-40.6.3/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/mutacc_auto.py` & `cg-40.6.3/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/orderform/excel_orderform_parser.py` & `cg-40.6.3/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/orderform/json_orderform_parser.py` & `cg-40.6.3/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/orderform/orderform_parser.py` & `cg-40.6.3/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/osticket.py` & `cg-40.6.3/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/scout/scout_export.py` & `cg-40.6.3/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/scout/scoutapi.py` & `cg-40.6.3/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/api.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-40.6.3/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/slurm/sbatch.py` & `cg-40.6.3/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/slurm/slurm_api.py` & `cg-40.6.3/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/tb/api.py` & `cg-40.6.3/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/apps/tb/models.py` & `cg-40.6.3/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/add.py` & `cg-40.6.3/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/backup.py` & `cg-40.6.3/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/base.py` & `cg-40.6.3/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/clean.py` & `cg-40.6.3/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/compress/base.py` & `cg-40.6.3/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/compress/fastq.py` & `cg-40.6.3/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/compress/helpers.py` & `cg-40.6.3/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/delete/base.py` & `cg-40.6.3/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/delete/case.py` & `cg-40.6.3/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/delete/cases.py` & `cg-40.6.3/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/delete/observations.py` & `cg-40.6.3/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/deliver/base.py` & `cg-40.6.3/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/demultiplex/add.py` & `cg-40.6.3/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/demultiplex/base.py` & `cg-40.6.3/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/demultiplex/demux.py` & `cg-40.6.3/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/demultiplex/finish.py` & `cg-40.6.3/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/demultiplex/report.py` & `cg-40.6.3/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/demultiplex/sample_sheet.py` & `cg-40.6.3/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/generate/report/base.py` & `cg-40.6.3/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/generate/report/options.py` & `cg-40.6.3/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/generate/report/utils.py` & `cg-40.6.3/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/get.py` & `cg-40.6.3/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/set/base.py` & `cg-40.6.3/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/set/case.py` & `cg-40.6.3/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/set/cases.py` & `cg-40.6.3/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/store/fastq.py` & `cg-40.6.3/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/store/store.py` & `cg-40.6.3/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/transfer.py` & `cg-40.6.3/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/base.py` & `cg-40.6.3/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/clinical_delivery.py` & `cg-40.6.3/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/coverage.py` & `cg-40.6.3/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/delivery_report.py` & `cg-40.6.3/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/fohm.py` & `cg-40.6.3/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/genotype.py` & `cg-40.6.3/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/gens.py` & `cg-40.6.3/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/gisaid.py` & `cg-40.6.3/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/mutacc.py` & `cg-40.6.3/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/nipt/base.py` & `cg-40.6.3/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/nipt/ftp.py` & `cg-40.6.3/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/nipt/statina.py` & `cg-40.6.3/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/observations/observations.py` & `cg-40.6.3/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/observations/utils.py` & `cg-40.6.3/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/scout.py` & `cg-40.6.3/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/utils.py` & `cg-40.6.3/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/upload/validate.py` & `cg-40.6.3/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/balsamic/base.py` & `cg-40.6.3/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/balsamic/options.py` & `cg-40.6.3/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/balsamic/pon.py` & `cg-40.6.3/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/balsamic/qc.py` & `cg-40.6.3/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/balsamic/umi.py` & `cg-40.6.3/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/base.py` & `cg-40.6.3/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/commands.py` & `cg-40.6.3/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/fastq/base.py` & `cg-40.6.3/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/fluffy/base.py` & `cg-40.6.3/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/microsalt/base.py` & `cg-40.6.3/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/mip/base.py` & `cg-40.6.3/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/mip/options.py` & `cg-40.6.3/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/mip_dna/base.py` & `cg-40.6.3/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/mip_rna/base.py` & `cg-40.6.3/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/mutant/base.py` & `cg-40.6.3/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/nextflow/options.py` & `cg-40.6.3/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/rnafusion/base.py` & `cg-40.6.3/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/rnafusion/options.py` & `cg-40.6.3/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/taxprofiler/base.py` & `cg-40.6.3/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/cli/workflow/taxprofiler/options.py` & `cg-40.6.3/cg/cli/workflow/taxprofiler/options.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/__init__.py` & `cg-40.6.3/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/bcl_convert_metrics.py` & `cg-40.6.3/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/compression.py` & `cg-40.6.3/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/constants.py` & `cg-40.6.3/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/delivery.py` & `cg-40.6.3/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/demultiplexing.py` & `cg-40.6.3/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/encryption.py` & `cg-40.6.3/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/gene_panel.py` & `cg-40.6.3/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/housekeeper_tags.py` & `cg-40.6.3/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/lims.py` & `cg-40.6.3/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/nextflow.py` & `cg-40.6.3/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/observations.py` & `cg-40.6.3/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/orderforms.py` & `cg-40.6.3/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/priority.py` & `cg-40.6.3/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/report.py` & `cg-40.6.3/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/rnafusion.py` & `cg-40.6.3/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/scout_upload.py` & `cg-40.6.3/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/sequencing.py` & `cg-40.6.3/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/subject.py` & `cg-40.6.3/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/constants/taxprofiler.py` & `cg-40.6.3/cg/constants/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/exc.py` & `cg-40.6.3/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/io/api.py` & `cg-40.6.3/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/io/controller.py` & `cg-40.6.3/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/io/csv.py` & `cg-40.6.3/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/io/json.py` & `cg-40.6.3/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/io/validate_path.py` & `cg-40.6.3/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/io/xml.py` & `cg-40.6.3/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/io/yaml.py` & `cg-40.6.3/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/archive/archive.py` & `cg-40.6.3/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/archive/ddn_dataflow.py` & `cg-40.6.3/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/archive/models.py` & `cg-40.6.3/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/backup/backup.py` & `cg-40.6.3/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/backup/pdc.py` & `cg-40.6.3/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/clean/api.py` & `cg-40.6.3/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-40.6.3/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/clean/flow_cell_run_directories.py` & `cg-40.6.3/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/compress/compress.py` & `cg-40.6.3/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/compress/files.py` & `cg-40.6.3/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/deliver.py` & `cg-40.6.3/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/deliver_ticket.py` & `cg-40.6.3/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-40.6.3/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/demultiplex/demux_post_processing.py` & `cg-40.6.3/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/demultiplex/files.py` & `cg-40.6.3/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-40.6.3/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-40.6.3/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/demultiplex/utils.py` & `cg-40.6.3/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/demultiplex/validation.py` & `cg-40.6.3/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/encryption/encryption.py` & `cg-40.6.3/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/invoice.py` & `cg-40.6.3/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/meta.py` & `cg-40.6.3/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/observations/balsamic_observations_api.py` & `cg-40.6.3/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/observations/mip_dna_observations_api.py` & `cg-40.6.3/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/observations/observations_api.py` & `cg-40.6.3/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/api.py` & `cg-40.6.3/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/case_submitter.py` & `cg-40.6.3/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/fastq_submitter.py` & `cg-40.6.3/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/lims.py` & `cg-40.6.3/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/metagenome_submitter.py` & `cg-40.6.3/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/microbial_submitter.py` & `cg-40.6.3/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/pool_submitter.py` & `cg-40.6.3/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/rnafusion_submitter.py` & `cg-40.6.3/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/sars_cov_2_submitter.py` & `cg-40.6.3/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/submitter.py` & `cg-40.6.3/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/orders/ticket_handler.py` & `cg-40.6.3/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/balsamic.py` & `cg-40.6.3/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/balsamic_umi.py` & `cg-40.6.3/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/field_validators.py` & `cg-40.6.3/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/mip_dna.py` & `cg-40.6.3/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/report_api.py` & `cg-40.6.3/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/rnafusion.py` & `cg-40.6.3/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/templates/balsamic_report.html` & `cg-40.6.3/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/templates/bootstrap.html` & `cg-40.6.3/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/templates/mip-dna_report.html` & `cg-40.6.3/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/report/templates/rnafusion_report.html` & `cg-40.6.3/cg/meta/report/templates/rnafusion_report.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/rsync/rsync_api.py` & `cg-40.6.3/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/tar/tar.py` & `cg-40.6.3/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/transfer/external_data.py` & `cg-40.6.3/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/transfer/flowcell.py` & `cg-40.6.3/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/transfer/lims.py` & `cg-40.6.3/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/balsamic/balsamic.py` & `cg-40.6.3/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/coverage.py` & `cg-40.6.3/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/fohm/fohm.py` & `cg-40.6.3/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/gisaid/constants.py` & `cg-40.6.3/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/gisaid/gisaid.py` & `cg-40.6.3/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/gisaid/models.py` & `cg-40.6.3/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/gt.py` & `cg-40.6.3/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/mip/mip_dna.py` & `cg-40.6.3/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/mip/mip_rna.py` & `cg-40.6.3/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/mutacc.py` & `cg-40.6.3/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/nipt/models.py` & `cg-40.6.3/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/nipt/nipt.py` & `cg-40.6.3/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/rnafusion/rnafusion.py` & `cg-40.6.3/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-40.6.3/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-40.6.3/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/scout/hk_tags.py` & `cg-40.6.3/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/scout/mip_config_builder.py` & `cg-40.6.3/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-40.6.3/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/scout/scout_config_builder.py` & `cg-40.6.3/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/scout/uploadscoutapi.py` & `cg-40.6.3/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/upload/upload_api.py` & `cg-40.6.3/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/analysis.py` & `cg-40.6.3/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/balsamic.py` & `cg-40.6.3/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/balsamic_pon.py` & `cg-40.6.3/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/balsamic_qc.py` & `cg-40.6.3/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/balsamic_umi.py` & `cg-40.6.3/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/fastq.py` & `cg-40.6.3/cg/meta/workflow/fastq.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import logging
 import os
 import re
 import shutil
 from pathlib import Path
 from typing import List, Optional
 
-
 LOG = logging.getLogger(__name__)
 
 DEFAULT_DATE_STR = (
     "171015"  # Stand in value to use if sequencing date cannot be extracted from header
 )
 DEFAULT_INDEX = (
     "XXXXXX"  # Stand in value to use if flowcell index is to be masked when renaming file
@@ -163,23 +162,27 @@
             if len(matches) > 0:
                 data["flowcell"] = f"{data['flowcell']}-{matches[0]}"
             return data
 
     @staticmethod
     def create_fastq_name(
         lane: str,
-        flowcell: str,
+        flow_cell: str,
         sample: str,
         read: str,
         date: dt.datetime = DEFAULT_DATE_STR,
         index: str = DEFAULT_INDEX,
         undetermined: Optional[str] = None,
         meta: Optional[str] = None,
-    ):
-        raise NotImplementedError
+    ) -> str:
+        """Name a FASTQ file with standard conventions and
+        no naming constrains from pipeline."""
+        flow_cell: str = f"{flow_cell}-undetermined" if undetermined else flow_cell
+        date: str = date if isinstance(date, str) else date.strftime("%y%m%d")
+        return f"{lane}_{date}_{flow_cell}_{sample}_{index}_{read}.fastq.gz"
 
 
 class BalsamicFastqHandler(FastqHandler):
     @staticmethod
     def create_fastq_name(
         lane: str,
         flowcell: str,
@@ -281,46 +284,7 @@
             header_line = handle.readline().decode()
             header_info: dict = MutantFastqHandler.get_nanopore_header_info(line=header_line)
             data = {
                 "path": fastq_path,
                 "flowcell": header_info["flowcell"],
             }
             return data
-
-
-class RnafusionFastqHandler(FastqHandler):
-    @staticmethod
-    def create_fastq_name(
-        lane: str,
-        flow_cell: str,
-        sample: str,
-        read: str,
-        date: dt.datetime = DEFAULT_DATE_STR,
-        index: str = DEFAULT_INDEX,
-        undetermined: Optional[str] = None,
-        meta: Optional[str] = None,
-    ) -> str:
-        """Name a FASTQ file following MIP conventions,
-        no naming constrains from pipeline."""
-        flow_cell: str = f"{flow_cell}-undetermined" if undetermined else flow_cell
-        date: str = date if isinstance(date, str) else date.strftime("%y%m%d")
-        return f"{lane}_{date}_{flow_cell}_{sample}_{index}_{read}.fastq.gz"
-
-
-class TaxprofilerFastqHandler(FastqHandler):
-    """Handles Taxprofiler fastq file linking."""
-
-    @staticmethod
-    def create_fastq_name(
-        lane: str,
-        flow_cell: str,
-        sample: str,
-        read: str,
-        date: dt.datetime = DEFAULT_DATE_STR,
-        index: str = DEFAULT_INDEX,
-        undetermined: Optional[str] = None,
-        meta: Optional[str] = None,
-    ) -> str:
-        """Name a FASTQ file, no naming constrains from pipeline."""
-        flow_cell: str = f"{flow_cell}-undetermined" if undetermined else flow_cell
-        date: str = date if isinstance(date, str) else date.strftime("%y%m%d")
-        return f"{lane}_{date}_{flow_cell}_{sample}_{index}_{read}.fastq.gz"
```

### Comparing `cg-40.6.2/cg/meta/workflow/fluffy.py` & `cg-40.6.3/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/microsalt.py` & `cg-40.6.3/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/mip.py` & `cg-40.6.3/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/mip_dna.py` & `cg-40.6.3/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/mip_rna.py` & `cg-40.6.3/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/mutant.py` & `cg-40.6.3/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/nextflow_common.py` & `cg-40.6.3/cg/meta/workflow/nextflow_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,14 @@
 
     @classmethod
     def get_case_path(cls, case_id: str, root_dir: str) -> Path:
         """Returns a path where the rnafusion case should be located."""
         return Path(root_dir, case_id)
 
     @classmethod
-    def verify_case_config_file_exists(
-        cls, case_id: str, root_dir: str, dry_run: bool = False
-    ) -> None:
-        if (
-            not dry_run
-            and not Path(cls.get_case_config_path(case_id=case_id, root_dir=root_dir)).exists()
-        ):
-            raise ValueError(f"No config file found for case {case_id}")
-
-    @classmethod
     def get_case_config_path(cls, case_id: str, root_dir: str) -> str:
         """Return a path where the sample sheet for the case_id should be located."""
         return (
             Path((cls.get_case_path(case_id, root_dir)), f"{case_id}_samplesheet.csv")
             .absolute()
             .as_posix()
         )
@@ -216,19 +206,14 @@
         """Read deliverables file template and return content."""
         return ReadFile.get_content_from_file(
             file_format=FileFormat.YAML,
             file_path=file_bundle_template,
         )
 
     @classmethod
-    def verify_deliverables_file_exists(cls, case_id, root_dir):
-        if not Path(cls.get_deliverables_file_path(case_id=case_id, root_dir=root_dir)).exists():
-            raise CgError(f"No deliverables file found for case {case_id}")
-
-    @classmethod
     def add_bundle_header(cls, deliverables_content: dict) -> dict:
         return {"files": deliverables_content}
 
     @classmethod
     def write_deliverables_bundle(
         cls, deliverables_content: dict, file_path: Path, file_format=FileFormat.YAML
     ) -> None:
```

### Comparing `cg-40.6.2/cg/meta/workflow/prepare_fastq.py` & `cg-40.6.3/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/meta/workflow/rnafusion.py` & `cg-40.6.3/cg/meta/workflow/rnafusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 from pathlib import Path
 from typing import Dict, List, Optional
 
 from pydantic.v1 import ValidationError
 
 from cg import resources
 from cg.constants import Pipeline
-from cg.constants.constants import FileFormat, WorkflowManager
+from cg.constants.constants import FileFormat
 from cg.constants.nextflow import NFX_READ1_HEADER, NFX_READ2_HEADER, NFX_SAMPLE_HEADER
 from cg.constants.rnafusion import (
     RNAFUSION_METRIC_CONDITIONS,
     RNAFUSION_SAMPLESHEET_HEADERS,
     RNAFUSION_STRANDEDNESS_HEADER,
     RnafusionDefaults,
 )
 from cg.constants.tb import AnalysisStatus
-from cg.exc import CgError, HousekeeperFileMissingError, MetricsQCError, MissingMetrics
+from cg.exc import CgError, MetricsQCError, MissingMetrics
 from cg.io.controller import ReadFile, WriteFile
 from cg.io.json import read_json
-from cg.meta.workflow.analysis import AnalysisAPI
-from cg.meta.workflow.fastq import RnafusionFastqHandler
 from cg.meta.workflow.nextflow_common import NextflowAnalysisAPI
+from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.meta.workflow.tower_common import TowerAnalysisAPI
 from cg.models.cg_config import CGConfig
 from cg.models.deliverables.metric_deliverables import (
     MetricsBase,
     MetricsDeliverablesCondition,
     MultiqcDataJson,
 )
@@ -36,15 +35,15 @@
 from cg.models.rnafusion.rnafusion_sample import RnafusionSample
 from cg.store.models import Family
 from cg.utils import Process
 
 LOG = logging.getLogger(__name__)
 
 
-class RnafusionAnalysisAPI(AnalysisAPI):
+class RnafusionAnalysisAPI(NfAnalysisAPI):
     """Handles communication between RNAFUSION processes
     and the rest of CG infrastructure."""
 
     def __init__(
         self,
         config: CGConfig,
         pipeline: Pipeline = Pipeline.RNAFUSION,
@@ -59,50 +58,14 @@
         self.tower_binary_path: str = config.rnafusion.tower_binary_path
         self.tower_pipeline: str = config.rnafusion.tower_pipeline
         self.account: str = config.rnafusion.slurm.account
         self.email: str = config.rnafusion.slurm.mail_user
         self.compute_env: str = config.rnafusion.compute_env
         self.revision: str = config.rnafusion.revision
 
-    @property
-    def root(self) -> str:
-        return self.root_dir
-
-    @property
-    def fastq_handler(self):
-        return RnafusionFastqHandler
-
-    @property
-    def process(self):
-        if not self._process:
-            self._process = Process(
-                binary=self.tower_binary_path,
-            )
-        return self._process
-
-    @process.setter
-    def process(self, process: Process):
-        self._process = process
-
-    def get_profile(self, profile: Optional[str] = None) -> str:
-        if profile:
-            return profile
-        return self.profile
-
-    def get_workflow_manager(self) -> str:
-        """Get workflow manager for rnafusion."""
-        return WorkflowManager.Tower.value
-
-    def get_case_path(self, case_id: str) -> Path:
-        """Path to case working directory."""
-        return NextflowAnalysisAPI.get_case_path(case_id=case_id, root_dir=self.root)
-
-    def get_case_config_path(self, case_id):
-        return NextflowAnalysisAPI.get_case_config_path(case_id=case_id, root_dir=self.root_dir)
-
     def verify_analysis_finished(self, case_id):
         return NextflowAnalysisAPI.verify_analysis_finished(case_id=case_id, root_dir=self.root_dir)
 
     @staticmethod
     def build_samplesheet_content(
         case_id: str, fastq_r1: List[str], fastq_r2: List[str], strandedness: str
     ) -> Dict[str, List[str]]:
@@ -173,18 +136,14 @@
         NextflowAnalysisAPI.write_nextflow_yaml(
             content=default_options,
             file_path=NextflowAnalysisAPI.get_params_file_path(
                 case_id=case_id, root_dir=self.root_dir
             ),
         )
 
-    def get_trailblazer_config_path(self, case_id: str) -> Path:
-        """Return the path to a trailblazer config file containing Tower IDs."""
-        return Path(self.root_dir, case_id, "tower_ids.yaml")
-
     def write_trailblazer_config(self, case_id: str, tower_id: str) -> None:
         """Write Tower IDs to a .YAML file used as the trailblazer config."""
         config_path = self.get_trailblazer_config_path(case_id=case_id)
         LOG.info(f"Writing Tower ID to {config_path.as_posix()}")
         WriteFile.write_file_from_content(
             content={case_id: [tower_id]},
             file_format=FileFormat.YAML,
@@ -308,32 +267,19 @@
             if self.process.stderr:
                 LOG.error(self.process.stderr)
             if not dry_run:
                 tower_id = TowerAnalysisAPI.get_tower_id(stdout_lines=self.process.stdout_lines())
                 self.write_trailblazer_config(case_id=case_id, tower_id=tower_id)
             LOG.info(self.process.stdout)
 
-    def verify_case_config_file_exists(self, case_id: str, dry_run: bool = False) -> None:
-        NextflowAnalysisAPI.verify_case_config_file_exists(
-            case_id=case_id, root_dir=self.root_dir, dry_run=dry_run
-        )
-
-    def get_deliverables_file_path(self, case_id: str) -> Path:
-        return NextflowAnalysisAPI.get_deliverables_file_path(
-            case_id=case_id, root_dir=self.root_dir
-        )
-
     def get_pipeline_version(self, case_id: str) -> str:
         return NextflowAnalysisAPI.get_pipeline_version(
             case_id=case_id, root_dir=self.root_dir, pipeline=self.pipeline
         )
 
-    def verify_deliverables_file_exists(self, case_id: str) -> None:
-        NextflowAnalysisAPI.verify_deliverables_file_exists(case_id=case_id, root_dir=self.root_dir)
-
     def report_deliver(self, case_id: str) -> None:
         """Get a deliverables file template from resources, parse it and, then write the deliverables file."""
         deliverables_content: dict = NextflowAnalysisAPI.get_template_deliverables_file_content(
             resources.RNAFUSION_BUNDLE_FILENAMES_PATH
         )
         try:
             for index, deliver_file in enumerate(deliverables_content):
@@ -363,18 +309,14 @@
             )
         )
 
     def get_multiqc_json_path(self, case_id: str) -> Path:
         """Return the path of the multiqc_data.json file."""
         return Path(self.root_dir, case_id, "multiqc", "multiqc_data", "multiqc_data.json")
 
-    def get_metrics_deliverables_path(self, case_id: str) -> Path:
-        """Return a path where the <case>_metrics_deliverables.yaml file should be located."""
-        return Path(self.root_dir, case_id, f"{case_id}_metrics_deliverables.yaml")
-
     def get_multiqc_json_metrics(self, case_id: str) -> List[MetricsBase]:
         """Get a multiqc_data.json file and returns metrics and values formatted."""
         case: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
         sample_id: str = case.links[0].sample.internal_id
         multiqc_json: MultiqcDataJson = MultiqcDataJson(
             **read_json(file_path=self.get_multiqc_json_path(case_id=case_id))
         )
```

### Comparing `cg-40.6.2/cg/meta/workflow/taxprofiler.py` & `cg-40.6.3/cg/meta/workflow/taxprofiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 from cg.constants.taxprofiler import (
     TAXPROFILER_FASTA_HEADER,
     TAXPROFILER_INSTRUMENT_PLATFORM,
     TAXPROFILER_RUN_ACCESSION,
     TAXPROFILER_SAMPLE_SHEET_HEADERS,
 )
 from cg.meta.workflow.analysis import AnalysisAPI
-from cg.meta.workflow.fastq import TaxprofilerFastqHandler
 from cg.meta.workflow.nextflow_common import NextflowAnalysisAPI
 from cg.models.cg_config import CGConfig
 from cg.models.taxprofiler.taxprofiler_sample import TaxprofilerSample
-from cg.store.models import Family, Sample
+from cg.store.models import Family
 
 LOG = logging.getLogger(__name__)
 
 
 class TaxprofilerAnalysisAPI(AnalysisAPI):
     """Handles communication between Taxprofiler processes
     and the rest of CG infrastructure."""
@@ -32,25 +31,14 @@
         self,
         config: CGConfig,
         pipeline: Pipeline = Pipeline.TAXPROFILER,
     ):
         super().__init__(config=config, pipeline=pipeline)
         self.root_dir: str = config.taxprofiler.root
 
-    @property
-    def root(self) -> str:
-        return self.root_dir
-
-    @property
-    def fastq_handler(self):
-        return TaxprofilerFastqHandler
-
-    def get_case_config_path(self, case_id):
-        return NextflowAnalysisAPI.get_case_config_path(case_id=case_id, root_dir=self.root_dir)
-
     @staticmethod
     def build_sample_sheet_content(
         sample_name: str,
         fastq_r1: List[str],
         fastq_r2: List[str],
         instrument_platform: SequencingPlatform.ILLUMINA,
         fasta: Optional[str] = "",
```

### Comparing `cg-40.6.2/cg/meta/workflow/tower_common.py` & `cg-40.6.3/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/balsamic/config.py` & `cg-40.6.3/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/balsamic/metrics.py` & `cg-40.6.3/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/cg_config.py` & `cg-40.6.3/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/cgstats/stats_sample.py` & `cg-40.6.3/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/compression_data.py` & `cg-40.6.3/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/deliverables/metric_deliverables.py` & `cg-40.6.3/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/demultiplex/demux_results.py` & `cg-40.6.3/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/demultiplex/flow_cell.py` & `cg-40.6.3/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/demultiplex/run_parameters.py` & `cg-40.6.3/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/demultiplex/sbatch.py` & `cg-40.6.3/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/file_data.py` & `cg-40.6.3/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/invoice/invoice.py` & `cg-40.6.3/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/lims/sample.py` & `cg-40.6.3/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/mip/mip_config.py` & `cg-40.6.3/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/mip/mip_metrics_deliverables.py` & `cg-40.6.3/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/mip/mip_sample_info.py` & `cg-40.6.3/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/nextflow/deliverables.py` & `cg-40.6.3/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/nextflow/sample.py` & `cg-40.6.3/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/observations/input_files.py` & `cg-40.6.3/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/orders/constants.py` & `cg-40.6.3/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/orders/excel_sample.py` & `cg-40.6.3/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/orders/json_sample.py` & `cg-40.6.3/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/orders/order.py` & `cg-40.6.3/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/orders/orderform_schema.py` & `cg-40.6.3/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/orders/sample_base.py` & `cg-40.6.3/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/orders/samples.py` & `cg-40.6.3/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/report/metadata.py` & `cg-40.6.3/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/report/report.py` & `cg-40.6.3/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/report/sample.py` & `cg-40.6.3/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/report/validators.py` & `cg-40.6.3/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/rnafusion/command_args.py` & `cg-40.6.3/cg/models/rnafusion/command_args.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/rnafusion/metrics.py` & `cg-40.6.3/cg/models/rnafusion/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/rnafusion/rnafusion_sample.py` & `cg-40.6.3/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/scout/scout_load_config.py` & `cg-40.6.3/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/slurm/sbatch.py` & `cg-40.6.3/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/models/workflow/mutant.py` & `cg-40.6.3/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/resources/20181012_Indices.csv` & `cg-40.6.3/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/resources/rnafusion_bundle_filenames.csv` & `cg-40.6.3/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/admin.py` & `cg-40.6.3/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/api.py` & `cg-40.6.3/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/app.py` & `cg-40.6.3/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/config.py` & `cg-40.6.3/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/ext.py` & `cg-40.6.3/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/invoices/templates/invoices/index.html` & `cg-40.6.3/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/invoices/templates/invoices/invoice.html` & `cg-40.6.3/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/invoices/templates/invoices/layout.html` & `cg-40.6.3/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/invoices/templates/invoices/new.html` & `cg-40.6.3/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/server/invoices/views.py` & `cg-40.6.3/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/api/add.py` & `cg-40.6.3/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/api/base.py` & `cg-40.6.3/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/api/core.py` & `cg-40.6.3/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/api/delete.py` & `cg-40.6.3/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/api/find_basic_data.py` & `cg-40.6.3/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/api/find_business_data.py` & `cg-40.6.3/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/api/status.py` & `cg-40.6.3/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_analysis_filters.py` & `cg-40.6.3/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_application_filters.py` & `cg-40.6.3/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_application_version_filters.py` & `cg-40.6.3/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_bed_filters.py` & `cg-40.6.3/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_bed_version_filters.py` & `cg-40.6.3/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_case_filters.py` & `cg-40.6.3/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_case_sample_filters.py` & `cg-40.6.3/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_collaboration_filters.py` & `cg-40.6.3/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_customer_filters.py` & `cg-40.6.3/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_flow_cell_filters.py` & `cg-40.6.3/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_invoice_filters.py` & `cg-40.6.3/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_metrics_filters.py` & `cg-40.6.3/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_organism_filters.py` & `cg-40.6.3/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_panel_filters.py` & `cg-40.6.3/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_pool_filters.py` & `cg-40.6.3/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_sample_filters.py` & `cg-40.6.3/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/filters/status_user_filters.py` & `cg-40.6.3/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/store/models.py` & `cg-40.6.3/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/checksum/checksum.py` & `cg-40.6.3/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/click/EnumChoice.py` & `cg-40.6.3/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/commands.py` & `cg-40.6.3/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/date.py` & `cg-40.6.3/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/dict.py` & `cg-40.6.3/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/dispatcher.py` & `cg-40.6.3/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/email.py` & `cg-40.6.3/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/files.py` & `cg-40.6.3/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/flask/enum.py` & `cg-40.6.3/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg/utils/utils.py` & `cg-40.6.3/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/cg.egg-info/PKG-INFO` & `cg-40.6.3/cg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 40.6.2
+Version: 40.6.3
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-40.6.2/cg.egg-info/SOURCES.txt` & `cg-40.6.3/cg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,15 @@
 cg/meta/workflow/fluffy.py
 cg/meta/workflow/microsalt.py
 cg/meta/workflow/mip.py
 cg/meta/workflow/mip_dna.py
 cg/meta/workflow/mip_rna.py
 cg/meta/workflow/mutant.py
 cg/meta/workflow/nextflow_common.py
+cg/meta/workflow/nf_analysis.py
 cg/meta/workflow/prepare_fastq.py
 cg/meta/workflow/rnafusion.py
 cg/meta/workflow/taxprofiler.py
 cg/meta/workflow/tower_common.py
 cg/models/__init__.py
 cg/models/analysis.py
 cg/models/cg_config.py
```

### Comparing `cg-40.6.2/requirements.txt` & `cg-40.6.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/setup.py` & `cg-40.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="40.6.2",
+    version="40.6.3",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-40.6.2/tests/apps/cgstats/conftest.py` & `cg-40.6.3/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-40.6.3/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/cgstats/crud/test_delete.py` & `cg-40.6.3/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-40.6.3/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-40.6.3/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/cgstats/parsers/test_run_info.py` & `cg-40.6.3/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/cgstats/test_cgstats_create.py` & `cg-40.6.3/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/cgstats/test_stats.py` & `cg-40.6.3/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/conftest.py` & `cg-40.6.3/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/coverage/test_coverage.py` & `cg-40.6.3/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/crunchy/conftest.py` & `cg-40.6.3/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/crunchy/test_compress_fastq.py` & `cg-40.6.3/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/crunchy/test_config.py` & `cg-40.6.3/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/crunchy/test_crunchy.py` & `cg-40.6.3/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/crunchy/test_spring_decompression.py` & `cg-40.6.3/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/demultiplex/conftest.py` & `cg-40.6.3/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-40.6.3/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/demultiplex/test_dummy_sample.py` & `cg-40.6.3/tests/apps/demultiplex/test_dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/demultiplex/test_index.py` & `cg-40.6.3/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-40.6.3/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-40.6.3/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/demultiplex/test_sample_sheet_creator_factory.py` & `cg-40.6.3/tests/apps/demultiplex/test_sample_sheet_creator_factory.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/gens/test_gens_api.py` & `cg-40.6.3/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/gt/conftest.py` & `cg-40.6.3/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/gt/test_gt_api.py` & `cg-40.6.3/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/hk/conftest.py` & `cg-40.6.3/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/hk/test__getattr__.py` & `cg-40.6.3/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/hk/test_add_file.py` & `cg-40.6.3/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/hk/test_bundles.py` & `cg-40.6.3/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/hk/test_core.py` & `cg-40.6.3/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/hk/test_file.py` & `cg-40.6.3/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/hk/test_version.py` & `cg-40.6.3/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/lims/conftest.py` & `cg-40.6.3/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/lims/test_api.py` & `cg-40.6.3/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/lims/test_sample_sheet.py` & `cg-40.6.3/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/loqus/conftest.py` & `cg-40.6.3/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/loqus/test_loqusdb_api.py` & `cg-40.6.3/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/madeline/conftest.py` & `cg-40.6.3/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/madeline/test_madeline.py` & `cg-40.6.3/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/mip/conftest.py` & `cg-40.6.3/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/mip/test_config_mip.py` & `cg-40.6.3/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/mutacc_auto/conftest.py` & `cg-40.6.3/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-40.6.3/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/orderform/conftest.py` & `cg-40.6.3/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-40.6.3/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/orderform/test_excel_sample_schema.py` & `cg-40.6.3/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/orderform/test_json_orderform_parser.py` & `cg-40.6.3/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/orderform/test_orderform_parser.py` & `cg-40.6.3/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/scout/conftest.py` & `cg-40.6.3/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/scout/test_get_causative_variants.py` & `cg-40.6.3/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/scout/test_get_scout_cases.py` & `cg-40.6.3/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/scout/test_scout_load_config.py` & `cg-40.6.3/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/scout/test_scout_models.py` & `cg-40.6.3/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-40.6.3/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-40.6.3/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-40.6.3/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/slurm/conftest.py` & `cg-40.6.3/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/slurm/test_slurm_api.py` & `cg-40.6.3/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/test_apps_environ.py` & `cg-40.6.3/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/apps/test_osticket.py` & `cg-40.6.3/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/add/test_cli_add.py` & `cg-40.6.3/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/add/test_cli_add_customer.py` & `cg-40.6.3/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/add/test_cli_add_family.py` & `cg-40.6.3/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/add/test_cli_add_relationship.py` & `cg-40.6.3/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/add/test_cli_add_sample.py` & `cg-40.6.3/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/backup/conftest.py` & `cg-40.6.3/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/backup/test_backup_command.py` & `cg-40.6.3/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/clean/conftest.py` & `cg-40.6.3/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/clean/test_balsamic_clean.py` & `cg-40.6.3/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-40.6.3/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/clean/test_hk_bundle_files.py` & `cg-40.6.3/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-40.6.3/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/clean/test_microbial_clean.py` & `cg-40.6.3/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-40.6.3/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/compress/conftest.py` & `cg-40.6.3/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/compress/test_cli_compress_fastq.py` & `cg-40.6.3/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/compress/test_cli_decompress_spring.py` & `cg-40.6.3/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/compress/test_compress_helpers.py` & `cg-40.6.3/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/compress/test_store_fastq.py` & `cg-40.6.3/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/conftest.py` & `cg-40.6.3/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/delete/test_cli_delete_case.py` & `cg-40.6.3/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/delete/test_cli_delete_cases.py` & `cg-40.6.3/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/deliver/conftest.py` & `cg-40.6.3/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/deliver/test_deliver_base.py` & `cg-40.6.3/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/deliver/test_rsync_base.py` & `cg-40.6.3/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-40.6.3/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/demultiplex/test_add_flowcell.py` & `cg-40.6.3/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-40.6.3/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-40.6.3/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/demultiplex/test_finish_demux.py` & `cg-40.6.3/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/demultiplex/test_stats_command.py` & `cg-40.6.3/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-40.6.3/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/generate/report/conftest.py` & `cg-40.6.3/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-40.6.3/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/generate/report/test_utils.py` & `cg-40.6.3/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/generate/test_cli_base.py` & `cg-40.6.3/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/get/test_cli_get.py` & `cg-40.6.3/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/get/test_cli_get_analysis.py` & `cg-40.6.3/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/get/test_cli_get_case.py` & `cg-40.6.3/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/get/test_cli_get_flow_cell.py` & `cg-40.6.3/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/get/test_cli_get_sample.py` & `cg-40.6.3/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/set/conftest.py` & `cg-40.6.3/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/set/test_cli_set_case.py` & `cg-40.6.3/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/set/test_cli_set_cases.py` & `cg-40.6.3/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/set/test_cli_set_flowcell.py` & `cg-40.6.3/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/set/test_cli_set_list_keys.py` & `cg-40.6.3/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/set/test_cli_set_sample.py` & `cg-40.6.3/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/set/test_cli_set_samples.py` & `cg-40.6.3/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/store/test_fastq.py` & `cg-40.6.3/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/test_base.py` & `cg-40.6.3/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/test_clean.py` & `cg-40.6.3/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/conftest.py` & `cg-40.6.3/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_scout.py` & `cg-40.6.3/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_auto.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_fastq.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_genotype.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_gens.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_nipt.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/upload/test_cli_upload_observations.py` & `cg-40.6.3/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/balsamic/conftest.py` & `cg-40.6.3/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-40.6.3/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-40.6.3/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/balsamic/test_link.py` & `cg-40.6.3/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-40.6.3/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/balsamic/test_run.py` & `cg-40.6.3/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-40.6.3/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/conftest.py` & `cg-40.6.3/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-40.6.3/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/fluffy/conftest.py` & `cg-40.6.3/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-40.6.3/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-40.6.3/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-40.6.3/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-40.6.3/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-40.6.3/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/microsalt/conftest.py` & `cg-40.6.3/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-40.6.3/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-40.6.3/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/conftest.py` & `cg-40.6.3/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-40.6.3/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-40.6.3/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/taxprofiler/conftest.py` & `cg-40.6.3/tests/cli/workflow/taxprofiler/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-40.6.3/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py` & `cg-40.6.3/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/test_cli_workflow.py` & `cg-40.6.3/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-40.6.3/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/conftest.py` & `cg-40.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-40.6.3/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-40.6.3/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-40.6.3/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/analysis/sample_coverage.bed` & `cg-40.6.3/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/balsamic/case/config.json` & `cg-40.6.3/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-40.6.3/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-40.6.3/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-40.6.3/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-40.6.3/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-40.6.3/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-40.6.3/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/madeline/madeline.xml` & `cg-40.6.3/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-40.6.3/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-40.6.3/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/scout/643594.config.yaml` & `cg-40.6.3/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/scout/case_export.json` & `cg-40.6.3/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/scout/export_causatives.json` & `cg-40.6.3/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/scout/none_case_export.json` & `cg-40.6.3/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/scout/other_sex_case.json` & `cg-40.6.3/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/scout/panel_export.bed` & `cg-40.6.3/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/scout/panel_export.csv` & `cg-40.6.3/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-40.6.3/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/balsamic.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/fastq.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/metagenome.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/microsalt.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/mip.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/rml.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-40.6.3/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/data/SampleSheet.csv` & `cg-40.6.3/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/data/cgfixture.db` & `cg-40.6.3/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/data/hkstore.db` & `cg-40.6.3/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/io/example_json.json` & `cg-40.6.3/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1508.28.balsamic.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1508.28.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1508.28.fastq.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1508.28.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1508.28.mip.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1508.28.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1508.28.mip_rna.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1508.28.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1508.28.rnafusion.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1508.28.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/1605.11.metagenome.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/1605.11.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-40.6.3/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/NIPT-json.json` & `cg-40.6.3/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-40.6.3/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-40.6.3/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/report/case_data.json` & `cg-40.6.3/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/report/lims_exported_samples.json` & `cg-40.6.3/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/fixtures/report/lims_family.json` & `cg-40.6.3/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/io/conftest.py` & `cg-40.6.3/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/io/test_io_controller.py` & `cg-40.6.3/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/io/test_io_csv.py` & `cg-40.6.3/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/io/test_io_json.py` & `cg-40.6.3/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/io/test_io_xml.py` & `cg-40.6.3/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/io/test_io_yaml.py` & `cg-40.6.3/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/io/test_validate_path.py` & `cg-40.6.3/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/archive/conftest.py` & `cg-40.6.3/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/archive/test_archive_api.py` & `cg-40.6.3/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/archive/test_archiving.py` & `cg-40.6.3/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/backup/conftest.py` & `cg-40.6.3/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/backup/test_meta_backup.py` & `cg-40.6.3/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/backup/test_meta_pdc.py` & `cg-40.6.3/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/clean/conftest.py` & `cg-40.6.3/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-40.6.3/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-40.6.3/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/clean/test_remove_old_dirs.py` & `cg-40.6.3/tests/meta/clean/test_remove_old_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/compress/conftest.py` & `cg-40.6.3/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/compress/test_clean_fastq.py` & `cg-40.6.3/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/compress/test_compress_files.py` & `cg-40.6.3/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/compress/test_compress_meta_fastq.py` & `cg-40.6.3/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/compress/test_decompress_spring_meta.py` & `cg-40.6.3/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-40.6.3/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/conftest.py` & `cg-40.6.3/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/deliver/conftest.py` & `cg-40.6.3/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/deliver/test_deliver_ticket.py` & `cg-40.6.3/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/deliver/test_delivery_api.py` & `cg-40.6.3/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/conftest.py` & `cg-40.6.3/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-40.6.3/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-40.6.3/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-40.6.3/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/test_rename_files.py` & `cg-40.6.3/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-40.6.3/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/test_utils.py` & `cg-40.6.3/tests/meta/demultiplex/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/demultiplex/test_validation.py` & `cg-40.6.3/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/encryption/conftest.py` & `cg-40.6.3/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/encryption/test_encryption.py` & `cg-40.6.3/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/observations/conftest.py` & `cg-40.6.3/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/observations/test_meta_upload_observations.py` & `cg-40.6.3/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/conftest.py` & `cg-40.6.3/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-40.6.3/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-40.6.3/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-40.6.3/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-40.6.3/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_meta_orders_api.py` & `cg-40.6.3/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_meta_orders_lims.py` & `cg-40.6.3/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_meta_orders_status.py` & `cg-40.6.3/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_rnafusion_submitter.py` & `cg-40.6.3/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/orders/test_ticket_handler.py` & `cg-40.6.3/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/report/conftest.py` & `cg-40.6.3/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/report/test_balsamic_api.py` & `cg-40.6.3/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/report/test_field_validators.py` & `cg-40.6.3/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/report/test_mip_dna_api.py` & `cg-40.6.3/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/report/test_report_api.py` & `cg-40.6.3/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/report/test_rnafusion_api.py` & `cg-40.6.3/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/rsync/conftest.py` & `cg-40.6.3/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/rsync/test_rsync.py` & `cg-40.6.3/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/test_invoice.py` & `cg-40.6.3/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/transfer/conftest.py` & `cg-40.6.3/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/transfer/test_external_data.py` & `cg-40.6.3/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-40.6.3/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-40.6.3/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/balsamic/test_balsamic.py` & `cg-40.6.3/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/conftest.py` & `cg-40.6.3/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-40.6.3/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/mutacc/conftest.py` & `cg-40.6.3/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-40.6.3/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/nipt/conftest.py` & `cg-40.6.3/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-40.6.3/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/scout/conftest.py` & `cg-40.6.3/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/scout/test_generate_load_config.py` & `cg-40.6.3/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-40.6.3/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-40.6.3/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-40.6.3/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/test_meta_upload_coverage.py` & `cg-40.6.3/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/test_upload_api.py` & `cg-40.6.3/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/upload/test_upload_genotypes_api.py` & `cg-40.6.3/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/workflow/conftest.py` & `cg-40.6.3/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/workflow/test_analysis.py` & `cg-40.6.3/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/workflow/test_balsamic.py` & `cg-40.6.3/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/workflow/test_microsalt.py` & `cg-40.6.3/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-40.6.3/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/meta/workflow/test_rnafusion.py` & `cg-40.6.3/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/balsamic_analysis_mock.py` & `cg-40.6.3/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/crunchy.py` & `cg-40.6.3/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/hk_mock.py` & `cg-40.6.3/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/limsmock.py` & `cg-40.6.3/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/madeline.py` & `cg-40.6.3/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/mip_analysis_mock.py` & `cg-40.6.3/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/osticket.py` & `cg-40.6.3/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/process_mock.py` & `cg-40.6.3/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/report.py` & `cg-40.6.3/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/scout.py` & `cg-40.6.3/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/store_model.py` & `cg-40.6.3/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/mocks/tb_mock.py` & `cg-40.6.3/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/balsamic/conftest.py` & `cg-40.6.3/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/balsamic/test_balsamic_analysis.py` & `cg-40.6.3/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/conftest.py` & `cg-40.6.3/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/demultiplexing/conftest.py` & `cg-40.6.3/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/demultiplexing/test_demux_results.py` & `cg-40.6.3/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/demultiplexing/test_flowcell_model.py` & `cg-40.6.3/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/demultiplexing/test_run_parameters.py` & `cg-40.6.3/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/mip/conftest.py` & `cg-40.6.3/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/mip/test_mip_analysis.py` & `cg-40.6.3/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/mip/test_mip_config.py` & `cg-40.6.3/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-40.6.3/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/mip/test_mip_sample_info.py` & `cg-40.6.3/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/nextflow/conftest.py` & `cg-40.6.3/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/nextflow/test_nextflow_deliver.py` & `cg-40.6.3/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/observations/conftest.py` & `cg-40.6.3/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/observations/test_observations_input_files.py` & `cg-40.6.3/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/report/test_validators.py` & `cg-40.6.3/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/rnafusion/conftest.py` & `cg-40.6.3/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-40.6.3/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/test_cg_models.py` & `cg-40.6.3/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/test_compression_data.py` & `cg-40.6.3/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/test_file_data.py` & `cg-40.6.3/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/models/test_flowcell_class.py` & `cg-40.6.3/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/server/conftest.py` & `cg-40.6.3/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/add/test_store_add_application_version.py` & `cg-40.6.3/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/add/test_store_add_base.py` & `cg-40.6.3/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/add/test_store_add_customer.py` & `cg-40.6.3/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/add/test_store_add_flow_celll.py` & `cg-40.6.3/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/conftest.py` & `cg-40.6.3/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/delete/test_store_api_delete.py` & `cg-40.6.3/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/find/test_find_basic_data.py` & `cg-40.6.3/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-40.6.3/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/find/test_find_business_data.py` & `cg-40.6.3/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/find/test_find_business_data_analysis.py` & `cg-40.6.3/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/find/test_find_business_data_case.py` & `cg-40.6.3/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/find/test_find_business_data_sample.py` & `cg-40.6.3/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_analyses_to_clean.py` & `cg-40.6.3/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-40.6.3/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_store_api_status.py` & `cg-40.6.3/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_store_api_status_analysis.py` & `cg-40.6.3/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_store_api_status_cases.py` & `cg-40.6.3/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_store_api_status_customer.py` & `cg-40.6.3/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_store_api_status_pool.py` & `cg-40.6.3/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/status/test_store_api_status_sample.py` & `cg-40.6.3/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/api/test_base.py` & `cg-40.6.3/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/conftest.py` & `cg-40.6.3/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_analyses_filters.py` & `cg-40.6.3/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_application_filters.py` & `cg-40.6.3/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_application_version_filters.py` & `cg-40.6.3/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_bed_filters.py` & `cg-40.6.3/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_bed_version_filters.py` & `cg-40.6.3/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_case_sample_filters.py` & `cg-40.6.3/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_cases_filters.py` & `cg-40.6.3/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_collaboration_filters.py` & `cg-40.6.3/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_customer_filters.py` & `cg-40.6.3/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_flow_cell_filters.py` & `cg-40.6.3/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_invoice_filters.py` & `cg-40.6.3/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_metrics_filters.py` & `cg-40.6.3/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_organism_filters.py` & `cg-40.6.3/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_panel_filters.py` & `cg-40.6.3/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_pool_filters.py` & `cg-40.6.3/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_samples_filters.py` & `cg-40.6.3/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/filters/test_status_user_filters.py` & `cg-40.6.3/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/test_delivery.py` & `cg-40.6.3/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store/test_store_models.py` & `cg-40.6.3/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/store_helpers.py` & `cg-40.6.3/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/test_store_helpers.py` & `cg-40.6.3/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/utils/conftest.py` & `cg-40.6.3/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/utils/test_commands.py` & `cg-40.6.3/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/utils/test_date.py` & `cg-40.6.3/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/utils/test_dict.py` & `cg-40.6.3/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/utils/test_dispatcher.py` & `cg-40.6.3/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-40.6.2/tests/utils/test_utils.py` & `cg-40.6.3/tests/utils/test_utils.py`

 * *Files identical despite different names*

